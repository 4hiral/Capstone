# Data Gap Prediction in IoT: An ML-Based Approach for Smart Systems

This project presents a machine learning-based solution to handle **data gaps in IoT systems**, particularly in **smart environments** like smart cities, agriculture, or industrial monitoring. Using historical sensor data and real-time inputs, our model predicts missing temperature values during transmission failures to maintain data continuity and support intelligent decision-making.

## 🚀 Project Overview

In real-world IoT deployments, sensor data may occasionally be **lost** due to network issues, power loss, or hardware glitches. This project aims to:

- Collect temperature and humidity data using **Arduino Uno** in real-time.
- Train a regression model to **predict missing temperature values** based on historical patterns.
- Handle **missing data** intelligently without compromising the accuracy of downstream analytics.
- Incorporate **seasonal trends** using time and month-based features for improved predictions.

## 🔧 Technologies Used

- **Python**
- **Arduino Uno** (for real-time data collection)
- **Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn**
- **CSV for data storage and model training**
- **Jupyter Notebook** for experimentation

## 📂 Project Structure

```bash
├── Arduino/
│   └── temperature_humidity_sensor.ino   # Arduino sketch for DHT11/DHT22 data reading
├── data/
│   └── real_time_data.csv                # Real-time collected data
│   └── historical_weather_data.csv       # One year of city weather data
├── model/
│   └── gap_prediction_model.pkl          # Trained ML model
├── notebooks/
│   └── EDA_and_Model_Training.ipynb      # Data exploration and ML modeling
├── utils/
│   └── preprocessing.py                  # Helper functions for data cleaning
├── README.md
└── requirements.txt
