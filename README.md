# TweetsSentimentAnalysis

This README describes the various machine learning models used for the 2021S2 COMP90049 Assignment 3.

The data used for the models are based on the provided data-sets on tweets, with feature-engineering performed in the following format:

- {type} refers to either full, count, tfidf, glove100:
    full: This contains the raw text of the corresponding tweets, one tweet per line, in the following format:
          sentiment, tweet_id, tweet (newline)
          where sentiment is the class label (to be predicted), the tweet_id identifies the tweet, and the Tweet-text the raw tweet

    count: For these files, we have pre-processed the corresponding tweets, and have recorded the term frequency for a subset of words (filtered by tfidf)
                    
    tfidf: For these files, we have pre-processed the corresponding tweets, and have recorded the tfidf (term frequency inverse document frequency) value for a subset of words (pre-filtered by tfidf). 
    
    glove100: For these files, we have pre-processed the corresponding tweets, and have mapped each word to its pre-trained word embedding (GloVe) and summed the embeddings of all words in the tweet


The models used in the Jupyter Labs file is a Zero R baseline, Multinomial Naive Bayes, Logistic Regression, Multilayer perceptron, Decision Trees and Random Forests.


Sklearn is used to import the classifiers for these models, including the standard scaler for logistic regression, learning curves, and metrics to evaluate performance.
