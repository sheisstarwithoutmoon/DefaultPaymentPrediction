# DefaultPaymentPrediction

# Overview
This repository contains a machine learning model for predicting default payment in credit card clients. The model is built using a dataset containing various features of credit card clients and their default payment status.

# Dataset
The dataset used for training and evaluation contains the following columns:

* `ID`: Client ID
* `LIMIT_BAL`: Credit limit
* `SEX`: Gender (1 = male, 2 = female)
* `EDUCATION`: Education level (1 = graduate school, 2 = university, 3 = high school, 4 = others)
* `MARRIAGE`: Marital status (1 = married, 2 = single, 3 = others)
* `AGE`: Age of the client
* `PAY_0 to PAY_6`: History of past payment status (PAY_0 = September 2005, PAY_2 = August 2005, ..., PAY_6 = April 2005)
* `BILL_AMT1 to BILL_AMT6`: Bill statement amount (BILL_AMT1 = amount of bill statement in September 2005, ..., BILL_AMT6 = amount of bill statement in April 2005)
* `PAY_AMT1 to PAY_AMT6`: Amount of previous payment (PAY_AMT1 = amount paid in September 2005, ..., PAY_AMT6 = amount paid in April 2005)
* `default.payment.next.month`: Default payment status (1 = default, 0 = non-default)

# Model Training
The model is trained using the following steps:

* Data Preprocessing: The dataset is preprocessed to handle missing values, encode categorical variables, and scale numerical features.
* Feature Selection: Relevant features are selected for training the model.
* Model Selection: Various machine learning algorithms are evaluated, and the best performing algorithm is selected.
* Model Training: The selected algorithm is trained on the preprocessed dataset.
* Model Evaluation: The trained model is evaluated using appropriate evaluation metrics to assess its performance.

# Usage
To use the trained model for prediction:

* Clone the repository to your local machine.
* Load the trained model using the provided file (model.pkl).
* Prepare input data with the same features used during model training.
* Use the loaded model to make predictions on the input data.
