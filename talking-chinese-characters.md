---
layout: default
---

## The "Talking (about) Chinese Characters" project



** UNDER CONSTRUCTION **

We develop a voice assistant that helps the user specify Chinese characters in personal names through dialog. In natural conversation this task arises when speakers want to know how the name of a person is written. Which characters the speaker is referring to can often not be directly inferred from the pronunciation of the name due to the large number of homophones in Mandarin Chinese personal names. Names can also contain a large number of possible, sometimes rare, characters, a few hundred possible pronunciations need to be mapped to several thousand possible characters. This makes modeling the capacity to specify Chinese characters through dialog a challenging task. The aim of this 2-year project of the <a href="http://llt.cbs.polyu.edu.hk/">PolyU Linguistics Theory and Language Technology (LTT) group</a> in Hong Kong is to develop a bot that is able to specify characters through a voice interface with the user. This involves an empirical analysis of strategies that speakers use to solve this task, the collection of relevant Chinese personal name databases and the development of a Natural Language Understanding (NLU) module that provides dialog flow, intent recognition and repair functions.

### User-driven conversation design and system development

In real-world conversation speakers employ various strategies to specify features or form of the Chinese characters in question. Two strategies are common. Speakers may describe components of the character in question. Or speakers may provide an example of a word that contains the character in question. 
	
(1) Component description strategy:
 
	 S1: "我姓张"
	     My last name is Zhang.
    	 
	 S2: "哪个张?"
	     Which Zhang?
    	 
	 S1: "弓长张"
	     The 'zhang' character (张) with a gong (弓) and a chang (长) component.}
	    	  
	
(2) Example word strategy:
	
	 S1: "我姓王 国王的王"
	     My last name is Wang. The 'wang'(王) character in the word 'king' (国王).




We model two strategies that speakers in real-world conversation use to disambiguate Chinese characters in personal names. Our bot is built around a range of Chinese character databases linked to a voice interface in form of a decision tree with a depth of 2 to 12 question-response pairs. The tree mainly consists of routines that select and confirm candidate characters, as well as several repair and fallback repair loops. 



<iframe allow="microphone;" width="350" height="430" src="https://console.dialogflow.com/api-client/demo/embedded/1779b520-551f-4bbf-bc9c-0a5154f217e0">
</iframe>


### User experience evaluation

To date, our system has undergone a round of user trails (n=100) as well as a conversation analysis-inspired qualitative test trail that both focused on improving intent recognition capabilities and user experience. 


[back](./)
