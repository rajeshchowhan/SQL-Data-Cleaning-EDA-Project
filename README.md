# 🔍 Layoffs 2022 – SQL Data Cleaning & EDA Project

## 📄 Overview

This project focuses on cleaning and analyzing a dataset of global tech layoffs using **SQL**. The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/swaptr/layoffs-2022), and includes information about companies, locations, total layoffs, industry, funding, and more.

The project is divided into two main parts:

1. **Data Cleaning** – preparing the data for analysis.
2. **Exploratory Data Analysis (EDA)** – identifying trends, outliers, and insights.

---

## 🧰 Tools Used

- **MySQL / SQL**


## 🧹 Data Cleaning Highlights

- Removed duplicate records using `ROW_NUMBER()`.
- Standardized inconsistent text values (e.g., "CryptoCurrency" → "Crypto").
- Replaced empty strings with `NULL` values and filled missing industry values using self-joins.
- Cleaned and converted the `date` column into proper `DATE` format.
- Removed rows with completely missing key metrics (`total_laid_off`, `percentage_laid_off`).
- Trimmed trailing punctuation (e.g., "United States.") from country names.

---

## 📊 EDA Highlights

- 📈 Identified companies and countries with the **highest layoffs**.
- 🏢 Found companies that laid off **100% of their workforce**.
- 📍 Analyzed layoffs by **location, industry, and company stage**.
- 📆 Analyzed layoffs over **years and months** with **rolling total trends**.
- 🥇 Identified **top 3 companies with most layoffs** per year using window functions.

---

## 🚀 How to Use

1. **Import `layoffs.csv`** into your SQL database as `world_layoffs.layoffs`.
2. Run the script in `Portfolio Project - Data Cleaning.sql` to clean the data and create `layoffs_staging2`.
3. Use `Portfolio Project - EDA.sql` to explore the cleaned data and generate insights.

---

## 👤 Author

**Korra Rajesh**  

> This project is part of my portfolio to demonstrate real-world SQL data cleaning and analytical skills.
