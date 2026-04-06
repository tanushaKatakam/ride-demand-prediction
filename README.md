<img width="1412" height="543" alt="image" src="https://github.com/user-attachments/assets/1768018d-7070-4afe-a4ed-925cf612c158" /># Ride Demand Prediction and Analysis Dashboard
Developed a ride demand forecasting system using Random Forest and Prophet, incorporating time-based features and lag variables, and built a Tableau dashboard to analyze demand patterns and forecast future trends.

1. PROJECT OVERVIEW

This project analyzes and predicts bike ride demand using:

-Time series forecasting (Prophet)
-Machine learning (Random Forest)
-Interactive visualization (Tableau Dashboard)

Goal:

To understand demand patterns and compare predictive model performance.

2. DATASET DESCRIPTION

The dataset contains:

datetime → timestamp
season, yr, mnth, hr → time-based features
temp, atemp, hum, windspeed → weather data
holiday, workingday, weekday → categorical features
count → target variable (ride demand)

3. DATA PREPROCESSING

Feature Engineering
-Extract useful time patterns
-Helps ML models understand seasonality

Lag Feature
-Uses previous demand to predict current demand
-Captures temporal dependency

Handling Missing Values
-Required because lag creates null values

4. MODEL

Model 1 : Random Forest

-Handles non-linear relationships
-Works well with mixed features
-Robust to noise


Model 2 : Prophet

-Built for time series
-Handles seasonality automatically
-Good baseline model

5. MODEL COMPARISON

Compared Actual Predictions vs Random Forest Predictions vs Prophet Predictions.
Visualized using Line Chart(Tableau)

<img width="1056" height="725" alt="image" src="https://github.com/user-attachments/assets/e8334f7d-4a0e-4d20-8403-8b08b472f5c3" />

WHICH MODEL WAS BETTER?

Random Forest performed better because it captured non-linear relationships and short-term fluctuations using features like lag, weather, and time variables. Prophet, on the other hand, was useful for capturing overall trends and seasonality but failed to model sudden demand spikes since it produces smoother predictions and doesn’t incorporate external features in its basic form.

6. TABLEAU DASHBOARD

<img width="1263" height="855" alt="image" src="https://github.com/user-attachments/assets/68bf1913-e342-4a1c-a8e7-dba4af58597c" />

<img width="775" height="855" alt="image" src="https://github.com/user-attachments/assets/a738ecd8-718e-406e-a4c4-72c92a8b3a93" />

<img width="534" height="855" alt="image" src="https://github.com/user-attachments/assets/fc0eba57-865e-4708-98a1-79b172babc58" />

<img width="1422" height="855" alt="image" src="https://github.com/user-attachments/assets/7cc3bf36-fb3d-4e18-819e-7884ab5129a3" />

<img width="2400" height="2000" alt="Ride Deamnd Prediction Dashboard" src="https://github.com/user-attachments/assets/6f5b877f-4e00-422e-9713-496476bfd7fe" />


7. BUSINESS INSIGHTS

Key Findings:
-Peak demand occurs at 5 PM, indicating commute usage
-Clear weather significantly increases demand
-Demand increases with temperature
-Random Forest captures variability better than Prophet

8. TOOLS & TECHNOLOGIES
   
-Python (Pandas, NumPy)
-Scikit-learn (Random Forest)
-Prophet (Time Series Forecasting)
-Tableau (Dashboard Visualization)

9. FINAL PROJECT

This project demonstrates:

*Time series forecasting
*Machine learning modeling
*Feature engineering
*Data visualization
*Business insight extraction
