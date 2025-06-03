# Predicting-Student-Performance-Using-Excel-Based-Regression
This project uses Multiple Linear Regression in Microsoft Excel to analyze and predict student performance based on academic and lifestyle factors. The goal is to understand how variables such as prior scores, study hours, sleep patterns, and extracurricular activities affect a student's Performance Index.

#  Student Performance Prediction using Multiple Linear Regression (Excel)

## Overview

This project uses **Multiple Linear Regression** in **Microsoft Excel** to analyze and predict student performance based on academic and lifestyle factors. The goal is to understand how variables such as prior scores, study hours, sleep patterns, and extracurricular activities affect a student's **Performance Index**.

> All analysis, modeling, and interpretation were done using **Excel's Data Analysis Toolpak**, emphasizing high interpretability and accessibility.

--------

## 📁 Dataset
- Source: [Kaggle - Student Performance Dataset](https://www.kaggle.com/datasets/nikhil7280/student-performance-multiple-linear-regression)
- Contains both **categorical** and **numerical** variables
- Target Variable: `Performance Index`

-------

##  Key Steps

### 1. **Exploratory Data Analysis (EDA)**
- Used boxplots and bar charts to explore distributions
- Observed narrow, near-normal distribution of performance index
- Analyzed impact of extracurricular activity on distribution

### 2. **Multicollinearity Check**
- Checked correlation among independent variables
- Confirmed no strong multicollinearity — model is stable

### 3. **Model 1 – Initial Regression**
- Predictors: Previous Scores, Sleep Hours, Sample Papers Practiced
- Achieved **Adjusted R² ≈ 0.84**
- All predictors statistically significant (p < 0.05)

### 4. **Model 2 – Improved Regression**
- Added `Hours Studied` and binary-encoded `Extracurricular Activity`
- Achieved **Adjusted R² ≈ 0.98**
- Key finding: **Every additional hour studied increases performance index by ~2.85**

### 5. **Final Prediction Formula**
```
Performance Index =
-34.07 + 0.62*Extracurricular_Yes + 2.85*Hours_Studied
+ 1.01*Previous_Scores + 0.48*Sleep_Hours + 0.19*Sample_Papers
```

---

##  Skills Demonstrated
- End-to-end regression modeling in Excel
- Data cleaning and encoding categorical variables
- Statistical evaluation using R², Adjusted R², and p-values
- Interpretable, actionable insights

---

##  Tools Used
- Microsoft Excel (Data Analysis Toolpak)
- Pivot Tables
- Basic charting (boxplots, bar charts)

---

## 📄 Files Included
- `Student_Performance.xlsx`: Cleaned dataset and regression output
- `Project_Report.pdf`: Step-by-step documentation and analysis
- `README.md`: GitHub project description

---

##  Key Insight
> Hours Studied is the **most impactful predictor**, showing a near-linear effect on student performance, with every additional hour yielding ~2.85 improvement in score — a powerful insight for both educators and students.
