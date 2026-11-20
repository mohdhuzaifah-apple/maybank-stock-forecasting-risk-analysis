# maybank-stock-forecasting-risk-analysis
A Python-based analysis of Maybank stock prices using ARIMA forecasting, Value-at-Risk, CVaR, and Monte Carlo simulation.

# Maybank Stock Price Forecasting & Downside Risk Analysis

## Project Overview

This project examines historical stock prices of Malayan Banking Berhad (Maybank, 1155.KL) using Python and the Autoregressive Integrated Moving Average (ARIMA) model.

It also incorporates financial risk analysis and Monte Carlo simulation to evaluate historical return behaviour, downside risk, and potential future price scenarios.

The project was developed as a personal learning project, applying concepts from Financial Mathematics and quantitative risk analysis.

## Tools and Libraries

- Python
- Jupyter Notebook
- pandas and NumPy
- Matplotlib
- Statsmodels
- yfinance

## Methodology

1. Historical data collection and cleaning
2. Exploratory Data Analysis and moving averages
3. Stationarity testing using the Augmented Dickey-Fuller test
4. ARIMA model selection using AIC and BIC
5. Stock price forecasting and performance evaluation
6. Residual diagnostics
7. Financial risk analysis
8. Historical bootstrap Monte Carlo simulation

## Key Results

| Metric | Result |
|---|---:|
| Selected ARIMA Model | ARIMA(1,1,1) |
| ARIMA Test RMSE | RM0.8139 |
| Random Walk Test RMSE | RM0.8664 |
| Annualised Average Log Return | 9.94% |
| Annualised Volatility | 12.32% |
| Historical VaR (95%) | 1.12% |
| Historical CVaR (95%) | 1.73% |
| Maximum Drawdown | -16.07% |
| Monte Carlo 30-Day Median | RM10.04 |
| Monte Carlo 30-Day 5th Percentile | RM9.35 |
| Monte Carlo 30-Day 95th Percentile | RM10.76 |

## Main Findings

The selected ARIMA(1,1,1) model achieved a lower RMSE than the fixed-origin random-walk benchmark over the test period.

Historical risk analysis identified significant downside variability, while Monte Carlo simulation illustrated a range of potential 30-observation outcomes.

## Limitations

The forecasting results are based on historical stock prices and do not guarantee future performance. The ARIMA test uses a fixed forecast origin, while the Monte Carlo simulation assumes independently resampled historical returns. The ARIMA price forecasts and dividend-adjusted simulation paths use different price bases and are not directly comparable.

## Reference

Inspired by [Stock Market Forecasting Using ARIMA by Nagesh Singh](https://www.kaggle.com/code/nageshsingh/stock-market-forecasting-arima/notebook), adapted for Maybank with additional financial risk and simulation analysis.

## Disclaimer

This project is for educational and analytical purposes only and does not constitute financial or investment advice.
