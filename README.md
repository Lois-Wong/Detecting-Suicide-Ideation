### Using Text Classification to Detect Suicide Ideation 

**Lois Wong**

#### Executive summary

**Project overview and goals:** The goal of this project is to identify better ways to detect people who are at risk for suicide by identifying and evaluating the best model for detecting suicide ideation in social media posts. W will be training and tuning four binary text classification models to accurately classify social media posts as suicidal or non-suicidal. Models will be able to predict, from future/unseen posts, whether their writer is at risk for suicide. We will then evaluate and compare the four models' performances to identify the best one, then further scrutinize it to find the most effective features (words) that enhance performance in this classification task. We will draw insights from this model by conducting a global analysis, using the ELI5 and LIME libraries identify the most important words/features used for making accurate predictions. We will also be locally analyzing this model and evaluating its class prediction process for individual posts. Lastly, we will draw insights from our analyses and recommmend areas to research and courses to undertake for future work in detecting suicide ideation.  


**Findings:** The best model for detecting suicide ideation is the Support Vector Classifier model, with an accuracy score of 0.924, a recall of 0.916, and an F-1 of 0.924. Its performance is followed by the Logistic Regression model, Naive Bayes model, and the Decision Tree model. This decision is based off comparing the finetuned models' accuracy, recall, and F1 scores (results summary below). The SVC model has the best accuracy (0.924), the Naive Bayes model has the best recall (0.955), and the SVC model has the best F1 score (0.924). As for the errors of each model, Logistic Regression has nearly twice as many FN (false negatives) as FP (false positives); Naive Bayes has nearly four times as many FP as FN; Decision Tree has similar FP and FN counts with slightly more FN, and SVC has slightly more FN than FP. 

[![Model-Scores.png](https://i.postimg.cc/tJKbRcwv/Model-Scores.png)](https://postimg.cc/30FVntK2)


**Conclusion and key takeaways:** Our evaluation of the best model returns a list of words associated with their feature importance, or how helpful/unhelpful they were in the classification task. A global model analysis revealing the most effective (stemmed) words to detect [+ suicide] across the entire data shows the top five features to be ["suicid", "kill", "end", "pill", "life"] (results below).

[![Model-Feature-Weights.png](https://i.postimg.cc/XqqF6syz/Model-Feature-Weights.png)](https://postimg.cc/BPWtxcpT)

A local model analysis consisting of two example predictions (one suicide, one non-suicide) returns the most prominent features of those individual posts in the class decision. 

Image (below): Feature weights of a non-suicidal post prediction 

[![Non-Suicidal-Example.png](https://i.postimg.cc/261qyV2H/Non-Suicidal-Example.png)](https://postimg.cc/S2pQtN08)

Image (below): Feature weight of a suicidal post prediction. A dark green highlight indicates substantial importance in the prediction while dark red indicates negative importance, or the word reduces the prediction value/increases the loss. 

[![Suicidal-Example.png](https://i.postimg.cc/D0D81FY2/Suicidal-Example.png)](https://postimg.cc/QKQ83L3P)


**Future research and development:** Comparing the two feature values shows an interesting dichotomy in the feature importance assigned "feel". It has a high positive score in classifying our first post as non-suicidal and a negative importance in classifying our second post as suicidal. This gives way to a theory that the absense of certain words is a significant feature in gauging a post's non-membership of a class -- and in a binary classification problem, its membership of the second class. Because it is impossible for a person/post to be both or neither suicidal nor non-suicidal, saying that a post is not [suicidal] is synonymous with saying it is [not suicidal].

The best model score can also be extended by experimenting with or incorporating other algorithms and techniques, such as ensemble methods or recurrent neural networks. 

+ main points of the report 
+ recommendations   

#### Rationale

+ why you should care about this report / work
+ who should care / who is this relevant for 


Suicide is a leading cause of death in the US 


#### Research Question

The question this project aims to answer is what are the the best features and models/model parameters for detecting those at risk for suicide? 

The problem this project tries to solve is the growing rate of suicide. A lot undetected. Stick in statistics. On prevention and detection, starting with ideation. 





#### Data Sources

The dataset is sourced from Kaggle and can be accessed at https://www.kaggle.com/datasets/nikhileswarkomati/suicide-watch 

The data are a collection of posts collected from the 'SuicideWatch' and 'teenagers' subreddits from the Reddit platform using PushshiftAPI. Posts were created between 16 December 2008 - 2 January 2021. Social media posts collected from the 'SuicideWatch' subreddit are labelled 'suicide', while posts collected from 'teenagers' are labelled 'non-suicide'

+ data used to answer question: where and how sourced 
+ cleaning/preparation and why/why not
+ present final dataset (variables, distribution, visualizations)

#### Methodology

+ methods used and logic behind it / why
+ for each method, describe the model building process and rationale 

#### Results 

+ method results and how it answers the research question (one model at a time) 
+ evaluate your multiple methods and recommend one and why it's best 


#### Outline of project

+ add the evaluation

- [Link to notebook] (http://localhost:8888/lab/tree/Downloads/ML%20ipynb/Capstone/Capstone.ipynb) 

- [Link to download data] (http://localhost:8888/files/Downloads/ML%20ipynb/Capstone/SuicideDetection.csv?_xsrf=2%7C01e7821a%7C54dac168862e9a75a5e46c1d11d7822e%7C1658864864) 

- [Link to download notebook] (http://localhost:8888/files/Downloads/ML%20ipynb/Capstone/Capstone.ipynb?_xsrf=2%7C01e7821a%7C54dac168862e9a75a5e46c1d11d7822e%7C1658864864)


##### Contact and Further Information

Lois Wong
Email: lois@berkeley.edu 
LinkedIn: linkedin.com/in/lois-wong


