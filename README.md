# SBI Stock Price Forecasting

This project aims to forecast the stock price of the State Bank of India (SBI) by analyzing historical data spanning 4.5 years. Various time series models were employed to decompose and understand the underlying components of the stock price and make future predictions.

## Project Overview

- **Objective**: To predict the future stock prices of SBI using time series analysis and forecasting techniques.
- **Data**: Historical stock prices of SBI over 4.5 years.

## Project Steps

1. **Data Analysis and Preprocessing**
   - Collected and analyzed the stock price data for SBI.
   - Decomposed the time series data into trend, seasonality, and noise components to better understand the underlying patterns.

2. **Stationarity Check**
   - Performed stationarity tests using the Augmented Dickey-Fuller (ADF) test.
   - Stabilized the time series by applying differencing (d) to remove trends and make the series stationary.

3. **Model Selection**
   - Plotted the Partial Autocorrelation Function (PACF) and Autocorrelation Function (ACF) to determine the optimal parameters for the time series models (p, d, q).
   - Considered the following models for forecasting:
     - **ARIMA** (AutoRegressive Integrated Moving Average)
     - **SARIMA** (Seasonal ARIMA)
     - **Exponential Smoothing**

4. **Forecasting**
   - After tuning the models, the best-performing model was identified as **ARIMA(2,1,2)**.
   - The model was used to predict the stock price for the next 60 days.

5. **Model Evaluation**
   - The performance of the models was evaluated using Root Mean Square Error (RMSE).
   - The ARIMA(2,1,2) model achieved an RMSE of **7.914**, indicating a good fit to the data.

## Results

- The best-tuned ARIMA(2,1,2) model was able to predict the SBI stock price with high accuracy for the next 60 days.
- The RMSE value of **7.914** reflects the model's ability to closely match the actual stock price data.

## Files in Repository

- `data/` : Folder containing the historical stock price data of SBI.
- `notebooks/` : Jupyter notebooks used for data analysis, model building, and evaluation.
- `models/` : Saved models and tuning parameters.
- `results/` : Plots and visualizations of the forecasting results.
- `README.md` : This file.

## Installation and Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/SBI-stock-price-forecasting.git
   cd SBI-stock-price-forecasting
