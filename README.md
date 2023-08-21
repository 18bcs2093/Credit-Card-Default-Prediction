# Credit-Card-Default-Prediction

The Credit Card Default Prediction project aims to develop an accurate and reliable predictive model that assesses the likelihood of credit card holders defaulting on their payments. This predictive model utilizes historical credit card transaction data, customer information, and various financial indicators to classify customers as either "likely to default" or "unlikely to default." By identifying high-risk customers in advance, financial institutions can take proactive measures to minimize potential losses and manage credit risk effectively.

This project is aimed at predicting the case of customers default payments in Taiwan. From the perspective of risk management, the result of predictive accuracy of the estimated probability of default will be more valuable than the binary result of classification - credible or not credible clients. We can use the K-S chart to evaluate which customers will default on their credit card payments

## 1. Solution Strategy
   
My strategy to solve this challenge was:

Step 01: Know Your Data: Use info(),head(),tail(),find missing values and impute them,remove duplicates.

Step 02: Understand Your Variables: find uniqueness, their datatypes, any irregularity among them,describing variables etc.

Step 03: Data Wrangling & Data Visualization: Explore the data to find insights and better understand the impact of variables on model learning.

Step 04: Feature Engineering: Selection, manipulation, handling missing & outliers, data transformation on selected features and train-test split of the most significant attributes for training the model.

Step 05: Machine Learning Modelling: Machine Learning model training.

Step 06: Hyperparameter Fine Tunning: Choose the best values for each of the parameters of the model selected from the previous step.

## 2. Top Data Insights

Dataset dose not contains any NA values, null values and duplicates.

I tracked the past monthly payment records from April to September, 2005.The measurement scale for the repayment status is: -1 = pay duly; 1 = payment delay for one month; 2 = payment delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay for nine months and above.

Both classes are not in proportion that is we have imbalanced dataset.

## 3. Machine Learning Model Applied

At this stage, 5 models were used for analysis:Logistic Regression, Decision Tree Classifier, SVC, Gradient Boosting, XG Boosting

## 4. Machine Learning Model Performance
   
Performance of Optimal XG Boosting:
Test Accuracy: 0.871,	Precision: 0.833, Recall: 0.901,	F1 Score: 0.866	AUC: 0.873

## 6. Conclusions
   
After cross validation and hyperparameter tunning, XG Boost shows highest test accuracy score of 87.10% and AUC is 0.874.
