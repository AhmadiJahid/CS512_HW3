# CS512_HW3

Sensorless Drive Diagnosis Using XGBoost
This project classifies cars based on features extracted from electric drive currents. It uses the Sensorless Drive Diagnosis dataset from the UCI Machine Learning Repository and leverages the XGBoost library for multi-class classification.

Overview
The dataset contains features from electric drive currents of cars with intact and defective components.
The goal is to classify cars into 11 distinct classes based on the extracted features.
The project demonstrates:
Data preprocessing
Hyperparameter tuning
Model evaluation using metrics like AUC and ROC curves
Dataset
Source: UCI Machine Learning Repository - Sensorless Drive Diagnosis Dataset
Description:
Features: 48 numerical features extracted from electric drive currents.
Labels: 11 classes representing different conditions of the car's components.
Size: 58,509 samples.
Model
Algorithm: Gradient Boosting using XGBoost.
Key Features:
Hyperparameter Tuning:
Number of trees (n_estimators)
Tree depth (max_depth)
Learning rate (learning_rate)
Metrics:
Micro-averaged AUC
ROC Curve for each class
Steps to Reproduce
Setup:

Install required libraries:
bash
Copy code
pip install xgboost scikit-learn matplotlib pandas
Download the dataset from the UCI Repository and save it as sensorless_drive_diagnosis.txt.
Run the Code:

Train the model and tune hyperparameters:
Number of trees (n_estimators)
Tree depth (max_depth)
Learning rate (learning_rate)
Select optimal hyperparameters based on AUC.
Final Model:

Combine training and validation datasets.
Retrain the model using the best hyperparameters.
Evaluate the model on the test set.
Evaluate:

Test AUC: 0.99999
Visualize the ROC curve.
Results
Best Hyperparameters:
Number of trees (n_estimators): 100
Tree depth (max_depth): 6
Learning rate (learning_rate): 0.01
Test AUC: 0.99999
ROC Curve:
Near-perfect classification with micro-average AUC of 1.000.
Project Structure
sensorless_drive_diagnosis.txt: Dataset file.
train_model.py: Python script for training and evaluating the model.
README.md: This documentation.
Dependencies
Python 3.8+
Required libraries:
xgboost
scikit-learn
matplotlib
pandas
numpy
Acknowledgements
Dataset provided by the UCI Machine Learning Repository.
Model implementation uses the XGBoost library.
