# Time Series Analysis of Retail Trade
This repository contains a detailed time series forecasting analysis on U.S. monthly retail trade and food services sales data.

## Dataset
[Dataset Source](https://www.census.gov/econ/currentdata/?programCode=MARTS)
- Source: U.S. Census Bureau (MARTS and MRTS)
- Period: 1992–2019
- Variable: Monthly sales (billions of dollars) for retail trade and food services

## Methods Used
- **SARIMA**
- **ETS (Exponential Smoothing)**
- **Holt-Winters**
- **TBATS & BATS**
- **NNETAR (Neural Network AutoRegressive)**
- **PROPHET**
- **GARCH-type models (eGARCH, sGARCH, gjrGARCH)**

## Preprocessing
- Seasonal decomposition and anomaly detection (STL)
- Train-test split (80/20, last 60 observations as test)
- Stationarity checks: KPSS, PP, HEGY, Canova-Hansen
- Differencing for trend and seasonal stationarity
- Anomaly interpolation and smoothing

## Model Diagnostics
- Residual checks: ACF, PACF, Shapiro-Wilk, Ljung-Box, White’s test
- GARCH model fitted on seasonally adjusted series due to heteroscedasticity
- Sign Bias test for asymmetric shock response
