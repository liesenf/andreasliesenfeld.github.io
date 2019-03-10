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

An important approach to capture 'language independent knowledge structures' (i.e. knowledge beyond lexical semantics) that are relevant in dialog are <i>associative network formalisms</i> (e.g. Schank's (1972, 1975, 1980) conceptual dependency theory). The goal of this kind of formalism is to enable directed and efficient mechanisms that model inference processes based on associations (including 'causal connections') between representations grounded in linguistic form and working up across different levels of abstraction (towards modeling higher cognitive functions). This line of work is relevant to dialog systems because these formal models of knowledge representations are indespensable for developing useful symbolic natural language understanding systems that deal with meaning beyond that what is 'directly' encoded in linguistic form. In talk-in-interaction this is (1) knowledge about the intentions, plans and goals of different agents, and (2) knowledge about the preceding discourse (Schank's work and Gillis et al. 2009).

To date, <i>speech act theory</i> (SAT) and its many variations are still the most popular framework to model speaker intention. Within this community linguistic behaviour is often conceived and modeled as some form of 'rational' behaviour. For example, Allen and Perrault (1979) view linguistic behaviour as goal-driven planning: speakers plan an utterance in order to achieve a communicative goal while the interlocutors aim to infer that goal from linguistic form (see also Cohen and Perrault (1979). Depending on the specific framework, formal SAT approaches then generally design formalisms that aim to capture the specific "communicative goals and plans" tied to various linguistic forms and represent this knowledge using Type Theory with records (TTR). This view of linguistic behaviour as goal-oriented and plan-based is still widely adopted in the dialog modeling community (e.g. Kobsa 1989; Carberry 1989; Cohen et al. 1990; see also the QUALM system (Lehnert 1978)). Of course there is more to linguistic behaviour than this, and these rather simple question-as-database-query models have been criticized for their lack to capture more complex dimensions of inference (e.g. Wilensky 1983). 

A common way to expand these simple speech act approaches is to add more sophisticated models of <i>context</i> and <i>cotext</i>. For an adequate interpretation of an utteance, the hearer needs to take into account both situational context, the interlocutor's knowledge of the domain as well as as sorts of links between current utterances those that precede it. Various aspects of 'context' have been studied under topics such as reference, anaphora resolution and discourse coherence. Many models in these field rely on defining larger discourse structures that go beyond turns and setences, such as <i>schemas</i> or <i>frames</i>. For instance, the pioneering work by McKeown (1985) and Sidner (1983, 1985) on discourse generation is based on formalisms of certain underlying patterns that structure discourse, e.g. "schemas of discourse generation for attaining discourse goals" that both speakers and listeners rely on when jointly producing stretches of talk (Carberry 1989). 

What do these 'discourse formalisms' look like? Well, most proposed formalisms for the comprehension and production of discourse still tend to ignore many of this complexities and treat discourse as a product, provide a discourse grammar that consists of formal discourse rules as well as as some kind of augmented transition network (ATN) formalism for analyzing discourse. In contrast, however, qualitative research traditions of discourse and talk, most prominently probably conversation analysis (CA), have long advocated that dialog is a joint interactional achievement of multiple parties. In fact, the highly dynamic and complex view of dialog that conversation analysis advocates is yet to find an adequate formal representation, though some attempts were made to fruitfully integrate insights from CA and dialog modeling (e.g. Luff et al. 1990; Gillis et al. 2009). 

One of the prerequisites to develop dialog systems in adherence to conversation analytic theory are models that capture and update knowledge of the participants of a dialog and numerous of such modules have been developed as part of dialog systems under to the topic of <i>user models</i> (Wilensky et al. 1988; Chin 1989; Morik 1989). In the context of dialog systems, user models are knowledge bases that contain (and update) all aspects of the user that may be relevant to the dialog behaviour of the system and that inform 'intelligent' interaction (Allen 1994). User models are crucial modules of dialog systems that, based on storing relevant information about the interlocutors, enable more appropriate linguistic behaviour through recipient-tailored language generation.
The knowledge that is gathered during interaction and stored in user models is kept seperable from the rest of the system as it has to be dynamically reconstructed during each dialog, but it also has to be connected and inform many other dialog system modules. The specific design of user models may significantly vary between different task-oriented dialog systems and non-task oriented dialog systems (Wahlster ad Kobsa 1989). Disourse models and user models are largely intertwined and the exact relationship and interaction between the two is subject to ongoing debate in the field of dialog modeling (see for instance Heland 1988; Norman 1989 and the special issue <i>Computational Linguistics 14/3</i>. User model design has been a fast-changing field in the past decades and many advanced designs are unfortunately developed behind closed doors and are not openly accessible to the scientific community. 
Generally, user models can be divided into canonical user models that store knowledge of all users in general and individual user models that store knowledge related to individual users and keep records per individual user. A second distinction can be made between long-term and short-term user models, where long-term models track more general knowledge such as a history of discussed topics and and pursued goals and short-term models track more fine-grained specifics of an interaction (and they often interact with discourse models) (for more on this distinction, see also Rich 1988; Kobsa 1989). 

User models are primarily constructed from the actual input of a user, from which knowledge, plans and goals of the particular user are inferred. This type of knowledge can be relatedt to other sources of data, such as user profiles or interaction histories. Combining all available knowledge, a user model is created and dynamically updated as the interaction procedes. Here the notion of a <i>stereotype</i.> (sometimes also prototype) is useful (Rosch and Mervis 1975). As part of building individual user models, users that display similar behaviour and traits can be grouped together and form user classes. The class attributes or stereotypes then enable the system to infer whole sets of user characteristics on the basis of a smaller number of observations. Stereotypes are useful to assign traits to individual users based on less data, but the particular inference process of assigning class membership is of course defeasible and involve adding all sorts of (arbitrary) uncertainty measures such as numerical confidence ratings (Rich 1989; Chin 1989). However, out of the approaches to stereotype management that have been proposed, many remain somewhat unintuitive due to the complexity involved in task such as the resolution of contractory inferences and the confidence management of the assigned properties. This active area of research is sometimes also referred to as <i>truth management</i>: the study of user model design that deals with assigning new properties to the model while maintaining its consistency and adequacy (Doyle 1983).  

Building on user models (that are already challenging enough to design), <i>language generation</i> is the even more complex task of deciding what to say and how to say it (for an overview of the field, see, for instance, Kempen 1989 or McDonald 1992). Generation of adequate turns needs to take knowledge into account related to many aspects including the current domain of discourse, user models and the situational context and cotext. A lot of work in this field is related to <i>Rhetorical Structure Theory</i> (RST) in one way or another. Generally, RST is used to identify rhetoric relations between units of speech, which are then used to produce larger stretches of discourse in a 'coherent' fashion. RST can be applied to various levels of discourse structure, ranging from sequential relations between turns and turn-constructional units to putting together whole sequences of talk in an ostensibly coherent manner (e.g. Hovy 1990, 1991l Cawsey 1990, Paris 1991, Scott and de Souza 1990). Other approaches have introduced the notion of <i>focus</i> (also question-under-discussion (QUD)), that broadly speaking aim to model attention and topic management in dialog (McCoy and Cheng 1991). Other increasingly important field in language generation are multimodality and backchannel generators (also 'linguistic feedback generators') that model 'non-linguistic' or non-lexical aspects of talk-in-interaction. 

In summary, current approaches to dialog modeling combine a multitude of different frameworks, each consisting of different representation techniques such as rules, logic, frames or grammars. Orchestrated as a whole these symbollic programming constructs can achieve an unprecedented level of abstraction that allows to mimic human-like linguistic flexibility and creativity. However, due to the high level of abstraction, today's symbolic systems have become extremely complex to handle as each exception requires additional rules and processing (see scalability problem). In recent years, data-intensive machine learning techniques have been added at many levels of these systems, further increasing complexity while promising potential solutions for existing scalability and robustness problems. Generally, the dialog modeling community seems to have moved away from the description of linguistic structure per se towards a description of more 'cognitive' aspects of talk-in-interaction in the form of large associative networks (e.g. semantic webs, framenets, construction networks etc.). In line with this trend, the remainder of this post focused on describing the links between linguistic structure to processes of 'social action formation'. First, I will review existing approaches in the field, such as speech act theories and dialog act taxonomies. Then I will outline an approach to this task that conceptualizes the links between structure and social action as a multitude of fine-grained, continuous, often ambiguous and always recipient-designed processes. Finally, I will explore how these processes of <i>reflexive action formation</i> (Levinson 2013) can inform a corpus-based method for the development of representations of speech acts as vectors. 

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
