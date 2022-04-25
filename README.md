# House Price Prediction

* result table and important features

## 1. Introduction

* Forecasted the price of listing houses with 84.6% R Square score based on dataset with 1461 rows and 81 columns.
* Conducted data cleansing, EDA (exploratory data analysis), and feature engineering.
* Implemented ML regression models (Lasso, Decision Tree, Random Forest, k-NN, SVM), showcasing the most crucial features.

## 2. Code and Packages

* Python Version: 3.9

* Packages: pandas, numpy, sklearn, matplotlib, seaborn

## 3. Data

The dataset is from Kaggle: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data

## 4. Methodology

* Dependent variable: SalePrice

* Independent variables: # of bedrooms/bathrooms/kitchen, # of basement bedrooms/bathrooms/kitchen, first floor square feet, type of dwelling involved in the sale, zoning classification of the sale, linear feet of street connected to property, lot size in square feet, etc (refer to the "data_description.txt").

* Machine Learning Regression Models: Lasso, Decision Tree, Random Forest, k-NN, SVM, Gradient Boosting.

* GridSearchCV to tune the hyperparameters.

## 5. Data Cleaning

* Numerical Variables (temporal/time, discrete, continous) 

* Categorical Variables.

* Missing Values: (encode with "missing", or replace with mean(numeric)/ mode(categorical))

## 6. EDA

### 6.1 Ouput Variables: Sale Price

<img width="500" alt="sale price" src="https://user-images.githubusercontent.com/64850893/165130005-42b0fe17-7667-4202-85ad-315385afc98d.png">

* The distribution is skewed to the right, we will conduct a log transformation as follows.

<img width="500" alt="sale price log" src="https://user-images.githubusercontent.com/64850893/165130459-aee16a12-6597-4304-b6a2-bbb3aac6b268.png">

### 6.2 Input Variables:

Year Between Built and Sold:

<img width="500" alt="year_built" src="https://user-images.githubusercontent.com/64850893/165131402-02be9bcd-9bae-4d30-8b3e-04966c6c6bac.png">

* The longer the time between the house was built and the sale date, the lower the sale price, which aligns with business logic.

## 7. Modelling

### 7.1 Procedure

* Train-test-split
* Cross validation
* Oversampling
* Machine learning algorithms (Logistic Regression and Random Forest)
* GridSearchCV

### 8.2 Model Performance:


* Considering the prediction accuracy as well as the model simplicity, Logistic Regression in Case 2 would be the optimal model, since it is more straightforward to interpret, with relevantly high prediction accuracy.

### 8.3 Confusion Matrix (Logistic Regression): 



### 8.4 Feature Importance (Logistic Regression): 

* Positive features – previous brand as MJN, negative features – previous brand as other brands.
* If the previous brand is "Abbott Specialty", it plays a positive impact on current MJN Stage 2 brand choice.
* Number of children is negatively influencing the MJN Stage 2 brand selection .

## 9. Conclusion

* Drive MFB members to become Stage 1 users, due to the fact that the previous brand is a primary indicator.
* Maintain/boost the quantity/quality of email campaigns, since the email performance is an essential driver.
* Conduct experimentation to market users with only 1 child, because this metric negatively impact the outcome.

## 10. Next Steps
 
* Modify the output and input variables to tailor other business use cases.
* More experimentation in terms of variables and models.


