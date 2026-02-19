# 📊 Smart Classroom Energy Forecasting using ARIMA

## 📌 Overview
This project predicts the **next-hour classroom electricity consumption** using historical energy data and Wi-Fi-based occupancy signals.  
It demonstrates how smart campus infrastructure can leverage time-series forecasting for energy optimization.

---

## 🧠 Problem Statement
Classrooms often consume electricity inefficiently due to unpredictable occupancy patterns.

This project answers:
> Can we forecast next-hour energy usage using historical electricity trends (influenced by occupancy)?

---

## 📂 Dataset Description

### 1️⃣ Wi-Fi Occupancy Data
- `timestamp` – Hourly time
- `room_id` – Classroom identifier
- `connected_devices` – Number of Wi-Fi connected devices (occupancy proxy)

### 2️⃣ Energy Consumption Data
- `timestamp` – Hourly time
- `room_id` – Classroom identifier
- `energy_kwh` – Electricity consumption (kWh)

Both datasets are merged using:
timestamp + room_id



---

## ⚙️ Tech Stack
- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels (ARIMA)
- Google Colab / Jupyter Notebook

---

## 📈 Model Used

### ARIMA (1,1,1)
- **AR** – Auto Regression
- **I** – Integrated (Differencing)
- **MA** – Moving Average

The model forecasts:
- 🔮 Next-hour energy usage
- 📉 Lower confidence bound
- 📈 Upper confidence bound (95%)

---

## 🚀 Workflow

1. Generate or collect Wi-Fi & energy data  
2. Merge datasets by timestamp  
3. Apply rolling mean smoothing  
4. Train ARIMA model  
5. Forecast next-hour energy  
6. Visualize prediction with confidence interval  

---

## 📊 Output Example
Next Hour Forecast: 2.32 kWh
Lower Bound: 1.45 kWh
Upper Bound: 3.19 kWh



Visualization includes:
- Historical energy trend
- Forecast line
- Shaded confidence interval

---

## 📦 Installation

Install required libraries: pip install pandas numpy matplotlib statsmodels


Or run directly in Google Colab.

---

## 🔬 Future Improvements
- Use SARIMAX with occupancy as external variable
- Multi-hour forecasting
- RMSE evaluation
- Deploy as Streamlit dashboard
- Integrate real IoT sensor data

---

## 🎯 Applications
- Smart Campus Systems
- Energy Optimization
- Classroom Usage Analytics
- Sustainable Infrastructure Planning







