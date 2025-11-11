# Gold Price Forecasting in India

This project focuses on forecasting gold prices in India using machine learning techniques. The goal is to analyze historical data, identify key trends, and build predictive models that can estimate future gold prices with reasonable accuracy. The notebook includes exploratory data analysis (EDA), data preprocessing, model training, and evaluation.

---

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Modeling](#modeling)
- [Results](#results)
- [Future Work](#future-work)
- [How to Run](#how-to-run)
- [Dependencies](#dependencies)
- [Author](#author)

---

## Overview

Gold is a critical asset in India, heavily influenced by global markets, currency exchange rates, and economic indicators. Predicting gold prices can provide valuable insights for investors and policy makers.

This notebook demonstrates a step-by-step approach to building a predictive model for gold prices using time series data and regression-based machine learning algorithms.

---

## Dataset

The dataset used for this project was sourced from publicly available financial records.  
Potential data sources include:

- [Reserve Bank of India Database (DBIE)](https://data.rbi.org.in/DBIE/#/dbie/home)
- World Gold Council
- Yahoo Finance (for USD/INR rates and gold futures)

The data includes daily or monthly gold prices in Indian Rupees (INR) along with other economic indicators.

---

## Methodology

1. **Data Collection:** Gathered historical gold prices and relevant financial variables.
2. **Data Preprocessing:** Handled missing values, formatted date columns, and normalized data.
3. **Exploratory Data Analysis (EDA):** Visualized trends, seasonality, and correlations.
4. **Feature Engineering:** Created lag features and moving averages to capture time-based patterns.
5. **Model Building:** Tested different models (e.g., XGBoost, Linear Regression, ARIMA).
6. **Evaluation:** Compared models using metrics like RMSE and R².

---

## Modeling

The notebook includes:
- **Baseline Model:** Simple Linear Regression
- **Advanced Models:** XGBoost and Random Forest
- **Evaluation Metrics:** MAE, RMSE, and R²
- **Visualization:** Actual vs Predicted Gold Prices

---

## Results

- The XGBoost model provided the most stable and accurate predictions.
- Observed strong temporal trends influenced by global price movement and currency rates.
- Feature importance analysis identified lagged gold price and exchange rate as key predictors.

---

## Future Work

- Incorporate external features such as inflation, crude oil price, or USD/INR rate.
- Deploy model using Streamlit or Flask for interactive forecasting.
- Automate data updates using APIs or scheduled jobs.

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/gold-price-forecasting.git

---



