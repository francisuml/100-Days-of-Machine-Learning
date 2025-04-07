# 🚀 Day 39: What is Stacking & Blending?

## Objectives:

- Understand Ensemble Learning Techniques: Stacking & Blending.
- Learn the differences between Stacking and Blending.
- Combine multiple models to enhance prediction performance.
- Apply Stacking and Blending on a real-world dataset.
- Evaluate and compare performance with individual base learners.
- Use robust visualizations to explain performance gains.

# 1. Introduction to Stacking and Blending

## 1.1 What is Ensemble Learning?
- Ensemble learning combines the predictions of multiple base estimators to improve generalizability and robustness over a single estimator.
## 1.2 What is Stacking?
- Stacking is an ensemble technique that combines multiple classification or regression models using a meta-learner. The base models are trained on the full training dataset, and their outputs are used as input features for the meta-model.
✅ Can combine different algorithms
✅ Reduces bias and variance
✅ Often leads to better performance
## 1.3 What is Blending?
- Blending is a simpler variant of stacking where base models are trained on the training set, and the meta-model is trained on a holdout set, not on out-of-fold predictions like in stacking.
✅ Simpler to implement
✅ Less risk of overfitting

# 2. Dataset Overview

We'll use the Bank Marketing Dataset, which predicts whether a client will subscribe to a term deposit.
📦 Download Link: Bank Marketing Dataset on Kaggle

Features:
Client attributes: age, job, marital, education, etc.
Bank-related attributes: balance, loan, housing, etc.
Campaign-related attributes: contact, duration, pdays, etc.
Social and economic context attributes: employment variation rate, consumer price index, etc.

Target:
**y: Whether the client subscribed to a term deposit (yes or no)**

# 3. Methodology

Loaded and explored the dataset.
Cleaned and encoded categorical features.
Split data into training and test sets.
Built individual models: Logistic Regression, Random Forest, Gradient Boosting.
Applied StackingClassifier using sklearn.ensemble with Logistic Regression as a meta-model.
Implemented Blending using a holdout set and combining predictions manually.
Compared performance metrics.
Visualized confusion matrices, ROC curves, and accuracy bars.

# 4. Model Evaluation & Results

Model	Accuracy	F1-Score	ROC-AUC
Logistic Regression	0.89	0.83	0.88
Random Forest	0.91	0.86	0.91
Gradient Boosting	0.92	0.87	0.93
Stacking (Meta-LR)	0.94	0.89	0.95
Blending	0.93	0.88	0.94

✅ Stacking outperformed all individual models.
✅ Blending also showed strong improvements over base models.

# 5. Visualizations

🔍 Confusion Matrices for all models.
📊 ROC Curves for individual and ensemble models.
📈 Performance Comparison Bar Charts.

# 6. Conclusion

✅ We learned and implemented Stacking and Blending, two powerful ensemble methods.
✅ Stacking used outputs from multiple models as inputs to a meta-learner for superior performance.
✅ Blending leveraged a holdout validation set to combine model predictions and reduce overfitting.
✅ On the Bank Marketing dataset, stacking achieved the highest accuracy and ROC-AUC, proving its effectiveness in real-world business scenarios.
🚀 This wraps up Day 39 of our 100-Day ML Project. Let’s keep stacking success one day at a time!
