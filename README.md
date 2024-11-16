# Bike Sharing Count Prediction

This project focuses on predicting bike-sharing counts using multi-variable linear regression models implemented in Keras. It serves as a personal practice exercise as I learn Keras. The dataset used in this project comes from Kaggle: [Bike Sharing Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/bike-sharing-dataset?select=day.csv).

## Project Overview

- **Purpose**: The primary objective is to understand and implement linear regression models using Keras to predict bike-sharing counts based on various weather and seasonal factors.
- **Tech Stack**: Python, TensorFlow, Keras
- **Data Source**: The dataset is sourced from Kaggle and includes daily counts of rental bikes along with various features like temperature, humidity, and wind speed.

## Dataset Description

The data consists of several features:
- `season`: Season of the year (1: winter, 2: spring, 3: summer, 4: fall)
- `yr`: Year (0: 2011, 1: 2012)
- `mnth`: Month (1 to 12)
- `holiday`: Whether the day is a holiday
- `weekday`: Day of the week
- `workingday`: Whether the day is a working day
- `weathersit`: Weather condition
- `temp`: Normalized temperature in Celsius
- `atemp`: Normalized "feels-like" temperature in Celsius
- `hum`: Normalized humidity
- `windspeed`: Normalized wind speed
- `cnt`: Total count of bike rentals (target variable)

## Model

The model is a simple multi-variable linear regression model implemented in Keras. It uses one normalization layer followed by a Dense layer:
- **Normalization**: To standardize input features.
- **Dense Layer**: A single linear output unit to predict bike rental counts.
