# Day 21: How Does Linear Regression Work?

---

## 📌 Objectives:

- Understand the fundamentals of **Linear Regression**.
- Implement **Linear Regression from scratch** using Python and NumPy.
- Apply Linear Regression to a **real-world dataset**.
- Visualize regression results and evaluate model performance.

---

## 📖 What is Linear Regression?

Linear Regression is one of the simplest and most widely used algorithms in supervised learning. It establishes a relationship between the dependent variable (target) and one or more independent variables (features) by fitting a straight line (in 2D) or hyperplane (in higher dimensions) that minimizes the error between predicted and actual values.

### **Mathematical Equation:**

\[
y = w_1x_1 + w_2x_2 + \dots + w_nx_n + b
\]

Where:
- \( x_1, x_2, \dots, x_n \) = Input features
- \( w_1, w_2, \dots, w_n \) = Weights (coefficients)
- \( b \) = Bias term
- \( y \) = Predicted output

---

## 💡 Why Learn Linear Regression?

- It's the **foundation** for many advanced machine learning algorithms.
- Easy to **implement** and **interpret**.
- Helps in understanding key concepts like:
  - **Loss functions**
  - **Optimization**
  - **Model evaluation**

---

## 🛠️ Topics Covered:

| Topic                                      | Description                                                                                           |
|-------------------------------------------|-------------------------------------------------------------------------------------------------------|
| What is Linear Regression?                | Learn the concept of Linear Regression and its applications.                                          |
| Linear Regression from Scratch            | Implement Linear Regression using Python, NumPy without libraries like Scikit-learn.                  |
| Training and Testing                      | Split dataset into training and testing sets and evaluate performance.                                 |
| Mean Squared Error (MSE) & MAE            | Use MSE and MAE to evaluate model accuracy.                                                            |
| Data Visualization                        | Plot actual vs predicted values using Matplotlib.                                                     |

---

## 📊 Dataset Used:

We used the **Fish Market Dataset** containing information about different fish species, including their weight, length, and width measurements.

| Feature          | Description                         |
|------------------|-------------------------------------|
| Species          | Fish species name (Categorical)     |
| Weight           | Weight of the fish (Target)         |
| Length1, Length2 | Length measurements (in cm)         |
| Width            | Width measurement (in cm)           |
| Height           | Height measurement (in cm)          |

---

## 🚀 Hands-On Practice:

In the Jupyter Notebook, you will:

1. **Load & Explore** the dataset.
2. **Preprocess** features (one-hot encoding for species).
3. **Split data** into training/testing sets.
4. **Implement Linear Regression manually.**
5. Calculate optimal weights using the **Normal Equation**:

\[
\theta = (X^T X)^{-1} X^T y
\]

6. Evaluate model using:
   - **Mean Absolute Error (MAE)**
   - **Mean Squared Error (MSE)**

7. Visualize **actual vs. predicted weights**.

---

## 📁 Files Included:

- `day21_LinearRegression.ipynb` → Full notebook implementation with explanations, visualization, and evaluation.
- `README.md` → This documentation.

---

## 📌 Key Takeaways:

- Learned how **Linear Regression** works mathematically.
- Implemented from scratch without ML libraries.
- Evaluated model on a **real-world dataset**.
- Built foundational knowledge for advanced regression models.

---

## 🔥 Next Steps:

In the next session, we'll dive deeper into **How do we interpret Linear Regression results?** 

---

