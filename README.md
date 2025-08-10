# AI Stock Predictions & Analysis
https://ai-finance-reporter.onrender.com/
This project is a Flask web application that provides stock market analysis and price predictions using time-series forecasting and technical indicators. Users can input a stock ticker symbol to generate a detailed HTML report.

## Overview

The application fetches historical stock data, fundamental company information, and relevant macroeconomic indicators. It then preprocesses this data, applies feature engineering (including technical indicators), trains a Facebook Prophet model for forecasting, and generates a comprehensive report summarizing the findings with interactive charts.

## Features

* **Web Interface:** Simple Flask-based UI to input stock tickers.
* **Data Collection:**
    * Fetches historical stock price data (Open, High, Low, Close, Volume) using yfinance.
    * Fetches fundamental company data (Sector, Industry, Market Cap, P/E, etc.) using yfinance.
    * Fetches macroeconomic indicators (e.g., Federal Funds Rate, S&P 500) from FRED using pandas\_datareader.
* **Data Processing:** Cleans, merges, and aligns stock and macroeconomic data.
* **Feature Engineering:** Calculates technical indicators like RSI, MACD, Bollinger Bands, and Moving Averages.
* **Forecasting:** Utilizes Facebook Prophet for time-series price forecasting.
* **Report Generation:** Creates detailed HTML reports including:
    * Forecast charts (vs. actuals).
    * Historical price/volume charts.
    * Technical indicator charts (Bollinger Bands, RSI, MACD).
    * Key metrics summary.
    * Fundamental data summary.
    * Risk analysis summary.
    * Overall sentiment and outlook.

## Tech Stack

* **Backend:** Python, Flask
* **Data Handling:** pandas, numpy
* **Time Series Forecasting:** Prophet (fbprophet)
* **Data Fetching:** yfinance, pandas-datareader
* **Technical Analysis:** ta (Technical Analysis Library)
* **Plotting:** Plotly
* **Web:** HTML, CSS

## Deployed
This application is deployed using Render, 
click on the link to access it 
https://ai-finance-reporter.onrender.com/
