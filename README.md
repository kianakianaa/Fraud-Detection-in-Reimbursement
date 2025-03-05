# Fraud-detection-in-reimbursement

## Problem Description
This project focuses on detecting fraudulent reimbursement claims from SAP. The dataset contains approximately 76 features, including but not limited to Transaction Date, Department Code, Vendor, City of Purchase, and Expense Amount. The key challenge is the absence of labeled data (i.e., whether a claim is fraudulent or not), necessitating the use of unsupervised machine learning techniques. 

## Approach
Due to the lack of labels, the goal is to leverage advanced unsupervised machine learning techniques to detect potential fraud by identifying hidden patterns in the data. We use an Autoencoder for feature extraction and apply Isolation Forest and Local Outlier Factor (LOF) for anomaly detection. Additionally, we explore other methods, including further enhancements with Isolation Forest, to improve detection performance.

To complement this, we also reformulated the problem as a supervised learning task, using expense amount as the target variable. Given the significant variation in expenses across departments and business purposes (e.g., staff welfare, travel, equipment purchases), simple statistical distribution-based methods were insufficient. Instead, we implemented XGBoost regression to model these variations effectively. In this context, we define that if the predicted expense amount is much smaller than actual amount, then there is higher probability of fraud.

![Methodology](https://github.com/user-attachments/assets/a3edc291-70bc-4f0f-9ac0-7d6379e2e5d8)


## Data Privacy
To ensure compliance with data privacy regulations, the source dataset cannot be shared. However, the methodology and logic used in this project are fully documented and can provide valuable insights for similar applications.

## Document Structure
autoencoder_oop.ipynb:
- A trial notebook for the first round of experiments, to get the rough and foundamental understanding of the methods.
- Explores the use of an Autoencoder to generate meaningful features for fraud detection.
- Includes a comparison of approaches, such as using Isolation Forest as a pre-filter before chaining it with the Autoencoder for improved detection.

Script for the first-round trial:
- Will be uploaded soon. This script will provide a streamlined implementation of data processing and the methods discussed in the initial experiments.

 ## Future Work
 - Tuning hyperparameters for the Autoencoder and Isolation Forest for better performance.
 - Utilizing NLP for feature engineering.
 - Improve the anomaly metrics.

