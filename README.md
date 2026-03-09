# Credit Card Fraud Detection using Logistic Regression

This project builds a simple **fraud detection model using Logistic Regression** to classify transactions as either legitimate (0) or fraudulent (1).

## Dataset

The dataset contains anonymized credit card transaction features and a target column `Class` where:

* `0` → Legitimate transaction
* `1` → Fraudulent transaction

The dataset is **highly imbalanced**, meaning the number of fraud cases is very small compared to normal transactions.

Dataset link:
https://www.kaggle.com/datasets/ranaghulamnabi/credit-card-fraud-detection-dataset

## Workflow

1. Loaded and explored the dataset.
2. Split the data using a normal train-test split.
3. Trained a Logistic Regression model and observed **very high accuracy (~0.995)** due to the model predicting mostly the majority class.
4. Identified that this happened because the dataset is **imbalanced**.
5. Fixed the issue by using **stratified splitting (`stratify=y`)** so that both training and test sets maintain the same class distribution.
6. Retrained the model and evaluated the results again.

## Technologies Used

* Python
* Pandas
* NumPy
* scikit-learn

## Model

Algorithm used: **Logistic Regression**
