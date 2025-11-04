PROJECT OVERVIEW:

This project focuses on analyzing and forecasting daily public transport passenger journeys using time series modeling.
The goal is to identify meaningful trends and predict future passenger volumes for different transport services such as Local Route, School, Light Rail, and others.
The dataset used is based on daily passenger counts from 2019 to 2024, showing clear seasonal patterns and long-term trends in usage.


METHODS UDES:
Data Cleaning & Preprocessing : handled missing values, sorted the dataset to avoid future data leakage to the training
Exploratory Data Analysis (EDA) : found patterns that shoes non stationarity, made the data stationarity using differencing
Modeling : used SARIMA because of the trend and seasonality in the dataset
Forecasting : predicted next 30 days passengers count

INSIGHTS:
Local Route Service

1.Passenger numbers show strong seasonal peaks — likely linked to workweek travel and holiday reductions.
2.Gradual upward trend post-2022, possibly indicating recovery after disruptions like COVID-19.
3.The dip during 2020–2021 likely reflects pandemic restrictions, followed by a consistent rise from 2022 onwards as public transport resumed normal operations.

School Service

1.Passenger counts show clear weekday patterns, with steep drops during holidays or weekends.
2.After differencing, the series became stationary — confirming seasonal school-based travel cycles.
3.The School service data exhibits sharp fluctuations aligned with school opening and closing periods.


Model Performance:
Model	Target	
SARIMA(1,1,1)(1,1,1,12)	Local Route	MAE: 7770.19	RMSE: 8901.87
SARIMA(1,1,1)(1,1,1,12)	School route	MAE: 1196.82, RMSE: 2271.87
