# Santander Value Prediction

This repository contains a solution for the "Santander Value Prediction" problem, which aims to predict the value of transactions for potential customers.

Access the dataset from [Kaggle](https://www.kaggle.com/competitions/santander-value-prediction-challenge/overview)

## Code Overview

The code is written in Python and utilizes the following libraries:

- **numpy:** For numerical computations and array manipulation
- **pandas:** For data manipulation and analysis
- **matplotlib and seaborn:** For data visualization
- **sklearn:** For various machine learning algorithms and evaluation metrics
- **lightgbm:** For training a gradient boosting model

Here's a summary of the major steps in the code:

- **Data Loading:** The training and test datasets are loaded from CSV files.
- **Data Overview:** The shape of the datasets and their contents are examined through exploration and visualization.
- **Data Preprocessing:** Columns with only one unique value or a high percentage of zeros are identified and dropped from the datasets.
- **Modeling:** Two models are trained and evaluated using k-fold cross-validation. The models used are Ridge regression and LightGBM (a gradient boosting model).
- **Feature Engineering:** Nearest neighbors features are calculated and added to the datasets to enhance the predictive power of the models.
- **Prediction:** The trained models are used to make predictions on the test dataset.
- **Submission:** The predictions are stored in a CSV file following the submission format.

## Usage

To use this code, follow these steps:

- Ensure that Python is installed on your system along with the required libraries mentioned in the code.
- Download the training and test datasets from the provided source and place them in the appropriate directory.
- Adjust the file paths in the code to match the location of the dataset files.
- Execute the code to preprocess the data, train the models, make predictions, and generate the submission file.
- Review the RMSLE (Root Mean Squared Logarithmic Error) scores to evaluate the performance of the models.
