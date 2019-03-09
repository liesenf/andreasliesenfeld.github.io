---
layout: default
---

# A new approach to dialog management: Towards a corpus-based method to model reflexive action formation

The aim of models of action formation for application in dialog systems is to develop computational models of the knowledge and processes involved in the reflexive processes of formatting and ascribing actions to turn-at-talk - an essential task to human or human-like participation in the turn-taking system. 

toward a method to model processes of action formation and ascription as vector space representations
Why now? Large speech corpora available

The development of models of these processes has both theoretical and practical applications. The motivation can be to use these models as a basis for theories about human (linguistic) interaction, but it can also be the development of speech technology that emulate this kind of social conduct for various applications.

### Theory testing and development: Computational modeling as new approach to solve old problems

Alishahi, computational modeling as scientific method



### Application in dialog systems


Generally speaking, the developement of speech technology in this area is guided by the following principles (Gillis et al. 2009):

<i>problem reduction</i>: a task is decomposed into a number of simpler substasks which can be further decomposed until subtasks are distinguished which can directly be modeled and implemented.

<i>modularity</i>: the program achieving a task is divided into different modules, often corresponding to major substasks, which are more or less autonomous, specialized information processors.

<i>formalization</i>: Within each module, a formalism is designed that puts together the necessary knowledge and methods needed for that module to accomplish its task. The respective formalism needs to capture the representation and manipulation of the specific slice of knowledge, i.e. it provides a bridge between theory and implementation. Such formalizations provide the means with which the necessary knowledge is organized in a certain way. However, this necessary step of (re)organizing the data is often problematic for a number of theoretical reasons (see section "On reductionism").
Formalization ultimately provides a means to enable inference for how the data can be used to solve the task at hand, either through 'procedual formal models' that enable direct inference based on specific instances or through 'declarative formal models' that exhibit a larger degree of separation between knowledge representation and inference aspects of a problem. Formalisms represent linguistic knowledge in various forms. In the area of grammar and linguistic structure the often take the form of state-space search models, logic-based or rule-based formalizations. In semantics the may come in form of graph-based representations such as semantic networks and frames (see section "framenets and constructicons").

As for dialog systems, the task of interpreting and generating natual language is usually decomposed into various subtasks tied to 'linguistic units', i.e. phoneme, word, turn (or sentence) and discourse. Based on this division, a larger architecture of various modules is established both on the language understanding and the language generation side. Possible modules in language understanding are: <i>speech recognition, morphological analysis, syntactic parsing, semantic analysis </i> and <i>discourse analysis</i>. And for language generation: <i>discourse planning, turn (or sentence) generation, morphological generation</i> and <i>speech production</i>.

The modules are often organized as part of a sequential architecture where the different modules are accessed in sequence and the output of one module is directly input into the next module. Recently, more interactive architectures have also gained popularity where the modules are not strictly accessed in a sequential fashion, but feature more links and feedback loops between different modules (i.e. distributed connectionist models). This is especially true for the syntax-semantics interface where a trend can be observed away from 'syntax first' strategies in which a syntactic parse is computed first and then fed into a semantic module. Instead, new approaches to the syntax-semantics interface enable an integration of these formely separate  modules, often drawing on cognitive grammars (see section "Framenets and Constructicons"). Noteably, this trend is a reminder that the division into modules is fact driven by design decisions based on the principles of 'problem reduction' and 'modularity', but that it is by no means garanteed that the dividing lines in such a system accurately reflect talk-in-interaction in humans. This also applies to the semantics-pragmatics interface.

### Existing approaches to representing knowledge and intentions in dialog systems

An important approach to capture 'language independent knowledge structures' (i.e. knowledge beyond lexical semantics) that are relevant in dialog are <i>associative network formalisms</i> (e.g. Schank's (1972, 1975, 1980) conceptual dependency theory). The goal of this kind of formalism is to enable directed and efficient mechanisms that model inference processes based on associations (including 'causal connections') between representations grounded in linguistic form and working up across different levels of abstraction (towards modeling higher cognitive functions). This line of work is relevant to dialog systems because these formal models of knowledge representations are indespensable for developing useful symbolic natural language understanding systems that deal with meaning beyond that what is 'directly' encoded in linguistic form. In talk-in-interaction this is (1) knowledge about the intentions, plans and goals of different agents, and (2) knowledge about the preceding discourse (Gillis et al. 2009).




## Corpus-based representations of dialog acts

Bloomfield and beyond

### Towards a method to identify properties of 'distributional dialog acts' 







## Dialog acts a construction networks

formalization is not an 'innocent' or theory-neural practice (Linell)
Grounded theory

### Labeling dialog acts: Exploratory data analysis 

### Modeling dialog acts: vector space representations

towards a method for (1) 'comparative' and (2) 'latent' speech act analysis





## Remaining challenges

modeling reflexivity (recursive loops)
open system properties (i.e. language as cas) operate not only on the level of (cognitive) knowledge representation but also intersubjectively

### On reductionism

linguistics as computational social science
beyond 'mainstream' scientific method

'mixed method' approach:
grounded theory (Glaser and Strauss)

### The Language as Complex Adaptive Systems (CAS) paradigm

Introductory readings on Complex Adaptive Systems and their relation to talk-in-interaction:

<a href="http://cnl.psych.cornell.edu/pubs/2009-LACAS-pos-LL.pdf">Position paper</a> by Clay Beckner, Nick C. Ellis, Richard, Blythe John Holland, Joan Bybee, Jinyun Ke, Morten H. Christiansen, Diane Larsen-Freeman, William Croft and Tom Schoenemann.



[back](./)
