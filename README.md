# GrowthLink-Task


# SMS Spam Classification

This project aims to develop a machine learning model that can classify SMS messages as either spam or ham (not spam).

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Conclusion](#conclusion)

## Introduction

SMS spam classification is a common task in natural language processing and machine learning. The goal is to build a model that can accurately identify unwanted or unsolicited messages, allowing users to filter them out and focus on legitimate communication.

## Dataset

The dataset used for this project is the "spam.csv" file, which contains a collection of SMS messages labeled as either spam or ham. The dataset is loaded and preprocessed using the pandas library in Python.

## Methodology

The following steps were taken to develop the SMS spam classification model:

1. **Data Loading:** The "spam.csv" file was loaded into a pandas DataFrame.
2. **Data Exploration:** The data was explored to understand its characteristics, such as the distribution of spam and ham messages, the presence of missing values, and the frequency of duplicate rows.
3. **Data Cleaning:** Duplicate rows were removed, and the text in the messages was converted to lowercase.
4. **Data Preparation:** The text data was prepared for modeling by removing punctuation, stop words, and performing stemming. The text was then converted into numerical features using TF-IDF vectorization.
5. **Data Splitting:** The data was split into training and testing sets to evaluate the model's performance.
6. **Model Training:** A Logistic Regression model was trained on the training data.
7. **Model Evaluation:** The trained model was evaluated using the test data, and metrics such as accuracy, precision, recall, and F1-score were calculated.
8. **Model Optimization:** The Logistic Regression model was optimized by tuning its hyperparameters using GridSearchCV to maximize the F1-score.

## Results

The initial Logistic Regression model achieved an accuracy of 0.943, precision of 0.967, recall of 0.608, and an F1-score of 0.747. After hyperparameter tuning with GridSearchCV, the optimized model achieved an accuracy of 0.961, precision of 0.933, recall of 0.776, and an F1-score of 0.847. The optimized model showed significant improvement in recall, indicating a better ability to correctly identify spam messages.

## Conclusion

This project demonstrates the development of an effective SMS spam classification model using Logistic Regression. The model achieved good performance on the test data, with an F1-score of 0.847 after optimization. Further improvements could be explored by addressing convergence issues during training and experimenting with alternative classification algorithms.
