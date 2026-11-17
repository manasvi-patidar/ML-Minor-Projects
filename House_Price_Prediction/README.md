# 🏠 House Price Prediction | Supervised Machine Learning

## 📌 Project Overview

This project focuses on building a **House Price Prediction System** using Supervised Machine Learning.

The objective of this project is to analyse historical housing data, perform data preprocessing, train a **Linear Regression model**, and evaluate its performance to predict house sale prices.

---

## 🎯 Problem Statement

The real estate company wants to develop an intelligent system that can automatically estimate the market price of a residential property.

The system should learn patterns from historical property sales data and predict the selling price of a house based on its characteristics.

**Machine Learning Task:** Regression

**Learning Type:** Supervised Learning

**Algorithm:** Linear Regression

**Target Variable:** `SalePrice`

---

## 📂 Dataset Information

The project uses the `HousePricePrediction.csv` dataset.

- **Total Records:** 2,919
- **Total Features:** 12 input columns
- **Target Variable:** `SalePrice`
- **Problem Type:** Regression

### Dataset Features

| Feature        | Description                                |
| -------------- | ------------------------------------------ |
| `Id`           | Unique identification number of each house |
| `MSSubClass`   | Type of dwelling involved in the sale      |
| `MSZoning`     | General zoning classification              |
| `LotArea`      | Lot size in square feet                    |
| `LotConfig`    | Lot configuration                          |
| `BldgType`     | Type of dwelling                           |
| `OverallCond`  | Overall condition rating (1–10)            |
| `YearBuilt`    | Original construction year                 |
| `YearRemodAdd` | Year of remodeling or additions            |
| `Exterior1st`  | Exterior covering of the house             |
| `BsmtFinSF2`   | Type 2 finished basement square feet       |
| `TotalBsmtSF`  | Total basement area in square feet         |
| `SalePrice`    | Final selling price (Target)               |

---

## 🛠️ Technologies & Libraries Used

- **Python** – Programming Language
- **Jupyter Notebook** – Development Environment
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical computations
- **Scikit-learn** – Machine Learning and model evaluation

---

## ⚙️ Project Workflow

The project follows these major Machine Learning steps:

1. Data Loading
2. Exploratory Data Analysis (EDA)
3. Data Cleaning & Missing Value Handling
4. Categorical Encoding using One-Hot Encoding
5. Train-Test Split (80:20)
6. Model Training using Linear Regression
7. Model Evaluation
8. Feature Scaling using StandardScaler

---

## 📊 Model Performance

The Linear Regression model achieved the following results in the current notebook:

| Evaluation Metric |    Result |
| ----------------- | --------: |
| R² Score          |    0.3741 |
| MAE               | 30,829.94 |
| RMSE              | 41,138.56 |
| MAPE              |    18.74% |

### Performance Observation

The model achieved an R² score of approximately 0.3741, indicating that it explains around 37.41% of the variation in house prices on the current test split.

Feature scaling produced practically identical evaluation results for Linear Regression.

---

## 👨‍💻 Author

Manasvi
