# Stock Price Prediction Using Deep Learning and ARIMA Residuals

## Overview
This project explores various machine learning techniques to predict stock prices using historical data from Yahoo Finance. The models implemented include **Convolutional Neural Networks (CNN)**, **CNN-LSTM hybrids**, and a combination of **ARIMA** with **XGBoost** to refine predictions based on residuals.

### Models Used:
1. **Convolutional Neural Network (CNN)**:
   - Captures short-term patterns in stock prices.
   - Achieved an **R² of 0.88**, **MSE of 104.15**, and **MAE of 7.42**.
   
2. **CNN-LSTM Hybrid**:
   - Designed to capture both short- and long-term trends in stock prices.
   - Achieved an **R² of 0.77**, **MSE of 143.87**, and **MAE of 8.63**.
   
3. **ARIMA + XGBoost**:
   - ARIMA models linear trends, and XGBoost refines residuals for non-linear patterns.
   - Produced the best performance with an **R² of 0.92**, **MSE of 75.12**, and **MAE of 5.86**.

### Dataset:
The project uses 5 years of historical data (Jan 2019 - Dec 2023) for 7 leading stocks: Apple, Microsoft, Google, Nvidia, Tesla, Amazon, and Meta.

## Key Features:
- **Bootstrap Sampling**: Used to test model reliability, with confidence intervals computed over 1,000 resamples.
- **Hybrid Modeling**: Combines the strengths of ARIMA (for linear trends) and XGBoost (for complex non-linearities).

## Results:
- **CNN Model**: Detected short-term price patterns, explaining **88%** of the variance.
- **CNN-LSTM Model**: Captured long-term dependencies but underperformed with an **R² of 0.77**.
- **ARIMA + XGBoost**: Achieved the best results, explaining **92%** of the variance with a **MSE of 75.12**.

## Conclusion:
The hybrid **ARIMA + XGBoost** approach outperforms CNN and CNN-LSTM models in stock price prediction, effectively capturing both linear and non-linear patterns in the data. Future improvements may focus on refining model performance in volatile markets through hyperparameter tuning and feature engineering.

## Resources:
- [Attention-based CNN-LSTM and XGBoost hybrid model for stock prediction](https://arxiv.org/abs/2204.02623) (ArXiv)
- [Convolutional Networks for Stock Trading](https://stanford.edu)
- [Graph-based CNN-LSTM stock price prediction algorithm](https://doi.org/10.1007/s00530-021-00758-w) (Multimedia Systems)

## How to Run:
1. Clone this repository.
2. Run `stock_prediction.py` to train models and evaluate results.
