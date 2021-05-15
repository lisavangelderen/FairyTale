# Gender Biases in Fairytales 

# Abstract

In this repository will be research into the possibility of gender bias in fairy tales. Fairy tales can give children important messages about gender roles, even though these messages might be based on outdated stereotypes [1]. Gender bias in fairy tales might include more focus on beauty in female characters and less on intelligence, and portraying female characters as passive agents [1]. A lot of children grow up hearing fairy tales before bed, or they learn reading by virtue of fairy tales. As such, these stories can have a big impact on the forming of opinions in young children. A lot of the stories are meant to teach children certain traditional values and are often very old. It is therefore worth it to investigate the way these stories handle gender roles. In old stories, usually written by men, gender roles can be quite stereotypical and patronizing towards women. The most classic fairy tale template is a great example of this: “A brave prince needs to rescue a beautiful but helpless princess from her perils.”. If we teach children values with stories that contain stereotypical gender roles, these roles will be perpetuated in the next generation. This is why this repository aims to map the way fairy tales deal with gender. 

# Research questions

* Is there gender bias in fairytales?  
	* Is there a difference when talking about 'the princess' or 'the prince' of the story or a side character 'girl'/'boy'?
		* If there is, is there a difference between the female or male difference?
	* How do the contexts female characters appear in alignment with the conventional stereotypical and prejudiced vision of women in our society?
	* Can the same conventional stereotypical vision of men be found in the stories?
		* If they can, are these stereotypes more negative or positive than the female ones? 

# What we’re expecting / hypothese 
* Female characters: 
	* soft spoken, gentle and considerate
	* Passive rol;: need a prince or other male character to help/rescue them
	* Obedient 
	* “Feminine appearance”: elegant, dresses, perfectly arranged hair…
* Male characters: 
	* Strong, handsome and brave
	* Commanding and listened to/respected by others
	* Appearance adapted to circumstances
	* More active role: travelling, fighting, discovering...

# Method
Look at adjectives, verbs and adverbs appearing in the context of female/male names and personal pronouns:
Adjectives: how characters are described, physical and mental attributes
Verbs: what type of actions the characters accomplish, how the contribute to the storyline
Adverbs: along with the adjectives, contribute to the image given by the characters 
We believe these groups will provide a good representation of possible gender biases in the corpora.
We will also use language modelling and language generation to check which words are most commonly associated with stereotypical male and female terms used in fairytales, such as "boy" and "girl", and "prince" and "princess".

# Dataset
For this project, we'll be using a partially preprocessed dataset. The dataset contains the following: 

* Number of stories: 453
* Number of words: 908,174
* Average words/story: 1891
* Shortest story: 75
* Longest story: 17,694
* Clusters: 365

The stories are from 5 different authors and have been POS tagged and lemmatized. This should be plenty of data to test our questions on whilst still being computationally feasible. The data file in the repository contains different clusters (created in a paper referenced at the bottom), where each cluster contains a number of stories. Each story looks like this:

There/EX --> there/EX
was/VBD --> be/VBD
a/DT --> a/DT
certain/JJ --> certain/JJ
merchant/NN --> merchant/NN
who/WP --> who/WP
had/VBD --> have/VBD
two/CD --> two/CD
children/NNS --> child/NNS
,/, --> ,/,
a/DT --> a/DT
boy/NN --> boy/NN
and/CC --> and/CC
a/DT --> a/DT
girl/NN --> girl/NN
;/: --> ;/:

To further preprocess the dataset, we remove punctuation and focus on only parts that we’re interested in. 

Link to the dataset: https://www.hlt.inesc-id.pt/w/Fairy_tale_corpus

In addition to the above mentionned dataset, a dataset that we assembled ourselves with stories has also been used. This can be found in the andersongrimm.txt file. The stories in that file come from project Gutenberg. 

# A tentative list of milestones for the project

* Milestone 1

To start we will do some further preprocessing (possibly removing some tokens), collect the stories in a way that makes them easy for us to use (right now the files are organised in a way that is not too user friendly, making some rearrangements and making sure we only take into account the lemmatized tokens, not the un-lemmatized ones.), and decide on different methods to answer our questions (we could look at the correlations of certain tokens with gender roles, or train a model to predict a word associated with a gender role).
Then we will make a new timeline according to our reorganisation and plans on how to tackle the problems at hand.

* Milestone 2

See issue 1

* Milestone 3

See issue 2


# Personal contributions

* Alexia

Data preprocessing, finding sources, milestone 2,3

* Lisa 

Data exploration, generating small texts, creating extra dataset, ngram model and analysis, milestone 1,2  

* Victor 

Building/writing paper, building powerpoint, milestone 2,3

* Zoë

training model, making visual representations, milestone 2,3

* Everyone

Maintaining repository, working out ideas, milestone 1, presentation



# Documentation

The repo is quite self-explenatory, in the readme all the required information for the project can be found. 
* The code is all in 1 jupyter notebook, codefile.ipynb, in here the all the code for the project can be found neatly organized and explained.
* The data used by the code is in the data file, the code extracts it from the different clusters.
* The extra dataset can be found in andersongrimm.txt
* The paper is written in LateX and can be found in the paper folder as a pdf, the LateX form can also be found here.
* The presentation can be found in the presentation folder and only holds a pptx file containing the slides. This is the only folder that is updated after the 16th of may.

# Sources

[1] M.R. Lieberman. ""Some Day My Prince Will Come": Female Acculturation through the Fairy Tale." _College English_. vol. 34, no.3, p.383, 1972. 

1. Paula Vaz Lobo, David Martins de Matos, Fairy Tale Corpus Organization Using Latent Semantic Mapping and an Item-to-item Top-n Recommendation Algorithm, In Language Resources and Evaluation Conference - LREC 2010, European Language Resources Association (ELRA), Malta, May 2010 
2. https://hilo.hawaii.edu/campuscenter/hohonu/volumes/documents/Vol07x07HappilyEverAfter.pdf
3. https://www.researchgate.net/publication/344922675_Challenging_gender_stereotypes_through_a_transformation_of_a_fairy_tale_Challenging_gender_stereotypes_through_a_transformation_of_a_fairy_tale
4. https://digitalcommons.butler.edu/cgi/viewcontent.cgi?article=1663&context=facsch_papers
5. https://www.gutenberg.org/ebooks/2591
6. https://www.gutenberg.org/ebooks/1597
7. https://www.gutenberg.org/ebooks/27200
 
