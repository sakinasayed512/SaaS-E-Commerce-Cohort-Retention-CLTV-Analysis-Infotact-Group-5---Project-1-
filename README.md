# SaaS / E-Commerce Cohort Retention & CLTV Analysis
Infotact Advanced Data Analytics Internship | Group 5

---

## What This Project Is About
We analyzed real customer transaction data from a UK-based online retailer 
to answer two simple business questions:

- Are customers coming back after their first purchase?
- Which customers are actually worth the most to the business?

To answer these we built a cohort retention analysis and calculated 
Customer Lifetime Value (CLTV) across different customer segments.

---

## Dataset
UCI Online Retail Dataset — 541,909 transactions from Dec 2010 to Dec 2011  
Source: https://archive.ics.uci.edu/dataset/352/online+retail  

The raw dataset is not uploaded here. Download it from the link above 
and place it in the project folder before running the notebook.

---

## Team — Group 5
| Name | Role |
|------|------|
| Sakina Sayed (Team Lead) | Week 1 - Data Cleaning & EDA, Week 3 - CLTV, Week 4 - Tableau Dashboard |
| Beckley | Week 2 — Cohort Retention Matrix |
| Sanket | Week 4 — Power BI Dashboard |

---

## Tools Used
Python, Pandas, NumPy, Seaborn, Matplotlib, Jupyter Notebook, 
Power BI, Tableau, Git, GitHub

---

## How We Did It

### Week 1 — Data Cleaning
We started with 541,909 raw transactions. After removing rows with 
missing customer IDs, cancelled orders, negative quantities and 
zero prices, we were left with 397,884 clean rows.

We also added three new columns the analysis depended on:
- CohortMonth — the month each customer made their very first purchase
- InvoiceMonth — the month each individual transaction happened
- TotalPrice — Quantity multiplied by UnitPrice

### Week 2 — Cohort Retention Matrix
We grouped customers by the month they first purchased and tracked 
how many came back each month after that. This gave us a retention 
matrix showing the percentage of each cohort still active in Month 1, 
Month 2, Month 3 and so on.

### Week 3 — CLTV Calculation
We calculated how much each customer was worth by looking at their 
Average Order Value and how frequently they purchased. We then split 
all customers into three equal groups — Low, Medium and High value.

### Week 4 — Visualization & Dashboard
We built the final cohort retention heatmap, retention decay line 
charts, CLTV segment charts and revenue by cohort visuals in both 
Python (Seaborn/Matplotlib) and Tableau/Power BI.

<img width="1163" height="734" alt="cohort dashboard" src="https://github.com/user-attachments/assets/454f1633-d513-4795-b58e-336e8a9c1b3d" />

<img width="818" height="374" alt="Retention % heatmap" src="https://github.com/user-attachments/assets/13e0e25c-8357-4c82-bb60-ee98785acc65" />


---

## What We Found

### Finding 1 — Most Customers Don't Come Back
Across almost every cohort, retention drops to between 15% and 25% 
by Month 2. This means roughly 75–85% of customers never return after 
their first purchase. The sharpest drop happens between Month 1 and 
Month 2 — that's the window the business needs to focus on.

### Finding 2 — December 2010 Customers Were the Most Loyal
The very first cohort (December 2010) showed the strongest long-term 
retention — still at around 26.6% after 13 months. Every cohort after 
that performed slightly worse, suggesting early customers were more 
engaged than later ones.

### Finding 3 — A Small Group of Customers Drive Almost All Revenue
When we segmented customers by CLTV, the top third (High value segment) 
turned out to be responsible for 84.9% of total revenue — despite being 
only 33% of the customer base. The bottom two thirds combined only 
contributed 15.1%. This is a classic Pareto pattern and a significant 
finding for the business.

---

## What We Recommend
1. Send an automated re-engagement message or discount offer to new 
   customers 3–4 weeks after their first purchase — this is the exact 
   window where most churn happens
2. Build a loyalty program specifically for High value customers — 
   losing even a small number of them would have a major impact on revenue
3. Look for ways to move Medium value customers upward — even a 10% 
   shift in that segment would meaningfully change the revenue split

---

## Project Structure
├── SaaS-E-Commerce-...ipynb(main analysis notebook)
├── beckley_week2_cohort_matrix.ipynb
├── dashboard_screenshots/(Tableau & Power BI visuals)
├── README.md
└── .gitignore

## How to Run
1. Download the dataset from the UCI link above
2. Place it in the project folder — do not commit it to GitHub
3. Open the main notebook in Jupyter
4. Run all cells from top to bottom
