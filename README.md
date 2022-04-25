# House Price Prediction

## 1.
Introduction

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

### 6.1 Ouput Variables (MJN - 1, others - 0):

<img width="989" alt="stage 2 brand 4" src="https://user-images.githubusercontent.com/64850893/155889230-1b53cca2-0e6b-477d-b9ff-a6c5efaf9112.png">

* Will oversample in the next session because of the imbalanced dataset.

### 6.2 Input Variables:

The below visualizations will follow a segment analysis 

Previous Brand (behavioral):

<img width="1115" alt="pre brand 3" src="https://user-images.githubusercontent.com/64850893/155889095-575b5a70-d3e2-4390-b735-14274bf40868.png">


* In terms of 


## 7. Modelling

### 7.1 Procedure

* Train-test-split
* Cross validation
* Oversampling
* Machine learning algorithms (Logistic Regression and Random Forest)
* GridSearchCV

### 8.2 Model Performance:

<img width="1011" alt="model_sum" src="https://user-images.githubusercontent.com/64850893/155891672-6e74397d-6133-4c9e-966d-d56be9b4a38c.png">

* Considering the prediction accuracy as well as the model simplicity, Logistic Regression in Case 2 would be the optimal model, since it is more straightforward to interpret, with relevantly high prediction accuracy.

### 8.3 Confusion Matrix (Logistic Regression): 

<img width="470" alt="cm_git" src="https://user-images.githubusercontent.com/64850893/155891735-bcfcc378-3bc3-4f0b-9d32-8691ab1ed777.png">

### 8.4 Feature Importance (Logistic Regression): 

<img width="921" alt="lr fea c2" src="https://user-images.githubusercontent.com/64850893/155887997-5a75e3d5-f43c-4752-b055-c1db284e5c3c.png">

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


