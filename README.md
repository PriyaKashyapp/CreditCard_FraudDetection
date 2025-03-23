# CreditCard_FraudDetection

This project focuses on detecting fraudulent credit card transactions using machine learning. The dataset contains anonymized credit card transactions, with features derived from PCA (Principal Component Analysis), transaction amounts, and timestamps. Given the highly imbalanced nature of the dataset, advanced techniques like SMOTE (Synthetic Minority Over-sampling Technique) and feature engineering are used to improve model performance.

## Overview

Fraud detection in credit card transactions is a critical challenge due to the rarity of fraudulent cases and the complexity of transaction data. This project demonstrates how to:

Handle class imbalance using SMOTE.
Engineer meaningful features (e.g., time-based transformations).
Train and evaluate machine learning models to detect fraud.
Visualize results using confusion matrices and classification reports.
 The goal is to build a robust model that achieves high recall and precision for detecting fraudulent transactions while minimizing false positives.

## Dataset

The dataset used in this project is the Credit Card Fraud Detection Dataset , which is publicly available on Kaggle . Key characteristics of the dataset include:

### Rows : 284,807 transactions

### Features :
28 anonymized features derived from PCA (V1, V2, ..., V28)
Time: Seconds elapsed between each transaction and the first transaction
Amount: Transaction amount
 
### Target Variable :
Class: Binary variable indicating whether a transaction is fraudulent (1) or legitimate (0)
Class Imbalance : Only ~0.17% of transactions are fraudulent.

## Methodology

The project follows these steps:

### Data Exploration :
Analyze the distribution of features and target variable.
Visualize class imbalance and feature correlations.

### Feature Engineering :
Normalize the Amount feature using StandardScaler.
Transform the Time feature into meaningful categories (Morning, Afternoon, Evening, Night) and binary indicators (Is_Night).
 
### Handling Class Imbalance :
Apply SMOTE to balance the training set by generating synthetic samples for the minority class.
 
### Model Training :
Train machine learning models such as Random Forest.
Perform hyperparameter tuning using Grid Search.

## Evaluation :
Evaluate models using metrics like Recall, Precision, F1-Score, and AUC-ROC.
Visualize results using confusion matrix heatmaps.


## Features

Key Features Implemented in the Project:

Feature Scaling : Normalization of the Amount feature.
Time-Based Features : Transformation of the Time feature into interpretable categories.
SMOTE : Synthetic Minority Over-sampling to address class imbalance.
Model Evaluation : Heatmaps, classification reports, and ROC curves for performance analysis.


