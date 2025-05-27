# Traffic-Volume-Prediction

# 🚦 Traffic Volume Prediction using Random Forest

This project predicts traffic volume based on time and weather features using a **Random Forest Regressor**. The dataset contains historical traffic data with time stamps, weather conditions, and volume measurements.

---

## 📁 Contents

- Data Preprocessing
- Feature Engineering
- Model Training
- Model Evaluation
- Feature Importance Analysis
- Visualizations

---

## 📊 Dataset Overview

The dataset includes the following columns:

- `date_time`: Timestamp of the observation
- `temp`, `rain_1h`, `snow_1h`, `clouds_all`: Weather features
- `weather_main`, `weather_description`: Categorical weather indicators
- `holiday`: Holiday indicator
- `traffic_volume`: Number of vehicles observed (target)

---

## 🔧 Preprocessing & Feature Engineering

- Converted `date_time` to datetime format.
- Extracted time features: `hour`, `dayofweek`, `month`, `is_weekend`, `is_rush_hour`.
- Dropped irrelevant columns: `date_time`, `holiday`, `weather_description`.
- One-hot encoded the `weather_main` categorical feature.
- Normalized continuous weather features using `StandardScaler`.

---
