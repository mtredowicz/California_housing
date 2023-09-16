# Project Description
This project focuses on building and evaluating machine learning models to predict binary housing price categories based on various features. 
The dataset used for this analysis is the California Housing dataset, which contains information about housing attributes and their corresponding prices. 
The primary goal is to develop models that can distinguish between over and under  100 000 $ housing units based on selected features.

**Code Description:**

1. **Import Libraries:** Import necessary libraries, including pandas, numpy, and scikit-learn modules.

2. **Load the Dataset:** Fetch the California Housing dataset using scikit-learn's `fetch_california_housing` function. Print a description of the dataset and its feature names.

3. **Data Preprocessing:**
   - Create data and target DataFrames.
   - Modify the target variable to binary values (1 for over  100k  $, 0 for under 100k $).

4. **Feature Selection:** Choose a subset of features for modeling.

5. **Data Preparation:**
   - Standardize the feature data using StandardScaler.

6. **Data Splitting:** Split the data into training and testing sets using a 80-20 split ratio.

7. **Model Selection and Tuning:**
   - Fit and tune various classifiers:
     - k-Nearest Neighbors (kNN) with hyperparameter tuning.
     - Ridge Classifier with hyperparameter tuning.
     - Lasso Regression with hyperparameter tuning.
     - Logistic Regression with L1 regularization and hyperparameter tuning.
     - Logistic Regression with L2 regularization and hyperparameter tuning.

8. **Model Evaluation:**
   - Evaluate each model using 5-fold cross-validation and report their mean ROC AUC scores, which measure the model's ability to distinguish between classes.

9. **Make Predictions:** Use the best-performing model (Logistic Regression with L2 regularization) to make predictions on the test set.

10. **Confusion Matrix:** Compute and display the confusion matrix to evaluate model performance.

11. **Accuracy:** Calculate and print the accuracy score, indicating the overall model accuracy on the test set.

12. **F1 Score:** Calculate and print the F1 score, which combines precision and recall to assess the model's performance.

This project aims to help users understand how different machine learning models perform in classifying housing units as high-priced or low-priced based on selected features. 
The project provides a clear pipeline for data preprocessing, model selection, tuning, and evaluation, making it a valuable resource for predictive modeling tasks.
