# digital-twin-health-model
A Virtual Patient Model (Digital Twin) fusing static EHR data with dynamic wearable sensor time-series to predict personalized health outcomes for the Digital Twin Challenge 2026.
# Digital Twin Health Model: Virtual Patient Simulator

> Built for the **Happiest Health Digital Twin Challenge 2026** under the *Reimagining & Reforming Healthcare in India Summit*.

---

## 📌 Problem Overview
In modern healthcare, static medical records (EHR) often fail to capture real-time physiological changes, while continuous wearable streams lack patient history context. 

This project implements a **Virtual Patient Model (Digital Twin)** that fuses static EHR data (patient demographics, medical history, baseline lab metrics) with dynamic continuous time-series data (heart rate, glucose, sleep, SpO2) from wearable sensors to predict personal health outcomes and early health risks.

---

## 🎯 Key Features
* **Multi-Modal Data Fusion:** Combines tabular EHR patient history with continuous IoT wearable streams.
* **Temporal Sequence Modeling:** Uses time-series models (LSTM/GRU) to track rolling metrics and volatility.
* **Real-Time Risk Scoring:** Predicts risk levels and early anomaly warnings for target health metrics.
* **Simulated Interventions:** Demonstrates how key physiological parameters respond dynamically under different simulated conditions.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python 3.10+
* **Data Processing:** `pandas`, `numpy`, `scikit-learn`
* **Machine Learning / Deep Learning:** `PyTorch` / `TensorFlow`, `XGBoost`
* **Visualization:** `matplotlib`, `seaborn`

---

## 📁 Repository Structure

```text
├── data/
│   ├── raw/                 # Sample raw datasets (EHR & wearable logs)
│   └── processed/           # Aligned and feature-engineered datasets
├── notebooks/
│   └── digital_twin_demo.ipynb  # Interactive demonstration & evaluation
├── src/
│   ├── preprocessing.py     # Data cleaning, normalization, & alignment
│   ├── feature_engineering.py # Rolling stats and volatility metrics
│   └── train_model.py       # Model architecture and training scripts
├── requirements.txt         # Dependencies
└── README.md                # Project documentation
