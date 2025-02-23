# Peer to Peer Money Lending Platform

## Introduction

The Peer-to-Peer (P2P) Money Lending Platform connects private lenders with borrowers, bypassing traditional banks. The platform facilitates secure and transparent lending and borrowing by incorporating advanced loan risk assessment and predictive interest rate models.

## Database Design

MongoDB is used for efficient data storage with multiple collections to handle users, loan requests, loans, lender profiles, borrower profiles, payments, and default prediction data. Key collections include:
1. Users: Stores personal details of lenders and borrowers.
2. Loan Requests: Contains loan request details, including loan amount, term, and interest rate predictions.
3. Loans: Tracks loan details once approved by lenders.
4. Lender and Borrower Profiles: Stores extensive profiles of lenders and borrowers.
5. Payments: Tracks loan repayment progress.
6. Default Prediction Data: Contains pre-processed data used for default prediction model training.

## Application Description

This platform is a command-line application allowing direct transactions between lenders and borrowers. Features include:
1. User Registration: Users can sign up as either lenders or borrowers.
2. Loan Management: Borrowers can request loans, while lenders can invest in loan requests.
3. Interest Rate and Default Prediction: Machine learning models predict interest rates and loan defaults.

## Data Collection and Preprocessing

The datasets used for the application were sourced from Kaggle. Preprocessing involved:
1. Handling missing values and normalizing data.
2. Encoding categorical data and splitting datasets for model training.

## Exploratory Data Analysis (EDA)
EDA was conducted using the Pandas library to uncover trends and correlations, such as the relationship between loan amounts, income, and payment statuses. Insights from EDA help improve loan approval and risk assessment features.

## Machine Learning Models

Two machine learning models are implemented:
1. Interest Rate Prediction: A Random Forest Regressor model predicts interest rates based on borrower characteristics.
2. Default Prediction: A Logistic Regression model predicts loan defaults, considering features such as credit score, income, and loan amount.

## Datasets

The datasets are taken from below:
1. https://www.kaggle.com/datasets/adarshsng/lending-club-loan-datacsv?resource=download - Datasets for the p2p_lending database collections except
users collection.
2. Random user.me web api – For syntesizing data for users collection.
3. https://www.kaggle.com/datasets/nikhil1e9/loan-default?resource=download - Datasets
for training the default on model
The datasets are preprocessed and only the necessary features are opted to store in the collection.


