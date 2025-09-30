# Credit_Risk_Modelling
# Credit Risk Modelling using Machine Learning

This repository contains a comprehensive workflow for credit risk modelling using machine learning, focusing on preprocessing, feature selection, and advanced model tuning with XGBoost. The project demonstrates a complete pipeline from data processing to hyperparameter optimization, with documented model comparison and results.

Project Overview

The workflow builds a multi-class credit risk classification system using historical applicant and account activity features. Core methods include:

Data loading, cleaning, and merging of multiple sources.

Categorical and numerical feature selection (Chi-square, ANOVA, VIF).

Encoding and scaling of features.

Training and evaluation of baseline models (Random Forest, Decision Tree).

Extensive hyperparameter search for XGBoost.

Analysis and export of the best hyperparameter combinations and results.

Features
Feature Engineering: De-duplication, null removal, categorical encoding, numerical scaling.

Modeling: Baseline (Random Forest, Decision Tree), advanced (XGBoost with multi-class outputs).

Hyperparameter Optimization: Grid search across key XGBoost settings (learning rate, tree depth, column sample, L1 regularization, estimators).

Result Analysis: Accuracy, precision-recall-F1 for all classes; best parameter set tracking and export to Excel.

Installation
Clone this repository and navigate to its folder.

Install the required libraries:

pip install numpy pandas matplotlib scikit-learn xgboost openpyxl
Usage

Place input Excel files (case studies) in the working directory.

Run the main notebook or script to execute the full pipeline:

Reads and merges data

Runs feature selection

Trains baseline models

Runs XGBoost with grid search optimization

Exports results as xgboost_hyperparameter_results.xlsx

Inspect the result files to analyze model performance and recommended configurations.


See full hyperparameter results in the xgboost_hyperparameter_results.xlsx file for details on all grid search runs.

Results

Best XGBoost Test Accuracy: Up to 0.822 observed during grid search.

Robust analysis of parameter influence, including accuracy tradeoffs, heatmaps, and class-wise precision/recall for each model.

