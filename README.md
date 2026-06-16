# 🛡️ SafePath — Early Health Risk Alert System for Pilgrims

A machine learning project that predicts health risk levels for pilgrims during Hajj, enabling proactive intervention before emergencies occur.

-----

## 📌 Problem

During Hajj, pilgrims face sudden health crises such as heatstroke, fainting, and dehydration. Current systems only respond *after* the crisis happens. SafePath aims to predict these risks *before* they occur.

-----

## 🎯 Objective

Build a classification model that predicts whether a pilgrim is at risk of a health emergency, using physiological and environmental data.

-----

## 📂 Dataset

- **Source:** Hajj & Umrah Crowd Management Dataset (Kaggle)
- **Size:** 10,000 records × 30 features
- **Target variable:** `Emergency_Event` (Yes / No)

-----

## ⚙️ Feature Engineering

Three composite features were created to improve model performance:

|Feature         |Description                                       |
|----------------|--------------------------------------------------|
|`Risk_Level`    |Combination of temperature and fatigue level      |
|`Heat_Risk`     |Correlation between temperature and age group     |
|`Crowd_Pressure`|Impact of crowd density and interpersonal distance|

-----

## 🤖 Models Trained

|Model        |Train Accuracy|Test Accuracy|
|-------------|--------------|-------------|
|Decision Tree|52.2%         |48.1%        |
|Random Forest|62.58%        |50.25%       |
|**XGBoost**  |**74.3%**     |**50.35%**   |

✅ XGBoost selected as the best performer.

-----

## 🔍 Top Predictive Features (Random Forest)

1. Crowd Pressure
1. Stress Level
1. Movement Speed
1. Age Group
1. Heat Risk
1. Crowd Density
1. Temperature
1. Distance Between People
1. Queue Time
1. Fatigue Level

-----

## 📊 Power BI Dashboard

An interactive dashboard was built to monitor pilgrim health in real time.

**Key metrics:**

- Total Pilgrims: 10,000
- Emergency Cases: 5,000
- Overall Risk Rate: 49.94%
- Medium Risk: 63.85% | High Risk: 36%

**Key insight:** Ages 31–50 and 70+ are the most vulnerable groups.

-----

## 🛠️ Tech Stack

- Python (pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn)
- Google Colab
- Power BI

-----

## 👩‍💻 Authors

- Ebdaa Btawi
- Ensherah Alghamdi
- Ghala Alzaydani

-----

## 🔮 Future Work

- Train on real pilgrim data for higher accuracy
- Explore deep learning for enhanced pattern detection
- Integrate with IoT sensors for real-time alerts
- Develop proactive intervention capabilities
