# 🛰️ Waze User Churn Prediction  
### *Google Advanced Data Analytics Professional Certificate*

![Project Banner](https://via.placeholder.com/1000x220.png?text=Waze+User+Churn+Prediction+Project)

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Model](https://img.shields.io/badge/Model-XGBoost-blue)
![Tech Stack](https://img.shields.io/badge/Tech%20Stack-Python%20%7C%20Pandas%20%7C%20Sklearn-orange)
![Focus](https://img.shields.io/badge/Focus-Churn%20Prediction-purple)

---

## 🚗 Project Overview

This project develops a **machine learning model** to predict **monthly user churn** for Waze. By identifying users at risk of uninstalling or becoming inactive, Waze can strengthen retention strategies and support long‑term business growth.
---

## 🎯 Business Case

Churn is a **critical performance metric** for Waze. High retention indicates satisfied users, which is essential for scaling the business and maintaining a healthy community of map editors and drivers.

This project addresses three strategic questions:
- **Who** is most likely to churn?
- **Why** users churn?
- **When** churn is likely to occur?
---

## 🛠️ Methodology — PACE Framework

<strong>1. Plan & Analyze</strong>
- Identified the business problem and defined *churn* as monthly inactivity or app uninstalls.
- Conducted **Exploratory Data Analysis (EDA)** to explore relationships between:
  - Drive frequency
  - Device type
  - Retention behavior

<summary><strong>2. Construct — Feature Engineering & Modeling</strong></summary>

**Feature Engineering:**
- Developed new predictors such as:
  - `km_per_driving_day`
  - `percent_sessions_in_last_month`

**Model Development:**
- Designed and implemented two ensemble learners:
  - **Random Forest** — robust baseline + feature importance analysis.
  - **XGBoost** — superior predictive accuracy and efficient gradient boosting.

<summary><strong>3. Execute — Evaluation & Recommendations</strong></summary>

- Evaluated models using **Precision**, **Recall**, and **F1‑score**.
- Applied **Threshold Tuning** (set to *0.089*) to increase recall.
- Achieved **50% identification** of users likely to churn.
---

## 📈 Key Results

- **Top Predictor:** `activity_days` — Total days the user was active in the app during the month was the strongest indicator of retention.
- **Model Performance:** The final **XGBoost model** achieved an **F1 score of 0.37** and a **Recall of 0.50**.
- **Business Impact:** Enables targeted re‑engagement campaigns (notifications, incentives) for high‑risk user segments.
---

## 📦 Project Deliverables

- **[Jupyter Notebook](./waze-churn-project(1).ipynb):** Full end‑to‑end analysis (cleaning → modeling → evaluation).
- **[PACE Strategy Document](./PACE_Strategy.pdf):** Structured planning and methodology.
- **[Executive Summary](./Executive_Summary.pdf):** Insights and recommendations for Finance & Operations.
---

## 💻 Tech Stack

- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit‑Learn, XGBoost
