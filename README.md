# Pandas_Analysis

This repository contains a detailed data analysis project using the pandas library to perform data cleaning, transformation, and exploration on athletes' bios and Olympic data. The main focus is on understanding and manipulating data using pandas functions such as grouping, merging, pivoting, and handling missing data. The project also explores advanced techniques like interpolation, ranking, and categorization.

## Project Overview

The project demonstrates various data analysis techniques with the following tasks:

1. **Data Cleaning and Preprocessing**:
   - Handling missing values and cleaning data.
   - Interpolating missing values in numerical columns like `height_cm` and `weight_kg`.

2. **Data Transformation**:
   - Performing `groupby` operations for aggregating and summarizing data.
   - Creating new columns based on conditions, such as `weight_category` and `height_category`.
   - Using `pivot` to restructure the dataset for easier analysis.

3. **Advanced Data Analysis**:
   - Merging datasets to combine related data.
   - Categorizing data based on attributes like country and weight.
   - Using pandas functions like `rank()`, `shift()`, and `interpolate()` for more advanced analysis.

4. **Exploratory Data Analysis (EDA)**:
   - Gaining insights into data distributions and correlations.
   - Using data aggregation to group athletes by country or other attributes.

## Repository Structure

- **analysis.ipynb**: Jupyter Notebook containing the full analysis, including data cleaning, transformation, and exploration steps.
- **athletes_bio.csv**: CSV file containing athlete biography data (including `athlete_id`, `born_country`, `height_cm`, `weight_kg`, etc.).
- **noc_regions.csv**: CSV file containing data about National Olympic Committees (NOCs) and regions.
- **athletes_bio.parquet**: Parquet file version of the athlete data for faster access.
- **noc_regions.parquet**: Parquet file version of the NOC regions data.

## Key Concepts Demonstrated

### 1. Data Cleaning and Interpolation
- Handling missing or `NaN` values in the `height_cm` and `weight_kg` columns using interpolation.
- Example:
  ```python
  df[['height_cm', 'weight_kg']] = df[['height_cm', 'weight_kg']].interpolate()
