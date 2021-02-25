---
layout: default
---

## Formal representations of talk for language technology

 <i> Keywords: ethnomethodology of formal linguistics *** Gestalt psychology *** Conversation Analysis </i>

** UNDER CONSTRUCTION **

### Introduction

I began my journey in academia with studying story-telling. I noticed that no two stories that I recorded were alike and that it was impossible for speakers to repeat  a story once it was told in exactly the same way. This observation has stuck with me since I switched to the field of language technology. 

In the real world, talk is interactionally accomplished as reflexive, ongoing social conduct. Formal representations are designed to take some aspects of it into account as tools for research and technology applications. But talk is more than spoken text. This project aims to tease out some of the implications that this has on for the tools that are used to study and engineer talk. I aim to illuminate some implications of the limited means that we have to formally represent talk for voice technology applications, the quantitative study of talk, and the possiblity of talking machines. I approach these questions through the empirical study of conversational corpora and NLP pipelines drawing on Conversation Analysis and Radical Construction Grammar.

### Reduce, compute, automate

Formal represenations of language link up various aspects of talk-in-interaction to symbolic representations. Through this, computational models become possible for various scientific or technological purposes. Text and speech processing pipelines rely on these representations to accomplish engineering tasks and enable automation. What are the limits of symbolic representations as appropriate representations of talk. How are representations used as part of different application? What is the relationship of the represenation to the real thing? And how can we slice the representation into useful units?

### The basics: Transcription - from audio recordings to symbolic representatations of speech

Transcription, either manual or automatic, is the task of mapping elements of speech from audio recordings to textual transcription symbols. This can be done by a human transcriber or automated by probabalistically determining the mappings using graphical representations of speech (spectrograms). 

Using machine learning methods, automatic speech recognition has become quite accurate for any transcription task where there is sufficient traning data available. Those with experience using current ASR can attest that transcribing clean, grammatical sentences works fine. But what about all the other things that humans do in conversation, such as the "uhs", "ahs", or "ohs", laughter, sighs, stutters and all the other exclamations and interjections? Transcribing such conduct is usually sidelined in current ASR because they do not add much commerical value to ASR products. But there is more. Other issues of form-function mapping become visible when looking at these small utterances that barely count as verbal conduct. Here, on the "margins of language" (Dingemanse 2017), one can see the gap between idiolect and language conventions more clearly. The "uhs", "ahs" and laughters of each speaker come with a unique footprint that is only vaguely coventionalised and that makes stable mappings between form and function across a population impossible. It turns out that both the small and large units in talk are private property of the speakers, characterized by unique variation, and ultimately resistant to formal generalization. A speaker's "ohs" and "ahs" are as hard to formalize as their long, elaborate story-telling sequences. This makes up the upper and lower boundaries of useful formalization of units in talk.


### Other mappings: Formalisms for Conversational AI - symbolic natural language understanding

After computing a useful textual representation of speech input, the processing pipeline of a typical Conversational AI usually feed this representation into Natural Language Understanding (NLU) module. This is where automation beyond single turns of conversation happen. The job of the NLU module is to determine what next turn the system will synthesize in service of accomplishing a defined range of tasks, such as ordering a pizza or booking a ticket. 

Task: dialog flow prediction

prediction of adjacency pairs (question-response pairs) , TRPs and other sequential patterns 

based on seq-to-seq models of spoken and subtitle corpora 

Getting rid of intents?

References:
Dingemanse, M., 2017. On the margins of language: Ideophones, interjections and dependencies in linguistic theory. Dependencies in language, pp.195-202.

[back](./)
