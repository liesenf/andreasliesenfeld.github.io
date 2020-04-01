---
layout: default
---

## Talking (about) Chinese Characters



 <i> Keywords: voice bot development *** conversation design *** dialog system </i>

We develop a voice assistant that helps the user specify Chinese characters in personal names through dialog. In natural conversation this task arises when speakers want to know how the name of a person is written. Which characters the speaker is referring to can often not be directly inferred from the pronunciation of the name due to the large number of homophones in Mandarin Chinese personal names. Names can also contain a large number of possible, sometimes rare, characters, a few hundred possible pronunciations need to be mapped to several thousand possible characters. This makes modeling the capacity to specify Chinese characters through dialog a challenging task. The aim of this 2-year project of the <a href="http://llt.cbs.polyu.edu.hk/">PolyU Linguistics Theory and Language Technology (LTT) group</a> in Hong Kong is to develop a bot that is able to specify characters through a voice interface with the user. This involves an empirical analysis of strategies that speakers use to solve this task, the collection of relevant Chinese personal name databases and the development of a Natural Language Understanding (NLU) module that provides dialog flow, intent recognition and repair functions.

### User-driven conversation design and system development

Our approach to voice interface design is grounded in understanding human interaction. How do speakers specify characters in real world talk? What strategies do they use and how can we describe their actions systematically? We employ video-based analysis of real-world interaction to explore these questions.

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


Building on these insights, we model strategies that speakers use to disambiguate Chinese characters in personal names. We use a decision tree-based bot development environment with integrated speech recognition capabilities [1] [2]. The bot consists of two main components:

(1) collections of relevant Chinese characters for Chinese last name processing (n=400) and given name processing (n=19000).

(2) a voice interface with integrated intent recognition (rule-based and machine learning-based) that navigates the decision tree with the user (currently of a depth of 2 to 12 question-response pairs).

In addition to these two main components the bot also features a ranking algortihm that selects Characters based on user input as well as a range of additional modules that provide additional navigation capabilities such as fallback repair loops and tree navigation shortcuts for advanced users. The bot can be employed as a stand-alone voice interface or integrated in existing voice assistant ecosystems such as Actions-on-Google, Alexa Skills or Wit.ai.


<iframe allow="microphone;" width="350" height="430" src="https://console.dialogflow.com/api-client/demo/embedded/1779b520-551f-4bbf-bc9c-0a5154f217e0">
</iframe>


### User experience evaluation

After the development of a working prototype, we ground the further development of our dialog flow and intent recognition capabilities on user feedback and user experience evaluation. To date, our system has undergone one round of preliminary user trails. Three types of data were collected:

(1) User analytics in form of system logs that provide information on user input and dialog progression.

(2) video recordings of human-voice bot interaction that provide observational data on user experience.

(3) self-reported user experience evaluation based on feeback surveys and semi-structured interviews.




#### References:

Google. 2020. Dialog Flow. https://dialogflow.com/ Accessed: 2020-03-02

Google. 2020. Google Cloud Speech API. https://cloud.google.com/speech-to-text Accessed: 2020-03-02

[back](./)
