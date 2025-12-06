# NLP
*This project prepared the $\mathbf{IMDB \ 50k \ Movie \ Review}$ dataset for a sentiment classification task.
*The primary steps involved were:
    * **Data Preparation:** The $\mathbf{50,000}$ text reviews were cleaned through lowercasing, removal of HTML tags, and removal of punctuation.
    * **Target Encoding:** The categorical $\mathbf{sentiment}$ column was converted using One-Hot Encoding (OHE) to prepare the target variable for machine learning.
    * **Feature Extraction(Vectorization):** The cleaned text was transformed into numerical feature vectors using N-gram models:
       * **Bag-of-Words (BoW):** Used to extract raw counts of Unigrams, Bigrams, and Trigrams.
       * **N-gram Dimensionality:** The vocabulary size was observed to increase dramatically, resulting in over $\mathbf{4.9 \text{ Million}}$ features when extracting Trigrams.
       * **N-gram Dimensionality:** The vocabulary size was observed to increase dramatically, resulting in over $\mathbf{4.9 \text{ Million}}$ features when extracting Trigrams.
