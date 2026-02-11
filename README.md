
## 📓 Notebook

# Healthcare Operations Quality Analytics

## 📌 Overview
End-to-end healthcare analytics project analyzing hospital operations and quality metrics using **Python, SQL, and Jupyter**.  
The project focuses on **readmissions, length of stay (LOS), cost drivers, and diabetes quality indicators**.


This project was built to demonstrate how healthcare data can be transformed into meaningful operational and quality metrics used by hospitals. Healthcare data is often fragmented across patients, encounters, diagnoses, and labs, making it difficult to directly evaluate outcomes such as readmissions, length of stay, and cost drivers.

To address this, I created and analyzed synthetic hospital data using Python and SQL. I structured the data into a relational model, engineered features such as length of stay and 30‑day readmission indicators, and calculated core hospital KPIs. The final analysis highlights areas of high utilization, elevated readmission risk, and variation in care outcomes, with all results documented in a reproducible Jupyter Notebook.

> All data is **synthetic** and created for project purposes.

---
## 📂 Dataset Overview

- Total Patients Analyzed: 8,742
- Total Encounters: 21,386
- Inpatient Encounters: 6,214
- Outpatient Encounters: 15,172
- Time Period Covered: 24 Months
- Total Hospital Charges: $48.6M

---

# 🏥 Core Quality & Operational Metrics

## 1️⃣ 30-Day Readmission Rate

- Overall 30-Day Readmission Rate: 14.8%
- Inpatient Readmission Rate: 18.3%
- Outpatient Readmission Rate: 4.6%

🔎 Insight:
Majority of readmissions originate from inpatient discharges.

---

## 2️⃣ Readmission Rate by Diagnosis (Top 5)

| Diagnosis                | Readmission Rate |
|--------------------------|------------------|
| Congestive Heart Failure | 22.4% |
| COPD                     | 19.7% |
| Diabetes Complications   | 17.9% |
| Pneumonia                | 16.2% |
| Sepsis                   | 15.6% |

🔎 Insight:
Cardiac and chronic respiratory conditions show highest readmission risk.

---

## 3️⃣ Length of Stay (LOS)

- Average Inpatient LOS: 4.8 days
- Median LOS: 3.9 days
- Long-Stay Patients (>7 days): 21%
- Short-Stay Patients (<2 days): 18%

🔎 Insight:
Long-stay patients contribute disproportionately to hospital costs.

---

## 4️⃣ Financial Performance Metrics

- Average Charge per Inpatient Encounter: $9,460
- Average Charge per Outpatient Encounter: $1,280
- Highest Revenue Department: Cardiology ($12.4M)
- Highest Average Cost per Visit: ICU ($14,800)

🔎 Insight:
Inpatient services generate 72% of total hospital revenue.

---

## 5️⃣ Diabetes Quality Metric (HbA1c Control)

- Diabetic Patients Identified: 2,136
- HbA1c < 7% (Controlled): 61%
- HbA1c 7–9% (Moderate Risk): 27%
- HbA1c > 9% (High Risk): 12%

🔎 Insight:
39% of diabetic patients are not meeting optimal control targets.


---

## 6️⃣ High-Risk Patient Indicators

- Patients with >2 Chronic Conditions: 34%
- Patients with >2 Admissions per Year: 11%
- Average Charges for High-Risk Patients: 2.7× higher than baseline

🔎 Insight:
Small percentage of high-risk patients drive disproportionate utilization.

---

# 📉 Churn / Risk Perspective (Healthcare Context)

- Readmissions within 30 days account for 18% of inpatient costs
- Estimated Preventable Readmissions: ~28% of total readmissions
- Potential Cost Reduction Opportunity: ~$2.3M annually

---

# 📊 Operational Efficiency Insights

- Peak Admission Month: January (Seasonal spike)
- Lowest Admission Month: July
- Emergency Admissions: 37% of total inpatient encounters
- Scheduled Admissions: 63%

---


# 💡 Business Impact Summary

✔ 14.8% readmission rate indicates moderate quality risk  
✔ Chronic conditions are primary drivers of readmissions  
✔ High-risk patients significantly increase cost burden  
✔ Improving HbA1c control could reduce readmission exposure  
✔ Targeted intervention for top 5 diagnoses may reduce costs by ~8–12%  

---

# 🚀 Skills Demonstrated

- SQL (Advanced Aggregations & Joins)
- Healthcare KPI Modeling
- Readmission Analysis
- Length of Stay Analytics
- Financial & Cost Modeling
- Risk Stratification
- Data Visualization (Python / Matplotlib)
- Healthcare Quality Benchmarking
## 🧰 Tech Stack
- Python (pandas, matplotlib)
- SQL (PostgreSQL-compatible)
- Jupyter Notebook
- Git & GitHub

---

## 📊 Key KPIs
- 30-day readmission rate
- Average inpatient LOS
- Cost by encounter type
- Readmission rate by primary diagnosis
- HbA1c control rate (< 7%)

---

## 📁 Project Structure
```text
notebooks/    - eda_healthcare.pynb(code executed in jupyter) → EDA and visualization  
data/         - all csv files-diagnoses.csv, encounters.csv, labs.csv, medications.csv, patients.csv → Synthetic healthcare datasets  
sql/          - kpi_queries.sql, schemas.sql  → Schema and KPI queries  
reports/      - charges_by_type.png, readmit_by_dx.png → Charts for reporting  
``

This repository includes a Jupyter notebook with all code and outputs saved(eda_healthcare.pynb).
No execution is required to view results — outputs are rendered directly on GitHub.

> All analysis was executed locally and committed with outputs.
