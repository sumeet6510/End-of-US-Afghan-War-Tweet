# End-of-US-Afghan-War-Tweet
A project on sentiment analysis


### Index
#### 1. Introduction
#### 2. Exploratory Data Analysis
#### 3. Data Preprocessing
#### 4. Model Training
#### 5. Evaluation


# 1. Introduction

Our objective is to build a classification model to predict the sentiment of COVID-19 tweets.The tweets have been pulled from Twitter and manual tagging has been done then. The names and usernames have been given codes to avoid any privacy concerns.

### We are given the following information:

* UserLocation: Location of the user
* Date: Date at which tweet sent 
* text: The exact tweet
* polarity: range between -1 to +1 (for neutral it is 0)
* Sentiment: Sentiment of the tweet
* hashtags: hastags in tweet
* Source: From which device tweet sent

### Workflow in this Project

![Capture](https://user-images.githubusercontent.com/82259772/130586521-be05913c-1b2f-4a20-85f2-1982a833daeb.PNG)

# 2. Exploratory Data Analysis

* The original dataset has 7 columns and 362566 rows.

* There are three types of sentiments- Negative, Neutral, and Positive.


# 3. Data Preprocessing

* The preprocessing of the text data is an essential step as it makes the raw text ready for mining.

* The objective of this step is to clean noise those are less relevant to find the sentiment of tweets such as punctuation, special characters, numbers, and terms which don’t carry much weightage in context to the text.

* Stop words are those words in natural language that have a very little meaning, such as "is", "an", "the", etc.To remove stop words from a sentence, you can divide your text into words and then remove the word if it exits in the list of stop words provided by NLTK.

* Stemming is a rule-based process of stripping the suffixes (“ing”, “ly”, “es”, “ed”, “s” etc) from a word. For example – “play”, “player”, “played”, “plays” and “playing” are the different variations of the word – “play”.

* Lemmatization is a more powerful operation, and it takes into consideration morphological analysis of the words. It returns the lemma which is the base form of all its inflectional forms.

* In tokenization we convert group of sentence into token . It is also called text segmentation or lexical analysis. It is basically splitting data into small chunk of words. Tokenization in python can be done by python NLTK library’s word_tokenize() function


### After cleaning text we also create wordblog

![image](https://user-images.githubusercontent.com/82259772/144591527-5a8e03fe-d6c9-4202-994f-679c5f733a4c.png)


# 4. Model Training

Trained Logistic Regression, Xgboost, perceptron and Multinomial Naive Bayes algorithms.

# 5. Evaluation

### we got accuracy as - 
![image](https://user-images.githubusercontent.com/82259772/144591433-f2307aad-38ed-4039-8f92-f52df08f791f.png)



![Capture9](https://user-images.githubusercontent.com/82259772/130586434-d070da2a-18df-4d34-aa76-3d38a1e77a7c.PNG)

