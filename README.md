## Module challenge 20: credit-risk-classification
 
# Description: 

The instructions for this challenge are divided into three key subsections:

1. Split the Data into Training and Testing Sets

  - Load the lending_data.csv into a Pandas DataFrame.

  - Separate the “loan_status” column as the target labels (y), with 0 representing healthy loans and 1 representing high-risk loans.

  - Create the features (X) from the remaining columns and split the data into training and testing sets using train_test_split.

2. Create a Logistic Regression Model with the Original Data

  - Fit a logistic regression model using the training data (X_train and y_train).

  - Use the fitted model to make predictions on the testing data (X_test).

  - Evaluate the model's performance by generating a confusion matrix and printing the classification report. Analyze how well the model predicts both healthy loans (0) and high-risk loans (1).

3. Write a Credit Risk Analysis Report

  - Write a brief report in the README.md file of your GitHub repository, summarizing the analysis.

  - Include the following in the report:

	  - Overview of the Analysis: Explain the purpose     of the analysis.

	  - Results: List key metrics, such as accuracy score, precision score, and recall score.

	  - Summary: Provide a summary of the results and justify whether the model is recommended for use or not, with reasons for your decision.