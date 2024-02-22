# Positive and Negative Sentiment Prediction in Movie Reviews

This project aimed to predict the sentiment of movie reviews, whether positive or negative, using a dataset that was created based on the 5-star rating given by reviewers. We used **Supervised Machine Learning methods** because they have proven to be effective in Classification problems and also help new engineers understand the fundamental principles of Machine Learning. Our project was developed in a notebook style to enhance readability and was implemented in the Google Colab environment to avoid memory issues and ensure collaboration.

To predict the sentiment, we used **Support Vector Machine, Logistic Regression, and Bayesian Classification methods**, all of which achieved an accuracy rate above 75%.


We structured our project into the following main parts:

## 1. Preprocessing
We started by cleaning the data by removing html, urls, stop words, non-alphabetic characters, and upper case letters. We then corrected spelling and normalized the words using Stemming and Lemmatization techniques. Finally, we split the dataset into training and test sets and vectorized the words using CountVectorizer and TfidfVectorizer.

## 2. Data Understanding
We analyzed the dataset to help the models make more accurate predictions. We created graphs showing the most common words in the dataset as well as in positive and negative reviews, the most frequent bigrams, and sentimental words.

## 3. Support Vector Machine Model
We trained a Support Vector Machine Model with poly and linear kernel to determine whether our data was linearly separable. We found that Tfidf Vectorizer used with linear kernel gave accurate results in 88% of the cases.

## 4. Naive Bayes Model
We trained a Naive Bayes Model with and without Laplacian Smoothing to determine whether negative probabilities affected the predictions. We found that Tfidf Vectorizer used with smoothing gave accurate results in 75% of the cases.

## 5. Logistic Regression Model
We trained a Logistic Regression Model with and without L2 penalty to manage overfitting. We found that Tfidf Vectorizer used with L2 penalty gave accurate results in 86% of the cases.

## 6. Results Comparison
We compared the results of all the methods used and found that they were mostly accurate, with the SVM model being the most effective.

## 7. Future Work
Our future work will include analyzing falsely classified reviews (in terms of spelling, unrecognized words by the models, and other data patterns), testing with more review or general datasets, and omitting non-sentimental words in the preprocessing step.