# World Layoffs Data Cleaning Project

## 📌 Project Overview
This project focuses on cleaning and preparing a real-world layoffs dataset using SQL.

The goal was to perform proper data cleaning before conducting exploratory data analysis (EDA).

---

## 🛠 Tools Used
- MySQL
- SQL (Window Functions, CTEs, Joins)
- GitHub

---

## 🔥 Data Cleaning Steps

### 1️⃣ Created Staging Table
- Copied raw data into a staging table to protect original dataset.

### 2️⃣ Removed Duplicates
- Used ROW_NUMBER() with PARTITION BY.
- Deleted records where row_num > 1.

### 3️⃣ Standardized Data
- Trimmed company names.
- Standardized industry values (e.g., Crypto variations).
- Cleaned country column (removed trailing dots).

### 4️⃣ Converted Date Column
- Converted text date to DATE datatype using STR_TO_DATE().
- Modified column datatype.

### 5️⃣ Handled Missing Values
- Converted blank values to NULL.
- Used self-join to populate missing industry values.
- Removed rows where total_laid_off and percentage_laid_off were both NULL.

---

## 📊 Outcome
The dataset is now clean and ready for exploratory data analysis.

---

## 📂 Files Included
- layoffs.csv
- data_cleaning.sql
