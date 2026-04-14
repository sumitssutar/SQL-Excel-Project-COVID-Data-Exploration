# 🦠 COVID-19 Data Exploration (Excel & SQL Project)

## 📌 Project Overview
This project explores global COVID-19 data using SQL and Excel to uncover trends in infections, deaths and vaccinations.  
The dataset was cleaned, transformed and analyzed to generate meaningful insights for understanding the pandemic impact.

---

## 🧩 Business Problem
There is a lack of structured insights to understand:
- Infection spread across countries  
- Death rates and severity  
- Vaccination progress globally  

This makes it difficult to analyze trends and support data-driven decisions.

---

## 🎯 Goal
Analyze COVID-19 data using SQL to identify patterns in cases, deaths and vaccinations for better global insights.

---

## 📊 Dataset Description

### 🗂 CovidDeaths
- location  
- date  
- total_cases  
- new_cases  
- total_deaths  
- population  
- continent
- etc...

### 🗂 CovidVaccinations
- location  
- date  
- new_vaccinations  
- continent
- etc...  

---

## 🧹 Data Preparation
- Cleaned and formatted Excel datasets  
- Ensured consistency for SQL joins  
- Converted data types for calculations  
- Handled NULL and division errors using `NULLIF()`  

---

## 🛠 SQL Techniques Used
- Aggregate Functions (SUM, MAX)  
- JOINS  
- Window Functions (`SUM() OVER PARTITION BY`)  
- CTE (Common Table Expressions)  
- Temp Tables  
- CREATE VIEW  
- Data Type Conversion  

---

## 🔍 Key Insights
- Infection and death rates vary significantly across countries  
- Some countries show high infection but lower death rates  
- Vaccination rollout differs widely across regions  
- Rolling vaccination trends show steady progress over time  
- Population size impacts overall COVID impact analysis  

---

## 💼 Business Impact
- Helps understand global pandemic trends  
- Supports public health analysis  
- Enables country-wise comparison  
- Provides foundation for BI tools like Power BI/Tableau  

---

## 🛠 Tools Used
- Microsoft Excel  
- SQL Server (SSMS)  
- SQL  

---

## 📂 Repository Structure

```bash
covid19-data-exploration-sql-excel/
│
├── sql/
│   └── SQL Queries=Data Exploration on Covid Data.sql
│
├── datasets/
│   ├── CovidDeaths.xlsx
│   ├── CovidVaccinations.xlsx
│
├── docs/
│   └── data_catalog.md
│
├── README.md
└── .gitignore
```

---

## 🛡️ License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and share this project with proper attribution.

## 🌟 About Me

Hi there! I'm **Sumit Sutar**. An experienced Data Analyst who uncovers hidden trends, patterns and anomalies and leverages business intelligence to generate insights, improve operational efficiency and drive organizational growth.

Let's stay in touch! Feel free to connect with me on the following platforms:

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sumitsutar321)
