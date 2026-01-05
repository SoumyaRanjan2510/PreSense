# Predictive Maintenance
# Predictive Maintenance System (Machine Learning)

## 📌 Project Overview

This project implements a **machine learning–based Predictive Maintenance system** that estimates **Remaining Useful Life (RUL)**, predicts **maintenance requirements**, and detects **anomalous equipment behavior** using sensor data. The solution is delivered through an **interactive Streamlit dashboard** for real-time analysis and visualization.

The system is trained and validated on a **balanced, simulated dataset** and demonstrates how ML models can support data-driven maintenance decisions.

---

## 🎯 Objectives

* Estimate Remaining Useful Life (RUL) of equipment
* Predict whether maintenance is required
* Detect anomalies in sensor behavior
* Provide an interactive and user-friendly dashboard

---

## 🧠 Machine Learning Models Used

* **Regression Model**: Predicts Remaining Useful Life (RUL)
* **Classification Model**: Predicts maintenance requirement (Normal / Needs Maintenance)
* **K-Means Clustering**: Supports anomaly detection
* **Scaler**: Feature normalization for model consistency

Hybrid anomaly detection is performed using:

* Low RUL threshold
* Distance from K-Means cluster centers

---

## 📊 Dataset Description

* **Records**: 1,000 (simulated and balanced)
* **Features**:

  * `sensor_temp`
  * `sensor_vib`
  * `sensor_voltage`
  * `operational_hours`
* **Target Variables**:

  * Remaining Useful Life (RUL)
  * Maintenance status

---

## 🖥️ Streamlit Dashboard Features

* Home page with system overview
* View historical sensor data
* Manual or random input of sensor values
* Prediction results (RUL, maintenance status, anomaly flag)
* Data visualizations:

  * Histograms
  * Scatter plots
  * Box plots
  * Correlation heatmap
  * Feature importance plot

---

## 📁 Project Structure

```
├── app.py                         # Streamlit application
├── balanced_simulated_data.csv    # Dataset
├── reg_model.pkl                  # RUL regression model
├── clf_model.pkl                  # Maintenance classification model
├── kmeans_model.pkl               # K-Means clustering model
├── scaler.pkl                     # Feature scaler
├── Final_Predictive_Maintenance_Notebook.ipynb  # Model development notebook
├── style.css                      # Optional UI styling
└── README.md                      # Project documentation
```

---

## ▶️ How to Run the Application

1. Install required dependencies:

```
pip install streamlit pandas numpy matplotlib seaborn scikit-learn scipy streamlit-option-menu
```

2. Run the Streamlit app:

```
streamlit run app.py
```

3. Open the browser link shown in the terminal.

---

## ✅ Key Outcomes

* Accurate RUL estimation using regression
* Reliable maintenance classification
* Effective anomaly detection using hybrid logic
* Clean and interactive visualization dashboard

---

## 📚 Applications

* Predictive maintenance systems
* Industrial equipment monitoring
* Smart manufacturing
* Condition-based maintenance research
---

## 📝 Note

This project uses **simulated data** for academic and training purposes and demonstrates the end-to-end predictive maintenance workflow.

