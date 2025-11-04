PROJECT OVERVIEW:

This project focuses on analyzing and forecasting daily public transport passenger journeys using time series modeling.
The goal is to identify meaningful trends and predict future passenger volumes for different transport services such as Local Route, School, Light Rail, and others.
The dataset used is based on daily passenger counts from 2019 to 2024, showing clear seasonal patterns and long-term trends in usage.


METHODS UDES:
Data Cleaning & Preprocessing
Exploratory Data Analysis (EDA)
Modeling
Forecasting

INSIGHTS:
Local Route Service

1.Passenger numbers show strong seasonal peaks — likely linked to workweek travel and holiday reductions.
2.Gradual upward trend post-2022, possibly indicating recovery after disruptions like COVID-19.

School Service

1.Passenger counts show clear weekday patterns, with steep drops during holidays or weekends.
2.After differencing, the series became stationary — confirming seasonal school-based travel cycles.


Model Performance:
Model	Target	MAE	RMSE
SARIMA(1,1,1)(1,1,1,12)	Local Route	7770.19	8901.87
SARIMA(1,1,1)(1,1,1,12)	School route	(similar range, showing strong seasonality)
