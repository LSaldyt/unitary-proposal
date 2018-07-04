# Quantum Probabilistic Programming

## Synopsis and Introduction

Programming quantum computers currently requires specialized knowledge.
This project aims to create a higher-level, quantum-hybrid programming language for expressing probabilistic computations in a non-expert manner.
Recently, the cognitive science community around MIT has produced many developments using probabilistic programming languages [1-4, 8].
In a nutshell, probabilistic programming allows reasoning about a world model with tolerance for uncertainty under a Bayesian framework.
  
Much like in quantum computing, probabilistic programming starts with random primitives (much like a qubit in, for example, the "plus" state) and produces as an answer to some query, amplitudes indicating the strength of various options.
Hofstaderian cognitive architectures also use a similar technique, where each level of the program makes a probabilistic decision, and when run multiple times, produces amplitudes as an answer [5].
Both of these probabilistic schemes have outperformed many techniques in conventional artificial intelligence (such as so-called "Deep Learning") on cognitively interesting tasks [3, 4, 7-9].
Additionally, any field that uses statistical modeling can benefit from probabilistic programming: simulation, stock trading, and medicine are a few among these.

In traditional probabilistic techniques, the backend is classical. However, quantum computers are fundamentally probabilistic, and will potentially be better suited to solving these kinds of problems in the future.  

This language will be implemented by compiling into currently-used quantum programming languages (Such as the Rigetti stack), and, through the hybrid model, including existing probabilistic programming libraries.
Additionally, probabilistic program learning can be used similarly to Gate Set Tomography, which has been used to improve existing quantum computers (Such as those produced by Rigetti). 
By implementing a more abstract probabilistic quantum programming language, the world's next set of quantum computers can potentially be used for deeply interesting tasks in cognitive science and statistical modeling in general.

## Preliminary Timeline

Total project duration is roughly one year, but preliminary versions will be available before then. 
Of course, this is all following Hofstadter's law: `It will take longer than you think it will take, even if you account for Hofstadter's law`.
 
 - Analysis of existing programming languages and platforms (classical, probabilistic, and quantum) (1-2w)
 - Syntax sketch and proof of concept (1-2w)
 - Analysis and implementation of an initial core inference algorithm (1mo).
 - Testing of published probabilistic programming examples (<1w).
 - Improvements of core inference algorithm (potentially infinite).

## Methods

Currently, these are slightly more technical ideas about how I'll approach the timeline steps above.
 
 - Research (*memorize* the Quil spec, read some of the motivations behind Clojure (one of the world's best intelligently designed programming languages, IMHO), and investigate the wealth of publications about probabilistic programming (Like the Goodman et al guide))
 - Create syntax in BNF-like language
 - Feed syntax to parser-generator (glossa, ari, or something official like ANTLR)
 - Write compiler to Rigetti stack (in Clojure or C++)
 - Experiment with hybrid inference algorithm (Classical w/ quantum building blocks)
 - Create a quantum inference algorithm... Consult with implementers of classical inference algorithms for advice
 - Demonstrate existing models, but in the quantum framework
 - Create new models in the quantum framework
 - Build language bindings
 - Testing, debugging, polishing, and publishing (if warranted).
 - If there is extra time, test the tangential ideas at the bottom of this document
 - Profit? 

## Unordered Sources

[1] (https://arxiv.org/abs/1206.3255)  
[2] (http://web.mit.edu/cocosci/josh.html)  
[3] (web.mit.edu/cocosci/Papers/Science-2015-Lake-1332-8.pdf)  
[4] (http://www.pnas.org/content/110/45/18327.short)  
[5] (https://github.com/fargonauts/copycat)  
[6] (https://github.com/fargonauts/FARGonautica)  
[7] (www.foundalis.com/res/Foundalis_dissertation.pdf)  
[8] (https://arxiv.org/abs/1804.04452)  
[9] (http://www.foundalis.com/res/poc/PrinciplesOfCognition.htm)  

## Related Rabbitholes

- Can Bayesian Program Learning be efficiently used for Quantum Gateset Tomography?
- Can a Hofstadterian architecture (like copycat) be implemented and sped up by a quantum computer? (sure, but how easily would it be done, and would it be useful?)
- What does one name a quantum programming language? 
