---
title: Restaurants trends through time series analysis
emoji: 🍗
date: 2024-10-27T15:31:32.937Z
summary: "Exploring Restaurant Trends Through Time Series Analysis: A
  Post-Pandemic Perspective"
metaDescription: "Exploring Restaurant Trends Through Time Series Analysis: A
  Post-Pandemic Perspective"
tags:
  - R
  - timeseries
  - LSTM
---
This project delves into how the recent years' restrictions have influenced dining habits by analyzing time series data from six restaurants in the Pavia area. Spanning from 2018 to 2022, the dataset allowed us to track trends in revenue, receipt volumes, and changes in average receipt values to examine the potential impacts of the COVID-19 pandemic on restaurant performance.

The analysis was conducted using R, where we applied several time series techniques, including Error-Trend-Seasonality (ETS), Double Seasonal Holt-Winters (DSHW), and ARIMA/SARIMA models, as well as Recurrent Neural Networks (RNN) using Long Short-Term Memory (LSTM) models. R’s robust libraries, such as forecast, facilitated the decomposition and modeling of the data, helping us identify key patterns and periodic trends. Seasonal trends were especially insightful in tracking customer flow on specific days of the week, while the LSTM model allowed us to capture more complex patterns over extended periods.

Our findings indicate that while the number of receipts declined, the average value per receipt increased post-pandemic. This could imply changes in customer spending behavior or pricing adjustments. Among the models tested, DSHW and LSTM showed the most promising results for capturing these intricate patterns, particularly when forecasting short-term fluctuations.

This study demonstrates how R can be effectively used for complex time series analysis, providing valuable insights into consumer trends and helping restaurant owners make data-driven decisions to optimize their operations in changing times.