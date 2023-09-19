# Instance-Based-Learning-Model-
Broad steps

Train
Feed knowledge in robot’s memory

Test
Shortlisting
Activation
Prob. ret.
Blended val.
AIM: 1) so the robot doesn’t have to start from zero.
	2) the robot can learn to mimic from the human’s  behavior.

In IBL model: Past experiences are stored as:
 <situation, decision, utility>  (SDU) triplets     → called instances.

So a vector can be created containing:
Situation
Take Screenshot of Player’s view of environment
To find distance b/w the current test situation vector ( situation in front of the robot ) and the memory situation vectors. ( past robot or human experiences )

Decision
The action that was taken

Utility
How good was that action in that situation 
A numeric value (reward earned on doing that action)
Feed knowledge in robot’s memory



Implementation in our problem:	

Instance SDU vector (mem experience) :


index:

1      2     3      4      5      6…………………………………………………………….155

Action

Robo co-ordinates

Situation

 150 values

Utility
AIM: to find out the past experiences similar to the current (test) situation.

Similarity function 

Need in our problem:
Similarity func finds distance b/w 2 vectors.
From screenshot img extract main features : encoded using principal component analysis (PCA) into a 150-length vector.

Methods:
Cosine distance, Euclidean distance (L2) …
Cosine distance being used currently

Working:
Pass both the vectors into the function and get the similarity value.
Inputs : current test situation, candidate memory experience
Outputs : similarity value in interval 0 to 1
Summary


Activation of each experience(instance):  
Analogous to relevance,
Frequency, recency, similarity with the current situation
Random noise component.


The probability of retrieval:
Equivalent to the weightage of the instance.

Blended Value:
A scoring mechanism for the alternatives.
maximum Blended Value → chosen decision.









Our Actual Task:


Search and acquire certain objects 




A single-player search-and-retrieval game was developed simulating several huge buildings spread over a grassy land.
The objective was to collect certain objects called targets (reward of +5) while avoiding contact with certain other objects called distractors (penalty of -5 ). 
Each participant played a training session, 15 minutes long, with the feedback (current game score displayed) and a test session 10 minutes long without the feedback.
For the training and the test session the target count was 14 and 28, while the distractor count was 7 and 14.
Four participants from Indian Institute of Technology Mandi, India, were recruited to participate in this study.
Situation/ State: The image of player’s view encoded using principal component analysis (PCA) into a 150-length vector.
The actions taken by the players, and the reward received along with the corresponding situation vector, were recorded as tuples.

Main work
Paper : Multi-human intelligence in Instance-Based Learning
https://www.researchgate.net/publication/364348448_Multi-human_intelligence_in_Instance-Based_Learning

Video: Iconip 2022 presentation                   			

Supplementary:

Video: ACS 2022  presentation ( different task )

Website:
Working of IBL ( link ) ( the “internals” part of the web article )

Paper:
Instance-based Learning: A General Model of Repeated Binary Choice (link)
Making Instance-based Learning Theory usable and understandable:The Instance-based Learning Tool (link)
Evaluation of Instance-Based Learning and Q-Learning Algorithms in Dynamic Environments (link)


