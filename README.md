# Telco-Churn-Analysis
"Churn prediction and business insights project using SQL, Python,Power BI and GenAI

Summary
This project tackles the challenge of **customer churn** for a fictional telecom provider.  
Using **SQL** for querying and EDA, **Python** for data prep and predictive modeling, and **Power BI** for interactive storytelling while leveraging **GenAi** , it delivers:
- **Predictive churn scores** for every customer
- **Actionable insights** into churn drivers

---

**Tech Stack**

| Layer         | Tools & Libraries |
|---------------|-------------------|
| Data Prep     | SQL, Pandas, NumPy |
| Modeling      | Scikit‑learn (Random Forest) |
| Visualization | Power BI| |
| Platform     | Jupyter Notebooks, GitHub |
|GenAI          | Copilot| 

---


---

 Business Problem
Customer churn directly impacts revenue and growth.  
By predicting churn and understanding its drivers, the business can **proactively retain customers** and **reduce revenue loss**.

---
Workflow
**Data Pipeline → Model Training → Business Insights → Model Validation**

1. **Data Extraction and Analysis (SQL)** — Pull customer, contract, and service data, Perform Explaratory Data Analysis
2. **Data Cleaning & Feature Engineering (Python)** — Handle missing values, encode categories, create business‑first KPIs.
3. **Model Training (Random Forest)** — Predict churn probability for each customer.
4. **Evaluation** — ROC AUC, precision, recall, accuracy, confusion matrix, ROC curve.
5. **Visualization (Power BI)** — Interactive dashboards for decision‑makers.

---

Key Insights
- **Month‑to‑month contracts** have the highest churn rate.
- **Electronic check payments** correlate with higher churn.
- **Tenure** is a strong retention indicator — longer‑term customers churn less.
- Model ROC AUC: **0.91** — strong predictive performance.

---

## 📷 Dashboard Preview
![Dashboard Page 1](images/page1_overview.png)  
![Dashboard Page 2](images/page2_drivers.png)  
![Dashboard Page 3](images/page3_predictions.png)  
![Dashboard Page 4](images/page4_model_performance.png)

---

 How to View
- **PBIX file**: [Download here](powerbi/telco_churn.pbix) *(requires Power BI Desktop)*
- **PDF export**: [View here](powerbi/telco_churn.pdf)
- **Live Power BI link** *(if published)*: [View Online](#)

