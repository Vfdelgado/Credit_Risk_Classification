# Overview of the Analysis

The purpose of this analysis is to develop machine learning models that can effectively assess the creditworthiness of borrowers using historical lending activity data from a peer-to-peer lending services company.

The dataset contains various financial information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The prediction target is the "loan_status" column, where a value of 0 indicates a healthy loan and a value of 1 indicates a high-risk loan.

## Variables to Predict:

The target variable, "loan_status," has two classes: 0 for healthy loans and 1 for high-risk loans.

Count of each class in the target variable:

Healthy loans (0): 18765 instances

High-risk loans (1): 619 instances

## Stages of the Machine Learning Process:

### Data Preprocessing: 

Reading the dataset, separating features and labels, and splitting the data into training and testing sets.

Model Training: Fitting a logistic regression model using the training data.

Model Evaluation: Assessing the model's performance using metrics such as confusion matrix, classification report, precision, recall, and accuracy.

### Methods Used:

Logistic Regression: Utilized for building the predictive model due to its effectiveness in binary classification tasks.

# Results
![image](https://github.com/Vfdelgado/Credit_Risk_Classification/assets/146504714/a8bd1e45-f370-4820-b88e-160037354daa)


Machine Learning Model 1 (Logistic Regression):

Accuracy: 99%

Precision (Healthy Loan - 0): 100%

Recall (Healthy Loan - 0): 99%

Precision (High-Risk Loan - 1): 85%

Recall (High-Risk Loan - 1): 91%

Support Size (High-Risk Loan - 1): 619 instances

# Summary
The logistic regression model demonstrates high performance in predicting the credit risk associated with loans:

Healthy Loan (0):
The model exhibits excellent precision and recall scores, indicating its ability to accurately identify customers likely to repay their loans.

High-Risk Loan (1):
Although the model's precision and recall for high-risk loans are slightly lower, they still remain relatively high. However, there is room for improvement, particularly in precision, given the potential consequences of default.

Support Size:
The lower support size for high-risk loans highlights the importance of precision in lending decisions, especially for loans with a higher risk of default.
Based on the model's performance, it is recommended for use by the company, particularly for assessing the credit risk associated with loans. However, continuous monitoring and potential model refinement should be considered to further enhance its effectiveness, especially for high-risk loans.
