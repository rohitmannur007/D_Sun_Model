Vitamin D Deficiency Prediction Project
Overview
This repository contains a Jupyter Notebook for predicting Vitamin D deficiency status using machine learning models. The project involves data exploration, preprocessing, model training (Logistic Regression and Random Forest), evaluation, and selection of the best model based on metrics like AUC, Precision, and Recall.
The dataset is synthetic/generated and includes features related to health and lifestyle factors that may influence Vitamin D levels.
Key Features:

Data Loading & EDA: Importing libraries, loading the dataset, checking distributions, and visualizing data types and target class balance.
Preprocessing: Handling missing values, encoding categorical variables, and splitting data into train/test sets.
Modeling: Training and hyperparameter tuning for Logistic Regression and Random Forest using GridSearchCV.
Evaluation: ROC curves, AUC scores, precision, recall, and confusion matrices.
Model Selection: Automatically selects the best model based on evaluation metrics.

Dataset

File: Enhanced_Vitamin_D_Deficiency_Prediction.xlsx
Description: A dataset with 50,000 entries (including headers) containing the following columns:

Age: Patient's age.
BMI: Body Mass Index.
Sun_Exposure_Hours_Per_Week: Weekly sun exposure in hours.
Physical_Activity_Level: Activity level (1-3 scale).
Vitamin_D_Intake_mcg_Per_Day: Daily Vitamin D intake in mcg.
Latitude: Geographic latitude (influences sunlight availability).
Risk_Score: Calculated risk score.
Deficiency_Status: Target variable ("Deficient" or "Normal").


Class Distribution: Approximately 71% Deficient, 29% Normal.
Source: Synthetic data; not based on real-world collection.

Requirements
To run the notebook, you'll need Python 3.x and the following libraries:

pandas
numpy
matplotlib
seaborn
plotly
scikit-learn (sklearn)

Install them via pip:
pip install pandas numpy matplotlib seaborn plotly scikit-learn
