# House Price Prediction

## 1. Introduction

* Forecasted the probability of a consumer choosing our Stage 2 (infant) product with 87.7% accuracy.
* Collected approximately 2k records from the customer data platform and a series of consumer surveys.
* Conducted data cleansing, EDA (exploratory data analysis), and feature engineering.
* Implemented ML classification models (Logistic Regression and Random Forest), showcasing the most crucial features.
> Due to NDA (Non-Disclosure Agreement), the dataset has been modified.

<img width="921" alt="lr fea c2" src="https://user-images.githubusercontent.com/64850893/155887997-5a75e3d5-f43c-4752-b055-c1db284e5c3c.png">

## 2. Code and Packages

* Python Version: 3.9

* Packages: pandas, numpy, sklearn, matplotlib, seaborn

## 3. Objectives

* Consumer insight: Stage 2 users are 12% more likely to become Stage 3 users.​

* Business goal: Understand the variables that trigger our enrolled members to be Stage 2 formula users.

## 4. Data Sources

The samples are collected from the customer data plarform and a set of surveys, and the time period is from Q1 2020 to Q1 2021. 

## 5. Methodology

* Dependent variable: Current Stage 2 formula brand.

* Independent variables: 

     - Behavioral variables: previous product brand, enrollment type, enrollment age, email open rate, click through rate, coupon redemption rate.

     - Demographic variables: hospital zone, province, educational status, number of children.​

* Machine Learning Models: Logistic Regression and Random Forest.​

* Oversampling due to the imbalanced dataset.

* GridSearchCV to tune the hyperparameters.

