---
title: AQI Pred
emoji: 📈
colorFrom: purple
colorTo: pink
sdk: streamlit
sdk_version: 1.39.0
app_file: app.py
pinned: false
license: mit
short_description: Air Quality Prediction Using Regression Techniques
---
# Air Quality Prediction Using Regression Techniques

This project implements a comparative analysis of different regression techniques for predicting air quality in smart cities, based on the research paper "Comparative Analysis Study for Air Quality Prediction in Smart Cities Using Regression Techniques" by Al-Eidi et al.

## Overview

The project uses machine learning regression models to predict Air Quality Index (AQI) values using various air pollutant measurements. Three regression techniques are compared:
- Random Forest Regression
- Linear Regression
- Decision Tree Regression

## Dataset

The project uses the Pune Smart City Dataset (2019) which includes:
- 103,205 records from 10 monitoring stations
- 28 features related to air pollution
- Key pollutants: NO2, O3, PM10, PM2.5, SO2, CO
- Source: [Pune Smart City Dataset on Kaggle](https://www.kaggle.com/datasets/akshman/pune-smartcity-test-dataset)


## Implementation Steps

1. Data Preprocessing
   - Handle missing values using mean imputation
   - Remove outliers using IQR method
   - Perform Exploratory Data Analysis (EDA)

2. AQI Calculation
   - Calculate Air Quality Index using standard formula
   - Categorize pollution levels

3. Feature Selection
   - Correlation analysis
   - Select most relevant features

4. Model Development
   - Data splitting (70:30 train-test split)
   - Data balancing using SMOTER
   - Implementation of regression models
   - Model evaluation using RMSE, R², and MAE

## Performance Metrics

The models are evaluated using:
- Root Mean Square Error (RMSE)
- R² Score
- Mean Absolute Error (MAE)

## Citation

```
S. Al-Eidi et al., "Comparative Analysis Study for Air Quality Prediction in Smart Cities Using Regression Techniques"
```