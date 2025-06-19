# Twitter Sentiment Analysis

This project focuses on analyzing the sentiment of tweets using Natural Language Processing (NLP) techniques and a Logistic Regression model. It classifies tweets as either **Positive** or **Negative**, based on the textual content.

## 🚀 Project Highlights

- Cleaned and preprocessed a dataset of 1.6 million tweets
- Applied stemming and stopword removal to normalize text
- Used **TF-IDF Vectorization** to convert text into numerical features
- Trained a **Logistic Regression** model for binary classification
- Achieved strong accuracy on unseen tweets
- Built a function to predict sentiment for any custom tweet

---

## 🛠️ Technologies Used

- Python
- NLTK (for NLP preprocessing)
- Scikit-learn (for vectorization, modeling, and evaluation)
- Pandas & NumPy (for data manipulation)

---

## 📊 Dataset

Dataset: `training.1600000.processed.noemoticon.csv`  
- Total Tweets: 1.6 Million  
- Target Label:  
  - `0` = Negative  
  - `4` = Positive → converted to `1` for binary classification  
- Columns Used: `text`, `target`

---

## 🧪 Workflow

1. **Load Dataset**
2. **Preprocess Text**  
   - Lowercasing, special character removal  
   - Stopwords removal using `nltk.corpus`  
   - Stemming using `PorterStemmer`  
3. **Vectorization**  
   - `TfidfVectorizer` to transform text into numerical vectors  
4. **Split Data**  
   - 80% Train / 20% Test  
5. **Model Training**  
   - `LogisticRegression` classifier  
6. **Evaluation**  
   - Accuracy score on test set  
7. **Prediction Function**  
   - Custom tweet sentiment checker

---

## 🧠 Model Used

- **Logistic Regression**: A simple linear classifier suitable for binary sentiment classification tasks.

---

## 📌 Sample Predictions

```python
predict_sentiment("I hate you") ➝ Negative
predict_sentiment("I love you") ➝ Positive
