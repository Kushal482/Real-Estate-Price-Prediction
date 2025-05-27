# Real-Estate-Price-Prediction
This project focuses on predicting real estate prices using machine learning. Built an end-to-end pipeline that includes data cleaning, feature engineering, model training, and deployment.

## 📌 Project Objective

Build a regression model that can accurately predict property prices using structured real estate data. This includes:
- Cleaning messy and inconsistent data
- Engineering relevant features
- Selecting the best ML model using cross-validation
- Packaging the model for future predictions

---

## 🗂️ Dataset

- Source: [Custom CSV file] (usually Kaggle or a company dataset)
- Key features:
  - `location`
  - `total_sqft`
  - `size` (e.g., 2 BHK)
  - `bath`, `balcony`
  - `price`

---

## 🔧 Data Preprocessing

- Handled missing values
- Converted `total_sqft` ranges (e.g., "2100–2850") to average
- Extracted `BHK` from `size` column
- Calculated `price_per_sqft` for better comparability
- Grouped rare locations into an `"other"` category
- Removed outliers (unrealistic sqft per BHK, extreme price per sqft)

---

## 🧠 Modeling

- Algorithms used:
  - Linear Regression
  - Lasso Regression
  - Decision Tree Regressor
- Hyperparameter tuning with `GridSearchCV`
- Performance measured using R² score and cross-validation

---

## 🚀 Deployment

- Final model exported using `joblib`
- Created a reusable function to make predictions based on:
  - Location
  - Square footage
  - Number of bathrooms
  - BHK

---
