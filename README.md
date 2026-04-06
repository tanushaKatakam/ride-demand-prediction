# Ride Demand Prediction and Analysis Dashboard
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

<img width="2072" height="1582" alt="Ride Demand by Hour of Day" src="https://github.com/user-attachments/assets/ff7e0fa1-6541-4115-bb9e-8d8c87fa36de" />


<img width="1488" height="1582" alt="Ride Demand by Day of Week" src="https://github.com/user-attachments/assets/abab71ae-2091-49db-a978-b6283b31ed69" />


<img width="1316" height="1616" alt="Ride Demand by Weather Condition" src="https://github.com/user-attachments/assets/ef829280-b5a2-4e83-84e9-116fb0e0d1f8" />


<img width="2092" height="1506" alt="Impact of Temperature on Ride Demand" src="https://github.com/user-attachments/assets/579a28af-acca-44fc-8e1f-1eef462d2961" />


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
