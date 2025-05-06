# 📊 Day 53: Evaluating Clustering & Anomaly Detection Models

This project focuses on understanding and applying quantitative metrics to evaluate clustering and anomaly detection models. Specifically, we explore:

- **Adjusted Rand Index (ARI)**
- **Silhouette Score**

These metrics help assess clustering quality and anomaly detection performance, especially when ground truth labels are available.

---

## 🎯 Objective

- Learn how to **evaluate clustering models quantitatively**.
- Apply **K-Means** clustering to high-dimensional text data and visualize results using **PCA**.
- Measure performance using **Adjusted Rand Index (ARI)** and **Silhouette Score**.
- Understand strengths and limitations of each metric.
- Visualize and interpret results for deeper insights.

---

## 📈 Metrics Overview

### 🔹 Adjusted Rand Index (ARI)

- **Purpose:** Measures similarity between predicted clusters and actual labels.
- **Range:** -1 to 1
  - 1 = perfect match with ground truth
  - 0 = random labeling
  - < 0 = worse than random
- **Use case:** Best when true labels are known (e.g., benchmarking clustering algorithms).

### 🔹 Silhouette Score

- **Purpose:** Measures how similar an object is to its own cluster (cohesion) compared to other clusters (separation).
- **Range:** -1 to 1
  - 1 = well-separated clusters
  - 0 = overlapping clusters
  - < 0 = poorly clustered
- **Use case:** Works well even **without ground truth labels**.

---

## 📁 Dataset

- **Type:** Synthetic or real-world high-dimensional dataset (e.g., TF-IDF features from tweets or documents)
- **Preprocessing:** PCA for dimensionality reduction to visualize clustering in 2D

---

## 🤖 Models Used

- **K-Means Clustering**
  - Unsupervised algorithm to group similar instances into `k` clusters.
  - Applied after dimensionality reduction.

---

## 📊 Evaluation Results

| Metric                | Value     |
|-----------------------|-----------|
| Adjusted Rand Index   | -0.0006   |
| Silhouette Score      | 0.5539    |

### 🔍 Insight

- **ARI = -0.0006**: Indicates **almost no alignment** between the predicted clusters and true labels (or worse than random).
- **Silhouette Score = 0.5539**: Suggests **moderate cluster separation**, meaning clusters are reasonably compact and distinct.

This implies that while the clustering formed coherent groups (Silhouette), those groups **do not align** with the original labels (ARI), which could be due to:
- High feature overlap between classes
- Inappropriate `k` value
- Irrelevant or noisy features

---

## 📊 Visualizations

- 2D scatter plots using PCA
- Clusters colored by predicted labels
- Interactive charts built with **Plotly** for exploration

---

## 💡 Conclusion

- Use **Silhouette Score** when ground truth is **not available** to validate cluster quality.
- Use **Adjusted Rand Index** to compare clustering with known class labels.
- A **high Silhouette + low ARI** indicates well-formed clusters that do **not align** with actual classes, revealing potential feature or label issues.
- Further experiments can include tuning `k`, trying **DBSCAN**, or improving feature engineering.

---
