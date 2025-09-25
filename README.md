# Telecom-Churn

- Preprocessing: Applied tailored preprocessing for each model; for CatBoost, two approaches were used — in one model categorical features were converted/encoded, while in the other they were passed in their original form. For other models (XGBoost, Logistic, RF, KNN), appropriate encoding was applied.

- Models: Trained Logistic Regression, Random Forest, KNN, XGBoost, and two CatBoost models (with and without categorical feature conversion).

- Hyperparameter Tuning: Used Optuna for KNN, CatBoost, Random Forest, and XGBoost to find the best parameters.

- Ensembles: Built Voting (hard & soft) and Stacking models combining top base learners.

- Evaluation: Compared base models and ensembles using appropriate metrics.

- Note: XGBoost tuned with Optuna gave the best results.
