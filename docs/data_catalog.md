# 📊 Data Catalog – COVID-19 Data Exploration Project

## 📌 Overview
This document provides detailed information about the datasets used in the COVID-19 Data Exploration project. It includes column definitions, data types, and descriptions for both datasets.

---

# 🗂 1. Dataset: CovidDeaths.xlsx

## 📊 Description
This dataset contains information about COVID-19 cases, deaths, and population across different countries and dates.

---

## 📑 Columns

| Column Name     | Data Type   | Description |
|----------------|------------|-------------|
| location       | Text       | Name of the country or region |
| continent      | Text       | Continent of the location (NULL for aggregated regions like World) |
| date           | Date       | Reporting date |
| total_cases    | Numeric    | Total confirmed COVID-19 cases |
| new_cases      | Numeric    | New cases reported on that date |
| total_deaths   | Numeric    | Total deaths due to COVID-19 |
| new_deaths     | Numeric    | New deaths reported on that date |
| population     | Numeric    | Total population of the country |

---

## ⚠️ Data Notes
- Some rows contain **NULL values** in the continent column (aggregated data)  
- Numeric columns may require **data type conversion** for calculations  
- Division operations handled using `NULLIF()` to avoid errors  

---

# 🗂 2. Dataset: CovidVaccinations.xlsx

## 📊 Description
This dataset contains information about COVID-19 vaccination progress across countries.

---

## 📑 Columns

| Column Name        | Data Type | Description |
|-------------------|----------|-------------|
| location          | Text     | Name of the country or region |
| continent         | Text     | Continent of the location |
| date              | Date     | Reporting date |
| new_vaccinations  | Numeric  | Number of new vaccinations administered on that date |

---

## ⚠️ Data Notes
- Vaccination data is recorded daily  
- Missing values may exist for some dates/countries  
- Used in combination with CovidDeaths dataset via JOIN  

---

# 🔗 Data Relationships

| Key Column | Description |
|-----------|------------|
| location  | Common key used to join both datasets |
| date      | Combined with location to ensure accurate mapping |

👉 Join Condition used in SQL:
```sql
ON dea.location = vac.location 
AND dea.date = vac.date
