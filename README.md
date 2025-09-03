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

## **Project Workflow**

| Stage | Tool | Purpose |
|-------|------|---------|
| **1. Data Preparation** | SQL | Cleaned, transformed, and enriched raw Telco data with business‑first KPIs and risk flags |
| **2. Model Development** | Python (via GenAI) | Built churn prediction model, evaluated performance, and exported scored data |
| **3. Dashboarding** | Power BI | Created interactive, recruiter‑friendly dashboards with uniform slicers, conditional formatting, and actionable tooltips |

---

## **1. SQL — Upstream Business Logic**
Used MySQL to prepare the Telco dataset for both machine learning and dashboarding.  
Key steps included:

- **Data validation** — Checked for missing `TotalCharges` values using `IS NULL`.  
- **Feature engineering** — Created a binary `churn_flag` for easier aggregation and modeling.  
- **Business insights** — Calculated overall churn rate, churn by contract type, and average monthly charges by churn status.  
- **Model input view** — Created `churn_model_data` view to serve as a clean, analysis‑ready table for the Python model.

---
## **2. Python with GenAI — Automated Model Development**
For the Python stage, leveraged **generative AI** to produce the code for data preprocessing, feature engineering, model training, and evaluation.  

**Key steps performed by the AI‑generated script:**
- **Data ingestion & cleaning** — Loaded dataset, handled missing values, converted `TotalCharges` to numeric.  
- **Feature preprocessing** — Median imputation for numeric features, most‑frequent imputation + one‑hot encoding for categorical features.  
- **Model training** — Random Forest Classifier to predict churn probability.  
- **Model evaluation** — ROC AUC, precision, recall, accuracy, classification report, confusion matrix.  
- **Feature importance** — Ranked drivers of churn.  
- **Output integration** — Saved predictions to CSV and MySQL for direct Power BI use.

---

## **3. Power BI — Interactive Dashboards**
**Pages & Features:**
- **Page 1 — Executive Summary**: High‑level KPIs, churn trends, top at‑risk segments, and revenue impact for quick decision‑making.
- **Page 2 — Churn Drivers**: Ranked predictors of churn with tooltips explaining business implications.
- **Page 3 — High‑Risk Customers**: Slicers to identify and filter churn‑prone customers.


**Design principles:**
- **Uniform slicers** across pages for consistent filtering.  
- **Business‑first KPIs** to keep focus on impact.  
- **Actionable tooltips** that explain *why* a metric matters.  

---

Key Insights
- **Month‑to‑month contracts** have the highest churn rate.
- **Electronic check payments** correlate with higher churn.
- **Tenure** is a strong retention indicator — longer‑term customers churn less.
- **Model ROC AUC**: **0.91** — strong predictive performance.

---

 Dashboard Preview
 Page 1
<img width="1551" height="872" alt="Screenshot 2025-09-03 142844" src="https://github.com/user-attachments/assets/d7955e71-1cbb-483d-af5e-d83841564fad" />

Page 2
<img width="1556" height="867" alt="Screenshot 2025-09-03 142916" src="https://github.com/user-attachments/assets/9a5d2bfd-d1dc-4744-acb0-84d37379066c" />

Page 3
<img width="1875" height="1055" alt="Screenshot 2025-09-03 143004" src="https://github.com/user-attachments/assets/a3019713-d83b-41fe-9c13-55b3c272f723" />



---

  View
- **PBIX file**: 
- **Live Power BI link** https://app.powerbi.com/links/eVZd7FxkO1?ctid=ae9579e4-bb8d-4db0-9b44-127a32feaa7e&pbi_source=linkShare&bookmarkGuid=c5ca50c0-7a98-468b-89ad-60c38e4f14a2

