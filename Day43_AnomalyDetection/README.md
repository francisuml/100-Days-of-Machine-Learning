# Day 43 – Anomaly Detection with Isolation Forest & One-Class SVM

🎯 **Objective**  
Build a robust anomaly detection system to identify fraudulent transactions using unsupervised machine learning techniques on a real-world credit card fraud dataset.

---

## 📌 Dataset

- **Source**: [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Features**:
  - `V1` to `V28`: Principal Components (PCA-transformed features)
  - `Amount`: Transaction amount
  - `Class`: Target (0 = normal, 1 = fraud)

---

## 🧠 Models Used

1. **Isolation Forest**
   - Detects anomalies by isolating outliers in tree-based splits.
   - Fast and effective for high-dimensional data.

2. **One-Class SVM**
   - Learns a boundary around the normal data points using kernel tricks.
   - Sensitive to parameters (`nu`, `gamma`) and outliers.

---

## 🛠 Pipeline

1. Load and explore the dataset
2. Standardize features using `StandardScaler`
3. Apply Isolation Forest & One-Class SVM
4. Compare model predictions with actual labels using:
   - Confusion Matrix
   - Classification Report
5. Visualize anomaly distribution with:
   - PCA (2D projection)
   - Plotly interactive scatter plot

---

## 📈 Results

- **Isolation Forest**:
  - Detected majority of frauds with fewer false positives.
- **One-Class SVM**:
  - Sensitive to hyperparameters; needs careful tuning.

---

## 📊 Visuals

- **PCA Scatter Plot** with:
  - Color: Model predictions (Outlier/Normal)
  - Symbol: Actual labels (Fraud/Normal)

<p align="center">
  <img src="example_plotly_output.png" alt="PCA Plotly Output" width="600">
</p>

---

## ✅ Conclusion

- Isolation Forest is well-suited for this anomaly detection task.
- PCA and Plotly helped visualize complex outlier behavior.
- Further improvements possible with model tuning and ensemble approaches.

