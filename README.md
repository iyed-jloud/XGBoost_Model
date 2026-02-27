# Li-Ion Battery Predictive Maintenance (RUL Estimation)

## Project Overview
This project focuses on **Predictive Maintenance** for Lithium-Ion batteries using Machine Learning. The goal is to estimate the **Remaining Useful Life (RUL)** of a battery based on sensor data (Voltage, Temperature, Cycles).

By using **XGBoost (Extreme Gradient Boosting)**, this system can predict battery failure before it happens, allowing for optimized maintenance schedules in electric vehicles or industrial systems.

## Repository Structure
This repository demonstrates my progression from theory to industrial application:

| File | Description | Level |
| :--- | :--- | :--- |
| **[`01_XGBoost_Fundamentals.ipynb`](./01_XGBoost_Fundamentals.ipynb)** | Introduction to XGBoost using the classic Boston Housing dataset. |  Educational |
| **[`02_RUL_Battery_Project.ipynb`](./02_RUL_Battery_Project.ipynb)** | **Main Project:** Simulating battery degradation and predicting RUL. |  **Industrial** |

## Technical Stack
* **Algorithm:** XGBRegressor (Gradient Boosting)
* **Language:** Python 3
* **Libraries:** `xgboost`, `pandas`, `numpy`, `scikit-learn`
* **Metric:** MSE (Mean Squared Error)

## The "Digital Twin" Approach
Since real-time battery degradation data is expensive to collect, I developed a **physics-based simulation** in the notebook to generate realistic sensor data:

* **Inputs ($X$):**
    * `Cycles`: Number of charge/discharge cycles.
    * `Temperature`: Operating temperature (simulating overheating risk).
    * `Voltage`: Terminal voltage drop over time.
* **Target ($y$):**
    * `RUL`: Remaining Useful Life (in hours/cycles).

## Model Performance
The model was trained on 1000 simulated battery instances.

* **Accuracy:** The model successfully captures the non-linear relationship between temperature stress and battery life.
* **Result:** `MSE ≈ 43.5` (The prediction is extremely close to the physical reality).

---
*Project developed by IYED JLOUD.*
