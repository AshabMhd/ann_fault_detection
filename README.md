# ann_fault_detection

This repository contains my solution to the Artificial Neural Network (ANN) Fault Detection Challenge hosted by ML league. The task was to develop an optimal ANN-based binary classification model to detect faults in a system using sensor data.

# Problem Statement
Given a labeled dataset of sensor readings, the goal is to train a neural network that accurately predicts whether a fault has occurred (Fault = 1) or not (Fault = 0). Evaluation is based on the F1-score on the test data and code neatness.

# Methodology
The following steps were followed:

## Data Preprocessing:
* Removed irrelevant rows
* Handled missing values using SimpleImputer
* Normalized features using StandardScaler
* Addressed class imbalance using class_weight

## Model Architecture:
* A simple yet effective Sequential ANN model using Keras
* Hidden layers with ReLU activation and dropout regularization
* Output layer with sigmoid activation for binary classification

## Training Strategy:
* Optimized using Adam optimizer
* Early stopping based on validation loss
* Binary crossentropy loss function

## Evaluation Metrics:
* Precision, Recall, F1-score
* Confusion Matrix
* ROC-AUC Score
