# Bank Customer Churn Prediction

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)

An Exploratory Data Analysis (EDA) project to identify key factors driving customer churn in the banking sector using Python.

## Overview

Customer churn refers to when existing customers stop doing business with the bank. High churn leads to revenue loss and increased customer acquisition costs. 
This project analyzes bank customer data to predict which customers are at risk of leaving and helps the bank develop targeted retention strategies.

## Problem Statement

- The bank is experiencing loss of customers
- Difficult to identify which customers are at risk
- Need predictive insights to detect high-risk churn customers early
- Help the bank retain valuable customers

## Dataset

**Source:** Kaggle - Bank Churn Dataset

**Size:** ~10,000 customer records with 14 features

**Key Features:**
- **Customer Demographics:** Age, Gender, Geography
- **Account Information:** Balance, Credit Score, Tenure
- **Product Usage:** Number of Products, Has Credit Card, Active Member Status
- **Financial:** Estimated Salary
- **Target Variable:** Exited (0 = Retained, 1 = Churned)

## Technology Stack

- **Python 3.8+**
- **Google Colab** - Development environment
- **Pandas & NumPy** - Data manipulation
- **Matplotlib & Seaborn** - Data visualization
- **Scikit-Learn** - Data preprocessing

## Project Structure
```
bank-customer-churn-prediction/
├── data/
│   ├── Churn_Modelling.csv          # Original dataset
│   └── bank_churn_cleaned.csv       # Processed dataset
├── notebooks/
│   └── Bank_Churn_EDA_Project.ipynb # Main analysis notebook
├── visualizations/                   # Generated charts and graphs
├── README.md
└── requirements.txt
```

## Analysis Workflow

### 1. Data Loading & Exploration
- Load dataset and examine structure
- Check for missing values and duplicates
- Generate statistical summaries

### 2. Data Preprocessing
- Handle missing values
- Remove duplicates
- Encode categorical variables (Gender, Geography)
- Scale numerical features using StandardScaler
- Create derived features (Age Groups, Balance Categories, Tenure Groups)

### 3. Exploratory Data Analysis (EDA)

**Univariate Analysis:**
- Churn distribution
- Feature distributions
- Statistical summaries

**Bivariate Analysis:**
- Churn vs Age
- Churn vs Gender
- Churn vs Geography
- Churn vs Account Balance
- Churn vs Number of Products
- Churn vs Active Membership Status

**Multivariate Analysis:**
- Correlation heatmap
- Feature interactions
- Customer segmentation

### 4. Visualizations
- Distribution plots
- Bar charts for categorical analysis
- Box plots for numerical features
- Correlation heatmaps
- Interactive dashboards

## Key Insights

### Geographic Patterns
- Germany shows the highest churn rate
- Significant variation across different countries

### Age Factor
- Older customers (51+) have significantly higher churn rates
- Age group 60+ shows the highest risk

### Product Holdings
- Customers with fewer products tend to churn more
- Single product customers are at higher risk
- Multi-product engagement reduces churn

### Activity Status
- Inactive members have much higher churn rates
- Active engagement is a strong retention indicator

### Balance & Tenure
- Customers with lower account balances show higher churn
- Tenure impacts churn patterns

## Requirements

Create a `requirements.txt` file with:
```
pandas
numpy
matplotlib
seaborn
scikit-learn
```

## Installation & Usage

1. Clone the repository:
```bash
git clone https://github.com/yourusername/bank-customer-churn-prediction.git
cd bank-customer-churn-prediction
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Open the Jupyter notebook:
```bash
jupyter notebook notebooks/Bank_Churn_EDA_Project.ipynb
```

Or use Google Colab:
- Upload the notebook to Google Colab
- Upload the dataset when prompted
- Run cells sequentially

## Results

The analysis successfully identifies key churn drivers:
- Geographic location (Germany has highest churn)
- Customer age (older customers at risk)
- Product engagement (single product holders vulnerable)
- Activity status (inactive members likely to churn)
- Account balance patterns

