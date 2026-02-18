# climate-intelligence-system
### IoT + Cloud + Machine Learning + Predictive Alerts

An end-to-end climate monitoring and forecasting system built using Raspberry Pi Pico 2W, MicroPython, ThingSpeak Cloud, and advanced Machine Learning models.

This project integrates real-time IoT data collection with time-series forecasting, anomaly detection, and interactive deployment.

---

## 🚀 Project Overview

This system simulates and validates a real-world IoT climate monitoring architecture:

IoT Device → Cloud Storage → Data Pipeline → ML Forecasting → Anomaly Detection → Predictive Alert → Dashboard

---

## 📡 IoT Layer

### 🔹 Hardware
- Raspberry Pi Pico 2W
- Temperature & Humidity Sensor

### 🔹 Firmware
- MicroPython
- WiFi-enabled data transmission

### 🔹 Features
- Periodic temperature & humidity logging
- Automatic upload to ThingSpeak cloud
- Telegram bot notification when threshold exceeded

---

## ☁️ Cloud Integration

- ThingSpeak used for IoT data ingestion
- REST API used for data retrieval
- Historical meteorological data used to simulate extended IoT backtesting

---

## 🧠 Machine Learning Pipeline

### 🔹 Feature Engineering
- Lag features (lag_1, lag_2, lag_24)
- Rolling mean & rolling standard deviation (24-hour window)
- Time features (hour, day_of_week)
- Temperature–humidity interaction feature

### 🔹 Models Implemented
- Linear Regression (R² ≈ 0.99)
- Random Forest
- XGBoost

### 🔹 Model Evaluation
- Time-based train-test split
- MAE, RMSE, R² metrics
- Residual analysis
- Feature importance visualization

---

## 🚨 Anomaly Detection

Isolation Forest used to detect unusual temperature patterns.

- Contamination rate: 2%
- ~15 anomalies detected in 31-day dataset

---

## 🔔 Alert System

Two types of alerts implemented:

1. Threshold-based Telegram alert (IoT layer)
2. Forecast-based predictive alert (ML layer)

Example:
If predicted next-hour temperature exceeds threshold → Trigger alert.

---

## 📊 Streamlit Dashboard

Interactive web application built using Streamlit.

Features:
- User input-based temperature forecasting
- Real-time model prediction
- Interactive UI
- Clean deployment structure

Run dashboard:

streamlit run dashboard/app.py

---
# 🌦 Climate Intelligence System  
### IoT + Cloud + Machine Learning + Predictive Alerts

An end-to-end climate monitoring and forecasting system built using Raspberry Pi Pico 2W, MicroPython, ThingSpeak Cloud, and advanced Machine Learning models.

This project integrates real-time IoT data collection with time-series forecasting, anomaly detection, and interactive deployment.

---

## 🚀 Project Overview

This system simulates and validates a real-world IoT climate monitoring architecture:

IoT Device → Cloud Storage → Data Pipeline → ML Forecasting → Anomaly Detection → Predictive Alert → Dashboard

---

## 📡 IoT Layer

### 🔹 Hardware
- Raspberry Pi Pico 2W
- Temperature & Humidity Sensor

### 🔹 Firmware
- MicroPython
- WiFi-enabled data transmission

### 🔹 Features
- Periodic temperature & humidity logging
- Automatic upload to ThingSpeak cloud
- Telegram bot notification when threshold exceeded

---

## ☁️ Cloud Integration

- ThingSpeak used for IoT data ingestion
- REST API used for data retrieval
- Historical meteorological data used to simulate extended IoT backtesting

---

## 🧠 Machine Learning Pipeline

### 🔹 Feature Engineering
- Lag features (lag_1, lag_2, lag_24)
- Rolling mean & rolling standard deviation (24-hour window)
- Time features (hour, day_of_week)
- Temperature–humidity interaction feature

### 🔹 Models Implemented
- Linear Regression (R² ≈ 0.99)
- Random Forest
- XGBoost

### 🔹 Model Evaluation
- Time-based train-test split
- MAE, RMSE, R² metrics
- Residual analysis
- Feature importance visualization

---

## 🚨 Anomaly Detection

Isolation Forest used to detect unusual temperature patterns.

- Contamination rate: 2%
- ~15 anomalies detected in 31-day dataset

---

## 🔔 Alert System

Two types of alerts implemented:

1. Threshold-based Telegram alert (IoT layer)
2. Forecast-based predictive alert (ML layer)

Example:
If predicted next-hour temperature exceeds threshold → Trigger alert.

---

## 📊 Streamlit Dashboard

Interactive web application built using Streamlit.

Features:
- User input-based temperature forecasting
- Real-time model prediction
- Interactive UI
- Clean deployment structure

Run dashboard:

streamlit run dashboard/app.py

---

## 📌 Key Insights

- Strong daily seasonality observed.
- Lag_24 emerged as most influential feature.
- Linear models outperformed tree models due to high autocorrelation.
- Isolation Forest successfully detected rare anomalies.
- System successfully integrates IoT + ML + deployment pipeline.

---

## ⚙ Tech Stack

- Python
- MicroPython
- Raspberry Pi Pico 2W
- ThingSpeak API
- Telegram Bot API
- Pandas
- Scikit-learn
- XGBoost
- Isolation Forest
- Streamlit
- Matplotlib / Seaborn

---

## 🎯 Skills Demonstrated

- IoT systems engineering
- Cloud-based data ingestion
- Time-series forecasting
- Feature engineering
- Model comparison & evaluation
- Anomaly detection
- Alert automation
- ML deployment

---

## 🏆 Outcome

Built a complete IoT-enabled predictive climate intelligence system integrating hardware, cloud infrastructure, and advanced machine learning models.

---

## 🌍 Real-World Applications

This system can be adapted for:

- Smart agriculture (temperature & humidity monitoring for crop optimization)
- Industrial environmental monitoring
- Smart buildings & HVAC optimization
- Early heatwave detection systems
- Energy demand forecasting
- Climate anomaly tracking

The modular design allows integration with real IoT hardware and production cloud systems.


