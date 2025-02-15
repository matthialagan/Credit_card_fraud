# Credit Card Fraud Detection Model

This repository contains the code and resources for building a **Credit Card Fraud Detection** machine learning model. The model is trained on a **Credit Card Fraud Detection dataset** available on Kaggle. The goal of this model is to predict whether a credit card transaction is fraudulent or legitimate.

## Dataset

The dataset used in this project is the **Credit Card Fraud Detection dataset** from Kaggle. You can download it from [this link](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

### Dataset Description:

- **Features**:
  The dataset contains 31 features:
  - **V1 to V28**: 28 anonymized features generated from PCA transformation of the original features.
  - **Time**: The number of seconds elapsed since the first transaction in the dataset.
  - **Amount**: The transaction amount.
  - **Class**: The target variable indicating whether the transaction is fraudulent (`1`) or legitimate (`0`).


 ## Steps for Building the Model

### 1. Data Preprocessing

- **Handling Missing Values**: We check for missing data and handle it accordingly.
- **Class Imbalance**: Due to the imbalanced nature of the dataset, techniques such as **SMOTE (Synthetic Minority Over-sampling Technique)** or **class weights** in the model can be used to address the imbalance.

### 2. Model Selection

We explore various classification algorithms, including:

- **Logistic Regression**
- **Desicsion Tree Classifier**

The model performance is evaluated using metrics such as:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**

### 3. Model Evaluation

The model is evaluated on:

- **Training data**: To check how well the model fits the data.
- **Test data**: To validate the model's generalization capability.

## How to Use

### 1. Train the Model:
   - Open the `credit_card_fraud.ipynb` notebook.
   - Run the steps sequentially to train the model. This includes data preprocessing, model selection, and training the chosen classifier.

### 2. Make Predictions:
   After training the model, you can use it to predict whether a new transaction is fraudulent or legitimate.

### 3. Evaluate the Model:
Evaluate the performance of the model using the classification_report() and confusion_matrix() functions from sklearn.

## Notes

 - Imbalanced Dataset: Due to the imbalanced nature of the dataset, traditional accuracy metrics may not be sufficient. It is important to focus on precision, recall, and F1-score.
 - Model Deployment: You can save the trained model using joblib or pickle and deploy it for real-time prediction in production.
   



