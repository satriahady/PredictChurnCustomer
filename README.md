# Predict Ecommerce Customer Churn using Supervised Learning

## Overview
The growth of customer is a key to more profitable company. As a result, many companies invest in campaign to acquire new customers to keep the company growth over time. But there is a problem. Acquire new customers could be a key for growth if the company could maintain their existing customer to keep loyal using their products. The Churn Customer--customer that stop using our products-- is a huge problem for company growth in the long run. Harvard Business Review says that acquiring a new customer is anywhere from five to 25 times more expensive than retaining an existing one. As a result, many companies trying to estimate the likelihood of customer churn and finding the necessary actions to minimize the churn rate.<br>


The aim of this project is to demonstrate predictive customer churn using supervised learning. The goals of this project is :
+ Minimize the Churn Rate
+ Maximize Potential Revenue

To accomplish the goals, we have some objectives:
+ Gain customer insight from our dataset
+ Determine factors that makes customer churn
+ Predict Customer who likely to churn
+ Create action plan to minimize churn and maximize potential revenue


## Dataset
We are using Ecommerce Dataset from [here](https://www.kaggle.com/ankitverma2010/ecommerce-customer-churn-analysis-and-prediction). The dataset contains features from every unique customer. These are the insight from the dataset: <br>
+ Our Target is `Churn` feature
+ Customer account information such as `CustomerID`,`Tenure`, `Preferred Login Device`, `Gender`, `CityTier`, `Number of Device Registered`, `Marital Status` and `Number of Address`
+ Customer transaction information such as `Warehouse to Home`,`Preferred Payment Mode`, `Hour Spend on App`, `Preferred Order Category`,`Satisfaction Score`, `Complain`, `Order Amount Hike From Last Year`,`Coupon Used`, `Order Count`, `Day Since Last Order`, and `Cashback Amount`

## Exploratory Data Analysis
This section consists some early insight of our data. We are checking the data distribution from each feature using univariate analysis. We found some data are skewed and some have outliers in the distribution. And then we gain feature correlation using correlation heatmap. And then we are grouping data into 2 categories: numerical and categories for data preprocessing

## Business Insight
This section is to determine the distribution data by our target from each feature. We have some insightful information from this.

## Data Preprocessing
### Handling Missing Value and Duplicate Data
We are checking the missing value from each feature. Based on the data and their distribution, we determine the strategy to impute each feature that have null values. And then we are checking if any data have duplication (which luckily we don't have in our dataset)

### Replacement Value
From Exploratory Data Analysis, we saw that there are some values that seems equal from our categorical feature. We replace the value that seems to be same so we have unique value from the feature

### Feature Engineering
For each of our categorical feature, we are using one hot encoding to transfrom each value into each feature.

### Data Transformation
We determine the data transformation strategy for our numerical feature based on their distribution data and we transform them for our modeling purpose. After that, we drop our outdated columns.
