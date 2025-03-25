# 📌 Day 28: Naïve Bayes - Probability-Based Classification

## 📖 Introduction

Naïve Bayes is a **probabilistic classifier** based on Bayes' Theorem, assuming that features are **conditionally independent** given the class label. It is widely used for **text classification, spam filtering, and sentiment analysis.**

---

## 🧠 Understanding Bayes' Theorem

Bayes' Theorem is expressed as:

\begin{equation}
P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}
\end{equation}

Where:

- \( P(A|B) \) → Probability of **A occurring given B is true** (posterior probability)
- \( P(B|A) \) → Probability of **B occurring given A is true** (likelihood)
- \( P(A) \) → **Prior probability** of A occurring
- \( P(B) \) → **Marginal probability** of B occurring

In classification, \( A \) represents the **class label**, and \( B \) represents **features**.

---

## 🏗️ Naïve Bayes Classifiers

The key assumption in Naïve Bayes is **feature independence**, meaning:

\begin{equation}
P(A|B_1, B_2, ..., B_n) = \frac{P(B_1|A) P(B_2|A) ... P(B_n|A) P(A)}{P(B_1, B_2, ..., B_n)}
\end{equation}

Common types of Naïve Bayes classifiers:

- **Gaussian Naïve Bayes** (for continuous data)
- **Multinomial Naïve Bayes** (for text classification)
- **Bernoulli Naïve Bayes** (for binary data)

---

## ✨ Hands-On Practice

For today's hands-on practice, we'll:

✅ Implement **Gaussian Naïve Bayes** on a real dataset.  
✅ Visualize the **decision boundaries** to understand classification regions.  
✅ Evaluate model **accuracy, precision, recall, and F1-score.**  

---

## 🔥 What's Next?

Tomorrow (Day 29), we will explore **What is Model Bias & Variance?** 🌳!  

Stay motivated and keep learning! 🚀  
