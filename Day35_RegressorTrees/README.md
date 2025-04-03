# Day 35: Decision Trees for Regression

## 📌 Objectives

- Understand how **Decision Trees** can be used for regression tasks.
- Learn about **Regression Trees**, including splitting criteria and leaf node predictions.
- Implement a **Decision Tree Regressor** on a real-world dataset.
- Visualize the decision tree structure and interpret model predictions.
- Evaluate model performance using regression metrics.

---

## 📚 Introduction

Decision Trees are commonly used for both classification and regression. In regression tasks, a **Decision Tree Regressor** splits the dataset into regions and assigns a predicted value (mean of the region) to each split.

Key concepts include:

- **Splitting Criteria**: Using **Mean Squared Error (MSE)** or **Mean Absolute Error (MAE)** to find the best splits.
- **Pruning**: Reducing tree depth to prevent overfitting.
- **Hyperparameters**: Controlling tree depth, minimum samples per leaf, and splitting thresholds.

---

## 📊 Dataset Details

For this exercise, we used the **California Housing Dataset**, which contains information about housing prices based on various features.

### Dataset Features:

- **Numerical Features:** Median Income, House Age, Total Rooms, Population, Latitude, Longitude
- **Target Variable:** Median House Value

---

## 🏰️ Methodology

1. **Data Preprocessing:**
   - Handle missing values (if any) using **median imputation**.
   - Normalize numerical features using **MinMax Scaling**.

2. **Training Decision Tree Regressor:**
   - Train a **DecisionTreeRegressor** with default settings.
   - Tune hyperparameters (**max_depth, min_samples_split, min_samples_leaf**).

3. **Feature Importance Analysis:**
   - Extract **feature importances** from the trained model.
   - Visualize top features affecting predictions.

4. **Model Evaluation:**
   - Use regression metrics: **Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-Squared (ℝ²)**.
   - Compare performance before and after hyperparameter tuning.

---

## 📉 Model Evaluation

| Model                     | MAE (Lower is Better) | MSE (Lower is Better) | R-Squared (Higher is Better) |
|---------------------------|----------------------|----------------------|----------------------------|
| Default Decision Tree     | 52,000              | 4.5e+09              | 0.65                       |
| Tuned Decision Tree       | 43,500              | 3.2e+09              | 0.74                       |

After tuning hyperparameters, the **Decision Tree Regressor showed significant improvement** in predictive accuracy! 🚀

---

## 📌 Key Takeaways

✅ Decision Trees can model complex **non-linear relationships** in regression problems.
✅ **Hyperparameter tuning** improves performance significantly.
✅ **Feature Importance analysis** helps in understanding model decisions.
✅ **Tree visualization** provides insights into how decisions are made.

---

## 🗓 Next Steps

For **Day 36**, we will:

- Dive into **What is Boosting in ML?g**

🚀 Stay tuned for the next step in our **100-Day ML Journey!**

