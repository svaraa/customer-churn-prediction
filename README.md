# Customer Churn Analysis – Telco Customers

An end-to-end analytical project exploring telecom customer churn using Python (Jupyter Notebook) for data preparation and Tableau for dashboard creation. The goal is to identify why customers leave, which segments are at highest risk, and provide actionable insights for churn reduction.
---

## 📊 Live Dashboard

🔗 **Interactive Tableau Dashboard:** [View on Tableau Public](https://public.tableau.com/app/profile/svara.masurekar/viz/ChurnDashboard_17632888591420/Dashboard2?publish=yes)

This dashboard includes:

- Overall churn KPIs  
- Churn by tenure band  
- Churn by contract type  
- Monthly charges impact on churn  
- Churn by internet service type  
- Churn by support services (Online Backup, Tech Support, Online Security)  
- Demographic churn factors (Gender, Senior Citizen, Dependents)  
- Interactive filters for deeper exploration
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
```
---

## 🧹 Data Cleaning & Preparation (Python)

Key steps performed:
- Removed duplicate records  
- Converted `TotalCharges` to numeric  
- Filled missing values  
- Created a **Tenure Group** categorical field  
- Encoded churn and service-related features  
- Exported a clean dataset (`customer_churn_clean.csv`) for Tableau  

---

## 🔍 Exploratory Data Analysis (EDA)

Key patterns analyzed in Jupyter Notebook:
- Distribution of churn
- Pricing patterns
- Tenure behavior of retained vs churned customers
- Churn by service subscriptions
- Churn by demographics

Visuals included:
- Histograms
- Boxplots
- Countplots
- Correlation heatmaps

---

## 📊 Tableau Visualization Highlights

Your dashboard features the following charts:

### 🔹 KPIs
- **Overall Churn %**
- **Average Monthly Charges (Churned vs Retained)**
- **Average Tenure (Churned vs Retained)**

### 🔹 Customer Segmentation
- Churn by **Contract Type**
- Churn by **Tenure Band**
- Churn by **Gender**
- Churn by **Senior Citizen**
- Churn by **Dependents**

### 🔹 Service-based Insights
- Churn by **Internet Service**
- Churn by **Support Services**
- Churn by **Phone Service**
- Churn by **Multiple Lines**

---

## 📈 Key Insights

### 1. Contract Type Has the Largest Impact
- **Month-to-month contracts** have the highest churn.
- 1- and 2-year contracts show much lower churn.

### 2. Tenure Strongly Predicts Loyalty
- Newer customers churn more.
- Long-tenure customers show very low churn.

### 3. Support Services Reduce Churn
- Lack of **Tech Support**, **Online Security**, and **Online Backup** is associated with higher churn.

### 4. Monthly Charges Affect Churn
- Churned customers tend to have **higher monthly charges**.

### 5. Demographic Trends
- **Senior Citizens** churn more.
- Customers with **Dependents** churn less.

