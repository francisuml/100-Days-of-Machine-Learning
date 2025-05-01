# Day 44 – What is Hierarchical Clustering?

🎯 **Objective**  
Understand and implement Hierarchical Clustering using both Agglomerative and Divisive approaches. Visualize the tree-like structure formed by clusters and compare clustering results on a real-world dataset.

---

## 📌 Dataset

- **Dataset**: Iris Dataset (`sklearn.datasets.load_iris`)
- **Features**: Sepal length, sepal width, petal length, petal width
- **Target**: Iris species (for reference only, unsupervised learning used)

---

## 🌳 Hierarchical Clustering

### 🔹 Agglomerative Clustering (Bottom-Up)
- Starts with each point as its own cluster.
- Merges closest clusters step-by-step.
- Implemented using `AgglomerativeClustering` from `sklearn`.

### 🔹 Divisive Clustering (Top-Down)
- Starts with all points in one cluster.
- Recursively splits clusters into smaller ones.
- Custom implementation using recursive KMeans (not in `sklearn` by default).

---

## 📈 Visualizations

- 📊 **Pairplot** to show original class separations.
- 🌲 **Dendrogram** to visualize hierarchical merges.
- 🎨 **Scatterplot** of clustering results with labels.

---

## ⚙️ Methods

- `StandardScaler` for feature normalization
- `linkage` and `dendrogram` (from `scipy`) for agglomerative tree
- `AgglomerativeClustering` from `sklearn.cluster`
- `KMeans` recursion to simulate divisive clustering
- `silhouette_score` for clustering evaluation

---

## 📊 Results

- **Agglomerative Clustering**:
  - Visually aligned well with real species.
  - Good silhouette score indicating strong cluster separation.
- **Divisive Clustering**:
  - Manually implemented using recursive KMeans.
  - Demonstrated the top-down approach effectively.

---

## ✅ Conclusion

- Hierarchical clustering builds a tree of clusters and does not require pre-specified number of clusters if dendrogram is used.
- Agglomerative clustering is more commonly used and easier to implement.
- Divisive clustering, while less supported, offers intuitive top-down insight and was simulated here successfully.
- This method is particularly useful when visualizing clustering structure is important.

