# Twitter Sentiment Analysis
## Overview

This project performs sentiment analysis on Twitter data using Natural Language Processing (NLP) and Machine Learning techniques.
The project uses the Sentiment140 dataset and classifies tweets into positive and negative sentiments.

## Objective

The main objective of this project is to build a machine learning model that can analyze the sentiment expressed in a tweet.
The project covers:

- Twitter text preprocessing
- Stopword removal
- Stemming
- TF-IDF feature extraction
- Machine learning model training
- Model evaluation
- Sentiment prediction for new tweets

## Dataset

The project uses the **Sentiment140 dataset**, which contains 1.6 million tweets.
The target labels are converted into two sentiment classes:

- `0` → Negative
- `1` → Positive

## Technologies Used

- Python
- NumPy
- Pandas
- NLTK
- Scikit-learn
- Kaggle API
- Jupyter Notebook

## NLP Preprocessing

The tweet text is processed using the following steps:

1. Remove non-alphabetic characters.
2. Convert text to lowercase.
3. Split text into individual words.
4. Remove English stopwords.
5. Apply Porter Stemming.

## Feature Extraction

The preprocessed text is converted into numerical features using:

**TF-IDF (Term Frequency-Inverse Document Frequency)**

The TF-IDF vectorizer is fitted on the training data and then used to transform both training and testing data.

## Machine Learning Models

The project trains and compares three classification algorithms:

1. Logistic Regression
2. Bernoulli Naive Bayes
3. Linear Support Vector Machine (SVM)

The models are evaluated using accuracy scores.

A classification report is also generated for the Logistic Regression model.

## Model Saving

The trained Logistic Regression model is saved using Pickle as:

```text
trained_model.sav
