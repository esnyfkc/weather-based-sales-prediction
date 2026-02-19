# Weather-Based Sales Prediction

## Problem Definition

Restaurants often make staffing and inventory decisions using static weekly patterns.  
However, weather significantly impacts daily demand.

**Goal:**  
Predict next-day (D+1) restaurant sales using:

- Historical POS data
- Local weather data

**Target Variable:**  
Daily total sales ($)

**Prediction Horizon:**  
D+1 (next day)

**Granularity:**  
Daily

**Evaluation Metric:**  
Mean Absolute Error (MAE)

---

## Why This Project?

While managing a restaurant, I observed:

- Rainy days were slower
- Sudden warm evenings caused unexpected rushes
- Seasonal transitions shifted demand

This project quantifies those patterns using machine learning.

---

## Project Structure

weather-based-sales-prediction/
│
├── data/
│ ├── raw/
│ ├── interim/
│ └── processed/
│
├── notebooks/
│
├── src/
│ ├── config.py
│ ├── ingest.py
│ ├── clean.py
│ ├── features.py
│ ├── split.py
│ ├── train.py
│ ├── evaluate.py
│ ├── predict.py
│ └── utils.py
│
├── requirements.txt
└── README.md

---

## Pipeline Overview

1. Data ingestion and merging (POS + weather)
2. Data cleaning and missing value handling
3. Feature engineering (time features, rolling averages, weather interactions)
4. Time-based train/test split
5. Model training (baseline → tree-based model)
6. Evaluation using MAE

---

## Future Improvements

- Add holiday calendar features
- Add D+7 forecast
- Deploy as simple API
- Add dashboard visualization

---

## How to Run

### 1. Create virtual environment

python3 -m venv venv
source venv/bin/activate

### 2. Install dependencies

pip install -r requirements.txt


### 3. Train the model

python src/train.py


---

## Future Improvements

- Add holiday calendar features
- Extend to D+7 forecasting
- Hyperparameter tuning
- Deploy as a simple API
- Add dashboard visualization

---

## Author

Esin Yufkaci  

