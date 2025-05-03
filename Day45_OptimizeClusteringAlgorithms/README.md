# 🧠  Day 45 :  Optimize Clustering Algorithms

This project explores unsupervised clustering using the **KMeans algorithm** on a preprocessed dataset. We used two major techniques to determine the optimal number of clusters: **Elbow Method** and **Silhouette Score**, and visualized the final clusters accordingly.

---

## 📌 Objectives

- Apply **KMeans clustering** to segment the dataset into meaningful groups.
- Use **Elbow Method** (WCSS) and **Silhouette Score** to determine optimal `k`.
- Visualize clustering results.
- Derive insights from the formed clusters.

---

## 📊 Methods Used

### 1. **Elbow Method**
- Plotted Within-Cluster Sum of Squares (WCSS) against values of `k` (1–10).
- Observed a visible "elbow" at **k = 5**, indicating diminishing returns beyond that point.

### 2. **Silhouette Score**
- Evaluated average silhouette scores for `k` from 2 to 10.
- Found the **maximum silhouette score (~0.56) at k = 5**, validating the Elbow Method result.

### 3. **Final Clustering**
- Applied `KMeans(n_clusters=5)` on the dataset.
- Assigned each data point to a cluster.
- Cluster assignments added to the original dataset as a new column `Cluster`.

---

## 📈 Visualizations

- **Elbow Curve:** Helped identify the point where WCSS starts to level off.
- **Silhouette Plot:** Highlighted how well-separated and cohesive each cluster is.
- **Cluster Visualization:** (Optional if PCA/t-SNE plot included)

---

## ✅ Conclusion

- The optimal number of clusters in the dataset is **5**, validated by both elbow and silhouette methods.
- KMeans successfully segmented the dataset into 5 meaningful groups.
- These clusters can now be further analyzed for trends, profiling, or downstream tasks.

---
