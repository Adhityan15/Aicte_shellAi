# 💧 Water Quality Prediction Using Machine Learning

This project predicts water pollution levels across 22 stations in India using a machine learning model trained on historical data from 2000–2021. The deployed app allows users to select a year and station ID and get predictions for six major pollutants.

---

## 🌊 Project Overview

- **Pollutants Tracked**: O₂, NO₃, NO₂, SO₄, PO₄, Cl
- **Dataset Used**: `waterqualitypred.csv`
- **Total Records**: 2,861
- **Features Used**: `id`, `year`
- **Target Outputs**: O₂, NO₃, NO₂, SO₄, PO₄, Cl

---

## ✅ Week 1: Data Preprocessing

- Loaded the CSV using **pandas**
- Converted `date` column to datetime format
- Extracted `year` and `month`
- Handled missing values using `dropna()`
- Encoded `station id` using `get_dummies()`
- Final features: `year`, `id_*` columns
- Target: Pollutant levels

---

## 🤖 Week 2: Model Training

- **Model Used**: `MultiOutputRegressor` with `RandomForestRegressor`
- Split: 80% Training, 20% Testing
- Evaluation Metrics:  
  - 📉 Mean Squared Error (MSE)  
  - 📈 R² Score
- Saved trained model with `joblib`

🔗 **Model File**:  
[Google Drive - pollution_model.pkl](https://drive.google.com/file/d/18RJzu35vyuMgpcAE590u1IaDvHY3-SWq/view)

---

## 🚀 Week 3: Deployment

- Developed interactive UI using **Streamlit**
- User inputs: Year & Station ID
- Output: Predicted values for all 6 pollutants
- Model loaded from `.pkl` file via Git LFS
- Deployed on **Streamlit Community Cloud**

🔗 **Live App**:  
[https://waterqualitypredictor.streamlit.app](https://waterqualitypredictor.streamlit.app)

---

## 🛠️ Tech Stack

- Python
- pandas, numpy
- scikit-learn
- joblib
- Streamlit
- Git LFS (for handling large model files)

---

## 📂 Repository Structure

├── app.py # Streamlit app
├── pollution_model.pkl # Trained model (via Git LFS)
├── model_columns.pkl # Columns used in the model
├── datasetwaterquality.csv # Original dataset
├── requirements.txt # Required Python packages
├── README.md # You're here!


## ✨ Future Scope

- Add station name auto-fill
- Visualize pollutant trends by year
- Mobile-responsive UI

---

Made with 💙 by [Adhityan](https://github.com/Adhityan15)
