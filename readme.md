# Tesla Stock Price Forecasting and Financial Analysis

## Project Overview

This project focuses on financial data analysis and stock price forecasting using historical Tesla stock market data. The project combines Exploratory Data Analysis (EDA), data visualization, deep learning, statistical forecasting, and dashboard development to analyze Tesla stock trends and predict future stock prices.

The project was implemented using Python for forecasting and Power BI for dashboard visualization.

---

# Objectives

- Analyze Tesla historical stock market data
- Perform data cleaning and preprocessing
- Conduct Exploratory Data Analysis (EDA)
- Visualize stock market trends
- Build forecasting models for stock price prediction
- Compare forecasting model performance
- Develop an interactive Power BI dashboard
- Generate business insights from financial data

---

# Dataset Information

## Source
- Yahoo Finance
- Data downloaded using the `yfinance` Python library

## Dataset Columns

| Column | Description |
|---|---|
| Date | Trading date |
| Open | Opening stock price |
| High | Highest stock price |
| Low | Lowest stock price |
| Close | Closing stock price |
| Adj Close | Adjusted closing price |
| Volume | Number of shares traded |

---

# Technologies Used

## Programming & Analysis
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- TensorFlow / Keras
- Statsmodels
- pmdarima

## Dashboard & Visualization
- Power BI

---

# Project Workflow

## 1. Data Collection
- Tesla stock data fetched using Yahoo Finance API (`yfinance`)

## 2. Data Cleaning
- Handling missing values
- Date formatting
- Sorting stock data chronologically
- Feature selection
- Data normalization using MinMaxScaler

## 3. Exploratory Data Analysis (EDA)
- Stock price trend analysis
- Trading volume analysis
- Monthly trend analysis
- Correlation analysis
- Financial trend identification

## 4. Data Visualization
Visualizations created include:
- Stock price trend charts
- Trading volume charts
- Monthly average stock price charts
- Forecast comparison charts
- RMSE and MSE comparison charts

## 5. Forecasting Models
The following forecasting models were implemented:

### Deep Learning Models
- SimpleRNN
- LSTM

### Statistical Forecasting Models
- ARIMA (2,1,2)
- Holt-Winters Exponential Smoothing

---

# Forecasting Strategy

## Window Size
- 60 previous trading days

## Forecast Horizons
- 1-Day Prediction
- 5-Day Prediction
- 10-Day Prediction

---

# Model Evaluation Metrics

The models were evaluated using:

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

---

# Model Performance Results

| Model | RMSE |
|---|---|
| SimpleRNN (1-Day) | 19.61 |
| LSTM (1-Day) | 19.87 |
| LSTM (5-Day) | 34.93 |
| LSTM (10-Day) | 44.40 |
| SimpleRNN (5-Day) | 60.70 |
| ARIMA (2,1,2) | 77.60 |
| SimpleRNN (10-Day) | 82.70 |
| Holt-Winters | 98.79 |

---

# Key Insights

- Deep learning models outperformed traditional forecasting techniques.
- SimpleRNN achieved the lowest forecasting error.
- LSTM demonstrated stable long-term forecasting capability.
- ARIMA captured linear stock trends moderately well.
- Holt-Winters struggled with highly volatile Tesla stock data.
- Tesla stock prices showed strong volatility and rapid trend fluctuations.

---

# Power BI Dashboard

The project dashboard contains 3 pages:

## Page 1 — Stock Market Overview
- KPI cards
- Tesla stock trend visualization
- Trading volume analysis
- Monthly average stock price
- Interactive slicers

## Page 2 — Forecasting Dashboard
- Actual vs predicted stock prices
- RNN forecast visualization
- LSTM forecast visualization
- ARIMA forecast visualization
- Holt-Winters forecast visualization

## Page 3 — Model Performance Dashboard
- RMSE comparison charts
- MSE comparison charts
- Best model indicators
- Model evaluation summary

---

# Project Structure

```bash
Tesla-Stock-Forecasting/
│
├── data/
│   ├── cleaned_tesla_stock.csv
│   ├── actual_vs_predicted.csv
│   └── model_comparison.csv
│
├── notebooks/
│   └── tesla_stock_forecasting.ipynb
│
├── dashboard/
│   └── tesla_forecasting_dashboard.pbix
│
├── report/
│   └── Tesla_Financial_Forecasting_Report.pdf
│
└── README.md
```

---

# Sample Visualizations

## Stock Price Trend
- Tesla stock movement over time

## Forecast Comparison
- Actual vs predicted stock prices

## Model Evaluation
- RMSE comparison of forecasting models

---

# Future Improvements

- Add Prophet forecasting model
- Include sentiment analysis from financial news
- Deploy forecasting model using Streamlit
- Real-time stock prediction using APIs
- Add more financial indicators and technical analysis

---

# Conclusion

This project successfully demonstrated financial data analysis and stock price forecasting using both deep learning and traditional statistical models.

The combination of Python-based forecasting and Power BI dashboard development created a complete end-to-end financial analytics solution. Deep learning models such as SimpleRNN and LSTM achieved the best forecasting performance for Tesla stock prediction.

---

# Author

Aayush Raj  
B.E. AIML Student  
Methodist College of Engineering
