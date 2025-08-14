# Time-Series-Forecasting-for-Portfolio-Management-Optimization

## Overview
This project performs **Exploratory Data Analysis (EDA)** and **Time Series Forecasting** on historical stock price data for multiple tickers.  
It includes:
- Data cleaning and preparation.
- Visualization of trends, volatility, and returns.
- Forecasting future prices using the `pmdarima` AutoARIMA model.


## 🛠️ Steps Performed

### 1. Data Acquisition & Cleaning
- Downloaded historical OHLCV data for selected tickers.
- Removed unnecessary header rows.
- Set `Date` as the index (`DatetimeIndex`) and sorted data.
- Checked and handled missing values.
- Computed daily returns using Adjusted Close.

### 2. Exploratory Data Analysis (EDA)
- Plotted price trends over time.
- Examined daily returns distribution.
- Calculated rolling volatility.
- Compared performance across tickers.

### 3. Time Series Forecasting
- Used `pmdarima` AutoARIMA to select optimal ARIMA parameters.
- Split data into training and testing sets (80/20 split).
- Evaluated model using RMSE and MAPE.
- Generated forecasts for future dates.

## 📦 Requirements
Install dependencies with:
```bash
pip install pandas numpy matplotlib seaborn pmdarima yfinance

##  How to Run
Clone the repository:
```bash
git clone <repo_url>
cd project
Run the EDA notebook:
```bash
jupyter notebook notebooks/1.0-eda.ipynb
Run the forecasting notebook:
```bash
jupyter notebook notebooks/2.0-forecasting.ipynb
