# **Understanding Naïve Bayes Classifier**

## **1. Bayes' Theorem**
The Naïve Bayes classifier is based on **Bayes' Theorem**, which states:

$$ P(A|B) = \frac{P(B|A) P(A)}{P(B)} $$

where:
- \( P(A|B) \) is the **posterior probability** (the probability of hypothesis \( A \) given the data \( B \)).
- \( P(B|A) \) is the **likelihood** (the probability of the data \( B \) given the hypothesis \( A \)).
- \( P(A) \) is the **prior probability** (the probability of hypothesis \( A \) before observing the data).
- \( P(B) \) is the **marginal probability** (the probability of observing the data \( B \) over all possible hypotheses).

---

## **2. Naïve Bayes Assumption**
The **Naïve Bayes classifier** assumes that features are **conditionally independent**, meaning:

$$ P(B_1, B_2, ..., B_n | A) = P(B_1 | A) P(B_2 | A) ... P(B_n | A) $$

Using this assumption, we can expand Bayes' Theorem:

$$ P(A|B_1, B_2, ..., B_n) = \frac{P(B_1|A) P(B_2|A) ... P(B_n|A) P(A)}{P(B_1, B_2, ..., B_n)} $$

Since the denominator \( P(B_1, B_2, ..., B_n) \) is the same for all classes, we can ignore it for classification purposes.

---

## **3. Naïve Bayes Decision Rule**
To classify a new data point \( X = (B_1, B_2, ..., B_n) \), we compute:

$$ \hat{y} = \arg\max_{A} P(A) \prod_{i=1}^{n} P(B_i | A) $$

where:
- \( \hat{y} \) is the predicted class.
- \( A \) represents different possible classes.
- \( P(A) \) is the prior probability of class \( A \).
- \( P(B_i | A) \) is the probability of feature \( B_i \) given class \( A \).

---

## **4. Types of Naïve Bayes Classifiers**
There are three main types of Naïve Bayes classifiers:
1. **Gaussian Naïve Bayes** – Assumes features follow a normal (Gaussian) distribution.
2. **Multinomial Naïve Bayes** – Used for text classification (e.g., spam detection).
3. **Bernoulli Naïve Bayes** – Used for binary feature data (e.g., word presence/absence).

---

## **5. Practical Implementation**
We will implement Naïve Bayes on a real-world dataset, visualize decision boundaries, and interpret model performance.

---

## **Next Day: Day 29 - What is Model Bias & Variance?**

🚀 **Stay motivated and keep learning!** 🚀
