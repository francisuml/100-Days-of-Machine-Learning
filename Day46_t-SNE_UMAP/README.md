# 🧠 Day 46: Visualizing High-Dimensional Data with t-SNE and UMAP

## 📌 Objective
Explore and compare two powerful dimensionality reduction techniques — **t-SNE** and **UMAP** — to visualize complex, high-dimensional datasets in 2D while preserving structural relationships.

---

## 📖 What You’ll Learn
- What is **t-SNE** and how it preserves local structures
- What is **UMAP** and how it balances local and global structures
- When and why to reduce data dimensions for visualization and modeling
- Visualize the **Fashion MNIST** dataset in 2D with Plotly

---

## 📊 Dataset
- **Fashion MNIST** (from `tensorflow.keras.datasets`)
- 28x28 grayscale images of clothing items (e.g., shirts, shoes, bags)
- 10 classes, 60,000 training images, 10,000 test images

---

## 🛠 Tools & Libraries
- `numpy`, `pandas`
- `matplotlib`, `plotly`
- `sklearn.manifold.TSNE`
- `umap-learn`
- `tensorflow` (for loading Fashion MNIST)

---

## 📈 Visualizations
- **2D scatter plots** of t-SNE and UMAP projections with color-coded classes
- Interactive plots using Plotly for better insight

---

## 🔍 Key Insights
- Both t-SNE and UMAP effectively revealed distinct clothing clusters.
- UMAP was significantly faster and preserved more global relationships.
- Dimensionality reduction helps us visually validate clustering tendencies.

---

## ✅ Conclusion
Dimensionality reduction is essential for:
- Understanding and visualizing high-dimensional datasets
- Preprocessing data for better model performance
- Exploring structure and grouping in data

**t-SNE** is best for deep, local patterns.  
**UMAP** is more scalable and balances structure.

---
