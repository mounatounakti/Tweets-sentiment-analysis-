# Tweets Sentiment Analysis – Mini Project
This mini project focuses on performing sentiment analysis on tweets by classifying them as **complaints** or **non-complaints** using machine learning techniques.

---

## Steps Followed

### 1. Data Preparation
- Imported two datasets:
  - One containing **complaint tweets**
  - One containing **non-complaint tweets**
- Created a new column named `target`:
  - Complaint tweets → `target = 0`
  - Non-complaint tweets → `target = 1`
- Concatenated both datasets into a single DataFrame

---

### 2. Text Cleaning and Preprocessing
Applied regular expressions to clean the tweets by:
- Removing URLs
- Removing `@` mentions
- Removing `#` hashtags
- Removing HTML tags
- Removing non-alphabetic characters
- Removing extra spaces

**Note:**  
Uppercase letters were kept because they may carry useful sentiment information.

---

### 3. Train–Test Split
- Split the dataset into (80% train & 20% test)

---

### 4. Text Encoding
- Converted tweets (`X_train` and `X_test`) into numerical features using TF-IDF Vectorization

---

### 5. Model Training
- Trained a Multinomial Naive Bayes classifier on the training data

---

### 6. Model Evaluation
- Evaluated the model using `accuracy`
- Achieved an accuracy score of `0.71`

---

## Possible Improvements to Increase Accuracy
- Apply lemmatization
- Tune TF-IDF parameters
- Try other ML models and compare results
- Test other word embeddings (Word2Vec, GloVe, or BERT)
