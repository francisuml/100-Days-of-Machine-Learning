# 📊 Feature Selection in Unsupervised Machine Learning
This project demonstrates the application of dimensionality reduction techniques—PCA, t-SNE, and LDA—to improve clustering performance and visualization in unsupervised machine learning tasks.

## 🎯 Objective
The primary objective of this project is to explore how feature selection and dimensionality reduction can enhance clustering effectiveness in unsupervised learning. We apply:

Principal Component Analysis (PCA)

t-Distributed Stochastic Neighbor Embedding (t-SNE)

Linear Discriminant Analysis (LDA) (used with labels for validation only)

These are followed by KMeans clustering and interactive visualizations using Plotly.

## 📂 Dataset
We use the Wine Dataset from the UCI Machine Learning Repository, which contains 13 numerical features related to the chemical properties of wines derived from 3 cultivars.

## 🧪 Project Workflow
Load and preprocess data

Standardize the dataset using StandardScaler

Apply Dimensionality Reduction

PCA (2 components)

t-SNE (2 components)

LDA (2 components, supervised for comparison)

Perform Clustering

Use KMeans with n_clusters=3

Fit on the reduced features

Visualize Results

Interactive 2D scatter plots using Plotly

Compare cluster separability across PCA, t-SNE, and LDA

## 📈 Results & Insights
PCA: Captures global structure and variance, but clusters may overlap.

t-SNE: Offers superior local cluster separation for visualization, though not suitable for model training.

LDA: Delivers the best separation (due to label use) and validates cluster structure.

## ✅ Conclusion
Dimensionality reduction plays a vital role in unsupervised machine learning:

Improves clustering results

Enhances interpretability and visualization

Reduces noise and irrelevant features

For exploratory data analysis and cluster detection, combining PCA or t-SNE with KMeans is highly effective.
