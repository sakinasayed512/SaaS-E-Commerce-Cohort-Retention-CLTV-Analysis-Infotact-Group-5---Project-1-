# SaaS & E-Commerce Cohort Retention & CLTV Analysis

## 📌 Project Overview
This project focuses on analyzing customer behavior for SaaS and E-Commerce business models. By implementing **Cohort Analysis** and calculating **Customer Lifetime Value (CLTV)**, the project aims to uncover patterns in user retention, identify high-value customer segments, isolate transaction anomalies (such as cancellations), and provide data-driven insights to optimize marketing spend and improve customer loyalty.

This analysis was developed by **Group 5 - Infotact Project 1**.

---

## 📂 Repository Structure & Workflow

The repository contains the data pipeline and incremental progress notebooks tracked across the project lifecycle:

* **`data/`**: Directory containing the core transactional dataset.
* **`beckley_week1_cleaning.ipynb`**: Focuses on initial data loading, data profile checking, establishing schema validation, and early exploratory data profiling.
* **`beckley_week2_cohort_matrix.ipynb`**: Builds the core behavioral cohort matrices to evaluate retention metrics across specific user groups over time.
* **`SaaS-E-Commerce-Cohort-Retention-CLTV-Analysis-Infotact-Group-5-Project-1.ipynb`**: The final master notebook documenting exploratory data analysis (EDA), localized cancellation patterns, and finalized cohort logic.

---

## 📊 Key Features & Dataset Highlights

* **Dataset Scale:** Processed and analyzed the `OnlineRetail` dataset containing **541,909 rows** and **8 columns**.
* **Global Footprint:** Checked date ranges and mapped customer behavior tracking **4,372 unique customers** across **38 different countries**.
* **Cohort Retention Analysis:** Tracks monthly/weekly user retention rates using behavioral heatmaps to pinpoint exactly when and where customers drop off.
* **Advanced Cancellation Logic:** Explicitly documents and handles transactional cancellation patterns within the data pipeline to prevent retention distortions.
* **CLTV Modeling:** Calculates the long-term financial value of different customer segments to evaluate brand health.

---

## 🛠️ Tech Stack & Prerequisites

* **Language:** Python
* **Core Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`

### Installation
Ensure you have the required data science libraries installed before running the notebooks:
```bash
pip install pandas numpy matplotlib seaborn jupyter
