# Module 20 - Report 

## Overview of the Analysis

**Purpose of the analysis**

 The purpose of this analysis is to assess whether the Logistic Regression machine learning model can more accurately predict healthy loans versus high-risk loans, using either the original dataset or a resampled dataset designed to increase the size of the minority class.

* **The Dataset** -The dataset used for this analysis contains information on 77,536 loans. The data includes columns for loan_size, interest_rate, borrower_income, debt_to_income ratio, number_of_accounts, derogatory_marks, total_debt, and loans_status. The category that we are attemting to predict with our analysis is **loan_status**. The data provided in the remaining columns will be used as features to train the data and inform the predictions.

* **Stages of the Machine Learning Process**  -The stages of the machine learning process are very scripted. If followed in order, they provide you with an accurate assessment of model's ability to make predictions. The stages of the machine learning process are as follows:

  - Prepare the Data: Import the file, establish the DataFrame, evaluate the columns and features.

  - Separate the Data into feature and labels: The labels represent the target variable
you're trying tp predict-whether the loan status is healthy(0) or high-risk(1). The feautures include all other data that will be used to train and test the model.

  - Split the Data: Use the train_test_split fuction to separate the feautures and labels data into training and testing datasets.

  - Import the Model: Import the machine learning model from the appropriate library, we will be importing logisticRegression model from scikit-learn (SKLearn).

  - Instantiate the model.

  - Fit the model using the training data.

  - Use the model to make predictions using the features test data.

  - Evaluate the predictions: Evaluation is performed by calculating and comparing metrics such as accuracy score, confusion matrix, and classification report.

* **Machine Learning Methods Utillized**  

  The primary model used in this analysis is:

    - LogisticRegression model from SKLearn

  Supporting functions used in this analysis are:

    - train_test_split from SKLearn

  Models are evaluated using the following functions:

  - confusion_matrix from SKLearn
  - classification_report from SKLearn

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model-Logistic Regression:
 * **Accuracy Score:** 99%
 * **Precision Scores:**
   * Class 0 (Healthy Loans): 100%
   * Class 1 (High-risk Loans): 84%
 * **Recall Scores:**
   * Class 0 (Healthy Loans): 99%
   * Class 1 (High-risk Loans): 94%

## Summary

The model does a great job in using the original data to predicting the values of the healty loans. Precision was 100% and recall was 99%.

The model is pretty good at prediction the values of high risk loans, but not as good as predicting the healty loans. Prediction was 84% and recall was 94%.

Given this information, it appears that the logic Regression model does a great job at predicting both healthy and high-risk loans, given the feautures that are used to train the data.



