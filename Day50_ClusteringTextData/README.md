# 📊 Text Clustering Using K-Means and Hierarchical Clustering

## 🧠 Objective

The goal of this project is to **cluster text data** (tweets) using unsupervised learning techniques, primarily **K-Means** and **Hierarchical Clustering**. We aim to group similar tweets together and visualize topic patterns using dimensionality reduction and interactive visualizations.

---

## 📂 Dataset

- **Source**: Real-world dataset of tweets
- **Columns**:
  - `id`: Unique identifier
  - `label`: (Optional) Sentiment or category label
  - `tweet`: The tweet content to be clustered

---

## 🔧 Steps Performed

### 1. Preprocessing
- Removed URLs (`http`, `https`, `www`)
- Removed special characters and punctuations
- Converted text to lowercase
- Removed stopwords
- Applied stemming using `PorterStemmer`

### 2. Vectorization
- Used `CountVectorizer` to convert text into numerical features

### 3. Clustering
- Applied **K-Means Clustering** to group similar tweets
- Also performed **Hierarchical Clustering** and visualized dendrograms

### 4. Dimensionality Reduction
- Used **PCA** (Principal Component Analysis) to reduce feature dimensions to 2D for plotting

### 5. Visualization
- Interactive 2D scatter plots with `Plotly` to explore clusters and distribution

---

## 📈 Visual Results

- **K-Means Clusters** visualized using PCA components
- Color-coded clusters show separation of tweet themes
- Dense and sparse clusters suggest both common and rare topics

---

## 📌 Key Insights

- Tweets were successfully grouped into semantically similar clusters
- PCA helped us interpret high-dimensional text data
- K-Means performed well; some overlapping areas may benefit from deep embedding or topic modeling

---

## ✅ Conclusion

This project showcases how to apply unsupervised machine learning to raw text data and uncover **hidden structures**. The combination of text cleaning, clustering, and visualization delivers a powerful toolset for **document organization, topic discovery, and content exploration**.

---

## 📚 Technologies Used

- Python
- Pandas, Numpy
- Scikit-learn
- NLTK
- Plotly
