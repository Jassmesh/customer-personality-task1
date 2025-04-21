# customer-personality-task1
Data Cleaning and Preprocessing for Customer Personality Analysis Dataset
# Task 1 – Data Cleaning and Preprocessing

## 🎯 Objective
Clean and prepare the raw Customer Personality Analysis dataset by handling:
- Missing values
- Duplicates
- Inconsistent formats
- Data types

## 🧰 Tools Used
- Python
- Pandas
- Google Colab

## ✅ Cleaning Steps Performed
1. Loaded dataset using `pd.read_csv()` with tab separator.
2. Filled missing values in the `Income` column using the **median**.
3. Removed duplicate rows using `.drop_duplicates()`.
4. Standardized text columns (`Education`, `Marital_Status`) using `.str.strip().str.title()`.
5. Converted the `Dt_Customer` column to `datetime` format.
6. Renamed all column headers to lowercase with underscores using `.str.lower().str.replace(' ', '_')`.
7. Fixed data types:
   - `year_birth` → int
   - `income` → float
   - `dt_customer` → datetime
8. Saved the final cleaned dataset to `cleaned_marketing_campaign.csv`.

## 📁 Files Included
- `marketing_campaign.csv` – Raw dataset (original data from Kaggle)
- `CustomerPersonalityanalysisDataCleaning.ipynb` – Colab notebook with all steps
- `cleaned_marketing_campaign.csv` – Final cleaned dataset
- `README.md` – Summary of work

## 🚀 Outcome
A clean, analysis-ready dataset that can be used for modeling or dashboarding.
