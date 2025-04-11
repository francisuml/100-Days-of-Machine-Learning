# 🧠 Day 40 – How Do We Structure ML Pipelines?

## 🚀 Objectives
- Learn how to structure end-to-end supervised machine learning pipelines.
- Understand how to automate machine learning workflows from raw data to deployment.
- Build an efficient ML pipeline using real-world business data.
- Visualize key pipeline stages for better understanding and maintainability.

---

## 📌 Introduction
Machine Learning (ML) pipelines are crucial for automating repetitive workflows, improving reproducibility, and managing data preprocessing, model training, evaluation, and deployment. On Day 40, we explored the design and implementation of an end-to-end supervised ML pipeline using the **Telco Customer Churn** dataset.

We also built a **schematic diagram** illustrating a real-world ML pipeline structure — from data storage and ingestion to model development, evaluation, and deployment.

---

## 📊 Dataset Overview
We used the **Telco Customer Churn Dataset**, which contains customer information for a telecom provider. The goal is to predict customer churn (whether a customer will leave the service).

- 📁 Dataset: `TelcoCustomerChurn.csv`
- 🎯 Target: `Churn`
- 📥 Download: [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

Features include:
- Demographics (gender, SeniorCitizen, tenure)
- Services (PhoneService, InternetService, StreamingTV)
- Charges (MonthlyCharges, TotalCharges)
- Contract and Payment (Contract, PaymentMethod)

---

## 🧠 Methodology

1. **Data Preprocessing**
   - Handled missing values in `TotalCharges`.
   - Encoded categorical features using OneHotEncoding.
   - Scaled numerical features using StandardScaler.

2. **Pipeline Construction**
   - Built a full pipeline using `ColumnTransformer` and `Pipeline` from `scikit-learn`.
   - Combined preprocessing and model training into one reusable structure.

3. **Model Training**
   - Used `RandomForestClassifier` as the baseline model.
   - Evaluated using accuracy, confusion matrix, and ROC-AUC curve.

4. **Automation**
   - Enabled scalability and repeatability with the ML pipeline structure.
   - Simplified feature engineering and model tuning.

5. **Visualization**
   - Confusion Matrix heatmap.
   - ROC Curve for model evaluation.

---

## ⚙️ Model Evaluation

- **Accuracy**: ~0.80+
- **Confusion Matrix**:
- **ROC AUC**: Visualized to assess class separation.

---

## 🧠 Key Takeaways

- ML pipelines help manage the complexity of end-to-end workflows.
- Automating preprocessing and modeling in a unified pipeline makes experimentation easier.
- Clean code and modular structures boost reproducibility and collaboration.
- Real-world datasets often require careful handling of data quality and feature types.

---

## 🔄 Next Steps

**Unsupervised Learning**

