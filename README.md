# Fraud-detection-in-reimbursement

## Problem Sescription
This project focuses on detecting fraudulent reimbursement claims from SAP. The key challenge is the absence of labeled data (i.e., whether a claim is fraudulent or not), necessitating the use of unsupervised machine learning techniques. The dataset contains approximately 76 features, including but not limited to Transaction Date, Department Code, Vendor, City of Purchase, and Expense Amount.

## Approach
The primary objective is to leverage advanced unsupervised machine learning methods to identify potential fraud. The initial approach involves using an Autoencoder for feature creation and using Isolation Forest/Local Outlier Factor for anomaly detection, followed by an exploration of methods such as Isolation Forest to enhance detection performance.

## Data Privacy
To ensure compliance with data privacy regulations, the source dataset cannot be shared. However, the methodology and logic used in this project are fully documented and can provide valuable insights for similar applications.

## Document Structure
autoencoder_oop.ipynb:
- A trial notebook for the first round of experiments, to get the rough and foundamental understanding of the methods.
- Explores the use of an Autoencoder to generate meaningful features for fraud detection.
- Includes a comparison of approaches, such as using Isolation Forest as a pre-filter before chaining it with the Autoencoder for improved detection.

Script for the first-round trial:
- Will be uploaded soon. This script will provide a streamlined implementation of the methods discussed in the initial experiments.

 ## Future Work
 - Tuning hyperparameters for the Autoencoder and Isolation Forest for better performance.
 - Utilizing NLP for feature engineering.
 - Improve the anomaly metrics.

