# Bank Customer Churn Prediction using Logistic Regression

## Project Overview

Customer churn is an important concern for banks because retaining existing customers is generally more beneficial than continuously acquiring new customers.

This project develops a Logistic Regression model to predict whether a bank customer is likely to churn based on demographic, financial, and banking-related features.

The project includes Exploratory Data Analysis (EDA), data preprocessing, model development, and evaluation using multiple classification metrics.

## Dataset

The Bank Customer Churn Dataset contains information about 10,000 bank customers.

### Features

- Credit Score
- Country
- Gender
- Age
- Tenure
- Balance
- Number of Products
- Credit Card
- Active Member
- Estimated Salary

### Target Variable

`churn`

- `0` – Customer stayed with the bank
- `1` – Customer churned

Dataset Source:

https://www.kaggle.com/datasets/gauravtopre/bank-customer-churn-dataset

## Exploratory Data Analysis

The EDA includes:

- Dataset structure and data types
- Missing value analysis
- Duplicate record analysis
- Churn distribution
- Numerical feature analysis
- Categorical feature analysis
- Churn rate by country
- Churn rate by gender
- Correlation analysis

### Key EDA Findings

- 79.63% of customers stayed with the bank.
- 20.37% of customers churned.
- Germany had the highest churn rate at 32.44%.
- Female customers had a higher churn rate than male customers.
- Age showed the strongest positive correlation with churn among the numerical features.
- Active membership showed a negative relationship with churn.

## Data Preprocessing

The following preprocessing steps were performed:

1. Removed `customer_id`.
2. Separated the features and target variable.
3. Applied one-hot encoding to categorical variables.
4. Split the dataset into 80% training and 20% testing data.
5. Applied feature scaling using StandardScaler.

## Model

### Logistic Regression

Logistic Regression was used to predict whether a customer would churn.

## Model Evaluation

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC-AUC

### Results

| Metric | Score |
|---|---:|
| Accuracy | 80.80% |
| Precision | 58.91% |
| Recall | 18.67% |
| F1-Score | 28.36% |
| ROC-AUC | 0.775 |

## Conclusion

The Logistic Regression model achieved an accuracy of 80.80% and a ROC-AUC score of 0.775.

The EDA identified age, balance, active membership, country, and gender as features showing noticeable relationships with customer churn.

Although the model achieved reasonable overall accuracy, its recall for the churn class was relatively low, indicating that many customers who actually churned were not identified by the model.

