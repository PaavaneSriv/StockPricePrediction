# Stock Price Prediction using LSTM
## Project Overview
This project aims to analyze historical stock price data and build an LSTM-based machine learning model to predict future stock prices.
Through exploratory data analysis (EDA), we extracted key insights about price trends, volatility, and volume behavior. The LSTM model was trained on historical prices to generate future predictions.

## About the Project
Stock market prediction is a classic data science and machine learning problem.
Accurate stock price forecasting can provide valuable insights to traders and investors to make informed decisions.

## Objective
* Perform basic EDA and extract useful KPIs (Key Performance Indicators).
* Build a deep learning model to predict the next day stock price.
* Evaluate model performance and visualize predictions.
* Demonstrate capability of LSTM architecture for time-series forecasting.

## Dataset
Data source: [Kaggle](https://www.kaggle.com/datasets/emrekaany/google-daily-stock-prices-2004-today/data?select=googl_daily_prices.csv)

The dataset used contains the following columns:
* Date — Trading date
* Open — Opening price on that day
* High — Highest price of the day
* Low — Lowest price of the day
* Close — Closing price of the day
* Volume — Total shares traded

Data preprocessing steps included:
* Handling missing values
* Converting Date to datetime format
* Sorting data by Date
* Scaling features using MinMaxScaler

## Tools and Libraries
* Programming Language: Python

* Libraries:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn
  - tensorflow / keras


## Methodology
1. Data Preprocessing:
  - Cleaned data
  - Sorted and formatted dates
  - Scaled numeric values using MinMaxScaler
  - Created input sequences for LSTM 

2. Exploratory Data Analysis (EDA):
  * Analyzed price trends and volatility
  * Extracted KPIs such as:
     - Average price volatility
     - Correlation between volume and price change
     - High/Low stock prices
     - Moving Averages

  * Visualized price trends and patterns

3. Model Development:
* Built an LSTM neural network
* Trained using past time_step days to predict next day's price
* Used MSE loss and Adam optimizer

4. Model Evaluation:
* Calculated RMSE for training and testing sets
* Visualized predicted vs actual prices
* Forecasted next day's stock price and cross-validated manually

## Model Architecture
* Type: LSTM Neural Network

* Layers:
    - LSTM layer(s)
    - Dense output layer
    - Activation: linear
    - Loss function: Mean Squared Error (MSE)
    - Optimizer: Adam
    - Epochs: 50

## Conclusion 
Insights:
* Model predictions are realistic and closely follow actual stock price trends.
* Model successfully captures short-term stock movements.
* Testing RMSE is reasonable, indicating the model generalizes well.
* Visual analysis shows model predictions aligned with actual data.
* Predicted next-day price (sample): 110.46 — consistent with recent trends.
