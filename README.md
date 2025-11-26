🔋 Energy Load Forecasting with HAR-ARIMA
📌 Overview

This project forecasts hourly electricity demand using the HAR-ARIMA model on PJM load data. Electricity usage follows clear hourly, daily, and weekly cycles, and HAR-ARIMA captures these patterns more efficiently than traditional ARIMA or complex ML models. The goal is to build a fast, interpretable, and accurate forecasting system.

🧠 Method

The model uses a hierarchical structure with three key components:

Lag-1: Short-term hourly behavior

24-hour mean: Daily diurnal pattern

168-hour mean: Weekly business cycle

These lag features are integrated directly into the ARIMA framework, allowing the model to learn multi-scale memory without heavy feature engineering.

📊 Results

HAR-ARIMA shows strong performance compared to SARIMA and XGBoost:

Better handling of hourly, daily, and weekly seasonality

Faster training time with fewer parameters

Clear and interpretable coefficient structure

This makes HAR-ARIMA a powerful baseline model for real-world energy load forecasting.
