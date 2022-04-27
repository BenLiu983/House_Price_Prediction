# House Price Prediction

* Model Performance

<img width="749" alt="model compa" src="https://user-images.githubusercontent.com/64850893/165354835-d50df04c-2df4-43ca-a618-5de7008ee29b.png">

* Feature Importance

<img width="1198" alt="fea imp" src="https://user-images.githubusercontent.com/64850893/165355037-ac919774-92dc-4f56-8822-a1a722da0fad.png">

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

* Machine Learning regression models: Lasso, Decision Tree, Random Forest, k-NN, SVM, Gradient Boosting.

* GridSearchCV to tune the hyperparameters.


## 5. EDA

### 5.1 Ouput Variables: Sale Price

<img width="500" alt="sale price" src="https://user-images.githubusercontent.com/64850893/165130005-42b0fe17-7667-4202-85ad-315385afc98d.png">

* The distribution is skewed to the right, we will conduct a log transformation as follows.

<img width="500" alt="sale price log" src="https://user-images.githubusercontent.com/64850893/165130459-aee16a12-6597-4304-b6a2-bbb3aac6b268.png">

### 5.2 Input Variables:

Year Between Built and Sold:

<img width="500" alt="year_built" src="https://user-images.githubusercontent.com/64850893/165131402-02be9bcd-9bae-4d30-8b3e-04966c6c6bac.png">

* The longer the time between the house was built and the sale date, the lower the sale price, which aligns with business logic.

Full Bathroom:

<img width="500" alt="full bath" src="https://user-images.githubusercontent.com/64850893/165351011-d2cf79cf-3e5f-44d3-942b-590587c9c96e.png">

* There is a positive relationship between the number of (full) bathrooms and the average sale price. 

Overall Condition:

<img width="500" alt="overall condition" src="https://user-images.githubusercontent.com/64850893/165350871-81df69cc-c95c-4503-bfc5-7a1fe76005dd.png">

* The higher the overall condition, the greater the sale price.


## 6 Feature Engineering

* Missing values (encode with "missing", or replace with mean(numeric)/ mode(categorical)).

* Numerical variables (temporal/time, discrete, continous). 

* Categorical variables (apply mappings, encoding).

* Refined version ("feature engineering with open source").

## 7. Modelling

### 7.1 Procedure

* Metric setting (R square)
* Feature selection (using Lasso)
* Train-test-split
* Cross validation
* Machine learning algorithms (Lasso, Decision Tree, Random Forest, k-NN, SVM, Gradient Boosting)
* GridSearchCV

### 7.2 Model Performance:

<img width="749" alt="model compa" src="https://user-images.githubusercontent.com/64850893/165354835-d50df04c-2df4-43ca-a618-5de7008ee29b.png">

* In terms of the model prediction accuracy, SVR, Lasso, and Random Forest outperform other algorithms.
* Considering the interpretability of the model, Lasso would be the optimal choice in this case.

### 7.3 Feature Importance (Lasso): 

<img width="1198" alt="fea imp" src="https://user-images.githubusercontent.com/64850893/165355037-ac919774-92dc-4f56-8822-a1a722da0fad.png">

* "GrLivArea" (above grade/ground living area square feet), "OverallQual" (rates the overall material and finish of the house), and "1stFlrSF" (first floor square feet) are the most crucial features when it comes to predicting the sale price of a house.

## 8. Conclusion

* Considering evaluation metric (R Square) and model interpretability, Lasso is the optimal model.
* Ground living area square feet, overall quality and first floor square feet are the most critical prediction indicators.

## 9. Next Steps

* Experiment other feature combination.
* Implement different models. 

