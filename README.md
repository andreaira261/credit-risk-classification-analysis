# Credit Risk Classification Analysis

## Overview 

## Languages/ Tools: 
  - Python
  - Pandas
  - scikit-learn

## Split the Data into Training and Testing Sets 
The data was loaded into a DataFrame and the "loan_status" column was set as the target variable (`y`). The remaining columns were set as the features (`X`)

The data was split into training and testing datasets by using `train_test_split`.

## Create a Logistic Regression Model
A logistic regression model was initialized and fitted by using the training data.

The predictions on the testing data labels were saved by using the testing feature data and the fitted model. 

The model's perfomance was then evaluated by calculating the accuracy score and generating a confusion matrix and classification report. 

## Credit Risk Analysis Report 
The analysis report can be found on the following file: [report.md](report.md).

