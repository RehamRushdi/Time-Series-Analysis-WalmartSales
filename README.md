# 🛒 Walmart Sales Forecasting with Time Series Analysis

This project focuses on analyzing and forecasting Walmart's weekly sales data using a combination of classical and modern time series techniques. It was developed as **Task 2** of my data science internship at **Elevvo**.

---

## 📌 Project Objectives

- Explore and clean historical Walmart sales data
- Visualize trends, seasonality, and anomalies
- Apply time series forecasting using:
  - Rolling Mean
  - Exponential Smoothing
  - Facebook Prophet with external regressors
- Evaluate the forecasting performance and insights

---

## 📁 Dataset

The dataset was sourced from [Kaggle – Walmart Sales Forecasting](https://www.kaggle.com/aslanahmedov/walmart-sales-forecast), and includes:
- `train.csv`: Weekly sales data
- `features.csv`: MarkDowns, CPI, Unemployment, etc.
- `stores.csv`: Store metadata

---

## 🛠️ Tools & Libraries Used

- Python (Pandas, Numpy)
- Seaborn & Matplotlib for visualization
- Statsmodels for smoothing & decomposition
- Prophet for forecasting
- KaggleHub for dataset access

---

## 📊 Time Series Techniques Applied

### 1. Rolling Mean
- Used a 3-month rolling average to smooth short-term fluctuations.

### 2. Exponential Smoothing
- Applied weighted smoothing with recent periods prioritized.

### 3. Seasonal Decomposition
- Broke down weekly sales into trend, seasonality, and residuals using `seasonal_decompose()`.

### 4. Prophet Model (with Regressors)
- Built a robust forecast using Prophet with external regressors:
  - `MarkDown1`
  - `CPI`
  - `Unemployment`

---

## 🔍 Key Insights

- **Strong seasonality** observed around November–December due to holiday shopping.
- **Upward trend** in sales between 2010 and 2012.
- Basic smoothing models struggled with seasonal peaks.
- Prophet showed improved forecasts when incorporating economic and promotional variables.

---

## 📈 Results

The final forecast projected the next 12 weeks of sales, accounting for trends, weekly seasonality, and external factors. Prophet outperformed basic models in accuracy and adaptability.

---

## 📌 Author

**Reham Mahmoud Rushdi**  
[LinkedIn](https://www.linkedin.com/in/reham-mahmoud-rushdi/)
