# Customer Churn Prediction using Machine Learning

## Overview

This project predicts whether a telecom customer is likely to churn (leave the service) using machine learning models.

Customer churn prediction helps companies identify at-risk customers early and improve retention strategies.

## Dataset

Dataset used: Telco Customer Churn Dataset from Kaggle

Kaggle Link: https://www.kaggle.com/datasets/blastchar/telco-customer-churn

Dataset contains:

* 7043 customer records
* 20+ features
* Target variable: Churn (Yes/No)

Features include:

* Customer demographics
* Subscription details
* Contract type
* Payment method
* Monthly charges
* Total charges
* Tenure

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Imbalanced-learn (SMOTE)
* Pickle

---

## Workflow

### 1. Data Preprocessing

* Removed unnecessary customerID column
* Handled missing values in TotalCharges
* Converted categorical columns using Label Encoding

### 2. Exploratory Data Analysis

Performed:

* Histogram plots
* Boxplots
* Scatter plots
* Correlation heatmaps

Key insights:

* Month-to-month customers showed higher churn
* Short tenure correlated with churn
* Higher monthly charges increased churn probability

### 3. Handling Class Imbalance

Applied SMOTE (Synthetic Minority Oversampling Technique) to balance churn classes.

### 4. Model Training

Models trained:

* Decision Tree Classifier
* Random Forest Classifier

Used:

* 80-20 train-test split
* 5-fold cross-validation

### 5. Model Evaluation

Metrics used:

* Accuracy
* Confusion Matrix
* Classification Report
* ROC-AUC Score

Final model achieved approximately:

* Accuracy: ~85%
* ROC-AUC: Strong classification performance

### 6. Model Persistence

Saved:

* Trained model (.pkl)
* Label encoders (.pkl)

This enables future inference on new customer data.

---

## Future Improvements

* Hyperparameter tuning
* XGBoost / LightGBM
* Streamlit web deployment
* Feature importance dashboard

## Author

Yash Jagwan
