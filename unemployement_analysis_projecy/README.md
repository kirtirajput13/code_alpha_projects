# 📉 Unemployment Analysis & Forecasting in India (2018–2020)

This project explores the unemployment rate trends in India using real-world data collected until November 2020. It includes exploratory data analysis (EDA), impact assessment of COVID-19 lockdown, and future trend forecasting using **Facebook Prophet**.

---

## 📊 Dataset

- **Source**: [CMIE / Kaggle Dataset](https://www.kaggle.com/datasets)
- **File**: `Unemployment_Rate_upto_11_2020.csv`
- **Attributes**:
  - `Region` (renamed to `State`)
  - `Date` (renamed to `Month`)
  - `Estimated Unemployment Rate (%)`
  - `Estimated Employed`
  - `Estimated Labour Participation Rate (%)`

---

## 🛠️ Project Workflow

### 1. **Data Cleaning & Preprocessing**
- Removed whitespace from column names and string data
- Renamed columns for clarity
- Converted date strings to `datetime` objects
- Dropped missing values
- Extracted `Year` and created `Period` labels (Pre-COVID vs During-COVID)

### 2. **Exploratory Data Analysis (EDA)**
- Line plot: Monthly average unemployment trend (2018–2020)
- Bar chart: Comparison of unemployment Pre- vs During-COVID
- Bar chart: Top 10 states with highest unemployment during lockdown (April–May 2020)
- Heatmap: State-wise unemployment rates across months

### 3. **Forecasting using Prophet**
- Averaged national unemployment rates by month
- Trained Prophet model on historical data
- Forecasted unemployment rate for the next 12 months
- Visualized trend prediction with confidence intervals

---

## 📈 Visualizations

| Chart | Description |
|-------|-------------|
| 📉 Line Plot | India’s monthly unemployment rate with COVID marker |
| 🟥 Bar Plot | State-wise unemployment during April–May 2020 |
| 🔥 Heatmap | Month-wise heatmap of unemployment by state |
| 🔮 Prophet Forecast | 12-month unemployment rate prediction |

---

## 📦 Requirements

Install required libraries using:

```bash
pip install pandas numpy matplotlib seaborn plotly prophet
