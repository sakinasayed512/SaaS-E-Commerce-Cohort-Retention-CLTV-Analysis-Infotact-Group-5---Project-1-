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
| Sakina | Team Lead, Week 1,Week 3 & Week 4(Data Cleaning & EDA), (CLTV Calculation), (Tableau Dashboard) |
| Beckley | Week 2 (Cohort Retention Matrix) |
| Sanket | Week 4 (PowerBI Dashboard) |


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

## Week 3 — CLTV Calculation ✅
- Calculated Average Order Value (AOV) and Purchase Frequency per customer
- Segmented customers into Low/Medium/High value tiers
- **Key finding:** High value segment (top third of customers) contributes 
  84.9% of total revenue

## Week 4 — Visualization & Dashboard ✅
- Power BI/Tableau dashboard
- Cohort retention heatmap added
- Final business report - main readme

## Tools Used
Python, Pandas, Jupyter Notebook, Power BI, Git/GitHub
