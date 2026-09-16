# 🛒 Market Basket Analysis

## 📌 Project Overview

Market Basket Analysis is a data analytics technique used to identify
relationships and purchasing patterns between products.

In this project, grocery transaction data is analyzed to discover which
products are frequently purchased together. The Apriori algorithm is used
to generate frequent itemsets and association rules.

The insights obtained can help retailers with product placement,
cross-selling, product recommendations, and promotional strategies.

---

## 🎯 Objectives

- Analyze customer purchasing patterns
- Identify frequently purchased products
- Find products that are commonly purchased together
- Generate association rules using the Apriori algorithm
- Analyze Support, Confidence, and Lift
- Extract useful business insights from transaction data

---

## 📊 Dataset

The dataset contains grocery store transaction records.

### Dataset Statistics

- **Total Transactions:** 9,835
- **Total Unique Products:** 169
- **Total Columns:** 33

Each row represents a customer transaction, while the item columns
represent products purchased during that transaction.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Mlxtend
- Google Colab
- Apriori Algorithm

---

## 🔍 Project Workflow

### 1. Data Loading
The grocery transaction dataset was loaded using Pandas.

### 2. Data Exploration
The dataset structure, dimensions, missing values, and unique products
were analyzed.

### 3. Exploratory Data Analysis
The most frequently purchased products were identified and visualized.

### 4. One-Hot Encoding
The transaction data was converted into a binary basket format.

- `1` → Product is present in the transaction
- `0` → Product is not present in the transaction

### 5. Frequent Itemset Mining
The Apriori algorithm was applied with a minimum support of 1%.

### 6. Association Rule Mining
Association rules were generated using a minimum confidence threshold
of 20%.

### 7. Rule Evaluation

The rules were evaluated using:

- **Support**
- **Confidence**
- **Lift**

---

## 📈 Key Metrics

### Support

Support represents how frequently an item or item combination occurs
in all transactions.

### Confidence

Confidence represents the probability of purchasing the consequent
product when the antecedent product or products are purchased.

### Lift

Lift measures the strength of association between products.

- Lift > 1 → Positive association
- Lift = 1 → No significant association
- Lift < 1 → Negative association

---

## 🔎 Sample Finding

One of the strongest association rules identified was:

**Other Vegetables + Citrus Fruit → Root Vegetables**

- **Support:** ~1.04%
- **Confidence:** ~35.9%
- **Lift:** ~3.30

This indicates a positive association between the products in this rule.

---

## 💡 Business Insights

The analysis can help retailers:

- Improve product placement
- Create product bundles
- Develop cross-selling strategies
- Provide product recommendations
- Design targeted promotional offers
- Understand customer purchasing behavior

---

## 📊 Visualizations

The project includes visualizations for:

- Top 10 Most Purchased Items
- Top Association Rules by Lift
- Top Association Rules by Confidence

---

## 📁 Project Structure

```text
Groceries-Market-Basket-Analysis/
│
├── Groceries_Market_Analysis.ipynb
├── groceries - groceries.csv
├── README.md
└── images/
    ├── top_10_items.png
    ├── top_rules_lift.png
    └── top_rules_confidence.png
