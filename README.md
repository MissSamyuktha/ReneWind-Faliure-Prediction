# ReneWind Failure Prediction

ReneWind Failure Prediction is a machine learning repository focused on predicting failures in wind turbines. The repository provides tools and models for analyzing wind turbine data, pre-processing datasets, training predictive models, and evaluating their performance. This project aims to improve maintenance planning and reduce downtime by forecasting potential failures before they occur.

## Requirements
To run this project, ensure you have the following dependencies installed:

- Python 3.6 or higher
- TensorFlow (2.x recommended)
- Keras
- NumPy
- Matplotlib
- Scikit-learn

## Features

- **Comprehensive Data Preprocessing**
  - Handles missing values, outliers, and normalizes input features.
  - Supports feature engineering to extract relevant attributes from raw sensor data.

- **Flexible Model Training**
  - Includes various machine learning algorithms (e.g., Random Forest, Gradient Boosting, Neural Networks).
  - Provides modular scripts for training, validating, and tuning models.

- **Robust Evaluation**
  - Implements performance metrics such as accuracy, F1-score, precision, recall, and ROC-AUC.
  - Offers confusion matrix visualization and classification reports for model assessment.

- **Automated Pipeline**
  - End-to-end automation from data loading to model evaluation.
  - Supports batch processing for large time-series datasets.

- **Extensive Visualization**
  - Plots feature importances, training curves, and evaluation metrics.
  - Visualizes failure distribution and sensor data patterns.

- **Customizable Configuration**
  - Easy-to-edit configuration files for data paths, model parameters, and evaluation settings.
  - Command-line arguments support for rapid experimentation.

- **Reproducibility**
  - Ensures reproducible results with fixed random seeds and consistent preprocessing.
  - Includes Jupyter notebooks for step-by-step analysis and demonstration.

- **Documentation and Examples**
  - Provides detailed usage instructions and example scripts.
  - Contains sample datasets for testing and experimentation.
# **Key Takeaways & Actionable Insights for ReneWind**

**Model Selection**
- **Model 6 (He Initialization + Dropout)** was selected as the best-performing model.
- It consistently achieved ~98% accuracy across train, validation, and test sets.
- **Recall** for failures (class 1) was high (85–90%) ensuring most failing generators are detected early.

**Cost-Sensitive Impact**
- **True Positives (TP)** means generators repaired before failure thereby lower cost.
- **False Negatives (FN)** minimized meaning fewer undetected failures thereby reduced replacement cost.
- **False Positives (FP)** are acceptable in moderation as inspections are cheaper than replacements.

**Business Benefits**
- **Significant reduction in maintenance costs** by shifting from reactive to predictive strategy.
- **Improved operational efficiency** and uptime of wind turbines.
- **Scalable solution:** model can be retrained periodically with new sensor data to adapt to evolving failure patterns.
---
