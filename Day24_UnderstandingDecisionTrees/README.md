# Day 24: Understanding and Implementing Decision Trees

## 📌 Objectives:
- Understand how Decision Trees work.
- Learn key concepts: Entropy, Gini Impurity, and Pruning.
- Build Decision Trees for classification tasks.
- Apply Decision Trees on a real-world dataset (Iris Dataset).
- Visualize the Decision Tree and decision boundaries.
- Prepare for the next phase: Ensemble Methods (Random Forests).

---

## 🌳 What is a Decision Tree?

A **Decision Tree** is a supervised learning algorithm used for both classification and regression tasks. It mimics human decision-making by creating a tree-like model of decisions.

- **Internal nodes** represent feature conditions.
- **Branches** represent the outcome of the condition.
- **Leaf nodes** represent the final prediction/class.

---

## 🧮 Key Concepts:

### 1. **Entropy**
Entropy measures the impurity or randomness in the dataset:

\[
Entropy = -\sum p_i \log_2(p_i)
\]

Where \( p_i \) is the probability of each class.

---

### 2. **Gini Impurity**
Another metric to measure impurity:

\[
Gini = 1 - \sum p_i^2
\]

It penalizes misclassification and is often faster to compute.

---

### 3. **Pruning**
Pruning reduces overfitting by removing unnecessary branches:

- **Pre-Pruning**: Limit tree depth or minimum samples per leaf.
- **Post-Pruning**: Remove branches after the tree is built based on performance.

---

## 📊 Dataset: **Iris Dataset**

We’ll use the popular Iris dataset, containing measurements of iris flowers' petals and sepals to classify them into species.

---

## 📁 What’s in this Notebook:
1. **Load Dataset**  
2. **Preprocess Data**  
3. **Train-Test Split**  
4. **Build Decision Tree Classifier**  
5. **Visualize Decision Tree & Decision Boundaries**  
6. **Evaluate Performance**  
7. **Interpret Results**

---

## 🚀 What's Next?
In **Day 25**, we will step up to **How does Random Forest work?**, specifically:

Stay tuned! 🌟
