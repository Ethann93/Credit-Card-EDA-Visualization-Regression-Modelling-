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

# Model Evaluation Report

### Overview

This report summarizes the performance of various machine learning models applied to the dataset. The goal is to predict [target variable], and the models have been evaluated using different regression techniques.

### Models and Evaluation Metrics

**Linear Regression:**
- Mean Absolute Error (MAE): 0.1823
- Mean Squared Error (MSE): 0.0847
- R-squared (R²) Score: -0.0012

**Random Forest:**
- Mean Absolute Error (MAE): 0.1672
- Mean Squared Error (MSE): 0.0889
- R-squared (R²) Score: -0.0500

**Ridge Regression:**
- Mean Absolute Error (MAE): 0.1825
- Mean Squared Error (MSE): 0.0849
- R-squared (R²) Score: -0.0032

**Gradient Boosting Regression:**
- Mean Absolute Error (MAE): 0.1702
- Mean Squared Error (MSE): 0.0845
- R-squared (R²) Score: 0.0016

**Stacking Regression Model:**
- Mean Absolute Error (MAE): 0.1702
- Mean Squared Error (MSE): 0.0845
- R-squared (R²) Score: 0.0016

### Model Comparison

Among the models evaluated, the Random Forest model achieved the lowest Mean Absolute Error (MAE) of 0.1672, indicating better predictive accuracy.
However, it's important to note that all models exhibit relatively similar performance, with R-squared scores close to zero, suggesting that the models struggle to explain the variance in the target variable.

### Future Steps

- Further feature engineering and data preprocessing may be necessary to improve model performance.
- Consider trying different regression techniques or more advanced machine learning models to see if they can better capture the underlying patterns in the data.
- Explore potential outliers or anomalies in the dataset that could be affecting model predictions.

### Conclusion

In this analysis, we evaluated multiple regression models for predicting [target variable]. While no model achieved a high R-squared score, the Random Forest model demonstrated the best performance among the tested models. Further refinement and exploration of the data may be required to achieve better results.

