# Project of Predicting Churn 

---

Merges four telecom CSVs (contract, personal, internet, phone), cleans and explores features like tenure and service add-ons, and trains models—from Logistic Regression to CatBoost—to predict which customers will leave, achieving about 0.85 ROC-AUC with a tuned Random Forest. Simply clone the repo, install Python 3 and libraries (pandas, scikit-learn, xgboost, lightgbm, catboost, etc.), open project_17.ipynb, and run each cell to reproduce the analysis, view charts, and see model metrics. The notebook also highlights key insights (e.g., early churn linked to month-to-month plans and missing add-ons) and offers business recommendations and next steps, making it easy for newcomers to follow and adapt for their own churn-prediction needs.

---

The notebook wraps up by noting that a Random Forest model—trained with upsampled churn cases and the new tenure-based feature—was the top performer. From the feature‐importance chart, customer tenure (begin_date), contract type, and monthly charges emerged as the strongest predictors of churn. To translate these insights into action, the conclusion recommends:

Incentivizing long-term contracts (to lock in early-stage customers)

Bundling add-on services (like online security or tech support)

Adjusting pricing for customers with higher monthly bills

These steps aim to reduce early churn by targeting the very factors the model identified as most influential.
