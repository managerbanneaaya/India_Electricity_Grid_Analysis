# India_Electricity_Grid_Analysis
Carbon Emission Analysis &amp; Prediction using Machine Learning (XGBoost, Linear Regression) and energy mix insights.
# 🌍 Carbon Emission Analysis & Prediction

## 📌 Overview

This project analyzes electricity generation data to understand the relationship between energy sources and carbon emissions. It also builds machine learning models to predict carbon intensity based on load and generation mix.

---

## 🎯 Objectives

* Analyze hourly, monthly, and seasonal emission patterns
* Understand the impact of energy mix on carbon intensity
* Build predictive ML models
* Validate model on unseen time-based data

---

## 📊 Key Insights

* Renewable energy (solar, hydro) significantly reduces carbon emissions
* Carbon intensity is driven more by **energy mix** than total load
* Peak emission periods are harder to predict
* No autocorrelation in residuals → model captures time patterns well

---

## 🧠 Features Used

* Hour
* Total Load (MW)
* Coal
* Solar
* Wind
* Hydro

---

## 🤖 Models Used

* Linear Regression (baseline)
* XGBoost (final model)

---

## 📈 Model Performance

| Dataset            | R²     | RMSE |
| ------------------ | ------ | ---- |
| Train              | ~0.99  | ~7   |
| Test               | ~0.99  | ~6   |
| Unseen Data (2023) | ~0.989 | ~5.4 |

✔ Strong generalization across time

---

## 🔍 Model Diagnostics

* Residuals centered around zero
* No autocorrelation (validated)
* Slight heteroscedasticity at extreme values
* Feature importance confirms energy mix dominance

---

## 📂 Project Structure

```
carbon-emission-analysis/
│
├── data/
├── notebooks/
├── plots/
├── models/
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
```

---

## 📊 Visualizations

* Hourly load vs carbon intensity
* Generation mix analysis
* Residual diagnostics
* Feature importance

---

## 🔥 Key Learning

* Importance of feature engineering
* Avoiding data leakage
* Time-based validation
* Residual analysis for model improvement

---

## 📌 Future Improvements

* Add weather data
* Use advanced models (LightGBM, LSTM)
* Deploy as API/dashboard

---

## 👨‍💻 Author

**Abhishek Gabhane**

---

## ⭐ If you like this project, give it a star!
