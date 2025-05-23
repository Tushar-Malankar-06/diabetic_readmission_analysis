# Diabetic Hospital Readmission Analysis

This repository presents a comprehensive data science project analyzing diabetic patient readmissions using graph algorithms, logistic regression, and linear/integer programming. The goal is to optimize clinical outcomes, reduce hospital readmission rates, and improve healthcare resource allocation.

## 📌 Project Overview

Hospital readmissions among diabetic patients pose significant challenges for healthcare systems, both in terms of cost and patient well-being. This project analyzes the UCI Diabetes 130-US Hospitals dataset to:

- Predict the risk of readmission within 30 days
- Identify high-risk care pathways
- Optimize patient triage and follow-up care resources
- Understand comorbidity clusters using network analysis

> **Team Members**:  
> Tushar E Malankar  
> Himanshu Sharma  
> Sai Nithin Godi

---

## 📊 Dataset

- **Source**: UCI Diabetes 130-US Hospitals Dataset  
- **Size**: 101,766 diabetic patient encounters from 130 US hospitals (1999–2008)  
- **Key Features**:
  - Admission type/source/disposition
  - Diagnoses (ICD-9 grouped)
  - Medication change status
  - Demographics (age, gender, race)
  - Length of stay, lab procedures, number of medications
  - Readmission status (`<30 days`, `>30 days`, `No`)

---

## 🔧 Techniques Used

### 1. Logistic Regression – Predicting Readmission Risk

- **Objective**: Predict 30-day readmissions using structured clinical and demographic features.
- **AUC**: 0.687 | **Accuracy**: 64%
- **Key Predictors**: Emergency admissions, certain diagnoses, discharge types

### 2. Integer Linear Programming – Patient Triage Optimization

- **Objective**: Identify the top 50 high-risk patients for follow-up under a $10,000 budget
- **Result**: Focused interventions for emergency admissions and patients with complex diagnoses

### 3. Linear Programming – Follow-Up Resource Allocation

- **Objective**: Allocate 600 follow-up hours across departments (Cardiology, Endocrinology, Nephrology)
- **Result**: Optimized cost of $61,000 with majority allocation to Endocrinology (250 hrs)

### 4. Graph Algorithms – Diagnosis Co-Occurrence Network

- **Objective**: Identify comorbid clusters among diagnoses
- **Findings**: Circulatory and Respiratory issues frequently co-occur with Diabetes

### 5. Graph Algorithms – Extended Patient Pathway Network

- **Objective**: Analyze patient journey from admission to discharge
- **Top Pathway**: Emergency Referral → Emergency Admission → No Medication Change → Discharged Home

---

## 🧠 Key Insights

- Emergency admissions are a major predictor of readmission and should be prioritized for post-discharge care.
- Endocrinology is the most resource-demanding department for follow-ups in diabetic care.
- Common comorbidity clusters support the development of bundled care protocols.
- Pathway variations (especially in medication change) may contribute to inconsistent patient outcomes.

---

## 📁 Folder Structure

