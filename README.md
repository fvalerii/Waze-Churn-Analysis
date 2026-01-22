## Waze User Churn Prediction Project - Google Advanced Data Analytics

🚗 Project Overview

This project was developed as part of the Google Advanced Data Analytics Professional Certificate. The goal is to build a machine learning model to predict monthly user churn for Waze. By identifying users at risk of uninstalls or inactivity, Waze can optimize retention strategies and drive long-term business growth.

🎯 Business Case

Churn is a critical metric for Waze. High retention indicates satisfied users, which is essential for scaling the business and maintaining a healthy community of map editors and drivers. This project addresses three core questions for Waze leadership:

1. Who are the users most likely to churn?

2. Why do users churn?

3. When do users churn?

🛠️ Methodology: The PACE Framework
I followed the PACE (Plan, Analyze, Construct, Execute) strategy to ensure a structured approach to problem-solving:

1. Plan & Analyze
Identified the business problem and defined "churn" (monthly inactivity/uninstalls).

Performed Exploratory Data Analysis (EDA) to find correlations between drive frequency, device type, and retention.

2. Construct (Feature Engineering & Modeling)
Feature Engineering: Developed new predictors such as km_per_driving_day and percent_sessions_in_last_month.

Model Selection: Designed and implemented two ensemble learners:

Random Forest: For robust baseline performance and feature importance analysis.

XGBoost: For superior predictive accuracy and gradient boosting efficiency.

3. Execute (Evaluation & Recommendations)
    Evaluated models using Precision, Recall, and F1-score.

    Implemented Threshold Tuning (lowered to 0.089) to increase recall, ensuring the model identifies 50% of the churning population.

📈 Key Results
Top Predictors: The most influential factor in predicting churn was activity_days (total days the user was active in the app during the month).

Model Performance: The final XGBoost model achieved an F1 score of 0.37, providing a data-driven baseline for identifying high-risk users.

Business Impact: By identifying at-risk users, Waze can now target the identified segment with proactive re-engagement offers.

📦 Project Deliverables
Jupyter Notebook: Complete end-to-end Python analysis, from cleaning to deployment.

PACE Strategy Document: Detailed project management and planning documentation.

Executive Summary: A concise report of findings and strategic recommendations for the Finance and Operations departments.

💻 Tech Stack
Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, XGBoost
