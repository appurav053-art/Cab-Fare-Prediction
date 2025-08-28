# Cab Fare Prediction ML Project

This machine learning project focuses on predicting "cab fare amount", "fuel consumption", and "combustion energy" based on various trip-related features. It uses regression techniques to build predictive models on a real-world dataset, applying effective data preprocessing, feature engineering, and model evaluation methods.


# Project Objectives

* Predict "fare amount" based on trip details like distance, time, and pickup/drop-off locations.
* Estimate "fuel consumption" using trip duration and environmental factors.
* Calculate "combustion energy" required per trip, considering fuel efficiency metrics.
* Apply machine learning techniques to create accurate, explainable models.


# Machine Learning Techniques Used

* Exploratory Data Analysis (EDA) with `matplotlib`, `seaborn`, and `pandas`
--> Feature Engineering:
  * Distance calculation using geolocation (Haversine formula)
  * Time-based features (hour of day, day of week)
--> Data Preprocessing:
  * Handling missing values and outliers
  * Feature scaling (StandardScaler / MinMaxScaler)
--> Modeling:
  * Linear Regression
  * Random Forest Regressor
  * XGBoost Regressor
--> Evaluation Metrics:
  * RMSE, MAE, R² Score


# Dataset Overview

--> The dataset includes the following key features:

| Column Name        | Description                                 |
|--------------------|---------------------------------------------|
| "pickup_datetime"  | Timestamp of the ride start                 |
| "pickup_longitude" | Pickup location longitude                   |
| "pickup_latitude"  | Pickup location latitude                    |
| "dropoff_longitude"| Drop-off location longitude                 |
| "dropoff_latitude" | Drop-off location latitude                  |
| "passenger_count"  | Number of passengers                        |
| "fare_amount"      | Fare charged for the trip (target)          |
| "trip_distance"    | Distance traveled (engineered feature)      |
| "trip_duration"    | Duration of the ride                        |
| "fuel_consumption" | Predicted fuel consumption (target)         |
| "combustion_energy"| Estimated combustion energy (target)        |


# Results Summary

| Target               | Best Model         | RMSE     | R² Score |
|----------------------|--------------------|----------|----------|
| **Fare Amount**       | XGBoost Regressor  | 2.54     | 0.92     |
| **Fuel Consumption**  | Random Forest      | 1.03     | 0.89     |
| **Combustion Energy** | Linear Regression  | 0.88     | 0.87     |


# Tools & Technologies

- **Languages:** Python 3.8+
- **Libraries:** Pandas, Numpy, Sckit-learn, Matplotlib, Seaborn, Xgboost
- **Platform:** Jupyter Notebook
- **Version Control:** Git, GitHub


# Visualizations

* Heatmaps for feature correlation
* Time-based ride patterns (rush hours, weekdays)
* Geospatial pickup/drop-off distributions
* Residual plots and prediction-vs-actual graphs

---

# How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/cab-fare-prediction.git
