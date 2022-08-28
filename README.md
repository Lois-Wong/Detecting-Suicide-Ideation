### Detecting Suicide Ideation from Social Media Posts  

**Lois Wong**

#### Executive summary
<> <><>><><><<>><><><><<><><>><><>><>><><><><

#### Rationale
<> <><>><><><<>><><><><<><><>><><>><>><><><><


"There is only one really serious philosophical problem and that is suicide" -- Albert Camus 

Suicide is a leading cause of death in the US 


#### Research Question
What are the the best features and model parameters for detecting those at risk for suicide? 


### Project Description

**Goal:** The goal of this project is to identify better ways to detect people who are at risk for suicide. 

To detect suicide ideation, we will be training and tuning several binary text classification models to group social media posts into suicidal vs non-suicidal classes. Models will be able to predict, from future/unseen posts, whether their writer is at risk for suicide. We will assess model performance and further scrutinize the predictive models to find the optimal features and parameters for this classification task, then identify measures to more effectively detect suicide ideation. 


**Data Overview ** 

The dataset is sourced from Kaggle and can be accessed at https://www.kaggle.com/datasets/nikhileswarkomati/suicide-watch 

The data are a collection of posts collected from the 'SuicideWatch' and 'teenagers' subreddits from the Reddit platform using PushshiftAPI. Posts were created between 16 December 2008 - 2 January 2021. Social media posts collected from the 'SuicideWatch' subreddit are labelled 'suicide', while posts collected from 'teenagers' are labelled 'non-suicide'



### Methodology

### Findings

**Stemmed Data Results**

Logistic Regression has the highest accuracy (0.894) followed by SVC (0.888) and Decision Tree (0.768)

Naive Bayes has the highest recall (0.946) followed by SVC (0.897) and Logistic Regression (0.896)

Logistic Regression has the highest F1 score (0.892) followed by SVC (0.889) and Naive Bayes (0.837)

**Lemmatized Data Results**

Logistic Regression has the highest accuracy score of 0.896, followed by SVC (0.886) and Naive Bayes (0.812)

Naive Bayes has the highest recall score of0.944, followed by SVC (0.903) and Logistic Regression (0.877)

Logistic Regression has the highest F1 score of 0.894, followed by SVC (0.887) and Naive Bayes (0.833)

**Comparing Stemming vs Lemmatization**

The biggest difference between stemming and lemmatizing is the training time: stemming is significantly faster than lemmatizing. The optimal max_features value is the same as with the lemmatized data; 3000 is the best number for every model except KNN. 

The accuracy scores of the Naive Bayes estimator is significantly higher when trained on lemmatized data. Other models' accuracy scores are similar: lemmatized data resulted in higher accuracy scores for KNN, Decision Tree, and Logistic Regression while stemmed dated resulted in higher accuracy for SVC and Naive Bayes. 

Lemmatized data resulted in higher recall for KNN, Decision Tree, and SVC while stemmed data resulted in higher recall for Naive Bayes; Logistic Regression has the same recall score for both stemmed and lemmatized data.

Lemmatized data resulted in higher F1 for KNN, Decision Tree, and Logistic Regression while stemmed data resulted in higher F1 for Naive Bayes and SVC.

**Overall**, the top models for accuracy are Logistic Regression + lem (0.896), SVC + stem (0.888), and Naive Bayes + lem (0.812)

The top models for recall are Naive Bayes + stem (0.946), SVC + lem (0.903), and Logistic Regression + lem (0.877)

The top models for F1 are Logistic Regression + lem (0.894), SVC + stem (0.889) and Naive Bayes (0.837)

- The Logistic Regression model has more false negatives than false positives 
- The Naive Bayes model has significantly more false positives than false negatives
- The Decision Tree model has more false positives than false negatives
- The SVC model has slightly more false positives than false negatives 
- The KNN model has significantly more false negatives than false positives

### Next Steps and Recommendations 



#### Outline of project

- [Link to notebook] (http://localhost:8888/lab/tree/Downloads/ML%20ipynb/Capstone/Capstone.ipynb) 

- [Link to download data] (http://localhost:8888/files/Downloads/ML%20ipynb/Capstone/SuicideDetection.csv?_xsrf=2%7C01e7821a%7C54dac168862e9a75a5e46c1d11d7822e%7C1658864864) 

- [Link to download notebook] (http://localhost:8888/files/Downloads/ML%20ipynb/Capstone/Capstone.ipynb?_xsrf=2%7C01e7821a%7C54dac168862e9a75a5e46c1d11d7822e%7C1658864864)


##### Contact and Further Information
Email: lois@berkeley.edu 

