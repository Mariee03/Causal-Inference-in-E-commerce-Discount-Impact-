# Causal Inference in E-commerce – Discount Impact 📉🛒

This project applies **causal inference techniques** to measure the impact of discounts on customer conversion rates in an e-commerce setting. It aims to identify **which customer segments are most responsive to price reductions**, enabling more effective and data-driven marketing strategies.

> Project by: Marie Elyse Bassil

---

## 🎯 Objective

While correlation can suggest relationships, it does not confirm causality. This project uses **causal inference** to answer a key business question:  
**Do discounts actually cause higher conversions, or are they targeting customers who would convert anyway?**

---

## 📦 Dataset Overview

The dataset includes:
- Historical customer behavior
- Discount exposure
- Conversion outcomes (purchased or not)

Features considered:
- Recency, Frequency, Monetary (RFM) variables
- Demographic or behavioral attributes
- Whether the customer received a discount

---

## 🔍 Methodology

### 🧹 1. Data Preparation
- Cleaned missing values
- Encoded categorical variables
- Created treatment variable (`received_discount`) and outcome (`converted`)

### ⚖️ 2. Causal Modeling
Used Python libraries for uplift modeling and causal inference:
- **DoWhy** for causal graphs and hypothesis testing
- **EconML** for treatment effect estimation (e.g., T-learner, Double ML)

### 🔬 3. Estimating Treatment Effect
- Estimated **Average Treatment Effect (ATE)** and **Conditional ATE (CATE)**
- Measured **heterogeneous treatment effects** across customer segments

---

## 📈 Key Findings

- Discounts were **causally effective** in increasing conversion for specific customer groups
- Not all users benefited equally — some showed **no uplift** or even **negative impact**
- **RFM-based segments** helped isolate where discount strategies should be focused

---

## 💼 Business Implications

- **Smarter Targeting**: Send discounts only to segments that benefit from them
- **Avoid Waste**: Don't discount for customers likely to convert anyway
- **Maximize ROI**: Focus on high-ATE segments to optimize marketing spend

---

## 🧰 Tools Used

- Python
- Pandas, NumPy, Seaborn
- DoWhy, EconML
- Scikit-learn
- Jupyter Notebook

---

## 🚀 How to Run

1. Clone the repo:
```bash
git clone https://github.com/Mariee03/Causal-Inference-in-E-commerce-Discount-Impact-.git
cd Causal-Inference-in-E-commerce-Discount-Impact-
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3.Run the notebook:
```bash
jupyter notebook causal_discount_analysis.ipynb
```

### 📬 Author

Created by Marie Elyse Bassil
Open to collaboration, feedback, or questions!
