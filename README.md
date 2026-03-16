# Wine Classification & Experiment Tracking with MLflow

An end-to-end machine learning pipeline for wine cultivar recognition, featuring systematic experiment tracking, hyperparameter logging, and model versioning.

---

## 📋 Project Overview
The objective of this project was to develop a robust classification model to identify the origin of wines based on their chemical signatures. Beyond model accuracy, the primary focus was on implementing **MLflow** to manage the machine learning lifecycle, ensuring every experiment is **reproducible, trackable, and comparable**.

## 🧬 Dataset Description
The project utilizes the **Wine Recognition Dataset**, consisting of chemical analyses of wines grown in the same region in Italy, derived from three different cultivars.

* **Samples:** 178 samples across 3 classes.
* **Key Features (13 total):** * **Acidity:** Malic acid, Ash, Alkalinity of ash.
    * **Phenols:** Total phenols, Flavanoids, Nonflavanoid phenols.
    * **Visual/Chemical:** Color intensity, Hue, Proline, Alcohol, Magnesium.

## ⚙️ Machine Learning Pipeline

### 1. Data Preprocessing
* **Standardization:** Scaling chemical measurements to handle varying magnitudes across features.
* **Validation:** Splitting data into training and testing sets to ensure robust performance metrics.

### 2. Experiment Tracking (MLflow)
The core of this project is the integration of **MLflow**, enabling:
* **Parameter Logging:** Systematic tracking of hyperparameters such as `n_estimators`, `max_depth`, and `learning_rate`.
* **Metric Logging:** Real-time recording of **Accuracy, F1-Score, and Precision** for every iteration.
* **Artifact Storage:** Automatic saving of generated plots (Confusion Matrices, Feature Importance) and serialized model files directly within the MLflow UI.

## 📊 Model Performance
* **Algorithm:** Random Forest Classifier.
* **Key Insight:** Through experiment tracking and feature importance analysis, **"Proline"** and **"Flavanoids"** were identified as the most significant indicators of wine cultivar.

## 🛠️ Tech Stack
* **Language:** Python
* **Machine Learning:** scikit-learn
* **Lifecycle Management:** MLflow
* **Data Science Tools:** pandas, numpy, matplotlib, seaborn

---

## 🚀 How to View Results
To explore the experiment dashboard and compare different model runs:

1. **Install MLflow:**
   ```bash
   pip install mlflow
