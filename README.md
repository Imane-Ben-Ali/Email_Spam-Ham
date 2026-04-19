# Email_Spam-Ham
# 📧 Spam Email Detection using NLP

## 📌 Project Overview

This project builds a **Spam Email Classifier** using Natural Language Processing (NLP) and Machine Learning.

The model processes raw email text and classifies it as:

* **SPAM (1)**
* **HAM (0)**

---

## ⚙️ Technologies Used

* Python 🐍
* Pandas
* NLTK
* Scikit-learn

---

## 🔍 Pipeline

### 1. Data Preparation

* Custom dataset of emails (spam & ham)
* Labels:

  * `1` → Spam
  * `0` → Ham

---

### 2. Text Preprocessing

* Lowercasing
* Removing:

  * URLs
  * HTML tags
  * Numbers
  * Punctuation
* Tokenization (NLTK)
* Stopwords removal
* Stemming & Lemmatization

---

### 3. Feature Extraction

* Bag of Words (CountVectorizer)
* TF-IDF (TfidfVectorizer)
* N-grams (Unigrams + Bigrams)

---

### 4. Models Used

* Naive Bayes (MultinomialNB)
* Logistic Regression

---

### 5. Evaluation

* Train/Test Split (70% / 30%)
* Metrics:

  * Precision
  * Recall
  * F1-score

---

## 🚀 Example Prediction

```python
text = ["FREE iphone click now to claim your reward"]

text_vect = vectorizer.transform(text)
prediction = model.predict(text_vect)

print("SPAM" if prediction[0] == 1 else "HAM")
```

---

## 📊 Output Example

* Spam messages correctly identified based on keywords like:

  * "FREE"
  * "Click now"
  * "Reward"

---

## 📁 Project Structure

```
spam-classifier/
│── main.py
│── README.md
│── requirements.txt
```

---

## 📦 Installation

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

```bash
python main.py
```

---

## 💡 Future Improvements

* Use larger real-world dataset
* Try Deep Learning (LSTM, BERT)
* Deploy as a web app

---

## 👩‍💻 Author

Imane Ben Ali
