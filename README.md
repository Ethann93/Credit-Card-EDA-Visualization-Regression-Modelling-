# Credit-Card-EDA-Visualization-Regression-Modelling-
EDA on credit card dataset with Visualizations and Regression modelling including: 
# Credit Card (EDA, Visualization & Regression Modeling)

This GitHub repository contains code and analysis for the "Credit Card" dataset. The primary goal of this project is to explore the dataset, visualize its features, perform data cleaning, and create regression models such as (Linear Regression, Random Forest,  Ridge Regression, Gradient Boosting Regression &amp; Stacking Regressing Model) for predicting a target variable labeled "label." The following stages are covered in this code: https://www.kaggle.com/datasets/rohitudageri/credit-card-details

## Importing and Merging Datasets

The code begins by importing necessary libraries, including pandas, numpy, matplotlib, seaborn, and scikit-learn. Two datasets, "Credit_card.csv" and "Credit_card_label.csv," are imported and merged based on a common column, 'Ind_ID.' The dataset can be found on Kaggle website: 

## DataFrame Exploration

A brief exploration of the dataset is conducted using the `describe()` and `info()` functions to gain insights into the data's structure.

## Data Cleaning

- **Check for NaN Values:** The code checks for missing values in the dataset and identifies that the 'Type_Occupation' column contains a significant number of NaN values.
- **Drop Type_Occupation Column:** The 'Type_Occupation' column is dropped, as its missing values could significantly impact the model.
- **Drop NaN Columns:** Rows with missing values are removed from the dataset to ensure data quality.
- **Check for Duplicates:** The dataset is checked for duplicate records.

## Data Visualization

Several data visualization techniques are applied to explore the dataset, including:

- **Calculating Average Income and Average Income by Gender**
- **Visualizing Label Counts**
- **Creating Heatmaps, Box Plots, and Violin Plots**
- **Comparing Data Using Groupby:** Visualizing average annual income by type of income, family members by housing type, family members by marital status, and the number of children's impact on average annual income.

## Preprocessing and Feature Engineering

The dataset is preprocessed, and feature engineering is applied to prepare it for modeling. Label encoding is performed to convert categorical variables into numerical format.

## Model

Regression models are built and evaluated, including **Linear Regression, Random Forest, Ridge Regression, Gradient Boosting Regression**, and a **Stacking Regressing Model**.

## Hyperparameter Tuning

Hyperparameter tuning is conducted on the Stacking Regressing Model using **RandomizedSearchCV** to find optimal hyperparameters.

## Model Comparison

The code concludes by comparing the performance of the different regression models, noting that while the **Random Forest model** achieved the lowest Mean Absolute Error (MAE), all models exhibit relatively similar performance with R-squared scores close to zero, indicating challenges in explaining the variance in the target variable.
