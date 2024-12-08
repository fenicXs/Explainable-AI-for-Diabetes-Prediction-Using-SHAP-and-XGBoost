# Explainable-AI-for-Diabetes-Prediction-Using-SHAP-and-XGBoost

This project utilizes **XGBoost**, a powerful gradient boosting algorithm which has achieved **97% accuracy** in diabetes prediction, and **SHAP (SHapley Additive exPlanations)**, an explainability tool to provide detailed feature-level explanations for the predictions. The dataset contains health and demographic data, and the goal is to classify individuals as diabetic or non-diabetic while understanding the model's decision-making process.

![Shap]()

## Project Overview

### Key Features
1. **Diabetes Prediction**:
   - Predict diabetes based on health indicators such as age, BMI, hypertension, HbA1c level, and blood glucose level using the XGBoost model.
2. **Model Explainability**:
   - Use SHAP to explain the contribution of each feature to the model's predictions.
3. **Data Visualization**:
   - Pairwise plots and correlation heatmaps to explore relationships in the data.
4. **Performance Metrics**:
   - Evaluate the model using accuracy, confusion matrix, classification report, and log-loss plots.

## Dataset

- **Source**: [Kaggle Dataset](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset)
- **Features Used**:
  - `age`: Age of the individual.
  - `hypertension`: Binary indicator of hypertension (1: Yes, 0: No).
  - `heart_disease`: Binary indicator of heart disease (1: Yes, 0: No).
  - `bmi`: Body Mass Index.
  - `HbA1c_level`: Hemoglobin A1c level.
  - `blood_glucose_level`: Blood glucose level.
 
![correlation heatmap]()

## Dependencies

  - Install the required Python packages:
    ```bash
    pip install numpy pandas matplotlib seaborn xgboost shap scikit-learn

## Implementation Details
  1. Data Exploration
    - Visualized relationships between features using pair plots with seaborn.
    - Explored feature correlations through a heatmap.
  2. Model Training
    - Trained an XGBoost model with logloss as the evaluation metric.
    - Split data into train (80%) and test (20%) sets for validation.
  3. Performance Evaluation
    - Accuracy: Evaluated the model's performance on the test set.
    - Confusion Matrix: Visualized the classification performance.
    - Classification Report: Detailed metrics for diabetic and non-diabetic classes.
  4. Model Explainability with SHAP
    - Generated global and local explanations for the model.
    - Summary Plot: Showed the importance of features globally.
    - Force Plot: Provided a visual explanation for individual predictions.

## RESULTS

### Confusion Matrix
![confusion matrix]()

## SHAP Explainability
  - Summary Plot: Identified HbA1c_level and blood_glucose_level as key predictors.
  - Force Plot: Explained individual predictions by showing feature contributions.

