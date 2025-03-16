# Day 19: Pipelines & Automation in Machine Learning
---

## 📌 Objective
In this session, we will:
- Understand **why pipelines & automation** are essential in ML workflows.
- Learn how to **create Scikit-learn Pipelines**.
- Automate common ML tasks like **preprocessing, feature selection, and model training**.
- Use a **real-world dataset** to implement pipelines and compare performance.

---

### Why Pipelines & Automation?
In machine learning workflows, we often repeat the same steps:
Data cleaning
Preprocessing (scaling, encoding, imputation)
Feature selection
Model training
Model evaluation
Manually performing these steps is:
Time-consuming
Error-prone
Difficult to reproduce (bad for collaboration!)
Pipelines allow you to:
Bundle preprocessing & model training steps.
Avoid data leakage by applying transformations only on training data during cross-validation.
Simplify hyperparameter tuning.
Make workflows cleaner, modular, and more reproducible.
What Are Pipelines in Scikit-learn?
A pipeline is a series of transformations and a final estimator (model), chained together into one object:
from sklearn.pipeline import Pipeline
Once defined, you can call .fit(), .predict(), and .score() on the entire pipeline, just like a normal model!

---
### 📝 What You Will Learn

How to construct basic pipelines in Scikit-learn.
How to combine:
Preprocessing steps (e.g., StandardScaler, OneHotEncoder)
Feature selection (SelectKBest)
Model (e.g., LogisticRegression, RandomForest)
How to use ColumnTransformer for handling numerical and categorical data differently.
How to automate end-to-end ML workflows.
Comparing model performance with and without pipelines.

---
### 🗂️ Dataset Used

We'll use the Titanic Dataset from Kaggle, a classic dataset for classification problems involving both numerical and categorical features:
Predict whether a passenger survived based on features like age, gender, class, etc.

---
### 💻 Hands-on Notebook

You will:
Load and clean the Titanic dataset.
Create a Pipeline that:
Imputes missing values.
Scales numerical features.
Encodes categorical features.
Selects features.
Trains a classifier.
Evaluate pipeline performance.
Compare results with manual preprocessing.

---
### 📊 Expected Outcome

A fully automated, reusable ML pipeline.
Clear understanding of how pipelines reduce errors, improve reproducibility, and streamline ML workflows.
Ready to integrate pipelines in future projects.
