BREAST CANCER PREDICTION USING SNOWFLAKE SCHEMA AND LOGISTIC REGRESSION
====================================================================

PROJECT OVERVIEW
----------------
This project focuses on predicting breast cancer diagnosis using Logistic Regression
applied to the Breast Cancer dataset. The dataset is modeled using a Snowflake Schema
to demonstrate basic data warehousing concepts alongside machine learning classification.

The goal is to show how structured data modeling (Snowflake Schema) can be integrated
with a classical statistical machine learning algorithm (Logistic Regression) for
binary classification.

This is a fundamental, interpretable approach suitable for academic and learning purposes.


PROBLEM STATEMENT
-----------------
Breast cancer diagnosis involves classifying tumors as either malignant or benign
based on measured features. Manual diagnosis can be time-consuming and subjective.

This project aims to:
- Store breast cancer data in a Snowflake Schema format
- Apply Logistic Regression for accurate and explainable classification
- Evaluate the model using standard performance metrics


DATASET
-------
Dataset Used:
- Breast Cancer Wisconsin Dataset

Target Variable:
- Diagnosis (Malignant / Benign)

Features:
- Tumor characteristics such as radius, texture, perimeter, area, smoothness, etc.

Data Structure:
- Fact table contains measurement values
- Dimension tables store related descriptive attributes
- Snowflake Schema is used to normalize dimension tables


TECHNOLOGIES USED
-----------------
- Python
- Pandas
- NumPy
- Scikit-learn
- SQL (for Snowflake Schema representation)


SNOWFLAKE SCHEMA DESIGN
----------------------
- Fact Table:
  - Measurement_ID
  - Feature values
  - Diagnosis label

- Dimension Tables:
  - Patient Dimension
  - Feature Dimension
  - Diagnosis Dimension

Purpose:
- Reduce redundancy
- Demonstrate normalized data warehousing design
- Enable structured analytical queries


ALGORITHM USED
--------------
Logistic Regression

Reason for Selection:
- Suitable for binary classification
- Easy to interpret
- Computationally efficient
- Widely accepted in medical data analysis

The model predicts the probability of a tumor being malignant or benign using a
logistic (sigmoid) function.


IMPLEMENTATION STEPS
--------------------
1. Load the Breast Cancer dataset
2. Clean and preprocess the data
3. Design Snowflake Schema tables
4. Normalize data into fact and dimension tables
5. Split data into training and testing sets
6. Train Logistic Regression model
7. Test the model on unseen data
8. Evaluate performance using metrics


EVALUATION METRICS
------------------
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

These metrics help assess classification performance and reliability.


RESULTS
-------
- The model achieves high accuracy due to clear feature separation
- Logistic Regression provides interpretable coefficients
- Snowflake Schema improves data organization but does not affect model accuracy directly


ADVANTAGES
----------
- Simple and explainable model
- Suitable for structured medical datasets
- Demonstrates both data warehousing and machine learning concepts
- Low computational cost


LIMITATIONS
-----------
- Logistic Regression assumes linear decision boundary
- Snowflake Schema adds complexity for small datasets
- Not suitable for highly complex or non-linear data patterns


FUTURE ENHANCEMENTS
-------------------
- Compare with other classifiers (SVM, Random Forest)
- Implement FP-Growth or advanced feature selection
- Integrate visualization dashboards
- Deploy model using a web application


CONCLUSION
----------
This project successfully demonstrates breast cancer prediction using Logistic
Regression combined with Snowflake Schema-based data modeling. It highlights the
importance of structured data design and interpretable machine learning models in
medical data analysis.


AUTHOR
------
Project Title : Breast Cancer Prediction Using Snowflake Schema and Logistic Regression
