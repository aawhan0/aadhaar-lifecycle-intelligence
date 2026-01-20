# Aadhaar Lifecycle Intelligence & Maturity Analysis

**UIDAI Data Hackathon 2026**  
**Team ID:** UIDAI_14145  

**Team Members:**  
- Aawhan Vyas  
- Akshat Sharma  

---

## 📌 Project Overview

Aadhaar has evolved from a one-time enrolment system into a lifelong digital identity. While new enrolments have largely stabilised, continuous demographic and biometric updates now drive the majority of operational demand on Aadhaar infrastructure.

This project presents a **lifecycle-based analytical framework** to study Aadhaar enrolment, demographic updates, and biometric updates together, rather than in isolation. The objective is to identify meaningful trends, detect operational anomalies, and derive early warning indicators that can support proactive governance and system planning.

---

## 🧠 Aadhaar Lifecycle Intelligence & Maturity Framework (ALIMF)

The **Aadhaar Lifecycle Intelligence & Maturity Framework (ALIMF)** integrates three key stages of Aadhaar usage:

1. **Enrolment Stage** – Initial Aadhaar creation and system expansion  
2. **Demographic Update Stage** – Life-event driven updates such as address or name changes  
3. **Biometric Update Stage** – Biometric refreshes due to ageing, biometric drift, or accessibility factors  

Built on top of these stages are:
- **Anomaly Detection** to identify district-level operational stress  
- **Predictive Indicators (Early Warning)** to anticipate short-term service demand  

This framework forms the conceptual foundation for all analysis in this repository.

---

## 📊 Datasets Used

All datasets are aggregated and anonymised Aadhaar datasets provided by UIDAI as part of the hackathon:

- **Enrolment Data** – New Aadhaar enrolments  
- **Demographic Update Data** – Life-event driven demographic updates  
- **Biometric Update Data** – Biometric refresh activity  

The datasets support univariate, bivariate, and trivariate analyses at temporal and district levels.

---

## 📁 Data Availability Note

The Aadhaar datasets used in this project are aggregated and anonymised datasets provided by UIDAI as part of the hackathon.

Due to file size constraints and data usage guidelines, processed CSV files are not included in this repository. All data processing steps are fully documented in the notebooks, and the analysis can be reproduced by re-running the notebooks using the original datasets provided by UIDAI.

---

## 🔍 Methodology

The analysis follows a structured and reproducible workflow:

- Consolidation of multiple CSV files for each dataset  
- Data cleaning, date parsing, and column standardisation  
- District-level and temporal aggregations  
- Exploratory data analysis (univariate, bivariate, trivariate)  
- Statistical anomaly detection using deviation from historical baselines  
- Short-term demand forecasting using moving-average based indicators  

All steps are implemented using Python and Jupyter notebooks.

---

## 📈 Key Analyses & Insights

- **Enrolment Trends:** New Aadhaar enrolments show stabilisation, indicating a mature identity ecosystem.  
- **Update Demand Patterns:** Demographic and biometric updates dominate Aadhaar activity in mature regions.  
- **Operational Anomalies:** District-level spikes in biometric and demographic updates highlight potential infrastructure stress, targeted update drives, or migration effects.  
- **Early Warning Signals:** Predictive indicators help flag periods of abnormal demand for proactive resource planning.

---

## 🗂 Repository Structure

```text
.
├── notebooks/
│   ├── 00_problem_framework_overview.ipynb
│   ├── 01_data_merge_clean.ipynb
│   ├── 02_eda_insights.ipynb
│   ├── 03_anomaly_detection.ipynb
│   └── 04_predictive_indicators.ipynb
│
├── processed/
│   ├── enrolment_clean.csv
│   ├── demographic_clean.csv
│   └── biometric_clean.csv
│
├── figures/
│   ├── alimf_framework.png
│   ├── univariate_enrolment.png
│   ├── bivariate_trend.png
│   ├── biometric_anomaly.png
│   ├── demographic_anomaly.png
│   └── prediction_trend.png
│
└── README.md


```

---

## ℹ️ Context

This project was developed as part of the UIDAI Data Hackathon 2026.  
Additional information about the hackathon and datasets is available on the official UIDAI hackathon portal.

