# CS512_HW3

🚗 Sensorless Drive Diagnosis with XGBoost 🚗
Classifying car conditions based on electric drive currents using machine learning. This project leverages the Sensorless Drive Diagnosis Dataset from the UCI Machine Learning Repository and the powerful XGBoost algorithm to achieve near-perfect classification accuracy.

📋 Overview
Predict the condition of car components using 48 numerical features extracted from electric drive currents.
11 distinct classes represent intact or defective car components.
Highlights:
Advanced gradient boosting via XGBoost.
Hyperparameter tuning for optimal performance.
Evaluation using AUC and multi-class ROC curves.
📊 Dataset
Source: UCI Machine Learning Repository
Details:
Features: 48 numerical features derived from electric currents.
Classes: 11 labels representing different component states.
Size: 58,509 samples.
Format: Text file (sensorless_drive_diagnosis.txt), space-delimited.
🧠 Model Details
Algorithm: XGBoost, a high-performance gradient boosting framework.
Metrics:
Micro-Averaged AUC for overall performance.
ROC Curves for individual class evaluation.
Hyperparameter Tuning:
Number of trees: n_estimators.
Tree depth: max_depth.
Learning rate: learning_rate.
🛠 How to Run
1️⃣ Environment Setup
Install the required libraries:

bash
Copy code
pip install xgboost scikit-learn matplotlib pandas numpy
2️⃣ Dataset
Download the dataset:

Sensorless Drive Diagnosis Dataset
Save it as sensorless_drive_diagnosis.txt in your project folder.
3️⃣ Run the Code
Execute the script to:

Train the model.
Tune hyperparameters:
n_estimators (trees): [10, 50, 100, 500]
max_depth (tree depth): [4, 6, 8]
learning_rate: [0.001, 0.01, 0.1]
Evaluate the model on the test set.
4️⃣ Results
The final model retrains on the combined training + validation data and evaluates on the test data.

🏆 Results
Best Hyperparameters:
Number of Trees (n_estimators): 100
Tree Depth (max_depth): 6
Learning Rate (learning_rate): 0.1
