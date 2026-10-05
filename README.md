# SWYNEX – Weather Data Cleaning & Analysis

## Project Overview

This project focuses on cleaning, validating, and analyzing historical rainfall data for India.

The dataset contains subdivision-wise monthly and annual rainfall data from 1901 to 2017. The project was completed as part of the SWYNEX Data Analyst Task 1.

## Dataset

- Source: Government of India Open Government Data (OGD) Platform
- Dataset: Sub Divisional Monthly Rainfall from 1901 to 2017
- Original Records: 4,188
- Records After Cleaning: 4,162
- Columns: 19
- Coverage: 1901–2017
- Subdivisions: 36

## Data Cleaning

The following data-cleaning steps were performed using Python:

- Checked dataset structure and data types
- Checked missing values
- Checked duplicate records
- Identified rows with missing monthly rainfall values
- Removed 26 rows containing missing monthly rainfall values
- Verified that no missing values remained
- Verified that no duplicate records remained
- Checked annual rainfall consistency with monthly rainfall totals
- Checked seasonal rainfall consistency

### Cleaning Result

| Check | Result |
|---|---:|
| Original Rows | 4,188 |
| Rows Removed | 26 |
| Final Rows | 4,162 |
| Missing Values After Cleaning | 0 |
| Duplicate Records After Cleaning | 0 |

Small differences between annual/seasonal totals and calculated values were observed due to decimal rounding in the original dataset. The original annual and seasonal values were retained.

## Exploratory Data Analysis

The following analyses were performed:

- Year-wise average annual rainfall
- Highest and lowest rainfall years
- Subdivision-wise average annual rainfall
- Top 10 and bottom 10 rainfall subdivisions
- Monthly average rainfall
- Seasonal rainfall analysis
- Annual rainfall statistics
- Outlier analysis using the IQR method
- Decade-wise rainfall trend

## SQL Analysis

The cleaned dataset was imported into PostgreSQL for analytical queries.

SQL analysis included:

- Total number of records
- Number of unique subdivisions
- Average annual rainfall by subdivision
- Highest and lowest rainfall years
- Monthly average rainfall
- Seasonal rainfall analysis
- Minimum, maximum, and average annual rainfall
- Highest rainfall records
- Decade-wise rainfall trend

## Tools Used

- Python
- Pandas
- Matplotlib
- PostgreSQL
- SQL
- Jupyter Notebook
- GitHub

## Project Outcome

The project transformed the raw historical rainfall dataset into a clean and analysis-ready dataset.

The analysis helps identify rainfall patterns across Indian subdivisions, years, months, seasons, and decades.

## Files

- `cleaned_weather_data.csv` – Cleaned dataset
- `Weather_Data_Cleaning_EDA.ipynb` – Python data cleaning and EDA notebook

## Conclusion

The cleaned dataset is ready for further visualization and dashboard development. The analysis provides useful insights into historical rainfall patterns across different regions and time periods.
