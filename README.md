# Apple Stock Market Price Prediction Using Time Series Forecasting Model
## User Interface:
#### https://anilwaded-stock-market-price-prediction-project-usin-app-8xdtyd.streamlit.app/

## Introduction: 
#### The Apple stock price prediction project can be helpful for investors and stock market analysts who are interested in trading Apple stocks. By using time series forecasting models, the project aims to provide insights and predictions on the future trend of Apple's stock prices. This information can assist investors in making informed decisions about buying or selling Apple stocks, thereby potentially maximizing their profits and minimizing their risks. Additionally, the project can serve as an example for others interested in using time series forecasting techniques for stock market analysis.

## Objective: 
#### The goal of this project is to predict the future stock price of Apple based on almost past 8 years stock market data of Apple.

## Raw dataset: 
#### https://drive.google.com/file/d/11MmxS7ta-1KPPRXfI4TP2LohvjlCdJac/view?usp=share_link

## Pre-processed dataset:
#### https://drive.google.com/file/d/1uVbwxLxa4PUNGlpIOvGS4bGMj5WJ1OwY/view?usp=share_link

## About Dataset:
### Content
#### The dataset for Apple stock prices contains the historical prices of Apple stocks from 2012 to 2019, with a total of almost 8 years of data. The dataset includes seven variables: date, open price, high price, low price, closing price, adjusted closing price, and trading volume. These variables provide information about the daily trading activity of Apple stocks, including the opening and closing prices, the highest and lowest prices, and the trading volume. The adjusted closing price takes into account any corporate actions such as stock splits or dividends, providing a more accurate reflection of the stock's value. The dataset is a valuable resource for analyzing and forecasting the performance of Apple stocks in the stock market.

## Acknowledgements:
#### The data has been taken and compiled from the Yahoo Finance.
#### The below will get you the source of the data
#### https://finance.yahoo.com/quote/AAPL/history?p=AAPL

## Tools
#### Python : Jupyter Notebook

## Project Summery:
### 1. EDA
####    From the data I came to Know that:
####    There are not any missing, duplicate and null values in the dataset.
####    Datatype of Date column was in object type

### 2. Data Preprocessing
####    Here, I converted the datatype of Date column to Datetime.
####    Checked wheather the dataset contains holidays or not, Concluded Time series data contains holidays other than weekends.

### 3. Model Building and Evaluation: 
####   I have built the model with 4 different Time series Forecasting Models:
####   1) ARIMA Model
####   2) ARIMA with Seasonal order using Maximum likelihood estimation
####   2) SARIMA with Quarterly Seasonality
####   3) Holt-Winter Triple Exponential Smoothing
####   As the exponential smoothing methods predict future patterns to heavily represent current ones they are less effective in long term forecasting. So selecting Arima with Seasonal order and Sarima with Quaterly seasonality as the best models for forecasting. As Sarima with Quaterly Seasonality looks computationally heavy, using Arima with seasonal order for the forecasting.

### 4. Deployment
####   I have deployed ARIMA with Seasonal Order using Maximum Likelyhood estimation with R2 Score of 45.75%

#### Script: https://github.com/Anilwaded/Apple_Stock_Market_Price_Prediction_Project_Deployment#readme

## Conclusion:
#### In conclusion, the project on Apple stock price prediction using time series models has demonstrated the effectiveness of ARIMA with seasonal order in forecasting the future stock prices of Apple Inc. The project involved data preprocessing, exploratory data analysis, and model building and evaluation. The selected model was deployed on a web app using Streamlit to allow users to input their preferred time range and obtain the predicted stock prices. This project is valuable to investors, traders, and analysts who seek to make informed decisions based on future stock price trends.
