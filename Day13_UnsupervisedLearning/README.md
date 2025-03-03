# Day 13: Unsupervised Learning 🚀

### Objective

Today, we explored Unsupervised Learning, a powerful machine learning technique used to identify patterns in data without predefined labels. Unlike Supervised Learning, where models learn from labeled data, Unsupervised Learning finds hidden structures within the dataset.
In this notebook, we will:<br>
✔️ Understand Clustering and Dimensionality Reduction<br>
✔️ Implement K-Means and DBSCAN for clustering<br>
✔️ Apply Principal Component Analysis (PCA) for feature reduction<br>
✔️ Visualize high-dimensional data in 2D and 3D using Plotly<br>
✔️ Analyze real-world applications of unsupervised learning<br>
1️⃣ Understanding Clustering<br>

Clustering is the process of grouping similar data points together. It is widely used in:
Customer segmentation (grouping customers based on behavior)
Anomaly detection (fraud detection in transactions)
Genomics (identifying gene expression patterns)
🔹 K-Means Clustering
K-Means is a centroid-based clustering algorithm that partitions data into K clusters. Each cluster is defined by a centroid, and points are assigned to the nearest centroid.
📌 Steps:
Choose the number of clusters (K).
Randomly initialize cluster centroids.
Assign each data point to the nearest centroid.
Update centroids based on cluster assignments.
Repeat until convergence.
🔍 Finding the Optimal K: We used the Elbow Method, which evaluates the Within-Cluster Sum of Squares (WCSS) to determine the best number of clusters.
🔹 DBSCAN (Density-Based Spatial Clustering)
Unlike K-Means, DBSCAN (Density-Based Spatial Clustering of Applications with Noise) does not require specifying the number of clusters. Instead, it groups points based on density, making it effective for datasets with varying cluster sizes and noise.
2️⃣ Dimensionality Reduction with PCA

High-dimensional data can be challenging to visualize and analyze. Principal Component Analysis (PCA) helps by transforming the data into a lower-dimensional space while preserving essential information.
✔️ Why Use PCA?
Reduces computation time
Helps visualize complex datasets in 2D/3D
Removes redundant information
📌 How It Works:
Standardize the data (mean = 0, variance = 1).
Compute the covariance matrix.
Extract eigenvalues and eigenvectors.
Project the data onto principal components.
We used PCA1 and PCA2 to visualize our clustering results effectively.
3️⃣ Visualizing the Clusters with Plotly

After applying clustering techniques, we created robust interactive 2D and 3D visualizations to interpret our results.
import plotly.express as px

🔍 Interpreting the Graphs
K-Means Clustering Plot: Shows distinct groups based on the optimal number of clusters selected.
DBSCAN Plot: Highlights how the density-based approach forms clusters while marking outliers.
4️⃣ Challenges & Solutions

🔸 Choosing the Optimal Number of Clusters
✔️ Used the Elbow Method to determine the best K value.
🔸 Handling High-Dimensional Data
✔️ Applied PCA to visualize clusters in a reduced feature space.
🔸 Noise & Outliers in DBSCAN
✔️ Tuned epsilon (ε) and minimum samples to balance sensitivity.
5️⃣ Real-World Applications

🚀 Unsupervised Learning is used in:
✅ Customer segmentation in marketing
✅ Fraud detection in financial transactions
✅ Anomaly detection in cybersecurity
✅ Pattern recognition in genetics
🔜 What’s Next?

Tomorrow, we will dive into a crucial topic:
📌 Day 14: Overfitting & Underfitting
Understand why models fail to generalize to new data
Learn techniques to balance bias and variance
Implement cross-validation and regularization to improve model performance
By mastering Unsupervised Learning, you are building a strong foundation for more advanced AI applications. Keep learning, stay curious, and let’s continue the journey! 🚀
