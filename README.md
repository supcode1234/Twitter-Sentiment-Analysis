# Twitter Sentiment-Analysis

## Overview
This repository contains a **Twitter sentiment analysis project** using classical machine learning models. The goal is to classify tweets into four sentiment categories: **Positive, Negative, Neutral, and Irrelevant**. The project includes full preprocessing, feature extraction, model training, evaluation, and saving the final model for deployment.

---

## Dataset
The dataset used for this project is taken from [Kaggle: Twitter Entity Sentiment Analysis](https://www.kaggle.com/datasets/jp797498e/twitter-entity-sentiment-analysis).

- **Training set:** `twitter_training.csv`  
- **Validation set:** `twitter_validation.csv`  
- **Columns:**  
  - `ID` → Tweet ID  
  - `Topic` → Topic of the tweet  
  - `Sentiment` → Sentiment label (Positive, Negative, Neutral, Irrelevant)  
  - `Text` → Original tweet text  

---

## Features & Preprocessing
1. **Text Cleaning**
   - Lowercasing, HTML decoding
   - Remove URLs, mentions (@user), hashtags, emojis, and special characters
   - Tokenization, stopwords removal, lemmatization

2. **Label Encoding**
   - Convert sentiment labels into integers for model training

3. **Feature Extraction**
   - TF-IDF vectorization with unigrams and bigrams
   - Max features: 10,000  

---

## Models Used
- Logistic Regression  
- Multinomial Naive Bayes  
- Decision Tree  
- Random Forest (**final model**)  
- Linear SVM  

**Evaluation metrics:** Accuracy, Precision, Recall, F1-score, Confusion Matrix, ROC Curve  

**Final Model:** Random Forest with 200 estimators trained on the full dataset.  

---
