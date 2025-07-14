# 🚗 Car Price Prediction Using Machine Learning

This repository contains an end-to-end machine learning pipeline for predicting used car prices using multiple regression techniques. It includes data preprocessing, feature engineering, model training, evaluation, hyperparameter tuning, and model saving.

---

## 📁 Dataset

The dataset used is `car data.csv`, which contains information about used cars such as:

- `Present_Price`: Current ex-showroom price
- `Selling_Price`: Price the car was sold at
- `Driven_kms`: Kilometers driven
- `Fuel_Type`: Petrol, Diesel, or CNG
- `Seller_Type`: Dealer or Individual
- `Transmission`: Manual or Automatic
- `Owner`: Number of previous owners
- `Year`: Manufacturing year

---

## ✅ Workflow

### 1. **Data Preprocessing**
- Dropped irrelevant columns (`Car_Name`)
- Converted `Year` to `Car_Age`
- Removed outliers in price and mileage
- Handled categorical variables with OneHotEncoding
- Scaled numerical features

### 2. **Exploratory Data Analysis**
- Correlation heatmap
- Distribution plots for outlier detection

### 3. **Modeling**
- Implemented regression models with Scikit-learn Pipelines:
  - Linear Regression
  - Ridge Regression
  - Random Forest Regressor
  - Gradient Boosting Regressor
- Evaluated with cross-validation (`R²` score)

### 4. **Hyperparameter Tuning**
- Tuned `RandomForestRegressor` using `GridSearchCV`
- Parameters tuned:
  - `n_estimators`
  - `max_depth`
  - `min_samples_split`

### 5. **Model Evaluation**
- Metrics:
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
  - R² Score
- Visualized Actual vs Predicted prices

### 6. **Model Persistence**
- Final model saved using `joblib`:
