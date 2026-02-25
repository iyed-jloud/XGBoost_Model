# XGBoost_Model
# ⚡ Li-Ion Battery RUL Prediction (XGBoost)

## 📌 Project Overview
This project focuses on **Predictive Maintenance** for embedded energy systems.
The goal is to estimate the **Remaining Useful Life (RUL)** of Lithium-Ion batteries based on sensor telemetry data using **Machine Learning (XGBoost)**.

## 🎯 Objective
In industrial contexts (EVs, IoT), battery failure can be critical. This algorithm processes raw sensor data to predict when maintenance is required, moving from a *preventive* to a *predictive* strategy.

## 🛠️ Tech Stack & Methodology
* **Algorithm:** XGBoost Regressor (Extreme Gradient Boosting).
* **Language:** Python 3.x.
* **Key Libraries:** Pandas (Data Processing), Scikit-Learn (Metrics).

### Why XGBoost?
* **Efficiency:** Optimized for structured data (Voltage, Current, Temp).
* **Speed:** Low latency inference suitable for future edge deployment.
* **Robustness:** Handles missing values effectively (simulating sensor faults).

## 📊 Dataset (Simulated POC)
For this Proof of Concept (POC), data is simulated based on battery physics principles:
* **Features:** Voltage (V), Temperature (°C), Vibration (Hz), Cycle Count.
* **Target:** RUL (Hours).

## 🚀 How to Run
1. Open the `.ipynb` file in Google Colab or Jupyter.
2. Run the training cell to generate the model.
3. View the prediction error (RMSE) and feature importance.

---
*Author: IYED JLOUD - Advanced Electronics Engineering Student*
