# Telecom Customer Churn Prediction
## Objective
This project aims to build a machine learning model that predicts customer churn for a telecom company. The goal is to identify customers at high risk of leaving, allowing the business to offer targeted promotions and improve customer retention.

## Key Highlights
Built and evaluated multiple classification models (CatBoost, Random Forest, XGBoost, LightGBM, Decision Tree)

Engineered features while avoiding data leakage (e.g., removing tenure)

Handled class imbalance with upsampling

Performed cross-validation with StratifiedKFold

Delivered actionable business recommendations based on feature importance

Achieved ROC-AUC score: 0.8126, with strong precision and recall on the churn class

# churn-prediction-project-flow

-data/                 # Raw datasets

-notebooks/

  -churn_EDA.ipynb     # Initial analysis and plan of action
  
  -Telecom Churn Prediction - Machine Learning.ipynb # tested machine learning models.
  
  -Telicom ML solution Report.ipynb # the solution report for the project

-README.md             # You're here!

-requirements.txt      # list of libraries used
