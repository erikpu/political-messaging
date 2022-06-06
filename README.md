# Political messaging and user engagement in The Netherlands
Author: Erik Puijk <br>
Date: February 17, 2022

## Introduction
This repository contains all relevant code used in my Master's Thesis project about political messaging and user engagement. <br>
The thesis aims to gain more insight into the extent to which different messaging strategies by political parties engage users on social media. It does so by examining the messaging of political parties and party leaders on Twitter during the 2021 elections for the House of Representatives in The Netherlands.

## Technologies
- Python 3
- Pip3
- Jupyter Notebook
- Scikit Learn

## Contents
### CreateUsers.ipynb
This notebook is used to create a text file containing all Twitter users that are analyzed in the thesis and other relevant information, such as the amount of followers for the user. The text file is used later on to retrieve Tweets.

### Krippendorff.ipynb
This notebook is used to calculate Krippendorff's alpha given a csv-file of codings.

### MergeAnnotations.ipynb
This notebook is used to merge a list of annotated Tweets (either annotated manually or automatically) with the JSON-formatted file that contains all the data about the Tweets.

### ModelTuning.ipynb
This notebook is used to find optimal parameters for the classification model. It uses k-fold cross validation to test various parameters to select an appropriate model for classifying Tweets.

### PreProcessing.ipynb
This notebook is used to pre-process the Tweets to prepare them for generating features for the machine learning algorithm.

### Results.ipynb
This notebook is used to visualize results based on the classified Tweets. The average engagement per messaging strategy is provided in table format. Also, the number of Tweets and average engagement per week can be visualized for all or a selection or parties. The use of messaging strategies per week can also be visualized for all or a selection of parties.

### RetrieveTweets.ipynb
This notebook is used to retrieve Tweets using Twitter API. The users file created in CreateUsers.ipynb is used and the Tweets are written in JSON-format to a text file.

### Sampling.ipynb
This notebook is used to generate random samples given a text file of Tweets. It is used to divide the data sets into subsets to perform the methodology described in the thesis.

### TweetClassification.ipynb
This notebook is used to classify the remaining (unlabeled) Tweets using the optimal model found in ModelTuning.ipynb.

## Getting started
1. Use CreateUsers.ipynb to create a local document containing user data for Tweet collection.
2. Use RetrieveTweets.ipynb to collect and format the Tweets.
3. Use Sampling.ipynb to create samples for the gold-standard dataset and intercoder reliability.
4. Use Krippendorff.ipynb to verify intercoder reliability.
5. Use PreProcessing.ipynb to pre-process the Tweets in preparation for machine learning.
6. Use MergeAnnotations.ipynb to merge manual annotations for the gold-standard dataset with the Tweet dataset.
7. Use ModelTuning.ipynb to find optimal parameter values for classifying Tweets using the gold-standard dataset.
8. Use TweetClassification.ipynb to classify the remaining (unlabeled) Tweets with the optimal model.
9. Use Results.ipynb to visualize the results for the selection of parties you wish to see.
