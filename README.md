# credit-risk-classification challenge

**_Background_**

In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

**_Instructions_**

The instructions for this Challenge are divided into the following subsections:

* Split the Data into Training and Testing Sets

* Create a Logistic Regression Model with the Original Data

* Write a Credit Risk Analysis Report

[Note]: I have used our knowledge of Python and supervised learning (activities of Days 1 and 2 in class) to finish this challenge.

# Credit Risk Analysis Report 
## Overview of the Analysis

Lending institutions offer loans or assets to borrowers with the understanding that the borrower will either return the asset or repay the loan. Credit risk occurs when a borrower is unable to return the asset or meet the loan repayment, leading to financial losses for the lender. Lenders evaluate this risk using a variety of methods. This study aims to utilize machine learning to analyze a dataset of previous lending transactions from a peer-to-peer lending platform to develop a model capable of assessing the creditworthiness of borrowers.
The machine learning model has been used to categorize loans based on the lending company's loan status as either low-risk (safe) or high-risk (risky).
After analyzing the lending company's historical lending activities, I developed a Logistic Regression Model with a 99% accuracy score. However, the model's recall value for high-risk loans is 0.89, lower than its recall value for healthy loans (1.00), indicating a discrepancy due to the dataset's imbalance.

## Results

### Machine Learning Model – Logistic Regression Model with the Original Data:

The figure below exhibits a high level of imbalance of the Dataset.

<img width="912" alt="Screenshot 2024-05-15 at 10 54 05 AM" src="https://github.com/hatkiet/credit-risk-classification/assets/154276115/9be5b75e-4890-451f-a845-5437644a2fc5">


Description of the Accuracy, Precision, and Recall of the Logistic Regression Model with the Original Data.
- Compared to the original dataset, the number of healthy loans is greater than that of unhealthy loans.
- The model has an impressive accuracy of 99%. The precision score for '0' (healthy loans) is 100%, and the precision for '1' (unhealthy loans) is also good at 87%.
- The recall score is high with 100% for predicting healthy loans with the label '0' and 89% for high-risk loans with the label '1'.

The Classification Report for the Logistic Model with the Original Data

<img width="476" alt="Screenshot 2024-05-15 at 10 53 47 AM" src="https://github.com/hatkiet/credit-risk-classification/assets/154276115/36f2973f-94df-4539-82ba-dcb7550fee7a">


## Summary

A lending company needs a model that accurately differentiates between healthy and high-risk loans to minimize potential costs. Misclassifying healthy loans as high-risk can lead to customer loss, while misclassifying high-risk loans as healthy can result in financial losses for the company.
However, the discrepancy due to the dataset's imbalance causes the model's recall value for high-risk loans to differ significantly from its recall value for healthy loans. This suggests that we should use a model that allows the machine to be capable of imbalanced learning to improve the outcome of accuracy, recall, and error in classifying high-risk loans. Because, the lending company prefers fewer false positives to minimize risks, where high-risk loans are mistakenly classified as healthy. 

The confusion matrix is:

<img width="173" alt="Screenshot 2024-05-15 at 10 54 41 AM" src="https://github.com/hatkiet/credit-risk-classification/assets/154276115/a5fb8063-7233-4a9c-a297-da651f751b66">

From the confusion matrix of the Logistic Regression Model with imbalanced data, there are:
- 67 false positives (actual value: healthy, predicted value: high-risk)
- 80 false negatives (actual value: high-risk, predicted value: healthy)
  
