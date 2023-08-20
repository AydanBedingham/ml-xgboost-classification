# Cardiovascular Disease XGBoost Classification
Jupyter Notebook that trains an XGBoost model to perform classification to detect the presence of cardiovascular disease in a person based on the given features. Trains an XGBoost model locally using SciKitLearn, performs hyperparameter tuning locally before finally training and deploying a SageMaker XGBoost model.

Original Data Source: https://www.kaggle.com/sulianova/cardiovascular-disease-dataset

## Features:
- Age | Objective Feature | age | int (days)
- Height | Objective Feature | height | int (cm) |
- Weight | Objective Feature | weight | float (kg) |
- Gender | Objective Feature | gender | categorical code |
- Systolic blood pressure | Examination Feature | ap_hi | int |
- Diastolic blood pressure | Examination Feature | ap_lo | int |
- Cholesterol | Examination Feature | cholesterol | 1: normal, 2: above normal, 3: well above normal |
- Glucose | Examination Feature | gluc | 1: normal, 2: above normal, 3: well above normal |
- Smoking | Subjective Feature | smoke | binary |
- Alcohol intake | Subjective Feature | alco | binary |
- Physical activity | Subjective Feature | active | binary |
- Presence or absence of cardiovascular disease | Target Variable | cardio | binary |

## Tasks:
- Load the Dataset 
- Perform Exploratory Data Analysis
- Perform Data Visualisation
- Create Training and Testing Datasets
- Train an XG-Boost classifier model (locally not using SageMaker)
- Perform GridSearch Hyperparameter Optimisation
- Train an XG-Boost classifier model (using Amazon SageMaker)
- Deploy trained model as an endpoint
- Assess trained model performance
- Delete the endpoint