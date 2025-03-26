# Day 29: Understanding Model Bias & Variance

## 📌 Objectives:
- Comprehend the concepts of **Bias and Variance** in machine learning.
- Understand the **Bias-Variance Tradeoff**.
- Study **Learning Curves** and **Model Diagnostics**.
- Implement practical strategies to **improve model generalization**.
- Apply the concepts on a **real-world dataset**.
- Utilize robust **visualizations** to interpret results.
- Prepare for the next phase: **Decision Trees & Model Complexity**.

---

## 🤔 What is Model Bias & Variance?

**Bias and Variance** are two key sources of error in machine learning models.

### 🔹 Bias:
- The **error introduced by approximating a real-world problem** with a simplified model.
- High-bias models **fail to capture** underlying patterns → **Underfitting**.

### 🔹 Variance:
- The **model’s sensitivity to small fluctuations** in the training data.
- High-variance models **overreact to noise** → **Overfitting**.

### 🎯 The Bias-Variance Tradeoff:
- **Low Bias + High Variance** → Overfitting ⚠️
- **High Bias + Low Variance** → Underfitting ⚠️
- **Balanced Bias & Variance** → Optimal Generalization ✅

---

## 🧠 How to Diagnose Bias & Variance?

We can analyze a model’s performance using **Learning Curves**:

1. **Training Error:** Measures how well the model fits the training data.
2. **Validation Error:** Measures the generalization of the model to unseen data.

#### 🔥 Key Observations:
- **High training & validation errors** → Underfitting (High Bias)
- **Low training error & high validation error** → Overfitting (High Variance)
- **Balanced errors** → Good generalization

---

## 📊 Dataset: **California Housing Prices**

For hands-on practice, we'll use the **California Housing Prices Dataset**, which includes:
- **Features:** Median income, house age, total rooms, total bedrooms, etc.
- **Target:** Median house value.

---

## 🛠️ Implementing Bias & Variance Analysis

We'll explore model behavior by:
- Training **Linear Regression** (High Bias model) ⚡
- Training **Decision Tree Regression** (High Variance model) 🌳
- Plotting **Learning Curves** 📈
- Using **Cross-Validation** to find the right balance ✅

---

## 📈 Visualizations

- **Learning Curves:** Observe model behavior with increasing training data.
- **Bias-Variance Analysis:** Compare different models.
- **Model Performance Metrics:** RMSE, R² scores, etc.

---

## 📁 What's in this Notebook:

1. **Load Dataset:** Import and explore California Housing data.
2. **Preprocess Data:** Handle missing values & feature scaling.
3. **Train-Test Split:** Prepare data for modeling.
4. **Train Models:** Implement Linear Regression & Decision Tree Regression.
5. **Plot Learning Curves:** Visualize bias & variance.
6. **Analyze Results:** Interpret learning curves & model performance.
7. **Improve Generalization:** Tune hyperparameters & cross-validation.
8. **Conclusions:** Summarize findings & prepare for the next topic.

---

## 🚀 What's Next?

In **Day 30**, we will dive into **How do we optimize ML models?**:

Stay tuned! 🌟
