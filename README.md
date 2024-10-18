# Quantitative Trading Strategies (ML Optimization)

This project implements an algorithmic trading strategy using **Backtrader** and **XGBoost** to optimize trading decisions based on technical indicators. The strategy is backtested using historical data and optimized through machine learning to improve its predictive accuracy.

## Project Overview

### Key Components:
- **Backtrader**: Used for backtesting and simulating the trading strategy on historical data.
- **XGBoost**: Applied to optimize the model's performance by tuning hyperparameters and improving prediction accuracy.
- **Technical Indicators**: Various technical indicators like SMA, RSI, Bollinger Bands, MACD, etc., are used to generate trading signals.
- **Data Sources**: Historical price data (Open, High, Low, Close, Volume) is utilized for backtesting the strategy.
- **Performance Metrics**: The project evaluates the strategy's performance based on metrics such as final portfolio value, accuracy of predictions, and other relevant financial indicators.

### Strategy Logic:
- The trading strategy is based on **RSI (Relative Strength Index)**, **SMA (Simple Moving Average)**, and **XGBoost** for predictive modeling.
- **Buy signals** are triggered when certain thresholds of technical indicators (e.g., RSI < 30, price crosses above SMA) are met.
- **Sell signals** are triggered when RSI > 70 or price crosses below the SMA.
- The strategy is fine-tuned using XGBoost to optimize the parameters and improve the overall portfolio performance.

## How it Works:
1. **Data Preprocessing**: The raw market data is cleaned and transformed into a format compatible with Backtrader.
2. **Strategy Development**: Define a trading strategy based on technical indicators.
3. **Backtesting**: The strategy is run through Backtrader’s backtesting engine, and performance metrics are collected.
4. **Optimization**: Hyperparameter tuning is performed using XGBoost to identify the optimal settings for the strategy.
5. **Evaluation**: The strategy's performance is evaluated based on various metrics like final portfolio value, Sharpe ratio, etc.

## Requirements
- Python 3
- Backtrader
- XGBoost
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Installation
```bash
pip install backtrader xgboost pandas matplotlib seaborn ta numpy scikit-learn
