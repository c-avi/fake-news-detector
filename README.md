## 📰 Fake News Detection using NLP & Machine Learning

This project aims to classify news articles as **Real** or **Fake** using Natural Language Processing (NLP) techniques and a supervised ML model (**LinearSVC**). The pipeline includes data preprocessing, feature extraction using **TF-IDF**, and model evaluation.

---

### 📂 Dataset

* **Source**: [Fake and Real News Dataset on Kaggle](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)
* Two CSV files:

  * `Fake.csv`
  * `True.csv`

---

### 🔧 Technologies Used

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* NLTK, spaCy, WordCloud
* Scikit-learn (TF-IDF, LinearSVC, Pipeline)
* **SQLite3 (SQL Integration)** ✅
* Jupyter Notebook / Kaggle Kernels

---

### 🚀 Steps Performed

1. **Data Cleaning**

   * Removed duplicates and blank text entries
   * Cleaned text using regex, lemmatization, and stopword removal

2. **Data Visualization**

   * Countplots of fake vs true news and subjects
   * Word clouds using `WordCloud` and custom image masks (thumbs-up for real, skull for fake)

3. **Feature Extraction**

   * Used `TfidfVectorizer` for vectorizing cleaned text

4. **Model Building**

   * Used `LinearSVC` with 99%+ accuracy
   * Trained and evaluated using `train_test_split`

5. **SQL Integration** ✅

   * Created an SQLite database: `fake_news.db`
   * Stored:

     * Cleaned dataset in `news_data` table
     * Model predictions (text, actual, predicted category) in `model_predictions` table
   * Used `sqlite3` and `pandas.to_sql()` for seamless storage and retrieval

---

### 📈 Results

* Achieved **\~99.3% accuracy** on test data
* High precision, recall, and F1-score for both real and fake classes
* All predictions and original data are saved in SQL tables for further querying and analytics




