# Day 34: Feature Engineering for Machine Learning

## 📌 Objectives

- Understand the importance of **Feature Engineering** in Machine Learning.
- Learn how to extract **meaningful features** from raw data.
- Apply Feature Engineering techniques to improve model performance.
- Implement Feature Engineering on a **real-world dataset**.
- Visualize the impact of Feature Engineering on model performance.

---

## 📖 Introduction

Feature Engineering is the process of transforming raw data into features that better represent the underlying patterns for a machine learning model. This step is crucial because **better features lead to better models**.

Key aspects of Feature Engineering include:

- **Handling missing values**
- **Creating new features** (Feature Extraction)
- **Transforming features** (Scaling, Encoding, etc.)
- **Selecting the most relevant features** (Feature Selection)

---

## 📊 Dataset Details

For this exercise, we used the **Telco Customer Churn Dataset**, which contains customer demographic and subscription details to predict churn.

### Dataset Features:

- **Categorical Features:** Gender, Contract Type, Payment Method
- **Numerical Features:** Monthly Charges, Tenure, Total Charges
- **Engineered Features:** Tenure in years, Charge Ratio

---

## 🏗️ Methodology

1. **Data Preprocessing:**

   - Handle missing values in **TotalCharges**.
   - Convert categorical features using **One-Hot Encoding**.
   - Normalize numerical features using **MinMax Scaling**.

2. **Feature Engineering:**

   - **TenureYears** = Tenure / 12
   - **ChargeRatio** = Monthly Charges / Total Charges
   - Extract new features from contract types and payment methods.

3. **Feature Selection:**

   - Compute **Feature Importances** using a tree-based model.
   - Select the top **10 most important features**.

4. **Model Training & Evaluation:**

   - Train models using **Logistic Regression, Random Forest, and XGBoost**.
   - Compare performance with and without Feature Engineering.

---

## 📌 Key Takeaways

✅ Feature Engineering **enhances model performance** by providing better input data.
✅ Creating domain-specific features (e.g., **TenureYears, ChargeRatio**) improves predictive power.
✅ **Feature Selection** ensures that the model focuses on the most relevant features.
✅ **Scaling and encoding** categorical and numerical features are essential for machine learning models.

---

## 📅 Next Steps

For **Day 35**, we will:

-How do we use Decision Trees for Regression?

🚀 Stay tuned for the next step in our **100-Day ML Journey!**

