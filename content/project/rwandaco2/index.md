---
title: Rwanda CO2 Forecasting
date: 2023-08-21
tags:
    - Forecasting
    - Machine Learning
    - Atmospheric Sciences
featured: false
---

A Kaggle competition tasked with forecasting carbon dioxide (CO<sub>2</sub>) emissions in Rwanda.

<!--more-->

Accurate CO<sub>2</sub> forecasting is important in the field for atmospheric sciences as it allows for climate change understanding and mitigation. Europe and North America both have systems in place to easily monitor CO<sub>2</sub> emissions; however, in Africa, these systems aren't as prevalent, making it currently difficult to monitor CO<sub>2</sub> emissions. This Kaggle competition was hosted for the task of creating an open source CO<sub>2</sub> emission forecasting tool using machine learning techniques. Data collected from the [Sentinel-5P](https://sentinels.copernicus.eu/web/sentinel/missions/sentinel-5p) satellite served as the input for the machine learning models in development, and the forecasted amount of CO<sub>2</sub> emissions was the output. Fields included in the data inputs were 75 columns with the latitude, longitude, year, and week number of the data recorded along with data regarding the SO<sub>2</sub>, CO, NO<sub>2</sub>, formaldehyde, UV aerosol index, ozone, and clouds recorded from the satellite.

Experience with feature engineering, forecasting, and working with time series data in general was gained through participating in this Kaggle competition. Prior to this project, I had not worked with time series data, and all the data I had worked with would always be discrete. With this project, I was able to work with the concept of time windows and methods for gathering data through those time windows - such as rolling mean - which is commonly used to augment and connect entries within time series data.

Models were evaluated using the root mean squared error between the true amount of CO<sub>2</sub> emissions at any record and the predicted amount of CO<sub>2</sub> emissions. 41% of the predictions were used for the [public leaderboard](https://www.kaggle.com/competitions/playground-series-s3e20/leaderboard?tab=public) and 59% of the predictions were used for the [private leaderboard](https://www.kaggle.com/competitions/playground-series-s3e20/leaderboard?). My predictions had a public RMSE of 21.07137, placing me at 169/1442, and a private RMSE of 13.42658, placing me at 241/1442.
