# Student Performance Prediction System

## Project Overview

The Student Performance Prediction System is a machine learning project that predicts whether a student is likely to pass or fail based on demographic, family, academic, and lifestyle information.

The project uses Python and Scikit-learn to preprocess student data, train classification models, evaluate their performance, and make predictions through an interactive Gradio web interface.

## Objectives

- Build a binary classification model for student pass/fail prediction.
- Apply data preprocessing using Scikit-learn pipelines.
- Compare multiple machine learning algorithms.
- Improve model selection using cross-validation and hyperparameter tuning.
- Develop an interactive interface for generating predictions.

## Dataset

- **Source:** UCI Machine Learning Repository — Student Performance dataset
- **Number of records:** 649 students
- **Input features:** 30
- **Target:** Pass or Fail
- **Target definition:** Pass if the final grade (G3) is at least 10 out of 20.

The dataset represents students from Portuguese schools.

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Gradio
- Joblib
- Google Colab

## Machine Learning Workflow

1. Loaded and explored the dataset.
2. Created a binary target from the final grade.
3. Split the data into training and testing sets.
4. Built preprocessing pipelines for numerical and categorical features.
5. Compared Logistic Regression, Decision Tree, and Random Forest models.
6. Used stratified cross-validation and GridSearchCV to tune Logistic Regression.
7. Evaluated the selected model using classification metrics.
8. Saved the trained pipeline and connected it to a Gradio interface.

## Model Evaluation

The tuned Logistic Regression model achieved the following test results:

| Metric | Result |
|---|---:|
| Accuracy | 68.5% |
| Fail precision | 23.1% |
| Fail recall | 45.0% |
| Fail F1-score | 30.5% |

Fail recall is especially important because it measures how many students who actually failed were correctly identified by the model.

## Interactive Application

The Gradio interface allows users to enter student information and receive a predicted pass/fail result along with estimated probabilities.

## Limitations

- The dataset represents Portuguese schools and may not generalize to other education systems.
- The model makes errors and should not be used as the sole basis for decisions about students.
- Predicted probabilities have not been verified as calibrated probabilities.
- The evaluation results are specific to this dataset and test split.

## Future Improvements

- Evaluate the model on more representative datasets.
- Improve the detection of students at risk of failing.
- Add input validation and further testing.
- Deploy the application on a persistent hosting platform.

## Learning Outcomes

This project provided practical experience with data preprocessing, classification, cross-validation, hyperparameter tuning, model evaluation, model persistence, and interactive machine learning application development.
