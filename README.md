<h1 align="center"> Credit-Risk-Classification </h1> <br>
Utilize machine learning models to develop a logistic regression model to make predictions based on historical data.


## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Build Process](#build-process)
- [Credit Risk Analysis Report](#credit-risk-analysis-report)
- [References](#references)


## Introduction

In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.


## Getting Started

Prior to execution, you must have Python installed. You must also have the necessary starter codes downloaded.


## Build Process

The instructions for this Challenge are divided into the following subsections:

    - Split the Data into Training and Testing Sets

    - Create a Logistic Regression Model with the Original Data
    
### Split the Data into Training and Testing Sets
Open the starter code notebook and use it to complete the following steps:

    1) Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.

    2) Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.

NOTE: A value of 0 in the “loan_status” column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

    3) Split the data into training and testing datasets by using train_test_split.
    
### Create a Logistic Regression Model with the Original Data
Use your knowledge of logistic regression to complete the following steps:

    1) Fit a logistic regression model by using the training data (X_train and y_train).

    2) Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.

    3) Evaluate the model’s performance by doing the following:

    - Generate a confusion matrix.

    - Print the classification report.

    4) Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?
    
    The logistic regression model does a great job of predicting both healthy and high-risk loans. For healthy loans, it almost always gets it right, with a precision of 100% and a recall of 99%. This means when the model says a loan is healthy, it's almost never wrong, and it catches nearly all healthy loans.

    For high-risk loans, the model's performance is slightly lower but still good, with a precision of 85% and a recall of 91%. This means it correctly identifies 85% of the high-risk loans it predicts and finds 91% of all actual high-risk loans.

    Overall, the model's accuracy is 99%, showing that it's very reliable in predicting loan status. While it excels at identifying healthy loans, it's also fairly good at catching high-risk ones, making it a strong tool for loan prediction.
    
    
## Credit Risk Analysis Report

### Overview of the Analysis:
The purpose of this analysis is to evaluate the performance of a logistic regression model in predicting loan statuses. Specifically, the model aims to classify loans as either healthy (0) or high-risk (1). By analyzing key performance metrics such as accuracy, precision, and recall, we can determine the model's reliability and effectiveness in identifying both healthy and high-risk loans.

### Results:
    - Accuracy Score: 99%
    - Precision Score:
        - Healthy Loans (0): 1.00
        - High-Risk Loans (1): 0.85
    - Recall Score:
        - Healthy Loans (0): 0.99
        - High-Risk Loans (1): 0.91
        
### Summary:
The logistic regression model demonstrates excellent performance in predicting loan statuses. It achieves a high accuracy score of 99%, indicating that it correctly classifies the vast majority of loans. The model is particularly effective at identifying healthy loans, with a perfect precision score of 1.00 and a recall score of 0.99. This means it almost never misclassifies a healthy loan and catches nearly all actual healthy loans.

For high-risk loans, the model's precision is 0.85, meaning 85% of the loans it predicts as high-risk are indeed high-risk. Its recall score for high-risk loans is 0.91, indicating it successfully identifies 91% of actual high-risk loans.

Recommendation: Based on these results, I recommend using this logistic regression model. Its high accuracy and strong performance in identifying both healthy and high-risk loans make it a reliable tool for loan prediction. The model's ability to accurately classify loan statuses can help the company in managing its loan portfolio more effectively and minimizing risk.

## References

Code was shown by the instructor on 07.18.2024

[Xpert Learning Assistant](https://bootcampspot.instructure.com/courses/5057/external_tools/313)

Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.
