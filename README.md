# Aicte_shellAi
Water Quality Prediction Using Machine Learning

🌊 Water Pollution Prediction (2000–2021)
This project predicts water pollutant levels across 22 stations using machine learning.

📁 Dataset
File: waterqualitypred.csv

Records: 2861

Pollutants Tracked: O2, NO3, NO2, SO4, PO4, CL

✅ Week 1: Data Preprocessing
Loaded CSV with pandas

Converted date to datetime, extracted year & month

Handled missing values using dropna()

Features: id, year (encoded using get_dummies)

Target: Selected pollutant columns

🤖 Week 2: Model Training & Prediction
Model: MultiOutputRegressor with RandomForestRegressor

Split data: 80% train, 20% test

Evaluation: MSE & R² score

Prediction: Given station_id and year, model predicts all 6 pollutant levels

Model saved using joblib
