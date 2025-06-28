# 📰 Fake News Detection using NLP and Machine Learning

This project aims to detect fake news by applying various natural language processing (NLP) techniques and machine learning models. It involves cleaning the text data, visualizing word patterns, and evaluating models to classify news as **real** or **fake**.

---

## 📁 Dataset
- Dataset used: [Kaggle Fake News Dataset](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)
- The dataset includes:
  - `title`: Headline of the news article
  - `text`: Full content of the news
  - `label`: Target variable (1 = Fake, 0 = Real)

---

## 🧰 Technologies & Libraries
- **Python 3**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **NLTK**, **spaCy**
- **Scikit-learn**
- **WordCloud**

---

## 🧠 Project Workflow

### 1. Data Cleaning & Preprocessing
- Checked for missing and blank text entries
- Combined title and text into a single column
- Removed stopwords using both `nltk` and `spaCy`
- Cleaned special characters and converted text to lowercase

### 2. Exploratory Data Analysis (EDA)
- Plotted word clouds for both fake and real news
- Analyzed word frequency and patterns

### 3. Feature Extraction
- Used **TF-IDF Vectorization** to transform text into numerical features

### 4. Model Training & Evaluation
Trained the following models:
- Logistic Regression
- Naive Bayes
- Random Forest

Evaluation metrics:
- Accuracy Score
- Confusion Matrix
- Classification Report

---

## ✅ Results
- The best model achieved an accuracy of **99%** 
- Visual comparisons of performance were plotted

---

