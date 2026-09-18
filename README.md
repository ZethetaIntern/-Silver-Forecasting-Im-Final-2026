# 1D Silver Price Forecasting Agent - Final Project 2026
Author: Iemun Kaloo | Internship: ZeTheta 1D

## Project Overview
This project forecasts Silver prices using Time Series and ML models from 2016-2026 data. Goal is accurate 30-day forecasting for trading decisions.

## Dataset
- File: silver_with_indicators.csv
- Source: Yahoo Finance SI=F
- Features: Close, MA, RSI, MACD, Volatility, Returns
- Period: 2016 to 2026

## Models Implemented
1. EDA and Stationarity Test (01_EDA_and_Stationarity.ipynb) - ADF Test, Seasonal Decomposition
2. ARIMA Improved (Day_4_Silver_ARIMA_improved) - Best ARIMA(5,1,0) - RMSE: 8.2
3. Prophet Model (Day_6_Prophet.ipynb) - RMSE: 6.8, MAE: 5.1 - Best for seasonality
4. LSTM Deep Learning (Day_7_LSTM.ipynb) - RMSE: 5.5, MAE: 4.2 - Best Model
5. XGBoost (XGBoost.ipynb) - RMSE: 7.1, Feature Importance via SHAP
6. Ensemble Model (Day 9) - Final Ensemble of Prophet + LSTM + XGBoost - RMSE: 5.1

## Final Results Comparison
| Model | RMSE | MAE | R2 Score |
|-------|------|-----|----------|
| ARIMA | 8.2 | 6.5 | 0.85 |
| Prophet | 6.8 | 5.1 | 0.89 |
| LSTM | 5.5 | 4.2 | 0.93 |
| XGBoost | 7.1 | 5.4 | 0.87 |
| Ensemble (Final) | 5.1 | 3.9 | 0.95 |

Best Model: Ensemble Model with R2 0.95 and RMSE 5.1

## Files in Repo
- All notebooks with code and outputs
- Predictions CSV for each model
- Forecast PNGs for visualization
- Final Metrics Comparison TXT
- SHAP Explainability Plots

## Tech Stack
Python, Pandas, NumPy, Matplotlib, Scikit-learn, Statsmodels, Prophet, TensorFlow/Keras, XGBoost, SHAP

## How to Run
pip install -r requirements.txt
jupyter notebook Day_7_LSTM.ipynb
