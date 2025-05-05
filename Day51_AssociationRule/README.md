# 🛒 Association Rule Learning with Apriori & FP-Growth

## 📌 Objective
The goal of this project is to explore **Association Rule Learning** using two powerful algorithms: **Apriori** and **FP-Growth**. We aim to uncover meaningful patterns and item relationships within transactional data, commonly used in market basket analysis.

---

## 📖 What is Association Rule Learning?

**Association Rule Learning** is an unsupervised machine learning technique that discovers interesting relations (rules) between variables in large datasets. It is widely used for:

- **Market Basket Analysis**
- Recommender systems
- Web usage mining
- Bioinformatics

Rules are derived in the form:
**If {item A, item B} → Then {item C}**

based on three key metrics:

- **Support**: How often an itemset appears in the dataset.
- **Confidence**: How often the rule has been found to be true.
- **Lift**: How much more likely item Y is purchased when item X is.

---

## 📂 Dataset Used
We used a synthetic transactional dataset (`groceries.csv`) resembling real-world grocery purchase patterns. Each row represents a list of items bought together by a customer.

---

## 🔧 Algorithms Applied

### 1. **Apriori**
- Generates frequent itemsets using breadth-first search.
- Efficient with small to medium datasets.
- Relies on support thresholds to prune search space.

### 2. **FP-Growth**
- Uses a compressed prefix-tree (FP-tree) structure.
- Eliminates candidate generation, making it faster on large datasets.
- Ideal for datasets with many frequent patterns and overlaps.

---

## 🧪 Implementation Steps

1. **Data Preprocessing**  
   - Load and clean the data
   - Convert transactions into the right format for mining

2. **Apply Apriori**  
   - Extract frequent itemsets
   - Generate rules based on min support and confidence

3. **Apply FP-Growth**  
   - Extract frequent patterns using `fpgrowth`
   - Generate association rules

4. **Time Comparison**

   | Algorithm   | Wall Time | Observations                                       |
   |-------------|-----------|----------------------------------------------------|
   | Apriori     | 31 ms     | Fast due to minimal overlap and efficient pruning  |
   | FP-Growth   | 9.38 s    | Slower here due to sparse data and FP-tree overhead |

5. **Visualization**
   - Support vs Confidence plot
   - Lift distribution for rules
   - Top rules by metrics

---

## 📊 Visualization

We used **matplotlib** to create clear, insightful plots:

- Top 10 frequent itemsets
- Rule scatter plots (Support vs Confidence)
- Lift histograms

---

## 🔍 Insights

- **Apriori** was faster in this specific dataset due to simple patterns and less overlap.
- **FP-Growth**, although generally faster on large datasets, was slower here due to the synthetic data's sparseness.
- High-confidence rules like `{milk, bread} → eggs` suggest co-purchasing trends.
- Lift scores >1 helped us identify truly interesting rules.

---

## ✅ Conclusion

- Both Apriori and FP-Growth successfully mined strong association rules.
- Algorithm efficiency depends heavily on dataset structure and density.
- Association rule learning is valuable for uncovering actionable insights in retail, web usage, and more.

---
