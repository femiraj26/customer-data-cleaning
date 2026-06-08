# customer-data-cleaning
A Python data cleaning pipeline built in Google Colab to preprocess customer profile data for future analytics and segmentation.
# Customer Data Cleaning & Preprocessing Pipeline

This repository contains a mini-project dedicated to cleaning and structuring an imperfect customer profiling dataset using Python and Pandas. The pipeline is designed to transform noisy raw data into a reliable format ready for exploratory data analysis (EDA) or machine learning segmentation.

## 📊 Dataset Overview
The raw dataset (`Customers.csv`) contains basic demographic and transactional records of retail customers, featuring columns like:
- `CustomerID`
- `Gender`
- `Age`
- `Annual Income ($)`
- `Spending Score (1-100)`
- `Profession`
- `Work Experience`
- `Family Size`

## 🧼 Cleaning Operations Performed
Using **Pandas** and **NumPy** in a Google Colab environment, the following inconsistencies were handled:
1. **Column Standardization:** Transformed messy, symbol-heavy column headers (like `Annual Income ($)`) into clean `snake_case` formats (`annual_income`).
2. **Categorical Normalization:** Handled trailing whitespaces and capitalization inconsistencies in text fields like `Gender` and `Profession`.
3. **Missing Value Imputation:** Addressed missing data systematically (e.g., filled missing structural integers with `0` or `1` depending on context).
4. **Invalid Entry Auditing:** Identified and filtered out structural anomalies (such as instances where recorded `work_experience` exceeded a customer's `age`).
5. **Deduplication:** Ensured data integrity by removing duplicate `CustomerID` attributes.

## 🚀 How to Run the Project
1. Clone this repository:
   ```bash
  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/femiraj26/customer-data-cleaning/blob/master/Customers_Data_Cleaning.ipynb)
