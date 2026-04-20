# 📊 HAVELLS Stock Time Series Analysis (Assignment)

## 📌 Overview

This project performs a **time series analysis** on the stock of **HAVELLS (NSE: HAVELLS.NS)** using historical data for the past 1 year.
The objective is to analyze trends and forecast future stock prices using the **ARIMA model**.

---

## 🎯 Objectives

* Perform data preprocessing on stock data
* Visualize stock price trends
* Check stationarity using ADF test
* Apply ARIMA model for time series forecasting
* Predict next 30 days stock prices
* Interpret the results

---

## 🧪 Methodology

### ✔ 1. Data Collection

* Historical stock data downloaded using **yfinance**
* Time period: Last 1 year
* Data includes daily closing prices

---

### ✔ 2. Data Preprocessing

* Converted date column into datetime format
* Set date as index
* Handled missing values using forward fill
* Extracted closing price for analysis

---

### ✔ 3. Data Visualization

* Plotted closing price trend over time
* Observed fluctuations and general trend

---

### ✔ 4. Stationarity Check (ADF Test)

* Applied Augmented Dickey-Fuller (ADF) test
* Result indicated that the series was **non-stationary**
* Applied differencing to make data stationary

---

### ✔ 5. ACF and PACF Analysis

* Generated ACF and PACF plots
* Used to determine ARIMA parameters (p, d, q)

---

### ✔ 6. ARIMA Model

* Applied ARIMA model with parameters (1,1,1)
* Trained model on historical data
* Evaluated using summary statistics

---

### ✔ 7. Forecasting

* Predicted stock prices for the next **30 days**
* Visualized forecast along with historical data

---

## 📊 Results & Observations

* The stock price shows fluctuations typical of market behavior
* After differencing, the series became stationary
* ARIMA model successfully captured the trend
* Forecast indicates a **(write: upward / downward / stable)** trend for the next 30 days

---

## 📁 Project Structure

```
HAVELLS_TimeSeries_Analysis/
│
├── data/
│   ├── havells_stock.csv
│   └── forecast_30_days.csv
│
├── output/
│   ├── closing_price.png
│   ├── acf_plot.png
│   ├── pacf_plot.png
│   ├── forecast_plot.png
│
├── code/
│   └── HAVELLS_analysis.ipynb
│
└── README.md
```

---

## 📷 Output Graphs

The following visualizations are included:

* Closing Price Trend
* ACF Plot
* PACF Plot
* Forecast Plot

(All graphs are available in the **output/** folder)

---

## ⚖️ AI Ethics & Responsible Usage Declaration

This project uses only publicly available stock market data.
No personal, confidential, or sensitive data has been used.
The analysis is conducted strictly for **educational purposes**.
All results are interpreted responsibly without misleading conclusions.

---

## ✅ Conclusion

The ARIMA model provides a reasonable short-term forecast for stock prices.
However, stock markets are influenced by external factors, so predictions may vary.
This analysis demonstrates how time series models can be applied in real-world financial data.

---
