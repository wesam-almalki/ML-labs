# Loan Data Analysis and Prediction

## Overview

This project explores a loan dataset and builds a machine learning model to predict whether a loan will be fully paid or not.

## Dataset

Key features include:

* fico: Credit score
* int.rate: Interest rate
* purpose: Loan purpose
* credit.policy: Credit policy status
* not.fully.paid: Target variable

## Workflow

* Performed Exploratory Data Analysis (EDA) using visualizations
* Converted categorical data using pd.get_dummies
* Split data into training and testing sets
* Trained a Logistic Regression model

## Evaluation

The model was evaluated using classification report and confusion matrix.

## Results

The model performs well on the majority class (0) but struggles with the minority class (1) due to imbalanced data.
