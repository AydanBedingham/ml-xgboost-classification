# Cardiovascular Disease XGBoost Classification
Jupyter Notebook that trains an XGBoost model to perform classification to detect the presence of cardiovascular disease in a person based on the given features. Trains an XGBoost model locally using SciKitLearn, performs hyperparameter tuning locally before finally training and deploying a SageMaker XGBoost model.

Original Data Source: https://www.kaggle.com/sulianova/cardiovascular-disease-dataset

Features:
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

Tasks:
- 1. Load the Dataset 
- 2. Perform Exploratory Data Analysis
- 3. Perform Data Visualisation
- 4. Create Training and Testing Datasets
- 5. Train an XG-Boost classifier model (locally not using SageMaker)
- 6. Perform GridSearch Hyperparameter Optimisation
- 7. Train an XG-Boost classifier model (using Amazon SageMaker)
- 8. Deploy trained model as an endpoint
- 9. Assess trained model performance
- 10. Delete the endpoint