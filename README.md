# IMDB sentiment analysis with Word2Vec (Kaggle) 

Project Created at Sep. 2020

[task link](https://www.kaggle.com/c/word2vec-nlp-tutorial/data)

> Use Google's Word2Vec for movie reviews

Data Set: <br>
* The labeled data set consists of 50,000 IMDB movie reviews, specially selected for sentiment analysis. <br>
* The sentiment of reviews is binary, meaning the IMDB rating < 5 results in a sentiment score of 0, and rating >=7 have a sentiment score of 1.<br>
* No individual movie has more than 30 reviews. The 25,000 review labeled training set does not include any of the same movies as the 25,000 review test set. <br>
* In addition, there are another 50,000 IMDB reviews provided without any rating labels.

Task: 

Method 1. Predict labeded Data by BOW, tf-idf and MultinomialNB.

    a. check basic info of dataset
    b. data cleaning with stopwords (use NLTK)
    c. Build model by CountVectorizer and MultinomialNB (use GridsearhCV and Pipline)
    d. Build model by TfidfVectorizer and MultinomialNB (use GridsearhCV and Pipline)
    e. Kaggle data submission

Method 2. Use Word2Vec and Tree-based models to do prediction.

    a. Train Word2Vec model by unlabeled data
    b. Turn labeled reviews data into vectors by trained Word2Vec model
    c. Fit the vector data by GBDT and do prediction.
    d. Fit the vector data by XGboost and do prediction.
    e. Kaggle data submission

#### Kaggle submission result

![subsmission result](result/word2vec_reviews.jpg)