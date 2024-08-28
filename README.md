# E-commerce-Fraud-Detection

#### Project Overview
This project aims to develop a machine learning model capable of accurately detecting fraudulent transactions in an e-commerce environment. By identifying fraudulent activities, businesses can protect themselves from financial losses and maintain customer trust.

The dataset used for this project consists of 1472952 transactions, with 16 features including transaction amount, transaction date, payment method, product category, customer information, and other relevant variables.

#### Link for the dataset: 
https://www.kaggle.com/datasets/shriyashjagtap/fraudulent-e-commerce-transactions

#### Methodology

1. Data Preprocessing:
Handled missing values.
Converted categorical features to numerical representations using one-hot encoding.
Standardized numerical features to ensure consistency.

2.Feature Engineering:
Created time-based features.
Engineered interaction terms between features .
Calculated customer-centric metrics .

3. Model Selection and Training:

Experimented with various machine learning algorithms, including Random Forest, Gradient Boosting, etc.
Optimized model hyperparameters using grid search or random search.
### Addressed class imbalance using SMOTE oversampling.

4. Model Evaluation:

Evaluated models using metrics such as accuracy, precision, recall, F1-score.
Conducted cross-validation to ensure robustness.

5.Final Model: Random Forest

#### Performance:
Accuracy: 0.97
F1-score: 0.96
The Random Forest model demonstrated strong performance in identifying both non-fraudulent and fraudulent transactions.

### Class Imbalance Handling

To address the class imbalance, SMOTE (Synthetic Minority Over-sampling Technique) was applied with the following parameters:
sampling_strategy='minority'
k_neighbors=15
This significantly improved the model's ability to detect fraudulent transactions.

## Future Work:
Future Work
Potential areas for future improvement include:

Exploring additional feature engineering techniques.
Experimenting with different ensemble methods.
Incorporating real-time fraud detection capabilities.
Investigating anomaly detection techniques for detecting unusual patterns.

#### Dependencies
Python
pandas
NumPy
scikit-learn
matplotlib
seaborn
imblearn (for SMOTE)

#### Usage
Install the required libraries.
Load the dataset.
Preprocess the data as described in the methodology.
Train the model using the provided code.
Make predictions on new data.
