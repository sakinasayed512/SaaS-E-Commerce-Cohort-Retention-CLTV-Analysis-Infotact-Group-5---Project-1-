# SaaS & E-Commerce Cohort Retention & CLTV Analysis

## 📌 Project Overview
This project focuses on analyzing customer behavior for SaaS and E-Commerce business models using the `OnlineRetail` dataset. By implementing **Cohort Analysis** and calculating **Customer Lifetime Value (CLTV)**, the project aims to:
* Uncover granular patterns in user retention and behavioral trends over time.
* Identify high-value customer segments to help optimize marketing spend.
* Isolate transaction anomalies (such as cancellations) to maintain data integrity.
* Provide data-driven insights to improve long-term customer loyalty and evaluate overall brand health.

This analysis was developed by **Group 5 - Infotact Project 1**.

---

## 📂 Repository Structure & Workflow
The repository contains the data pipeline and incremental progress notebooks tracked across the project lifecycle:

* **`data/`**: Directory containing the core transactional dataset.
* **`feature-sakina-work`**: Focuses on initial data loading, data profile checking, establishing schema validation, and early exploratory data profiling.
* **`beckley_week2_cohort_matrix.ipynb`**: Builds the core behavioral cohort matrices to evaluate retention metrics across specific user groups over time.
* **`SaaS-E-Commerce-Cohort-Retention-CLTV-Analysis-Infotact-Group-5-Project-1.ipynb`**: The final master notebook documenting advanced exploratory data analysis (EDA), localized cancellation patterns, and finalized cohort logic.

---

## 📊 Key Features & Dataset Highlights
* **Dataset Scale**: Processed and analyzed a transactional dataset containing over **540,000 rows** and **8 core columns**.
* **Global Footprint**: Tracked unique customer behavior across more than **4,300 unique customers** spanning **38 different countries**.
* **Cohort Retention Analysis**: Tracks monthly and weekly user retention rates using behavioral heatmaps to pinpoint exactly when and where customers drop off.
* **Advanced Cancellation Logic**: Explicitly documents and handles transactional cancellation patterns within the data pipeline to prevent retention distortions.
* **CLTV Modeling**: Calculates the long-term financial value of different customer segments to forecast revenue and guide acquisition strategy.

---

## 🛠️ Tech Stack & Prerequisites
* **Language**: Python
* **Core Libraries**: `pandas`, `numpy`, `matplotlib`, `seaborn`

### Installation
Ensure you have the required data science libraries installed before running the notebooks:

```bash
pip install pandas numpy matplotlib seaborn jupyter
