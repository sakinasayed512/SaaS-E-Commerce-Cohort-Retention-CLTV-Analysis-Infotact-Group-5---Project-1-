# SaaS / E-Commerce Cohort Retention & CLTV Analysis
**Infotact Internship — Group 5 | Personal Branch: Sakina Sayed**

## About This Branch
This is my personal working branch where I've built the complete end-to-end 
analysis independently, from raw data cleaning through to final 
visualizations. It runs parallel to the team's work and reflects my 
individual contribution and learning across all 4 weeks.

---

## Project Overview
A real-world data analytics project analyzing customer retention and 
lifetime value using the UCI Online Retail Dataset — 541,909 transactions 
from a UK-based e-commerce retailer (Dec 2010 – Dec 2011).

**Business Questions Answered:**
- How many customers return after their first purchase?
- When exactly do customers churn?
- Which customers generate the most revenue?
- How much is each customer worth to the business over time?

---

## Dataset
UCI Online Retail Dataset  
Source: https://archive.ics.uci.edu/dataset/352/online+retail  
**Raw data is not committed to this repo.** Download from the link above 
and place in the project folder before running the notebook.

---

## Tools Used
Python, Pandas, NumPy, Seaborn, Matplotlib, Jupyter Notebook, Git/GitHub

---

## Week by Week Breakdown

### Week 1 — Data Cleaning & EDA ✅
- Loaded 541,909 raw transactions with encoding='latin1'
- Removed missing CustomerIDs, cancelled orders (InvoiceNo starting with C),
  negative quantities and zero unit prices
- Converted CustomerID to integer, InvoiceDate to datetime
- Added InvoiceMonth, CohortMonth and TotalPrice columns
- Final cleaned shape: 397,884 rows x 10 columns

### Week 2 — Cohort Retention Matrix ✅
- Calculated CohortIndex (months since each customer's first purchase)
- Built raw cohort matrix using Pandas groupby and pivot_table
- Converted to percentage retention by dividing each row by Month 1 size
- Validated all Month 1 values equal 100%

### Week 3 — CLTV Calculation ✅
- Calculated Average Order Value (AOV) per customer
- Calculated Purchase Frequency across customer base
- Computed historical CLTV (AOV x Purchase Frequency) per customer
- Segmented customers into Low/Medium/High value tiers using pd.qcut

### Week 4 — Visualization & Insights ✅
- Built cohort retention heatmap using Seaborn (cmap='Greens')
- Plotted retention decay line chart by cohort
- Built CLTV bar chart by customer segment
- Built revenue contribution chart by cohort month

---

## Key Findings

### 1. Sharp Early Churn
Retention drops to 15–25% by Month 2 across almost all cohorts.
75–85% of customers do not return after their first purchase.

### 2. Strongest Cohort
December 2010 cohort shows the best long-term retention —
still at ~26.6% retained after 13 months.

### 3. Revenue Concentration
The top third of customers (High value segment) contribute **84.9%** 
of total revenue despite being only 33% of the customer base.
A strong Pareto pattern — the business is highly dependent on a 
small core of high-value customers.

---

## Business Recommendations
1. Launch an automated re-engagement campaign targeting customers 
   3–4 weeks after first purchase to combat the Month 1→2 drop-off
2. Prioritize retention programs and loyalty incentives for the 
   High value segment — losing even a few of these customers 
   significantly impacts revenue
3. Explore upsell strategies to migrate Medium segment customers 
   into the High value tier

---

## How to Run
1. Download the dataset from the UCI link above
2. Place it in the same folder as the notebook
3. Open Jupyter Notebook and run all cells top to bottom
4. cleaned_online_retail.csv will be exported automatically for Tableau

