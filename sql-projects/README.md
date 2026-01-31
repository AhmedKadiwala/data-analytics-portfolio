# SQL Project: Layoffs Analysis (2020 March – 2023 March)

## Overview
This project demonstrates **data cleaning and exploratory data analysis (EDA)** on a layoffs dataset containing company, industry, location, and layoff information from **March 2020 to March 2023**. The goal was to clean the raw dataset and analyze trends in layoffs by company, industry, location, and time.

## Project Structure
- `01_data_cleaning.sql` : SQL scripts for cleaning the dataset
- `02_eda.sql` : SQL scripts for exploratory data analysis
- `layoffs_dataset.csv` : Original dataset used for this project

## Data Cleaning Performed
- Created **staging tables** to safely work with raw data.
- Removed **duplicate rows** using `ROW_NUMBER()` and CTEs.
- Standardized text fields:
  - Fixed variations in `industry` (e.g., "Crypto Currency" → "Crypto").
  - Standardized `country` names (removed trailing dots, corrected inconsistencies).
- Converted `date` column from text to proper SQL `DATE` format.
- Handled null and blank values for key columns.
- Dropped unnecessary columns and rows with missing crucial information.

## Exploratory Data Analysis (EDA)
- Identified **companies with the largest layoffs** (single day and total layoffs).  
- Analyzed **layoffs by industry, stage, country, and location**.  
- Generated **monthly and yearly trends**, including rolling totals.  
- Used SQL window functions (`ROW_NUMBER()`, `DENSE_RANK()`) for ranking companies and tracking layoffs over time.

## Key Skills Demonstrated
- SQL Data Cleaning & Transformation
- Window Functions & CTEs
- Aggregations & Grouping
- Handling Nulls & Data Standardization
- Exploratory Data Analysis (EDA)

## Dataset
The dataset contains layoffs data including: company, location, industry, total laid off, percentage laid off, date, stage, country, and funds raised (in millions). The dataset spans **March 2020 to March 2023** and was used for all cleaning and analysis in this project.

