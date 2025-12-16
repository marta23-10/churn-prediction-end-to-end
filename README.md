<div align="center">

# Customer Retention Intelligence
### Predict. Analyze. Retain.

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-Machine%20Learning-orange?style=for-the-badge&logo=scikit-learn)
![Power BI](https://img.shields.io/badge/Power%20BI-Business%20Intelligence-F2C811?style=for-the-badge&logo=powerbi)

<br>

<p align="center">
  <b>An end-to-end Data Science project focusing on reducing customer churn.</b><br>
  From cleaning messy data with Regex to building Machine Learning models and actionable Power BI dashboards.
</p>

[View Notebook](notebooks/customer_churn.ipynb) 

</div>

---

## Business Problem
In the subscription-based economy, acquiring a new customer is **5-25x more expensive** than retaining an existing one. 

**The Goal:** Build a predictive system to identify customers at high risk of churning (`Churn=1`) and understand the key drivers behind their decision.

**Key Questions:**
* Which customers are leaving and why?
* How does customer support interaction (tickets, CSAT) impact loyalty?
* What is the financial impact of potential churn?

---

## Project Workflow

<div align="center">

| Step | Description | Tools Used |
| :--- | :--- | :--- |
| **1. Data Cleaning** | Advanced cleaning using **Regex** to validate numerical columns (removing typos, negative values). | `Pandas`, `Re` |
| **2. EDA** | Exploratory Data Analysis to find correlations (e.g., Contract Type vs. Churn). | `Seaborn`, `Matplotlib` |
| **3. Modeling** | Building a **Random Forest** classifier to predict churn probability. | `Scikit-Learn` |
| **4. Evaluation** | Assessing model performance using Recall (to minimize false negatives) and Feature Importance. | `Confusion Matrix`, `SHAP` |
| **5. Dashboarding** | Interactive dashboard for stakeholders to filter "High Risk" customers. | `Power BI` |

</div>

---

## Key Insights & Visualizations

### 1. Correlation Analysis
*We discovered that `Payment Failures` and `Support Tickets` are the strongest predictors of churn, while high `CSAT Scores` significantly reduce the risk.*

<div align="center">
  <img src="images/correlation_heatmap.png" alt="Correlation Heatmap" width="700"/>
</div>

### 2. Churn Distribution
*Approximately 20% of the customer base churned. The imbalance was handled using class weighting in the model.*

<div align="center">
  <img src="images/churn_distribution1.png" alt="Churn Pie Chart" width="500"/>
</div>

---
