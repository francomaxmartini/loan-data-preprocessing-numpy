# Loan Data Preprocessing with NumPy

## Overview

This project focuses on cleaning, preprocessing, and preparing a real-world loan dataset from LendingClub using primarily NumPy operations and vectorized workflows.

The objective is to transform raw financial data into a structured, machine-learning-ready dataset while demonstrating strong proficiency in low-level data manipulation techniques without relying heavily on higher-level libraries such as pandas.

The preprocessing pipeline includes:

- Handling missing values  
- Cleaning and transforming categorical variables  
- Feature engineering  
- Currency standardization using historical exchange rates  
- Dataset restructuring and exportation  

The final output is a fully cleaned dataset ready for future applications such as credit risk modeling, default prediction, and financial data analysis.

---

## Dataset

The project uses a LendingClub loan dataset containing information related to issued loans and borrower characteristics, including:

- Loan amount  
- Funded amount  
- Interest rate  
- Installment values  
- Loan status  
- Verification status  
- Loan term  
- Credit grade and sub-grade  
- State information  
- Payment information  

An additional EUR/USD exchange rate dataset is used to standardize monetary values into EUR.

---

## Objectives

- Clean and preprocess raw financial data  
- Handle incomplete and inconsistent observations  
- Encode categorical variables into numerical formats  
- Standardize financial variables across currencies  
- Build a machine-learning-ready dataset using NumPy  
- Demonstrate efficient vectorized preprocessing techniques  

---

## Technologies Used

- Python  
- NumPy  
- Jupyter Notebook  

---

## Workflow

### 1. Data Import
- Import raw LendingClub loan data

### 2. Dataset Separation
- Separate numerical and categorical features
- Extract and organize column headers

### 3. String Feature Processing
- Clean issue dates
- Encode loan status
- Process loan terms
- Handle grade and sub-grade variables
- Encode verification status
- Process geographic state information

### 4. Numerical Feature Processing
- Handle missing numerical values
- Apply statistical replacements
- Standardize interest rates

### 5. Currency Conversion
- Match exchange rates by loan issue month
- Convert USD-denominated variables into EUR

### 6. Dataset Finalization
- Merge processed numerical and categorical datasets
- Sort observations
- Export final preprocessed dataset

---

## Final Output

The project produces a fully cleaned and structured dataset:

`loan-data-preprocessed.csv`

This dataset is prepared for future applications such as:

- Credit risk modeling  
- Loan default prediction  
- Financial analytics  
- Machine learning workflows  

---

## Key Skills Demonstrated

- NumPy vectorized operations  
- Financial data preprocessing  
- Feature engineering  
- Missing value handling  
- Categorical variable encoding  
- Currency standardization  
- Data pipeline organization  
- Machine learning data preparation  

---

## Repository Structure

```text
loan-data-preprocessing-numpy/
│
├── data/
│   ├── loan-data.csv
│   ├── EUR-USD.csv
│   └── loan-data-preprocessed.csv
│
├── checkpoints/
│   ├── checkpoint-test.npz
│   ├── checkpoint-strings.npz
│   └── checkpoint-numeric.npz
│
├── notebooks/
│   └── 01_loan_data_preprocessing_numpy.ipynb
│
├── README.md
```
---
