# Political messaging and user engagement in The Netherlands
Author: Erik Puijk <br>
Date: February 17, 2022

## Introduction
This repository contains all relevant code used in my Master's Thesis project about political messaging and user engagement. <br>
The thesis aims to gain more insight into the extent to which different messaging strategies by political parties engage users on social media. It does so by examining the messaging of political parties and party leaders on Twitter during the 2021 elections for the House of Representatives in The Netherlands.

## Technologies
- Python 3.6
- Jupyter Notebook

## Contents
### CreateUsers.ipynb
This notebook is used to create a text file containing all Twitter users that are analyzed in the thesis and other relevant information, such as the amount of followers for the user. The text file is used later on to retrieve Tweets.

### RetrieveTweets.ipynb
This notebook is used to retrieve Tweets using Twitter API. The users file created in CreateUsers.ipynb is used and the Tweets are written in JSON-format to a text file.

### Sampling.ipynb
This notebook is used to generate random samples given a text file of Tweets. It is used to divide the data sets into subsets to perform the methodology described in the thesis.

### Krippendorff.ipynb
This notebook is used to calculate Krippendorff's alpha given a csv-file of codings.
