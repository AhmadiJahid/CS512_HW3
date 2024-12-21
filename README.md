🚗 Sensorless Drive Diagnosis with XGBoost 🚗
Classify car conditions based on electric drive currents using machine learning!
This project leverages the Sensorless Drive Diagnosis Dataset from the UCI Machine Learning Repository and the powerful XGBoost algorithm to achieve near-perfect classification accuracy.

📋 Overview
Predict the condition of car components using 48 numerical features extracted from electric drive currents.

Highlights:
11 distinct classes representing intact and defective car components.
Advanced gradient boosting with XGBoost.
Hyperparameter tuning for optimal performance.
Evaluation using AUC and multi-class ROC curves.
📊 Dataset Details
Source: UCI Machine Learning Repository
Features: 48 numerical features derived from electric currents.
Classes: 11 labels representing different component states.
Size: 58,509 samples.
Format: Space-delimited text file (sensorless_drive_diagnosis.txt).
🧠 Model Details
Algorithm: XGBoost, a high-performance gradient boosting framework.
Metrics:
Micro-averaged AUC for overall performance.
ROC Curves for individual class evaluation.
Hyperparameter Tuning:
Number of Trees: n_estimators ([10, 50, 100, 500]).
Tree Depth: max_depth ([4, 6, 8]).
Learning Rate: learning_rate ([0.001, 0.01, 0.1]).
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
Train the model and tune hyperparameters:
n_estimators (Number of Trees).
max_depth (Tree Depth).
learning_rate (Learning Rate).
Retrain the model with the best hyperparameters.
Evaluate on the test set.
🏆 Results
Best Hyperparameters:
Parameter	Value
Number of Trees	100
Tree Depth	6
Learning Rate	0.01
Performance:
Test AUC: 0.99999 🎯
ROC Curve:

📂 Project Structure
plaintext
Copy code
📁 sensorless-drive-diagnosis/
├── sensorless_drive_diagnosis.txt   # Dataset
├── train_model.py                   # Training and evaluation script
├── roc_curve.png                    # Generated ROC Curve
└── README.md                        # Project documentation
📚 Dependencies
Library	Version
Python	>= 3.8
XGBoost	>= 1.5.0
scikit-learn	>= 1.0
pandas	>= 1.3
numpy	>= 1.21
matplotlib	>= 3.4
Install them all with:

bash
Copy code
pip install -r requirements.txt
🙏 Acknowledgements
Dataset provided by the UCI Machine Learning Repository.
Model implementation powered by XGBoost.
