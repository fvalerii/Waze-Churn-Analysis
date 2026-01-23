# 🛰️ Waze User Churn Prediction  
### *Google Advanced Data Analytics Capstone Project*

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Model](https://img.shields.io/badge/Model-XGBoost-blue)
![Tech Stack](https://img.shields.io/badge/Tech%20Stack-Python%20%7C%20Pandas%20%7C%20Sklearn-orange)
![Focus](https://img.shields.io/badge/Focus-Churn%20Prediction-purple)

---

## 🚗 Project Overview
This project focuses on building a machine learning model to predict **monthly user churn** for Waze. In this context, "churn" is defined as users who have uninstalled the app or stopped using it for the month. Identifying these users early allows Waze to optimize retention strategies, enhance user experience, and make data-driven decisions about product development.



---

## 🎯 Business Case
User retention is a primary growth driver for Waze. High retention indicates satisfied users and a stable community of map editors and drivers. This project addresses three strategic questions for Waze leadership:
- **Who** are the users most likely to churn?
- **Why** do users churn (identifying the key behaviors)?
- **When** is churn likely to occur?

---

## 🛠️ Methodology — PACE Framework

### 1. Plan & Analyze
* **Problem Definition:** Defined the business goal—preventing monthly churn—and mapped out the project milestones using the PACE framework.
* **Exploratory Data Analysis (EDA):** Investigated data distributions and handled extreme outliers. I analyzed correlations between drive frequency, device types (iPhone vs. Android), and retention behavior.
* **Data Cleaning:** Prepared the dataset for modeling by handling missing values and ensuring consistent variable types for the modeling pipeline.

### 2. Construct (Feature Engineering & Modeling)
* **Feature Engineering:** Developed new behavioral predictors to better capture user intent, including:
    * `km_per_driving_day`: Captures average daily usage intensity.
    * `percent_sessions_in_last_month`: Measures recent engagement drops.
* **Model Development:** Designed and tuned two ensemble machine learning models:
    * **Random Forest:** Used as a robust baseline for performance and feature importance.
    * **XGBoost:** Implemented to achieve superior predictive accuracy through gradient boosting.

### 3. Execute (Evaluation & Recommendations)
* **Performance Metrics:** Evaluated models using Precision, Recall, and F1-score.
* **Threshold Tuning:** To meet the business need of capturing more potential churners, I adjusted the decision threshold to **0.089**. This increased recall to **0.50**, successfully identifying half of the churning population.
* **Strategy:** Summarized findings for cross-departmental stakeholders to assist in data-driven decision-making.

---

## 📈 Key Results
* **Strongest Predictor:** `activity_days` was the most influential feature. A decrease in active days within the month is the strongest signal that a user is about to churn.
* **Final Model Performance:** The optimized XGBoost model achieved an **F1 score of 0.373** and an **Accuracy of 70.2%** on the test set.
* **Business Impact:** By utilizing the tuned threshold, Waze can now target at-risk users with proactive re-engagement offers (e.g., push notifications or localized promotions) before they leave the platform.



---

## 📦 Project Deliverables
- **[Jupyter Notebook](./waze-churn-project(1).ipynb):** The complete end-to-end technical analysis and model build.
- **PACE Strategy Document:** Detailed documentation of project management and strategic planning.
- **Executive Summary:** A concise report of findings and recommendations tailored for non-technical leadership.

---

## 💻 Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, XGBoost
- **Framework:** PACE (Plan, Analyze, Construct, Execute)

---
