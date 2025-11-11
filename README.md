# Gold Price Forecasting in India

This project focuses on forecasting gold prices in India using machine learning techniques. The goal is to analyze historical data, identify key trends, and build predictive models that can estimate future gold prices with reasonable accuracy. The notebook includes exploratory data analysis (EDA), data preprocessing, model training, and evaluation.

---

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Modeling](#modeling)
- [Results and Insights](#results-and-insights)
- [Future Work](#future-work)
- [How to Run](#how-to-run)
- [Dependencies](#dependencies)
- [Author](#author)
- [License](#license)

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
5. **Model Building:** Tested different models (e.g., XGBoost, Linear Regression, Random Forest, and Ensemble models).
6. **Evaluation:** Compared models using metrics like RMSE and R².

---

## Modeling

The notebook includes:
- **Baseline Model:** Simple Linear Regression
- **Advanced Models:** XGBoost and Ensemble Learning
- **Evaluation Metrics:** MAE, RMSE, and R²
- **Visualization:** Actual vs Predicted Gold Prices

---

## Results and Insights

### Model Performance Overview
Two models were evaluated: **XGBoost** and an **Ensemble model** combining multiple algorithms.  
- **XGBoost Model:** Stable predictions but slightly underestimates during rapid price spikes.  
- **Ensemble Model:** Balanced results with lower error and consistent trend prediction.

### Actual vs Predicted Trends
Both models captured long-term gold price direction effectively. Predictions were smoother, performing best during stable periods but lagging slightly during sharp increases.

### Prediction Error Distribution
Errors mostly fall within **500–700 USD**, confirming a stable and moderate prediction error. Outliers occur mainly during sudden market volatility.

### Feature Importance Insights
- **Top Predictors:** `Price_Rolling_Max_7`, `MA_30`, and `Price_Lag_1` dominate, indicating strong dependence on recent trends and rolling averages.
- **Short-Term Lags:** (1–3 days) show momentum behavior.
- **Technical Indicators:** RSI and other indicators play secondary roles compared to price-based trends.

### Strategic Implications
- **Forecast Reliability:** Effective for medium-term planning and trend tracking.
- **Retail and Investment Use:** Helps optimize buying, selling, and hedging strategies.
- **Model Enhancement:** Adding macroeconomic indicators (USD/INR, inflation) can improve sensitivity to market shocks.

### Summary Table

| Aspect | Observation | Business Interpretation |
|--------|--------------|-------------------------|
| Model Accuracy | High (R² ≈ 0.90) | Reliable for medium-term forecasts |
| Error Pattern | Underestimates during spikes | Add volatility-aware features |
| Key Features | Rolling Max, MA_30, Lag_1 | Gold follows historical momentum |
| Forecast Utility | Trend prediction & planning | Supports investment decisions |

---

## Future Work

- Integrate real-time data sources (live market APIs).
- Deploy model using Streamlit or Flask for interactive forecasting.
- Automate retraining with updated data to adapt to market trends.
- Extend to multi-feature economic forecasting.

---

