
# Identifying Gaps in Aadhaar Enrolment: A Demographic and Regional Analysis

**UIDAI Government Hackathon 2025 | End-to-End Data Analysis Project**

---

## 📌 Project Overview

This project was developed during the **UIDAI Government Hackathon** to analyze real Aadhaar enrolment data (2020–2025) and identify critical **demographic and regional gaps** in India’s largest digital identity programme.

By combining **data cleaning, feature engineering, exploratory data analysis (EDA), and risk scoring**, the project delivers **actionable insights** and **policy recommendations** to help UIDAI and state governments achieve 100% inclusive enrolment — especially for children (0-5 years).

**Full PDF Report** (included in repo): [UIDAI-DATA-ANALYSIS-HACKATHON.pdf]
**Live Jupyter Notebook**: [Aadhaar_Enrolment_Analysis.ipynb]

---

## 🎯 Problem Statement

Despite nationwide coverage, significant enrolment gaps persist across age groups and geographies. Children (0-5 years) and certain districts show alarmingly low enrolment, impacting access to welfare, education, and financial services.

**Key Questions Answered:**
1. Which regions show low Aadhaar enrolment among children (0-5)?
2. Are school-age children (5-17) being systematically missed?
3. Do some districts lag significantly in adult (18+) enrolment?
4. How does enrolment change over time?
5. Can we flag high-risk districts needing urgent intervention?

---

## 📍 Objectives

- Perform exploratory data analysis on Aadhaar enrolment data
- Conduct geographic and temporal gap analysis
- Identify districts and age groups for targeted intervention
- Build a **District Risk Score** for prioritized government action

---

## 📊 Dataset

- **Source**: UIDAI-provided enrolment records (hackathon dataset)
- **Files**: 
  - `Aadhaar_enrolment_0-5.csv`
  - `Aadhaar_enrolment_5-17.csv`
  - `Aadhaar_enrolment_18+.csv`
- **Time Period**: 2020-03 to 2026-01
- **Columns**: Date, State, District, Pincode, Age_0-5, Age_5-17, Age_18+, Total_Enrolment
- **Size**: ~1 million+ rows after merging

---

## 🛠️ Tech Stack & Skills Demonstrated

| Category              | Technologies Used                          |
|-----------------------|--------------------------------------------|
| **Language**          | Python 3.12                                |
| **Data Processing**   | Pandas, NumPy                              |
| **Visualization**     | Matplotlib, Seaborn                        |
| **Environment**       | Jupyter Notebook                           |
| **Others**            | Data Cleaning, Feature Engineering, Risk Scoring Logic |


---

## 🔍 Key Exploratory Data Analysis (EDA) Highlights

### 1. National Age-wise Distribution
- **0-5 years**: Only ~5-7% of total enrolments (critically low)
- **5-17 years**: Highest enrolment (school & welfare driven)
- **18+ years**: Strong but plateaued

### 2. Top 10 States by Age Group (Heatmap)
| State            | 0-5      | 5-17      | 18+       | Total     |
|------------------|----------|-----------|-----------|-----------|
| Uttar Pradesh    | 311,727  | 473,205   | 1,002,431 | 1,787,363 |
| Bihar            | 254,813  | 327,043   | 393,733   | 975,589   |
| Madhya Pradesh   | 363,244  | 115,172   | 5,476     | 483,892   |
| ...              | ...      | ...       | ...       | ...       |

### 3. Districts with Lowest Child (0-5) Enrolment
- Multiple districts in Jharkhand, Assam, and Northeast show **zero or near-zero** child coverage.

### 4. Monthly Time-Series Trend (2020-2026)
- Sharp rise in 2023-2024
- Seasonal dips during monsoon months
- Recent recovery in 2025-26

### 5. District Risk Scoring System (Built-in Logic)
- High-risk districts flagged using weighted formula:
  - Low child enrolment (weight 40%)
  - Low school-age enrolment (weight 30%)
  - Low total enrolment (weight 30%)

**Top 5 High-Risk Districts** shown in report.

---

## 💡 Key Insights

1. **Children 0-5 years** are the most underserved age group — risking exclusion from nutrition & education schemes.
2. Uttar Pradesh, Bihar, and Madhya Pradesh contribute ~40% of national enrolments.
3. Several districts show near-zero child coverage despite high adult enrolment.
4. Enrolment spikes align with government outreach programs and school registration drives.
5. Clear seasonal patterns — mid-year months need targeted campaigns.

---

## 📌 Policy Recommendations

1. **Mobile Aadhaar Units** in high-risk districts
2. **School-linked drives** for ages 5-17
3. **Hospital & Anganwadi-based enrolment** for newborns (0-5)
4. **Pincode-level monitoring dashboards** for real-time tracking
5. **Incentive programs** for parents in low-coverage areas

---

## 🎯 Conclusion

This project transforms raw UIDAI enrolment data into **actionable intelligence**. The combination of **EDA, feature engineering, risk scoring, and policy recommendations** demonstrates how data can directly support government initiatives for inclusive digital identity coverage.



---

## 📂 Project Structure
