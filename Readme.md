# UIDAI Data Hackathon 2026  
## Aadhaar Enrollment, Demographic & Biometric Data Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-EDA-green)
![Hackathon](https://img.shields.io/badge/UIDAI-Data%20Hackathon%202026-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 👥 Team
- **Isha Shukla**  
- **Yash Bhatt**

---

## 📌 Short Description (Hackathon Summary)

This project analyzes anonymized Aadhaar enrollment, demographic update, and biometric update data to uncover meaningful patterns, trends, and anomalies across time, geography, and age groups. The goal is to convert large-scale administrative data into actionable insights that support inclusive, data-driven governance and improved Aadhaar-enabled service delivery.

---

## 🧠 Problem Statement

Aadhaar is a foundational pillar of India’s digital public infrastructure, with over 1.3 billion issued identities and billions of transactions annually. While coverage is high, regional disparities, update spikes, and anomalies still exist. Understanding these patterns is critical for improving service accessibility, identifying migration or compliance-driven behavior, and strengthening governance decisions.

---

## 🎯 Objectives

- Analyze Aadhaar activity **over time** (day, month, seasonality)
- Perform **geographical analysis** (state, district, region)
- Study **age-wise enrollment and update behavior**
- Detect **spikes, anomalies, and unusual penetration patterns**
- Identify insights linked to **migration, policy drives, or compliance**

---

## 📂 Dataset Overview

The analysis uses anonymized datasets provided for the **UIDAI Data Hackathon 2026**:

### 1️⃣ Enrollment Dataset
- Age groups: `0–5`, `5–17`, `18+`
- Attributes: Date, State, District, Pincode, Enrollment counts

### 2️⃣ Demographic Update Dataset
- Age groups: `5–17`, `18+`
- Attributes: Date, State, District, Pincode, Update counts

### 3️⃣ Biometric Update Dataset
- Age groups: `5–17`, `18+`
- Attributes: Date, State, District, Pincode, Update counts

Each dataset is split across multiple CSV files and aggregated during preprocessing.

---

## 🛠 Methodology

### 1. Data Aggregation
- Merged multiple CSV files per dataset
- Verified schema consistency and data types

### 2. Data Cleaning
- Removed invalid entries (e.g., garbage state values)
- Standardized state and district names
- Applied **pin-code based reverse mapping** for geographic accuracy

### 3. Feature Engineering
- Converted date fields to datetime format
- Extracted `Month`, `Weekday`, and `Region`
- Created total activity metrics across age groups

### 4. Exploratory Data Analysis (EDA)
- Descriptive statistics
- Trend and seasonality analysis
- Region-wise, state-wise, and district-level insights
- Comparative analysis across all three datasets

---

## 📊 Key Insights

- Clear **weekday and seasonal trends** in Aadhaar interactions
- Significant **regional variation** in enrollment and update intensity
- Certain districts show **sudden spikes**, indicating migration or policy drives
- North and North-East regions exhibit notable behavioral differences
- Over-100% penetration in some regions suggests migration or correction cycles

---

## 🧩 Tools & Technologies

- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **Jupyter Notebook**

---

## 📁 Repository Structure

```text
├── api_data_aadhar_enrollment/
├── api_data_aadhar_demographic/
├── api_data_aadhar_biometric/
├── notebooks/
│   ├── enrollment_analysis.ipynb
│   ├── demographic_analysis.ipynb
│   └── biometric_analysis.ipynb
├── appendix/
│   └── reusable_analysis_code.py
├── README.md
