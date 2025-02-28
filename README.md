# Sentiment Analysis of COVID-19 Tweets

This project involves developing a deep learning model to classify sentiments (positive, negative, neutral) in COVID-19-related tweets using NLP techniques.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Preprocessing](#preprocessing)
- [Model Architecture](#model-architecture)
- [Evaluation](#evaluation)
- [Results](#results)
- [Requirements](#requirements)
- [Usage](#usage)

## Introduction
The goal of this project is to analyze the sentiment of tweets related to COVID-19. We use a deep learning model with a bidirectional GRU layer to classify tweets into three categories: positive, negative, and neutral.

## Dataset
The datasets used are:
- `Corona_NLP_train.csv` (training data)
- `Corona_NLP_test.csv` (test data)

Both datasets are preprocessed to remove duplicates and NaN values.

## Preprocessing
The following preprocessing steps were applied:
1. Removing URLs, mentions, hashtags, digits, and HTML tags.
2. Simplifying sentiment categories (positive, negative, neutral).
3. Tokenizing text and padding sequences to ensure uniform length across the dataset.

## Model Architecture
The model consists of:
- Embedding layer
- Bidirectional GRU layer
- Global Average Pooling layer
- Dense layers with dropout for regularization

## Evaluation
The model is evaluated using precision, recall, and F1-score metrics on the validation data.

## Results
- **Training Accuracy:** 94.38%
- **Validation Accuracy:** 83.97%
- **Performance Metrics (Validation Data):**
  - Positive: Precision (0.85), Recall (0.82), F1-Score (0.83)
  - Negative: Precision (0.82), Recall (0.88), F1-Score (0.85)
  - Neutral: Precision (0.86), Recall (0.81), F1-Score (0.83)
  - Overall accuracy: 84%

## Requirements
- NLTK
- BeautifulSoup
- Keras
- TensorFlow
- Sklearn
- Matplotlib
- Seaborn

Install the required libraries using:
```bash
pip install nltk beautifulsoup4 keras tensorflow scikit-learn matplotlib seaborn
