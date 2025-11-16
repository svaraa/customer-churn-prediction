# Customer Churn Analysis – Telco Customers

End-to-end data analysis and BI project exploring telecom customer churn using Python and Tableau.  
The goal is to understand **why customers leave** and which segments are at highest risk.

---

## 📊 Live Dashboard

🔗 **Interactive Tableau Dashboard:** [View on Tableau Public](https://public.tableau.com/app/profile/svara.masurekar/viz/ChurnDashboard_17632888591420/Dashboard2?publish=yes)

---

## 🧾 Dataset

- Source: Open Telco Customer Churn dataset (7,000+ customers)
- Each row = one customer
- Key fields:
  - Demographics: gender, senior citizen, dependents
  - Services: phone, internet, streaming, support services
  - Billing: contract, payment method, monthly and total charges
  - Target: `Churn` (Yes/No)

---

## 🔍 Business Questions

1. What is the **overall churn rate**?
2. Which **contract types** and **tenure bands** have the highest churn?
3. Do **support services** (online security, tech support, backup) reduce churn?
4. How do **monthly charges** and **internet type** relate to churn?
5. Are there notable differences by **senior citizen status, gender or dependents**?

---

## 🛠️ Tech Stack

- **Python**: pandas, numpy, matplotlib, seaborn
- **Jupyter Notebooks**: data cleaning & exploratory analysis
- **Tableau Public**: interactive dashboard & visual storytelling
- **Git & GitHub**: version control and project hosting

---

## 📂 Project Structure

```text
data/
  Telco-Customer-Churn.csv          # raw dataset
  customer_churn_clean.csv          # cleaned dataset

notebooks/
  01_data_cleaning.ipynb            # data loading & cleaning pipeline
  02_data_analysis.ipynb            # exploratory analysis & feature summaries

dashboards/
  customer_churn_dashboard.twbx     # Tableau workbook

images/
  dashboard_overview.png            # screenshot used in README
