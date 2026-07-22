# 🎓 Student Dropout & Academic Success Analysis

A data analytics and visualization project focused on identifying early risk factors, financial drivers, and academic indicators that lead to university student dropouts.

---

## 📌 1. Executive Summary & Context

Understanding the root causes of student attrition is vital for higher education institutions to implement early-intervention strategies. Using a dataset of **4,424 students** across **35 attributes**, this project analyzes key drivers—such as financial stability, academic performance, and demographics—that influence whether a student graduates, remains enrolled, or drops out.

### **Key Metrics at a Glance**
* **Total Students Analyzed:** 4,424
* **Overall Dropout Rate:** 32.1%
* **Graduate Rate:** 49.9%
* **Currently Enrolled:** 18.0%

---

## 💡 2. Primary Findings (Key Business Insights)

* 💳 **Tuition Fee Defaulters:** Students whose tuition fees are **not up to date** have a staggering **86.6% dropout rate**, compared to **24.7%** for those with up-to-date fees. Fee payment status is the single strongest predictor of attrition.
* 🎓 **Scholarship Impact:** Non-scholarship holders exhibit a **38.7% dropout rate**, whereas scholarship holders have a dropout rate of only **12.2%** (more than 3x lower).
* 📚 **Academic Progression:** Dropouts exhibit a sharp decline in approved curricular units by the end of the 2nd semester compared to graduates.

---

## 🖥️ 3. Dashboard Architecture (Power BI / Excel)

The interactive dashboard is structured into **3 core pages**:

### **Page 1: Executive Overview**
* **KPI Cards:** Total Students (4,424) | Overall Dropout Rate (32.1%)
* **Donut Chart:** Target Split (Graduate vs Dropout vs Enrolled)

### **Page 2: Risk Factor Analysis**
* **Bar Charts:**
  * Dropout Rate % by **Scholarship Holder** (Yes vs No)
  * Dropout Rate % by **Tuition Fee Status** (Up to Date vs Pending)
  * Dropout Rate % by **Gender**
  * Dropout Rate % by **Debtor Status** (Financial liabilities)

### **Page 3: Academic Performance Trends**
* **Scatter / Bar Chart:** Average *Curricular units 2nd sem (approved)* grouped by Target outcome.
* **Bar Chart Comparison:** 1st Semester Average Grade comparison across Graduates vs Dropouts.

---

## 🔍 4. Exploratory Data Analysis (Python Focus)

The accompanying Python Notebook (`student_analysis.ipynb`) includes exploratory data analysis using Pandas crosstabs and groupbys to evaluate additional factors:
* **Age at Enrollment:** Segmenting into `<20`, `20-25`, and `25+` age buckets to measure mature student risk.
* **Displaced Status:** Evaluating dropout variance among relocated vs local students.
* **Parental Qualifications:** Analyzing correlations between parent education levels and student completion rates.

---

## 📦 5. Deliverables & Repository Structure

```text
├── README.md                           <- Project Overview and Documentation
├── data/
│   └── student_dropout.csv             <- Raw Dataset (4,424 rows, 35 columns)
├── notebooks/
│   └── student_analysis.ipynb          <- Python EDA Notebook (Pandas Crosstabs/Groupbys)
├── dashboards/
│   └── student_dropout_analysis.pbix   <- Power BI Dashboard (3 Pages)
└── assets/
    ├── dashboard_overview.png          <- Dashboard Screenshots
    └── dashboard_risk_factors.png