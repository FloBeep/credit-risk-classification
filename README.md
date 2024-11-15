# credit-risk-classification

In this Challenge, you’ll use various techniques to train and evaluate a model based on loan risk. You’ll use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

### Instructions

The instructions for this Challenge are divided into the following subsections:

* Split the Data into Training and Testing Sets
* Create a Logistic Regression Model with the Original Data
* Write a Credit Risk Analysis Report

### Split the Data into Training and Testing Sets

To receive all points, you must:

* Read the `lending_data.csv` data from the Resources folder into a Pandas DataFrame.
* Create the labels set (`y`) from the “loan_status” column, and then create the features (`X`) DataFrame from the remaining columns.
* Split the data into training and testing datasets by using `train_test_split`.

### Create a Logistic Regression Model

To receive all points, you must:

* Fit a logistic regression model by using the training data (`X_train` and `y_train`).
* Save the predictions on the testing data labels by using the testing feature data (`X_test`) and the fitted model.
* Evaluate the model’s performance by doing the following:
  * Generate a confusion matrix.
  * Generate a classification report.
  * Answer the following question: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?

### Write a Credit Risk Analysis Report

To receive all points, you must:

* Provide an overview that explains the purpose of this analysis.
* Using a bulleted list, describe the accuracy, precision, and recall scores of the machine learning model.
* Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.
