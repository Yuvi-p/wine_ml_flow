# wine_ml_flow
Wine Classification &amp; Experiment Tracking with MLflow | An end-to-end machine learning pipeline for wine recognition, featuring systematic experiment tracking, hyperparameter logging, and model versioning using MLflow.

Project Overview
The objective of this project was to develop a robust classification model to identify the origin of wines based on their chemical signatures. Beyond the model itself, the primary focus was on implementing MLflow to manage the machine learning lifecycle, ensuring every experiment is reproducible, trackable, and comparable.


Dataset Description
The project utilizes the Wine Recognition Dataset, which consists of chemical analyses of wines grown in the same region in Italy but derived from three different cultivars.

Samples: 178 samples across 3 classes.

Features: 13 constituent measurements, including:

Alcohol, Malic acid, and Ash.

Alkalinity of ash, Magnesium, and Total phenols.

Flavanoids, Nonflavanoid phenols, and Proanthocyanins.

Color intensity, Hue, and Proline.

Machine Learning Pipeline
1. Data Preprocessing

Standardizing features to handle varying scales across chemical measurements.

Splitting the data into training and testing sets to validate model performance.


2. Experiment Tracking (MLflow)

The core of this project is the integration of MLflow Flow, which allows for:

Parameter Logging: Tracking hyperparameters such as n_estimators, max_depth, and learning_rate.

Metric Logging: Recording Accuracy, F1-Score, and Precision for every run to compare model iterations.

Artifact Storage: Saving generated plots (Confusion Matrices, Feature Importance) and the trained model files directly within the MLflow UI.


3. Model Performance

Model Used: Random Forest Classifier.

Key Results: The model achieved high classification accuracy, with the experiment tracking revealing that "Proline" and "Flavanoids" were the most significant indicators of wine cultivar.

🛠️ Tech Stack
Language: Python

Machine Learning: scikit-learn

Lifecycle Management: MLflow

Data Manipulation: pandas, numpy

Visualization: matplotlib, seaborn

How to View Results
To view the experiment dashboard:

Ensure MLflow is installed (pip install mlflow).

Run mlflow ui in the project directory.

Project developed as part of Assignment 2 in Machine Learning Course.
