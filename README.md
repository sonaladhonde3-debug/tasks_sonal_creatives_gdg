# tasks_sonal_creatives_gdg

Here is a concise version of the README for your project.

GDG Task 2: Regression & Classification
Overview
This project implements two supervised learning models:

Regression: Predicting Crab Age using Support Vector Regression (SVR).

Classification: classifying anonymous data using K-Nearest Neighbors (KNN).

1. Regression (Crab Age Prediction)
Goal: Predict age based on physical measurements.

Preprocessing: Cleaned data (dropped id, filtered Height=0), engineered Lost Weight feature, and one-hot encoded Sex.

Model: SVR (Linear Kernel).

Results:

R² Score: 0.531 (Moderate fit).

RMSE: 2.15 years.

Insight: Used SHAP values to explain feature importance.

2. Classification (Anonymous Data)
Goal: Classify data points into Target Class 0 or 1.

Preprocessing: Standardized features using StandardScaler to normalize scales.

Model: KNN (K-Nearest Neighbors).

Optimization: Used the Elbow Method to find the best K.

Best K: 5

Best Accuracy: 95.3% (Improved from 92.7% baseline).

Tools Used
Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, shap.
