# Module 12 Report Template

## Overview of the Analysis

A lending company needs a creditworthiness model to assess borrower risk and reduce defaults, safeguarding lenders' capital. The model helps assign accurate risk-based interest rates and ensures only reliable borrowers are approved, building trust and a strong reputation. The automation enables scalable, cost-efficient processing of loan applications. It supports regulatory compliance by adhering to risk assessment standards. Data insights from the model refine loan offerings and improve borrower-lender matching. By minimizing losses and offering competitive rates, the platform gains a market edge. Ultimately, the model balances risk management, operational efficiency, and profitability, ensuring sustainable growth.

The data includes financial details such as loan size, interest rate, borrower income, debt-to-income ratio, and credit history. The goal is to predict the loan status (good standing or default) based on these attributes.

The target variable,  **loan_status** , has the following distribution:

* **0** (presumably indicating loans in good standing): 75,036 instances
* **1** (indicating loans potentially in default): 2,500 instances

This shows an imbalance, with the majority of loans being in good standing. 

We outlined several stages in the machine learning process for credit risk classification:

1. **Data Preparation** : The dataset is preprocessed, and features are selected for the model. This involves creating separate feature (`X`) and target (`y`) datasets.
2. **Data Splitting** : The data is split into training and testing sets using `train_test_split`.
3. **Model Creation and Training** : A logistic regression model is created and trained using the training data (`X_train` and `y_train`).
4. **Model Evaluation** : The model's performance is assessed using a confusion matrix and classification report, which include metrics like precision, recall, and F1-score for predicting "Healthy Loan" and "High-Risk Loan" classifications.

primarily used the **Logistic Regression** algorithm for credit risk classification. Logistic regression is well-suited for binary classification tasks like predicting loan status (healthy vs. high-risk) based on borrower attributes. This model was chosen for its interpretability and efficiency, providing a clear probabilistic output for each class. Model performance was evaluated using metrics such as precision, recall, and F1-score to understand its effectiveness in predicting both classes accurately.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* **Machine Learning Model 1** : Logistic Regression
  * **Accuracy** : 99%
  * **Precision** :
    * Healthy Loan: 1.00
    * High-Risk Loan: 0.84
  * **Recall** :
    * Healthy Loan: 0.99
    * High-Risk Loan: 0.94

This indicates that the model performs very well, especially in predicting healthy loans with high precision and recall, and also shows strong results for high-risk loans, despite the class imbalance. 

## Summary

The logistic regression model showed exceptional performance with an overall accuracy of 99%, proving its effectiveness in classifying loans as either healthy or high-risk. It achieved a perfect precision score of 1.00 for healthy loans and a strong precision of 0.84 for high-risk loans, alongside recall scores of 0.99 and 0.94 for healthy and high-risk loans, respectively. This indicates the model’s capability to correctly identify most healthy loans while maintaining a solid performance in capturing high-risk cases. 

Given the critical importance in a lending context of accurately identifying high-risk loans (to mitigate financial loss and manage risk), the model’s high recall for high-risk cases is particularly valuable. 

Therefore, the logistic regression model is recommended, as it provides a reliable balance of precision and recall, ensuring the effective identification of high-risk loans without significantly increasing false positives. This balance makes it an optimal choice for managing credit risk while supporting operational efficiency.
