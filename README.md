# Breast Cancer Prediction – Capstone Project
Machine Learning Model for Early Diagnosis using the Wisconsin Diagnostic Breast Cancer Dataset
  
  
  1. Project Overview
     
Breast cancer remains one of the leading causes of death among women globally. Early detection significantly improves survival rates, but access to reliable diagnostics is limited in many regions.
This project builds a machine learning model that predicts whether a breast tumor is benign or malignant using diagnostic features derived from breast mass cell nuclei. The goal is to support early detection and provide a foundation for decision-support systems in healthcare.
This project was completed as part of the Capstone requirement for the Machine Learning Program.

2. Objectives
Build a supervised classification model to distinguish malignant vs. benign breast tumors.
Compare multiple machine learning algorithms and select the best-performing model.
Assess model performance using clinically meaningful metrics (recall, precision, ROC-AUC).
Document the workflow clearly and reproducibly using GitHub and a written report.
Provide insights, limitations, and recommendations for real-world application.

3. Dataset
Source: Kaggle Datasets
Dataset: Breast Cancer Wisconsin (Diagnostic) Dataset
Dataset link:
https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data
Dataset Description
569 samples
30 numerical features computed from cell nucleus characteristics
Diagnosis column (target):
M = Malignant
B = Benign

4. Methodology
Preprocessing
Removed ID column
Checked and handled missing values
Feature scaling using StandardScaler
Train–test split (80/20)

Models Tested
Logistic Regression
Support Vector Machine
Random Forest Classifier
XGBoost (if available)
Evaluation Metrics
Because false negatives in cancer are extremely dangerous, we emphasized:
Precision
Recall
F1 Score
ROC–AUC
Confusion Matrix

5. Key Insights
Texture, smoothness, and perimeter-related features were most predictive.
High recall is achievable, meaning the model rarely misses malignant cases.
Dataset is clean and balanced enough for classical ML models to perform strongly.

6. Limitations
Dataset is small and may not generalize to diverse populations.
Features are handcrafted and may not capture deeper tumor characteristics.
Model should not be used for real medical diagnosis without clinical validation.

7. Recommendations
Train on larger, diverse medical datasets.
Integrate deep learning models on medical imaging.
Deploy as a clinical decision-support tool (Flask, FastAPI).
Add explainability tools (SHAP, LIME).
