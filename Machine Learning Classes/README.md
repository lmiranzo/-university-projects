# Car Accident Mortality Prediction Project

The primary objective of this project is to predict whether a car accident in Canada (based on Transport Canada data 
from 1999 to 2014) will result in a fatality. 

## Part 1: Descriptive Analysis

In this initial phase, we perform an exploratory analysis to understand the data at a high level. 
This involves examining the data for missing values, outliers, and potential transformations. 
Some key questions to answer:

- Which types of vehicles (model, age, etc.) and driver profiles are most prone to accidents?
- Which types are less prone to accidents and could be eligible for premium discounts?
- What factors most contribute to fatalities in accidents?
- Can we develop a model that predicts whether medical treatment will be needed following an accident? Insurers would benefit by allocating reserves based on such predictions.

## Part 2: Data Preparation and Modeling

In this second phase, we clean and prepare the data for modeling, based on the findings from Part 1. 
Once prepared, we apply and evaluate different classification models:
- Logistic Regression
- Gradient Boosting
- Decision Tree
- Bagging
- XGBoost


Our main target variable is `passenger_fatality`, which indicates whether individuals in an accident were unharmed, injured, or deceased. For our classification model, we assume that injuries indicate a need for medical treatment, while fatalities are excluded. This simplifies our objective to a binary classification problem: predicting whether an accident will require medical assistance or not.


## Model Evaluation

Below are the results of our model evaluations:

| Model                | Accuracy | Precision | Recall | F1 Score | AUC    |
|----------------------|----------|-----------|--------|----------|--------|
| Logistic Regression  | 0.6296   | 0.6184    | 0.6768 | 0.6463   | 0.6296 |
| Gradient Boosting    | 0.6707   | 0.6625    | 0.6963 | 0.6789   | 0.7428 |
| Decision Tree        | 0.7473   | 0.7123    | 0.8297 | 0.7665   | 0.8306 |
| Bagging              | 0.7473   | 0.7120    | 0.8304 | 0.7667   | 0.8309 |
| XGBoost              | 0.6912   | 0.6790    | 0.7253 | 0.7014   | 0.7661 |

