# Bank Dataset Cleaning Project

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-1.5%2B-orange)
![Plotly](https://img.shields.io/badge/Plotly-5.0%2B-lightgrey)

A comprehensive data cleaning and exploratory analysis project for a bank customer dataset. This project handles missing values, outliers, data type corrections, and feature engineering to prepare the data for analysis.

## 📌 Overview
This project focuses on cleaning and preprocessing a bank customer dataset to ensure data quality for further analysis. Key tasks include:
- Handling missing values and outliers.
- Correcting data types.
- Feature engineering.
- Exploratory Data Analysis (EDA) with visualizations.

## 🛠️ Technologies Used
- **Python** (Pandas, NumPy)
- **Data Cleaning**: `SimpleImputer`, `KNNImputer`, `datasist`
- **Visualization**: Plotly Express, Plotly Figure Factory

## 📂 Dataset
The dataset (`Bank Data.csv`) contains customer banking information, including:
- Demographic data (Age, Occupation)
- Financial metrics (Annual Income, Monthly Balance)
- Loan details (Type of Loan, Number of Loans)
- Credit history (Credit Mix, Payment Behavior)

## 🔍 Key Steps
### 1. Data Cleaning
- Dropped redundant columns (`ID`, `SSN`, `Credit_Utilization_Ratio`).
- Handled missing values (imputed with KNN for numerical data, mode for categorical).
- Corrected data types.
- Fixed corrupted entries.

### 2. Feature Engineering
- Extracted `Credit_History_Age` in months/years from a string column.
- Created binary columns for loan types (e.g., `Has_Auto_Loan`).
- Extracted `Age_Category` (Teens/Adults/Mature Adults).

### 3. Outlier Handling
- Replaced extreme values in numerical columns with median.

### 4. EDA & Visualizations
- Analyzed distributions (Age, Occupation, Payment Behavior).
- Explored relationships:
  - `Annual_Income` vs. `Monthly_Inhand_Salary`.
  - `Num_of_Loan` vs. `Num_Credit_Inquiries`.
- Identified top customers by metrics (Monthly Balance, Delayed Payments).

### 5. Saved result
**The cleaned dataset is saved as Bank Data (cleaned).csv.**
