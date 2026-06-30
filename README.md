# SaaS / E-Commerce Cohort Retention & CLTV Analysis
**Infotact Internship — Group 5**

## Project Overview
This project analyzes customer retention and lifetime value using the UCI 
Online Retail Dataset (541,909 transactions, Dec 2010 – Dec 2011). The goal 
is to understand how long customers stay active after their first purchase, 
and how much value different customer segments bring to the business.

## Team
| Member | Role |
|--------|------|
| Sakina | Team Lead, Week 1 & Week 3(Data Cleaning & EDA), (CLTV Calculation) |
| Beckley | Week 2 (Cohort Retention Matrix) |
| Sanket | Week 4 (Visualization & Dashboard) |


## Dataset
UCI Online Retail Dataset — Online Retail.csv  
Source: https://archive.ics.uci.edu/dataset/352/online+retail  
**Note:** Raw dataset is not committed to this repo per data privacy 
guidelines. Download it directly from the link above.

## Week 1 — Data Cleaning & EDA ✅
- Removed missing CustomerIDs, cancelled orders, negative quantities/prices
- Converted CustomerID to integer, InvoiceDate to datetime
- Calculated CohortMonth (each customer's first purchase month)
- Added TotalPrice column (Quantity x UnitPrice)
- Final cleaned shape: 397,884 rows x 10 columns

## Week 2 — Cohort Retention Matrix ✅
- Calculated CohortIndex (months since first purchase)
- Built retention matrix using groupby and pivot
- Converted to percentage retention
- **Key finding:** Retention drops to ~15-25% by Month 2 across most 
  cohorts. December 2010 cohort retains best long-term (~26.6% at Month 13)

## Week 3 — CLTV Calculation 🔄 In Progress
- Calculated Average Order Value (AOV) and Purchase Frequency per customer
- Segmented customers into Low/Medium/High value tiers
- **Key finding:** High value segment (top third of customers) contributes 
  84.9% of total revenue

## Week 4 — Visualization & Dashboard 🔄 In Progress
- Power BI dashboard in development
- Cohort retention heatmap to be added
- Final business report to follow

## Tools Used
Python, Pandas, Jupyter Notebook, Power BI, Git/GitHub

## Repository Structure
├── SaaS-E-Commerce-Cohort-Retention...ipynb   (main analysis notebook)
├── beckley_week2_cohort_matrix.ipynb
├── README.md
├── .gitignore

## How to Run
1. Download the dataset from the UCI link above
2. Place it in the project folder (do not commit it)
3. Open the main notebook in Jupyter and run cells top to bottom
