
# Predicting PM2.5 Concentration from Weather Data

This repository contains code and data for building a predictive model to estimate PM2.5 pollutants based on weather data. The goal is to provide actionable intelligence without the need for additional PM2.5 monitoring stations.



## Deployment

The dataset is imported and cleaned using pandas. Missing values in the PM2.5 column are interpolated linearly based on temporally adjacent values.

An initial predictive model is built using ordinary least squares regression (OLS). The R-squared value and RMSE are calculated to evaluate the model's performance.

Feature engineering is performed, including adding new features like lagged PM2.5 concentrations and encoding wind direction. These features are integrated into the dataset.

The dataset is split into training and test sets, and OLS regression is re-evaluated with the added features. The RMSE improves significantly.

Extreme Gradient Boosting (XGBoost) is applied to the dataset to build a predictive model. The RMSE is calculated, and it performs slightly better than OLS.


## Conclusion
This project demonstrates that using statistical modeling with Python can be a cost-effective solution for predicting PM2.5 concentration based on weather data, potentially reducing the need for additional monitoring stations.
