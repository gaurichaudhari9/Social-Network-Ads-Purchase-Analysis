# Social Network Ads Targeted Advertising Project

This is a machine learning project aimed at predicting whether a targeted audience is likely to positively respond to ads on social networks. The project uses a dataset containing information about individuals' age, estimated salary, and whether they purchased a product after seeing an ad on a social network.

## Table of Contents

- [Introduction](#introduction)
- [Problem Definition](#problem-definition)
- [Data](#data)
- [Evaluation](#evaluation)
- [Features](#features)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Modeling](#modeling)
- [Model Evaluation](#model-evaluation)
- [Conclusion](#conclusion)
- [Future Improvements](#future-improvements)

## Introduction

In the age of digital marketing, understanding the demographics and preferences of your target audience is crucial for the success of advertising campaigns. This project leverages machine learning techniques to predict whether an individual will purchase a product after viewing an ad on a social network. By identifying patterns and relationships in the data, we can optimize ad targeting to increase the conversion rate and improve ROI.

## Problem Definition

The main goal of this project is to build a predictive model that can determine whether a person is likely to purchase a product based on their age and estimated salary. This predictive capability will help businesses tailor their advertising strategies to reach individuals who are more likely to respond positively to their ads.

## Data

The dataset used in this project can be found [here](https://www.kaggle.com/d4rklucif3r/social-network-ads). It consists of 400 records, each containing the following features:

1. **Age**: The age of the individual.
2. **EstimatedSalary**: The estimated annual salary of the individual.
   
And one target label:

3. **Purchased**: Whether the individual purchased the product or not (0 for not purchased, 1 for purchased).

## Evaluation

To evaluate the performance of the predictive model, we use various classification metrics, including:

- Accuracy
- Precision
- Recall
- F1-score
- Support

These metrics will provide insights into how well the model can classify individuals as potential purchasers based on their age and estimated salary.

## Features

**Input Features:**

1. Age - Age of the person.
2. EstimatedSalary - Estimated salary of the person.

**Output/Label:**

3. PurchasedItem - Indicates whether the person purchased the product or not (0 or 1).

## Exploratory Data Analysis

Before diving into modeling, we performed exploratory data analysis (EDA) to gain insights into the dataset. Here are some key observations from our EDA:

- No missing values in the dataset.
- The majority of customers did not make a purchase (imbalance in the data).
- Age distribution is slightly right-skewed with two peaks.
- Estimated salary distribution is also slightly right-skewed, with potential outliers at the high end.

We also observed that age and estimated salary are important factors influencing an individual's purchase decision.

## Modeling

In the modeling phase, we experimented with several machine learning models, including:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Classifier (SVC)
- Decision Tree Classifier
- Random Forest Classifier
- AdaBoost Classifier
- Gradient Boosting Classifier
- XGBoost Classifier
- XGBoost Random Forest Classifier

We used a baseline model as a reference point to compare and evaluate the performance of these advanced models. The KNeighborsClassifier model performed the best with an accuracy of 94%, outperforming the baseline models.

## Model Evaluation

We conducted hyperparameter tuning using Random Search CV to optimize the selected models. The hyperparameter tuning process led to further improvements in model accuracy. For example:

- KNeighborsClassifier achieved an accuracy of 94%.
- XGBoost Classifier achieved an accuracy of 91%.
- XGBoost Random Forest Classifier achieved an accuracy of 91%.
- SVC achieved an accuracy of 93%.

## Conclusion

This project demonstrates the power of machine learning in predicting the likelihood of a social network user making a purchase after seeing an ad. By leveraging age and estimated salary data, businesses can make data-driven decisions to target their ads more effectively, ultimately leading to better conversion rates and higher ROI.

## Future Improvements

While the current models perform well, there are always opportunities for further improvement:

1. **Feature Engineering**: Explore additional features or interactions between features that might improve predictive performance.

2. **Data Collection**: Collect more diverse and comprehensive data to enhance the model's accuracy.

3. **Imbalanced Data Handling**: Implement techniques like oversampling or undersampling to address the class imbalance issue in the dataset.

4. **Ensemble Methods**: Experiment with ensemble methods to combine the strengths of multiple models for better predictive performance.

5. **Deployment**: Deploy the model as a web service or integrate it into a marketing automation platform for real-time ad targeting.

6. **Continuous Monitoring**: Continuously monitor and update the model to adapt to changing user behavior and preferences.

7. **A/B Testing**: Implement A/B testing to validate the model's effectiveness in real-world advertising campaigns.

By considering these future improvements, this project can continue to deliver value and insights to businesses seeking to optimize their social network advertising efforts.
