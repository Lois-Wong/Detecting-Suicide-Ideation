## Detecting Suicide Ideation from Social Media Posts  


### Project Description

**Research Question**: What are the best features and model parameters for detecting those at risk for suicide? 

**Goal:** The goal of this project is to identify how to best detect those at risk for suicide. I will be comparing the performance of different classification algorithms by training several models (Naive Bayes, Logistic Regression, and Decision Trees) to detect suicide ideation from social media posts. After comparing model performance, we will further scrutinize the best classification model to **identify the features and parameters which most effectively predict whether a user is at risk for suicide**.

**Data Overview**: The dataset is sourced from Kaggle and can be accessed at https://www.kaggle.com/datasets/nikhileswarkomati/suicide-watch 

The data are a collection of posts collected from the 'SuicideWatch' and 'teenagers' subreddits from the Reddit platform using PushshiftAPI. Posts were created between 16 December 2008 - 2 January 2021. Social media posts collected from the 'SuicideWatch' subreddit are labelled 'suicide', while posts collected from 'teenagers' are labelled 'non-suicide'


**Data Problem**: The data task is to train and tune multiple binary text classification models that group social media posts into suicidal vs non-suicidal. Models with high accuracy can be used to predict, from future/unseen posts, whether their writer is at risk for suicide. Further scrutinizing the most important features and parameters which compose the best model will indicate better ways to detect suicide risk. 

### Motivation

This project is completed to fulfill the requirements of UC Berkeley's Professional Certificate in Machine Learning and Artificial Intelligence.

### Findings

Logistic Regression + TF-IDF vectorization has the highest accuracy score, out-performing the Naïve Bayes and Decision Tree algorithms. 


### Next Steps and Recommendations 



### Access
Link to Notebook
Part I: http://localhost:8888/lab/tree/Downloads/ML%20ipynb/Capstone/Capstone.ipynb


Link to Download 
Data: http://localhost:8888/files/Downloads/ML%20ipynb/Capstone/SuicideDetection.csv?_xsrf=2%7C01e7821a%7C54dac168862e9a75a5e46c1d11d7822e%7C1658864864

Part I: http://localhost:8888/files/Downloads/ML%20ipynb/Capstone/Capstone.ipynb?_xsrf=2%7C01e7821a%7C54dac168862e9a75a5e46c1d11d7822e%7C1658864864

