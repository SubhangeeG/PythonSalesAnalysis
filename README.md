# Diwali Sales Exploratory Data Analysis (EDA)

## Project Overview
This project performs data cleaning, preprocessing, and exploratory data analysis (EDA) on a Diwali sales dataset containing 11,251 customer transaction records. The objective is to clean raw retail data, handle missing values, correct data types, and uncover key demographic and purchasing insights to help business stakeholders understand customer behavior and sales performance.

## Key Technical Contributions & Data Pipeline

### 1. Data Cleaning & Preprocessing
- **Blanks & Unused Column Removal**: Evaluated missing data using `pd.isnull().sum()` and dropped unpopulated columns (`Status`, `unnamed1`) to optimize memory usage and reduce clutter.
- **Null Value Handling**: Identified and removed rows containing null values in the `Amount` field to ensure analytical accuracy.
- **Data Type Casting**: Converted floating-point values in the `Amount` column into integer format (`int32`) for cleaner numerical operations and consistency.
- **Feature Inspection & Schema Assessment**: Inspected DataFrame shape (11,251 rows × 15 initial columns), datatypes via `.info()`, and key column names.

### 2. Exploratory Data Analysis (EDA)
- **Statistical Profiling**: Conducted summary statistics using `.describe()` on key numerical fields (`Age`, `Orders`, `Amount`) to assess central tendencies, standard deviations, and quartiles across transactions.
- **Demographic Segmentation**: Initiated demographic analysis on customer segments (e.g., analyzing purchasing trends by `Gender`, `Age Group`, `Occupation`, and `Zone`).

