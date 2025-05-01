# 📊 Day 42: Principal Component Analysis (PCA) – Dimensionality Reduction

## 🧠 Objective
The goal of this notebook is to understand **Principal Component Analysis (PCA)** and its role in **dimensionality reduction** in machine learning. We apply PCA to the Wine dataset to:
- Visualize high-dimensional data in 2D.
- Reduce the number of features while preserving most of the information.
- Evaluate the effect of PCA on machine learning model performance.

---

## 📚 What is PCA?

Principal Component Analysis (PCA) is an **unsupervised linear transformation** technique that:
- Projects high-dimensional data to a lower-dimensional space.
- Maximizes variance capture in fewer dimensions.
- Produces new, uncorrelated features called **principal components**.

### 🚀 Why PCA?
- Reduces **noise** and **redundancy**.
- Improves **visualization** and **model training speed**.
- Helps prevent **overfitting** in high-dimensional spaces.

---

## 📦 Dataset: Wine Classification
- Source: `sklearn.datasets.load_wine()`
- 13 numerical features (e.g., alcohol, flavanoids, magnesium)
- 3 wine cultivars (target classes)
- Task: Classify wine type based on chemical features.

---

## 📌 Steps Covered in `day42_PCA.ipynb`

1. **Data Preprocessing**  
   - Standardized features using `StandardScaler`.
2. **PCA Transformation**  
   - Applied PCA to reduce 13 features → 2 principal components.
   - Explained ~55% of variance with the first 2 components.
3. **Visualization**  
   - Plotted PCA-reduced data in 2D with class labels.
4. **Modeling**  
   - Used Random Forest for classification.
   - Compared performance before and after PCA.

---

## 📈 Results

| Model Type            | Features Used | Accuracy |
|-----------------------|---------------|----------|
| Random Forest (Full)  | All 13         | ~97.2%   |
| Random Forest (PCA)   | 2 PCs          | ~94.4%   |

---

## 🧠 Insights

- Even with only **2 dimensions**, the PCA-transformed dataset retains strong class separability.
- **Over half of the data's structure** is retained in just two principal components.
- PCA helped reduce complexity **without a major drop in accuracy**.

---

## ✅ Conclusion

PCA is a powerful technique for reducing feature space, improving efficiency, and enabling visualization — especially useful when dealing with high-dimensional datasets. While some detail is lost, the **core patterns remain**, making it ideal for preprocessing and exploratory analysis.

---
