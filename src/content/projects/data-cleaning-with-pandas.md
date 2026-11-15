---
title: "Data Cleaning With Pandas"
repo: "aniekanudo-MD/Data_cleaning_with_Pandas"
category: "Data Science"
description: "A data cleaning project that transforms a messy sales dataset into a clean, analysis-ready format using Pandas. Demonstrates essential data preprocessing techniques including duplicate removal, missing value handling, outlier detection, and data type standardization — all documented in a Jupyter..."
excerpt: "A data cleaning project that transforms a messy sales dataset into a clean, analysis-ready format using Pandas. Demonstrates essential data preprocessing techniques including duplicate removal, missing value handling, outlier detection, and data type standardization — all documented in a Jupyter..."
thumbnail: "/default-thumbnail.svg"
githubUrl: "https://github.com/aniekanudo-MD/Data_cleaning_with_Pandas"
stars: 0
language: ""
featured: false
priority: 13
tags: []
techStack:
  - "Python"
  - "Pandas"
  - "Jupyter Notebook"
status: "Complete"
liveDemo: ""
features:
  - "**Duplicate Removal**: Identify and remove duplicate transaction records"
  - "**Missing Value Handling**: Detect and address gaps in the dataset"
  - "**Date Standardization**: Ensure consistent date formatting across all entries"
  - "**Payment Type Standardization**: Unify naming (Credit Card, Debit Card, Cash, Paypal)"
  - "**Outlier Detection**: Identify negative values and unrealistic entries"
  - "**Typo Correction**: Fix spelling errors in product names"
  - "**Data Type Enforcement**: Ensure correct types for each column"
  - "**Column Renaming**: Correct misspelled column headers"
---

# Data Cleaning With Pandas

# Data Cleaning with Pandas
**Category:** Data Science  
**Tech Stack:** Python, Pandas, Jupyter Notebook  
**Status:** Complete  
**Thumbnail:** assets/thumbnail.png
## Overview
A data cleaning project that transforms a messy sales dataset into a clean, analysis-ready format using Pandas. Demonstrates essential data preprocessing techniques including duplicate removal, missing value handling, outlier detection, and data type standardization — all documented in a Jupyter notebook.
## Features
- **Duplicate Removal**: Identify and remove duplicate transaction records
- **Missing Value Handling**: Detect and address gaps in the dataset
- **Date Standardization**: Ensure consistent date formatting across all entries
- **Payment Type Standardization**: Unify naming (Credit Card, Debit Card, Cash, Paypal)
- **Outlier Detection**: Identify negative values and unrealistic entries
- **Typo Correction**: Fix spelling errors in product names
- **Data Type Enforcement**: Ensure correct types for each column
- **Column Renaming**: Correct misspelled column headers
## Dataset
**Columns:**
- `TransactionID` — Unique transaction identifier
- `Date` — Transaction date
- `CustomerID` — Customer identifier
- `ProductID` — Product identifier
- `ProductName` — Book titles (e.g., Book A, Book B, Book E)
- `Quantity` — Items purchased
- `Prize` → `Price` — Unit price (renamed during cleaning)
- `TotalSales` — Total transaction value
- `PaymentType` — Payment method used
- `CustomerAge` — Age of customer
## Cleaning Steps
| Step | Task |
|------|------|
| 1 | Remove duplicate records |
| 2 | Handle missing values |
| 3 | Standardize date formats |
| 4 | Unify payment type names |
| 5 | Remove negative values |
| 6 | Identify unrealistic outliers |
| 7 | Correct product name typos |
| 8 | Fix data types |
| 9 | Rename misspelled columns |
## Project Structure
```
Data_cleaning_with_Pandas/
├── messy_data.csv                # Original uncleaned dataset
├── cleaned_data.csv              # Processed clean dataset
├── Skillharvest_data_cleaning_assignment.ipynb  # Cleaning notebook
├── LICENSE                       # MIT License
└── README.md
```
## Getting Started
### Prerequisites
- Python 3.8+
- Jupyter Notebook
### Installation
```bash
git clone https://github.com/aniekanudo-MD/Data_cleaning_with_Pandas.git
cd Data_cleaning_with_Pandas
pip install pandas jupyter
```
### Run the Notebook
```bash
jupyter notebook Skillharvest_data_cleaning_assignment.ipynb
```
## Tech Stack
- **Language**: Python 3.8+
- **Library**: Pandas
- **Environment**: Jupyter Notebook
## Contact
- **Email**: [Aniekan Udo @Gmail](mailto:aniekanetimudo+reachout@gmail.com)
- **LinkedIn**: [Aniekan Udo @Linkedin](https://www.linkedin.com/in/aniekan-etim-udo)
## License
MIT
