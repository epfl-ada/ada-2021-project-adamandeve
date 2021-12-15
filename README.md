# A COMMUNICATION CRISIS ? Inequalities in media representation through quotes


### ABSTRACT 

Whether we are aware of it or not, we are all assigned multiple social identities. Over the last few years, many revolutionary movements have become more and more important in our society regarding gender equality, racism or even overall discrimination against groups. Is this evolution reflected in the press ? 


We will analyse the stakes of this question based on the Quotbank dataset. Indeed, we can regroup the main different topics appearing in the press and find the social and cultural background of the most influential speakers that are quoted for each topic. This would underlie which characteristics of the speaker the press considers to have the most chance to attract readers. Therefore, the possible evolution from 2015 until 2020 of the above findings can reveal the progression of our society regarding the representation of all cultural, social or gender identities through the voice they are given across different press sources. 


### RESEARCH QUESTIONS 

What are the most talked about topics in the press  over the years  ? 


Which topics have the most varied speakers in terms of nationality ? 


Are women as much quoted as men in the press ? Is there a significant evolution  from 2015 to 2020 ? 


What is the mean age of the speakers in each topic group ? Is there a significant evolution from 2015 to 2020? 


Is there an overrepresentation of a particular nationality in the press ? 


Does this mean age variates significantly according to the different topics ? 


Is there an overall difference across the news sources regarding the most represented type of population ? 


How did two of the most polarized news sources do in terms of diverse speakers? Did they do better or worse than expected in 2020?


Which of the two news sources made more progress in terms of diversity in the quoted speakers?

### PROPOSED ADDITIONAL DATASETS 

One additional data is necessary to carry out our project. We will need a dataset containing labeled text. For this we make use of the BBC news dataset available on Kaggle (https://www.kaggle.com/c/learn-ai-bbc/data). This dataset contains 2225 news articles each labeled with one of five categories: business, entertainment, politics, sport, or tech. The dataset is already broken down in the train and test set. We explored and cleaned the train data set.
Another additional dataset that we will use is the wikidata, which provides metadata about the speakers. From this metadata we extract information about the nationality and the gender of the speaker. Some lines of the metadata had to be dropped because either the gender or the nationality was not present.

### METHODS

The first step of our project will be to perform clusterization of quotations. We can systematize quotations based on the subject of discussion and split quotations into meaningful groups, such as business, entertainment, politics, sport and tech. So, the goal here is to perform clustering and assign each quote to a specific group based on its content. To do this, we will use the transfer learning paradigm - perform supervised learning - train a ML pipeline to classify a labelled dataset of BBC news and then apply this trained model to clusterize our quotes. As a Machine Learning method we will try different algorithms such as random forest, logistic regression, k neighbors classifier and naive bayes classifier in order to select the one giving the best performance. 
After clusterization we will perform analysis of our results using descriptive statistics. To do so, we will explore the distribution, compute the mean, variance, median and quartiles. We will also assess the significance of our results using p-value hypothesis testing. A regression analysis will be performed on the attributes of the speakers in order to reveal the possible correlation between them
In a final step, we will perform a linear regression to predict the proportion of underrepresented speakers in 2020. This mean that we will train our model on the quotes and speakers from 2015 to 2019, make a prediction of the proportion of quoted minorities and women and compare it to the actual proportions recorded for 2020. 

### PROPOSED TIMELINE 
26 november - 17 december 


##### TASK 1 : 30 November-5 December 

* reorganization of the data in groups of main topics using the BBC news Dataset

* visualization of the data (repartition of number of quotes for each group, evolution from 2015 )

 * statistical analysis : Is the difference of occurrence across the different subjects significant ?
 
 * analysis of the results :  the main spoken subject from 2015 until 2020 

##### TASK 2 : 5-10 December 

* categorization of the speakers regarding : gender (female or male) , age (18-30, 30-50, > 50), nationality using Wikidata 
* find occurrence within each category of speaker from 2015 to 2020  
* Classify across the different news sources 
* visualization of the data : curve evolution of mean age of speaker for each topics + across news sources / evolution of the main represented nationalities for the different news sources /  representation of the main represented speaker characteristics across time 
* statistical analysis : Is there a correlation between represented population (age and nationality) and news sources / Is the evolution from 2015 to 2020 of the main represented speaker for each topic significant ? 
* Analysis of the results 

##### TASK 3 : 10-14  December
 
* overall analysis of the results : accuracy, meaning, consequences

##### TASK 4 : 14-17 December 
* writing of the Data Story 
* update of the ReadME file 
* cleaning of the code 

 ### ORGANISATION WITHIN THE TEAM 

##### TASK 1 : Training of the machine learning model

* Training of multiple models : Justine 
* analysis of the results :  Justine 


###### TASK 2 : Generation of labels for QuoteBank Dataset 
* Assessment of doc2vec and TFiDF matrix: Filippo
* Application of logistic regression model : Filippo 
* Classify across the different news sources (and demographic groups) : Filippo 
* visualization of the data : Filippo 


##### TASK 3 : Categorization of the speakers
* Age analysis: Fanny
* Gender analysis: Justine
* Nationality analysis: Filippo
* overall analysis of the results: Justine, Fanny, Filippo

##### TASK 4 : Prediction for the main two news sources with distinct political bias
* Age, gender and nationality predictions: Fanny and Filippo

##### TASK 5 : Presentation and Data story
* writing of the Data Story  : Kseniia 
* Presentation of notebook: Fanny
* update of the ReadME file :  Justine
* cleaning of the code : Justine, Fanny





