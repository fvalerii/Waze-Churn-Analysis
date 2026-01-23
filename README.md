# 🛰️ Waze User Churn Prediction  
### *Google Advanced Data Analytics Capstone Project*

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Model](https://img.shields.io/badge/Model-XGBoost-blue)
![Tech Stack](https://img.shields.io/badge/Tech%20Stack-Python%20%7C%20Pandas%20%7C%20Sklearn-orange)
![Focus](https://img.shields.io/badge/Focus-Churn%20Prediction-purple)

---

## 🚗 Project Overview
This project develops a machine learning model to predict **monthly user churn** for Waze. By identifying users at risk of uninstalling or becoming inactive, the goal is to provide Waze with actionable insights to optimize retention and product development.

---

## 🎯 Business Case
Churn is a critical performance metric for Waze. High retention indicates satisfied users and a stable community. In collaboration with stakeholders from **Finance (Emrick Larson)** and **Operations (Ursula Sayo)**, this project investigates:
- **Who** is most likely to churn?
- **Why** do users churn (key behavioral drivers)?
- **What** additional data is needed to improve predictive accuracy?

---

## 🛠️ Methodology — PACE Framework

### 1. Plan & Analyze
* **Exploratory Data Analysis (EDA):** Investigated relationships between drive frequency, device types, and retention behavior.
* **Data Assessment:** Identified that existing features had relatively low predictive power regarding churn, suggesting that user behavior is complex and likely influenced by factors outside the current dataset.

### 2. Construct (Feature Engineering & Modeling)
* **Feature Engineering:** Created several new predictors; notably, **6 of the top 10 features** in the final model were engineered features (e.g., `km_per_driving_day`).
* **Model Development:** Compared **Logistic Regression**, **Random Forest**, and **XGBoost**. The ensemble tree-based models (RF and XGBoost) significantly outperformed the linear model.

### 3. Execute (Evaluation & Recommendations)
* **Performance Metrics:** While the XGBoost model achieved a high accuracy (~70%), the baseline **Recall was low (~16%)**.
* **Threshold Tuning:** To explore business utility, I adjusted the decision threshold to **0.089**, which boosted **Recall to 50%** at the cost of Precision. 
* **Final Verdict:** Due to the high number of false negatives, the current model serves as a strong **baseline** but requires further data refinement before being deployed for high-stakes business decisions.

---

## 📈 Key Results & Recommendations
* **Top Predictor:** `activity_days` was the strongest indicator of retention.
* **Model Selection:** **XGBoost** was selected as the champion model for its superior performance on the validation and test sets.
* **Strategic Recommendation:** I recommend **not deploying this model for automated business decisions** until more granular data is gathered (e.g., geographic locations, specific destination counts, and more detailed app interaction logs).
* **Future Work:** Focus on gathering "intent-based" data to help differentiate between casual users and those truly at risk of leaving the platform.

---

## 📦 Project Deliverables
- **[Jupyter Notebook](./notebooks/Waze-Churn-Analysis.ipynb):** Full end-to-end Python analysis (cleaning → modeling → threshold tuning).
- **[Executive Summary](./docs/Waze-Executive-Summary.pdf):** A high-level report on model performance and data recommendations for leadership.
- **[PACE Strategy Document](./docs/Waze/PACE-Strategy-Document):** Detailed project planning and methodology documentation.

---

## 💻 Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, XGBoost
- **Framework:** PACE (Plan, Analyze, Construct, Execute)

---

> **Note:** The data, characters, and incidents portrayed in this project are synthetic and were created by Google for pedagogical purposes as part of the Advanced Data Analytics Certificate.
