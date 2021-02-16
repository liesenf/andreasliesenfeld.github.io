---
layout: default
---

## The limits of automation in Conversational AI



 <i> Keywords: human-computer interaction *** voice bot development *** conversational user interface </i>

 
We develop a voice assistant skill that helps the user specify Chinese characters in personal names through dialog. In natural conversation this task arises when speakers want to know how the name of a person is written. Which characters the speaker is referring to can often not be directly inferred from the pronunciation of the name due to the large number of homophones in Mandarin Chinese personal names. Names can also contain a large number of possible, sometimes rare, characters, a few hundred possible pronunciations need to be mapped to several thousand possible characters. This makes modeling the capacity to specify Chinese characters through dialog a challenging task. The aim of this project of the <a href="http://llt.cbs.polyu.edu.hk/">PolyU Linguistics Theory and Language Technology (LTT) group</a> in Hong Kong is to develop a bot skill that is able to specify characters through a conversational interface with the user. 


### User-driven conversation design and system development

We take a user-driven approach to voice bot development centered on user experience [3]. We begin by exploring the task that we eventually want to model in human-human conversation. To better understand the potential user, we examine how speakers solve our task in natural talk based on video recordings. The aim is to come up with a detailed description of strategies as they are used in real-world converasations. Next, we develop a prototype conversational user interface for the task that simulates the identified strategies. Part of this prototype is the development of databases of all the relevant information that is needed to complete the task. In our case, databases that contain Chinese personal names and their pronounciations. Third, we test our prototype system with real users. Our system undergoes iterative testing cycles with embedded user testing. After each iteration we evaluate system performance and fine-tune dialog flow, intent recognition, and repair functions. Step-by-step, we improve user experience through adapting a turn design enables adequate interaction between user and interface. The challenge is to strike a balance between generalizations over user input that model idealized types of dialog flow, and accounting for individual preference by implementing a large number of alternative ways to solve the task. 

Preliminary results show that speakers use at least two strategies to specify features or form of Chinese characters in question. Speakers may describe components of the character in question (1). Or speakers may provide an example of a word that contains the character in question (2). 
	
(1) Component description strategy:
 
	 S1: "我姓张"
	     My last name is Zhang.
    	 
	 S2: "哪个张?"
	     Which Zhang?
    	 
	 S1: "弓长张"
	     The 'zhang' character (张) with a gong (弓) and a chang (长) component.
	    	  
(2) Example word strategy:
	
	 S1: "我姓王 国王的王"
	     My last name is Wang. The 'wang'(王) character in the word 'king' (国王).


We then model the identifies strategies that speakers use to disambiguate Chinese characters in personal names. We use a decision tree-based bot development environment with integrated speech recognition capabilities [1] [2]. The bot consists of two main components:

(1) Database of relevant Chinese characters for Chinese last name candidates (n=400) and given name candidates (n=5500).

(2) a voice interface with integrated intent recognition that navigates the decision tree with the user (currently of a depth of 2 to 12 question-response pairs).

The bot also features a ranking algortihm that selects Characters based on user input as well as a range of additional modules that provide additional navigation capabilities such as fallback repair loops and tree navigation shortcuts for advanced users. The bot can be employed as a stand-alone voice interface or integrated in existing voice assistant ecosystems such as Actions-on-Google, Alexa Skills or Wit.ai.


<iframe allow="microphone;" width="350" height="430" src="https://console.dialogflow.com/api-client/demo/embedded/1779b520-551f-4bbf-bc9c-0a5154f217e0">
</iframe>


### User experience evaluation

We evaluate user experience based on three types of data:

(1) User analytics in form of system logs that provide information on user input and dialog progression.

(2) Video recordings of human-voice bot interaction that provide observational data on user experience.

(3) Self-reported user experience evaluation based on feeback surveys and semi-structured interviews.




#### References:

[1] Google. 2020. Dialog Flow. https://dialogflow.com/ Accessed: 2020-03-02

[2] Google. 2020. Google Cloud Speech API. https://cloud.google.com/speech-to-text Accessed: 2020-03-02

[3] Gould, J. D., & Lewis, C. (1985). Designing for usability: key principles and what designers think. Communications of the ACM, 28(3), 300-311.

[back](./)
