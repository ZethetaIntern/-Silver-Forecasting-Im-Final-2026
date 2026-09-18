# 1D Silver Price Forecasting Agent - Commodity Forecasting

## Project Overview
This project forecasts 1D Silver prices using multiple time-series models for Data Analyst work experience.

## Dataset
- File: silver_with_indicators.csv
- Period: 2000-2025 daily prices
- Features: OHLC, RSI, MACD, Moving Averages

## Models Implemented
1. ARIMA - Day_4_Silver_ARIMA_improved.ipynb
2. Prophet - Day_6_Prophet.ipynb
3. LSTM (Deep Learning) - Day_7_LSTM.ipynb - BEST MODEL
4. XGBoost - XGBoost.ipynb
5. Final Comparison - Day8_Final_Comparison.ipynb

## Results
- Best Model: LSTM with lowest RMSE and MAE
- Metrics: RMSE, MAE, MAPE compared in Day_8_Final_Metrics_Comparison
- Visuals: Prophet, LSTM, Ensemble forecasts included as PNG

## Files
- All notebooks are executable
- Predictions CSVs show forecast results
- Final Report: 1D-Silver_final_report.pdf

## Conclusion
LSTM outperformed traditional models for Silver price forecasting.
