# 💧 Water Quality Prediction using Machine Learning

This project aims to predict the concentration of key water pollutants such as **O2, NO3, NO2, SO4, PO4, and CL** using machine learning techniques. The dataset used includes historical water quality data from multiple monitoring stations, and the model is trained to forecast future pollutant levels based on date and station information.

---

## 📁 Dataset Overview

- **File Name:** `PB_All_2000_2021.csv`
- **Format:** CSV (`;` separated)
- **Columns Include:**
  - `id`: Station identifier
  - `date`: Measurement date
  - `O2`, `NO3`, `NO2`, `SO4`, `PO4`, `CL`: Target pollutants
- **Years Covered:** 2000 to 2021

---

## 🎯 Goal

To predict six important water pollutants using:
- Station ID
- Year
- Month

---

## 🛠️ Technologies Used

- **Language:** Python
- **Libraries:**
  - `pandas`, `numpy` for data handling
  - `matplotlib`, `seaborn` for visualization
  - `scikit-learn` for machine learning
  - `joblib` for model saving

---

## 🔍 Steps Followed

1. **Data Preprocessing**
   - Convert date column to datetime
   - Extract `year` and `month`
   - Sort and clean dataset
   - Drop rows with missing pollutant values

2. **Feature Engineering**
   - One-hot encode the `id` (station)

3. **Modeling**
   - Train a **RandomForestRegressor** wrapped in a **MultiOutputRegressor**
   - Use `train_test_split` to split data into training/testing sets

4. **Prediction**
   - Custom prediction based on selected station, year, and month

5. **Evaluation**
   - Display R² Score, MAE, RMSE for each pollutant

6. **Saving**
   - Save trained model and feature list using `joblib`

---

## 📈 Sample Output

```text
Predicted pollutant levels for station 22 in June 2024:
O2   : 7.18
NO3  : 2.95
NO2  : 0.43
SO4  : 20.87
PO4  : 0.35
CL   : 12.60



