# Proposal for Unitary Fund

Programming quantum computers currently requires specialized knowledge.
This project aims to create a higher-level, programming language for expressing probabilistic computations in a non-expert manner.
Recently, the cognitive science community around MIT has produced many developments using probabilistic programming languages [1-4, 8].
In a nutshell, probabilistic programming allows reasoning about a world model with tolerance for uncertainty under a bayesian framework.
  
Much like in quantum computing, probabilistic programming starts with random primitives (much like a qubit in, for example, the "plus" state) and produces as an answer to some query, amplitudes indicating the strength of various options.
Hofstaderian cognitive architectures also use a similar technique, where each level of the program makes a probabilistic decision, and when run multiple times, produces amplitudes as an answer [5].
Both of these probabilistic schemes have outperformed many techniques in conventional artificial intelligence (such as so-called "Deep Learning") on cognitively interesting tasks [3, 4, 7-9].
Additionally, any field that uses statistical modeling can benefit from probabilistic programming: simulation, stock trading, and medicine are a few among these.
Classical probabilistic techniques are used as a backend to these languages, but quantum computers are fundamentally probabilistic, and will potentially be better suited to solving these kinds of problems in the future.  

This language will be implemented by creating a new language the compiles into currently-used quantum programming languages (Such as the rigetti stack).
Additionally, probabilistic program learning can be used similarly to Gate Set Tomography, which has been used to improve existing quantum computers (Such as those produced by Rigetti). 
By implementing a more abstract probabilistic quantum programming language, the world's next set of quantum computers can potentially be used for deeply interesting tasks in cognitive science and statistical modeling in general.

[1] (https://arxiv.org/abs/1206.3255)  
[2] (http://web.mit.edu/cocosci/josh.html)  
[3] (web.mit.edu/cocosci/Papers/Science-2015-Lake-1332-8.pdf)  
[4] (http://www.pnas.org/content/110/45/18327.short)  
[5] (https://github.com/fargonauts/copycat)  
[6] (https://github.com/fargonauts/FARGonautica)  
[7] (www.foundalis.com/res/Foundalis_dissertation.pdf)  
[8] (https://arxiv.org/abs/1804.04452)  
[9] (http://www.foundalis.com/res/poc/PrinciplesOfCognition.htm)  

(I know sources don't usually go in an abstract, but I felt they were needed in this informal case)
