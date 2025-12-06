# NLP
# NLP Feature Engineering for Sentiment Analysis

This project focuses on the rigorous data preparation and feature engineering steps necessary to build a machine learning model for sentiment classification using the **IMDB 50k Movie Review Dataset**.

## Goal
To transform raw text data into dense numerical features using classical Natural Language Processing (NLP) techniques.

## Methodology & Implementation

### 1. Preprocessing
The dataset of 50,000 movie reviews underwent extensive cleaning:
* **Text Normalization:** Lowercasing was applied across the entire corpus.
* **Noise Removal:** HTML tags and punctuation were removed.
* **Stop Word Filtering:** Common, non-informative English stop words were excluded during vectorization to focus on meaningful features.

### 2. Target and Feature Encoding

| Component | Technique Used | Description |
| :--- | :--- | :--- |
| **Target Variable (Sentiment)** | One-Hot Encoding (OHE) | Converted the categorical ('positive'/'negative') labels into binary vectors. |
| **Feature Extraction (Review Text)** | Count Vectorizer (BoW) & TF-IDF | Used to transform the cleaned text into numerical matrices. |

### 3. N-gram Analysis & Dimensionality

Feature matrices were generated using both simple counts (BoW) and weighted scores (TF-IDF) across various n-gram ranges:

* **Unigram:** Single-word features.
* **Bigram:** Two-word sequential features.
* **Trigram:** Three-word sequential features.

**Dimensionality Observation:** Extracting N-grams resulted in a vast expansion of the feature space. The vocabulary size grew to over **4.9 million unique features** when using Trigrams, underscoring the necessity of using sparse matrix representation for efficiency.
