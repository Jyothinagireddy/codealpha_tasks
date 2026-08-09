# Twitter Sentiment Analysis Using Machine Learning

## 📌 Project Overview

This project performs sentiment analysis on Twitter data using Machine Learning.

The objective is to classify tweets into two sentiment categories:

- **0 → Negative**
- **1 → Positive**

The project follows a complete Machine Learning workflow including data preprocessing, text feature extraction, model training, evaluation, comparison, and model saving.

---

## 🎯 Problem Statement

Social media platforms contain a large amount of textual data expressing people's opinions and emotions.

Manually analyzing millions of tweets is difficult and time-consuming. This project uses Machine Learning and Natural Language Processing techniques to automatically classify tweets based on their sentiment.

---

## 📊 Dataset

The dataset contains **1,600,000 labeled tweets**.

The original target labels were converted into binary sentiment classes:

- `0` → Negative
- `4` → Positive

The positive label `4` was mapped to `1` for binary classification.

### Class Distribution

| Sentiment | Number of Tweets |
|-----------|------------------:|
| Negative (0) | 800,000 |
| Positive (1) | 800,000 |
| **Total** | **1,600,000** |

The dataset is therefore balanced between the two sentiment classes.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Natural Language Processing (NLP)
- Jupyter Notebook
- Pickle

---

## 🔄 Project Workflow

The project follows these major steps:

1. Load the Twitter dataset
2. Explore the dataset
3. Analyze the target distribution
4. Convert sentiment labels into binary classes
5. Preprocess the text data
6. Split the dataset into training and testing sets
7. Convert text into numerical features
8. Train Machine Learning models
9. Evaluate model performance
10. Compare the models
11. Save the trained model using Pickle

---

## 🤖 Machine Learning Models

Three Machine Learning algorithms were implemented and compared:

### 1. Logistic Regression

A linear classification algorithm used as one of the primary models for binary sentiment classification.

### 2. Bernoulli Naive Bayes

A probabilistic classification algorithm suitable for binary/feature-based text classification.

### 3. Linear Support Vector Machine

A linear SVM classifier used to identify the decision boundary between positive and negative sentiment classes.

---

## 📈 Model Performance

The models were evaluated using test data.

| Model | Test Accuracy |
|-------|--------------:|
| Logistic Regression | **76.67%** |
| Bernoulli Naive Bayes | **76.48%** |
| Linear SVM | **76.97%** |

### Best Performing Model

Based on test accuracy, **Linear SVM achieved the highest accuracy of 76.97%** among the three evaluated models.

Logistic Regression achieved a very close accuracy of **76.67%**.

---

## 📋 Logistic Regression Classification Report

The Logistic Regression model achieved approximately **78% F1-score** across both sentiment classes.

| Class | Precision | Recall | F1-Score |
|------|----------:|-------:|---------:|
| Negative (0) | 0.79 | 0.76 | 0.77 |
| Positive (1) | 0.77 | 0.80 | 0.78 |

### Overall Performance

- **Accuracy:** ~78%
- **Macro Average F1-score:** ~0.78
- **Weighted Average F1-score:** ~0.78

---

## 💾 Model Saving

The trained Machine Learning model is saved using Python's `pickle` module.

This allows the trained model to be reused later without retraining it from scratch.

The saved models are stored inside the `models/` directory.

---

## 📁 Project Structure

```text
Sentiment_Analysis_Python/
│
├── models/
│   └── Saved Machine Learning Models
│
├── twitter_sentiment_analysis.ipynb
├── requirements.txt
└── README.md
