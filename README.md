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

## churn-prediction-project-flow

-data/                 # Raw datasets

-notebooks/

  -churn_EDA.ipynb     # Initial analysis and plan of action
  
  -Telecom Churn Prediction - Machine Learning.ipynb # tested machine learning models.
  
  -Telicom ML solution Report.ipynb # the solution report for the project

-README.md             # You're here!

-requirements.txt      # list of libraries used

## Tools & Libraries Used
Python, Jupyter Notebook

pandas, numpy

matplotlib, seaborn

scikit-learn

xgboost, lightgbm, catboost

## Data Cleaning & Preparation
Removed high-leakage features like tenure, BeginDate, and EndDate

Dropped irrelevant columns like customerID and gender

Applied one-hot encoding to categorical variables

Created new target variable churn from existing date columns

## Models trained and compared:

Decision Tree

Random Forest

XGBoost

LightGBM

CatBoost (Best performer)

## best performing model peramiters
{
  'random_strength': 9,
  'learning_rate': 0.1,
  'l2_leaf_reg': 9,
  'iterations': 100,
  'depth': 4,
  'bootstrap_type': 'Bayesian',
  'bagging_temperature': 2
}

## Evaluation Metrics
ROC-AUC Score: 0.8126

Precision: 0.66

Recall: 0.55

F1 Score: Balanced and strong across classes

## Key Insights & Business Impact
Top churn drivers:

MonthlyCharges

TotalCharges

ContractLengthMonths (engineered feature)

Customers with higher monthly bills and short-term (month-to-month) contracts are more likely to churn.

Business Recommendations
Encourage customers to sign longer-term contracts with benefits (e.g., discounted rates or perks) to reduce churn risk.

## Future Improvements
Improve recall further through advanced feature engineering

Deploy model with Streamlit or Flask for real-time predictions

## How to Run This Project
To explore or reproduce the full workflow of this project, follow these steps:

1. Clone the Repository

git clone https://github.com/your-username/churn-prediction-project.git

cd churn-prediction-project

3. Set Up the Environment

Make sure you have Python 3.7+ installed. Then install required packages:

pip install -r requirements.txt

Alternatively, launch in a virtual environment or Conda environment if you prefer.

3. Open the Jupyter Notebook or in a text editor that suports .ipynb files. (i use vscode)
   
Launch Jupyter Notebook:

jupyter notebook

Then open and follow the notebooks in this order:

1. churn_EDA.ipynb
Initial data exploration and planning.

2. Telecom Churn Prediction - Machine Learning.ipynb
Model building and evaluation.

3. Telicom ML Solution Report.ipynb
Summary report with business recommendations.


## Contact
Author: Zach Thomas
LinkedIn: linkedin.com/in/zachary-thomas01
GitHub: github.com/ZacharyThomas767
