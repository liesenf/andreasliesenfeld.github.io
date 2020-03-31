---
layout: default
---

## The "Talking (about) Chinese Characters" project

**UNDER CONSTRUCTION**

We present a voice bot that specifies Chinese characters in personal names through dialog with the user. In natural conversation this task arises when speakers want to know how the name of a person is written. Which characters the speaker is referring to can often not be directly inferred from the pronunciation of the name due to the large number of homophones in Mandarin Chinese personal names. Modeling this task using a voice interface is challenging due to a number of reasons. 

Personal names can contain a large number of possible, sometimes rare, characters, a few hundred possible pronunciations need to be mapped to several thousand possible characters. This usually requires the speaker to provide additional information of the features or form of the characters in question. To do this two strategies are common: Speakers may describe components of the character in question (1). Or speakers may provide an example of a word that contains the character in question (2). 
<i>

	
         (1) Component description stratgey:
	 
	 S1: "我姓张"
	     My last name is Zhang.
    	 
	 S2: "哪个张?"
	     Which Zhang?
    	 
	 S1: "弓长张"
	     The `zhang' character (张) with a gong (弓) and a chang (长) component.}
	
	(2) Example word strategy:
	
	 S1: "我姓王 国王的王"
	     "My last name is Wang. The 'wang'(王) character in the word 'king' (国王).

</i>

Namespec is an attempt to model these two strategies that speakers in real-world conversation use to disambiguate Chinese characters in personal names. To achieve this, Namespec consists of several Chinese character databases and a voice interface linked to a decision tree with a depth of 2 to 12 question-response pairs. The tree mainly consists of routines that select and confirm candidate characters, as well as several repair and fallback repair loops. To date, Namespec has undergone a round of user trails (n=100) as well as a conversation analysis-inspired qualitative test trail that both focused on improving intent recognition capabilities and user experience. 


<iframe
    allow="microphone;"
    width="350"
    height="430"
    src="https://console.dialogflow.com/api-client/demo/embedded/1779b520-551f-4bbf-bc9c-0a5154f217e0">
</iframe>


[back](./)
