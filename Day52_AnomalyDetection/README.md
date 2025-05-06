# 🕵️‍♂️ Anomaly Detection: Fraud Detection using Isolation Forest & One-Class SVM

This project explores **anomaly detection techniques** to identify fraudulent transactions using the real-world **credit card fraud dataset**. We implemented and compared two powerful unsupervised machine learning algorithms: **Isolation Forest** and **One-Class SVM**, with a focus on detecting rare events and fraudulent behavior.

---

## 📌 Objective

- Detect anomalies (frauds) in a highly imbalanced dataset.
- Implement **Isolation Forest** and **One-Class SVM** in a Jupyter Notebook.
- Evaluate model performance using confusion matrix and classification metrics.
- Visualize and compare results using robust plots.
- Perform **hyperparameter tuning** using GridSearchCV.
- Derive expert insights and real-world conclusions.

---

## 📁 Dataset

We used the **[Credit Card Fraud Detection dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)** from Kaggle:
- 284,807 transactions
- Only 492 frauds (highly imbalanced)
- Features are numerical (PCA-transformed), except for `Time` and `Amount`

---

## 🔧 Models Used

### ✅ Isolation Forest
- Efficient for high-dimensional, imbalanced data.
- Works by isolating anomalies via random partitioning.
- Detects outliers as points with shorter average path lengths in trees.

### ✅ One-Class SVM
- Learns a decision boundary around the majority class (normal).
- Classifies points far from this boundary as anomalies.
- Sensitive to hyperparameters like `nu` and `gamma`.

---

## 🧪 Evaluation Metrics

| Model            | Precision | Recall | F1-Score | Time     |
|------------------|-----------|--------|----------|----------|
| Isolation Forest | High      | High   | Strong   | Fast     |
| One-Class SVM    | Very Low  | High   | Poor     | Very Slow|

### ✅ Isolation Forest Confusion Matrix

|                | Predicted Normal | Predicted Fraud |
|----------------|------------------|-----------------|
| **Actual Normal** | 274,823          | 9,492           |
| **Actual Fraud**  | 89               | 403             |

### ❌ One-Class SVM Confusion Matrix

|                | Predicted Normal | Predicted Fraud |
|----------------|------------------|-----------------|
| **Actual Normal** | 142,157          | 142,158         |
| **Actual Fraud**  | 14               | 478             |

---

## 🔍 Insights

- **Isolation Forest** achieves a **good trade-off** between detecting fraud and minimizing false positives.
- **One-Class SVM** captures more fraudulent cases (**high recall**), but at the cost of **overwhelming false positives**.
- For real-world deployment, **Isolation Forest is more reliable**.
- Hyperparameter tuning improved the performance slightly, but base behavior remained consistent.

---

## 📈 Visualizations

- Confusion matrices for both models
- Comparison charts of classification metrics (Precision, Recall, F1-Score)
- GridSearchCV results showing best hyperparameters

---

## 🧠 Conclusion

Isolation Forest offers a **robust and scalable** solution for anomaly detection in large, imbalanced datasets such as fraud detection. One-Class SVM, while conceptually appealing, is **less practical** for large-scale fraud detection due to its sensitivity and performance cost.

---
