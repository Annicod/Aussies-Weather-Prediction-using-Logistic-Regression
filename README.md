# Aussies-Weather-Prediction-using-Logistic-Regression

# Overview

This project applies a Logistic Regression model to predict weather conditions using a dataset from Australia. The model is trained to predict the likelihood of rain based on various weather features. The project includes preprocessing steps for handling missing values, scaling numerical data, and encoding categorical variables.

# Dataset

The dataset used in this project is an Australian weather dataset that includes both numerical and categorical features. The target variable is whether it will rain tomorrow (RainTomorrow).

# Data Preprocessing

The data is preprocessed in the following ways:

Missing Values:

For numerical columns, missing values were filled using Scikit-learn's SimpleImputer with the mean strategy.
For categorical columns, missing values were handled using OneHotEncoder, which transforms categorical features into binary-encoded vectors.
Scaling:
Numerical data was scaled between 0 and 1 using MinMaxScaler to ensure that all features contribute equally to the model, assigning the correct weight to each column.

# Data Splitting

The dataset was divided into three parts:

Training Data: Used to train the Logistic Regression model.
Validation Data: Used to tune hyperparameters and validate the model during training.
Test Data: Used to evaluate the final performance of the model.

# Logistic Regression Model

The model used in this project is a Logistic Regression classifier from Scikit-learn. The model was trained on both the numerical and categorical features.

# Model Performance
The best performing model achieved an accuracy of 85.51% on the validation set.
The model performance is consistent across the training, validation, and test sets, indicating that the model is well generalized.
Categorical features showed slightly lower predictive power compared to numerical features.

