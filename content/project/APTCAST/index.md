---
title: APTCAST
date: 2025-08-03
tags: 
    - Forecasting
    - Time Series Analysis
    - Atmospheric Science
featured: true
---

A project using data from the National Oceanic and Atmospheric Administration (NOAA) to forecast specific atmospheric features.

<!--more-->

The atmospheric precipitation, temperature, and cloudiness forecast (APTCAST) project where statistics and forecasting methods are used to have forecasts of rain, temperature, and cloudiness. Each of these atmospheric features when forecasted could help with making informed decisions. One local example for the island of Maui - where I live - is that when temperature goes higher there's a higher risk of fires, which can be devastating in Maui as shown in the 2023 Lahaina fires. Current progress only includes non machine learning temperature forecasts, and this project page will be updated as progress is made.

The initial scope of this project was to forecast global data; however the global data I found was shown to be limited to one year of data. The work for this was shown in the main_old.ipynb file in the GitHub below. I had lowered the scope to be for Maui specifically, as I am currently residing in Maui, and I could see the benefit of the forecasting. Local Climatological Data (LCD) was then ordered from NOAA's Climate Data Online (CDO) tool on their Kahului station. While there is also a station near Kapalua, there was no data regarding the temperature on Maui for that station. The data in Kahului included temperature information from 1996-2025.

To create the temperature forecasting tool, I followed the process of exploratory data analysis (EDA), feature engineering, non-machine learning (ML) forecasting, and ML forecasting. During the EDA phase I had used Polars as my main dataframe management library, Matplotlib for plotting data, and Statsmodels for statistical analysis. Plotting the data I was able to identify outliers, as well as plot autocorrelations and partial autocorrelations to show the nature of seasonality/trend as well as which lagged values are important for the forecasting in future steps. During feature engineering, I studied the correlations of each of the fields in the data, and found that the months had a high correlation with the temperature. This had me thinking to model the seasons; however, with normal seasons by month, I found a slightly lower correlation than I anticipated, so I used specific equinox and solstice times to model more specific seasons true to the Earth's nature. This correlation was higher than the normal season by month. I've also encoded the data to be efficiently read by ML models in the future when implemented, with methods such as normalization and sin/cos encoding. Lastly, in the non-ML forecasting phase I decomposed the data into seasonality, trend, and error. Decomposing the data helped as seasonality and trend can be modeled separately, seasonality would be modeled as a simple sin function, and I used ARIMA to get the trend. Using the Akaike Information Criterion (AIC) to do a grid search and optimize the model hyperparameters. The model developed yielded an mean absolute error (MAE) of about 2.5, mean squared error (MSE) of 9.8, and root mean squared error of 3.1. Below is a forecast for the previous year plotted against the ground truth values, with ground truth being blue and forecast being orange.

![Temperature Forecast](APTCAST-results.png "Temperature Forecast")

During this project I had learned how to use Polars, which is much like Pandas but it supports multi-threading, unlike Pandas. While Polars is new and has a much faster framework with it's lazyframes, I was also able to learn of Polars' drawbacks, such as the lack of integration with external libraries, such as statsmodels. I've also learned much about the forecasting process of time series data, as I've done forecasting on data before, but not with extensive data in the past. In my undergraduate studies I had learned about error, trend, and seasonality decomposition as well as autocorrelation but never applied it as I have during this project. For future endeavors with the APTCAST project I intend on implementing ML forecasting with Recurrent Neural Networks using the ARIMA model, forecast the other atmospheric features, and extend the scope to global atmospheric features.

Source: <a href="https://github.com/PrestonTGarcia/APTCAST"><i class="large github icon"></i>PrestonTGarcia/APTCAST</a>

