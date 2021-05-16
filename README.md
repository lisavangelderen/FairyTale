# Gender Biases in Fairytales 

# Abstract

Fairy tales can give children important lessons about life and the world that they live in and are mostly viewed as such. In the western world one is unlikely to find a single person that does not know the story of Snow White and many of the other famous fairy tales. These stories however often contain messages about gender roles, even though these messages might be based on outdated stereotypes (Lieberman). A lot of children grow up hearing fairy tales before bed, or they learn reading by virtue of fairy tales. As such, these stories can have a big impact on the forming of opinions in young children (Wardetzky). We map and visualize the gender bias found in fairy tales by analyzing a corpus of European fairy tales written largely by the brothers Grimm (Aho, 2010). Using bi-grams, n-grams, a ppmi space and a Gensim Word2Vec model to show that gender bias exists on multiple levels in most fairy tales. Not only are women represented mostly as passive agents that require male characters to drive them forward, we show that female characters are largely characterized by their outward appearance instead of personality.


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

In addition to the above mentioned dataset, a dataset that we assembled ourselves with stories has also been used. This can be found in the andersongrimm.txt file. The stories in that file come from project Gutenberg. 

# A tentative list of milestones for the project

* Milestone 1

To start we will do some further preprocessing (possibly removing some tokens), collect the stories in a way that makes them easy for us to use (right now the files are organised in a way that is not too user friendly, making some rearrangements and making sure we only take into account the lemmatized tokens, not the un-lemmatized ones.), and decide on different methods to answer our questions (we could look at the correlations of certain tokens with gender roles, or train a model to predict a word associated with a gender role).
Then we will make a new timeline according to our reorganisation and plans on how to tackle the problems at hand.

* Milestone 2

See issue: "update 1" 

* Milestone 3

See issue: "project update 2" 


# Personal contributions

* Alexia

Data preprocessing, finding sources

* Lisa 

Data exploration, generating small texts, creating extra dataset, ngram model and analysis

* Victor 

Building/writing paper, building powerpoint

* Zoë

training model, making visual representations

* Everyone

Maintaining repository, working out conceptual ideas, presentation, paper, milestones



# Documentation

The repo is quite self-explanatory, in the readme all the required information for the project can be found. 
* The code is all in 1 jupyter notebook, codefile.ipynb, in here the all the code for the project can be found neatly organized and explained.
* The data used by the code is in the data file, the code extracts it from the different clusters.
* The extra dataset can be found in andersongrimm.txt
* The paper is written in LateX and can be found in the paper folder as a pdf, the LateX form can also be found here. Our paper is slightly longer than the the maximum 4 pages as we are with an extra individual in our group. 
* The presentation can be found in the presentation folder and only holds a pptx file containing the slides. This is the only folder that is updated after the 16th of may.

# Sources

* Baker-Sperry, Lori and Liz Grauerholz. 2003. The Pervasiveness and Persistence of the Feminine Beauty Ideal in Children’s Fairy Tales. Gender and Society, pp. 711-726
* Lieberman, M.R. 1972. ””Some Day My Prince Will Come”: Female Acculturation through the Fairy Tale.”. College English. vol. 34, no.3, p.383 
* Marshall E. 2004d. The Daughter’s Disenchantment: Incest as Pedagogy in Fairy Tales and Kathryn Harrison’s “The Kiss.”. College English, 66(4), 403–426.
* Meland, Aud T. 2020 Challenging gender stereotypes through a transformation of a fairy tale Challenging gender stereotypes through a transformation of a fairy tale.. European Early Childhood Education Research Journal. 28. 
* Neikirk, A. 2013. ””...Happily Ever After” (or What Fairy Tales Teach Girls About Being Women”. Anthropology, 38-42. 
* Vaz Lobo, Paula and de Matos, David M. 2010. Fairy Tale Corpus Organization Using Latent Semantic Mapping and an Item-to-item Top-n Recommendation Algorithm. European Language Resources Association (ELRA), Malta. 
* Wardetzky, K. 1990. The Structure and Interpretation of Fairy Tales Composed by Children. The Journal of American Folklore. The Journal of American Folklore, 103(408), 157–176. 
* Weingart, Scott and Jorgensen, Jeana. 2013. Computational Analysis of the Body in European Fairy Tales. Literary and Linguistic Computing/ (2013): 404-416. 
* https://www.gutenberg.org/ebooks/2591
* https://www.gutenberg.org/ebooks/1597
* https://www.gutenberg.org/ebooks/27200
 
