# Jigsaw-Toxicity-Comment-Text-Classification
Case Study on text classification based on AI, Machine Learning , Deep Learning , NLP

Visit Blog: https://medium.com/@gujaraditya9623/jigsaw-unintended-bias-in-toxicity-classification-81073e0b91f6

# Introduction:
In this world of online conversations, as this brings the world to communicate on various social media and other platforms. This comes with great responsibilities for the platforms to analyze the comments by users that might be offensive, threatening, targeting to some identity or other such toxic comments. Organizations are attempting to build advanced AI mechanisms using Natural Language Processing ways to deal with such text based problems.
The Conversation AI team, a research initiative founded by Jigsaw and Google (both part of Alphabet), builds technology to protect voices in conversation. Jigsaw extended annotations of this data by human raters for various toxic conversations and set a kaggle competition to build ML/DL models to identify toxic comments.  

# Business Problem:
The Conversation AI team initially had built models that classify comments with toxicity, but incorrectly learned to associate the names of frequently attacked identities with toxicity. Whereas toxicity is defined as anything rude, disrespectful or otherwise likely to make someone leave a discussion. The dataset also labels certain comments as bias/targeted towards certain identity, where the source of comment states it as toxic which is actually not - this the unintended bias. So our objective is to build a model that finds the toxic comments and minimize the unintended bias with respect to mentioned identities.

# About Data:

Data downloaded from  https://www.kaggle.com/c/jigsaw-unintended-bias-in-toxicity-classification/data

Required files:

•	test.csv

•	train.csv

•	sample_submission.csv

Disclaimer: The dataset for this competition contains text that may be considered profane, vulgar, or offensive. 

This is a binary classification problem, 0 means non-toxic and 1 means toxic comment. The categories of identities which are important to consider ethnicity- asian , black, white; gender- male, female, transgender; sexual orientation- bi_homosexual_gay_or_lesbian; religion-hindu, muslim, cristian; disability-psychiatric_or_mental_illness. 

## Columns Information:
•	Id: Each comment assigned a number.

•	target: ranges from 0 to 1, degree of toxicity

•	comment_text: commented text to analyze.

•	severe_toxicity: comments which are highly toxic.

•	Degree of toxicity mentioned for following identities:


### Demographic Category:	                     Identities

Gender	            :                       Male, Female, Transgender, Other gender

Sexual Orientation	 :                      Heterosexual, Homosexual, Bisexual,Other sexual orientation

Religion	            :                     Christian, Jewish, Muslim, Hindu, Buddhist, Atheist, Other religion

Race or ethnicity	     :                    Black, White, Latino/Latina/Latinx,Other race or ethnicity

Disability	            :                   Physical disability,Intellectual or learning disability, Psychiatric disability or mental illness, Other disability

•	created_date: date when comment updated

•	Other expressions with the count each expression received: funny , wow , sad , likes, disagree

•	sexual_explicit: sexually targeted toxicity degree.

•	Other annotator count columns for identity and toxicity: identity_annotator_count, toxicity_annotator_count

