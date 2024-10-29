# Gold Price Prediction

This project demonstrates a machine learning approach to predict the price of gold using the Random Forest Regressor model. The dataset used in this project includes various features that potentially influence the price of gold.

## Overview

The code performs the following steps:

1. **Import Libraries**: Essential libraries such as [Pandas](https://pandas.pydata.org/) for data manipulation, [Matplotlib](https://matplotlib.org/) and [Seaborn](https://seaborn.pydata.org/) for data visualization, and [Scikit-learn](https://scikit-learn.org/stable/) for model training and evaluation are imported.

2. **Data Loading and Exploration**:
   - The dataset is loaded using Pandas.
   - Initial exploration is done using `head()` to view the first few rows of the dataset.
   - Missing values are checked using `isnull().sum()`.

3. **Data Preprocessing**:
   - The `Date` column is dropped as it is not needed for the prediction.
   - A correlation matrix is computed and visualized using a heatmap to understand the relationships between features.

4. **Data Visualization**:
   - A distribution plot of the `GLD` (Gold Price) feature is created to visualize its distribution.

5. **Feature and Target Variable Separation**:
   - The features are separated from the target variable `GLD`.

6. **Data Splitting**:
   - The dataset is split into training and testing sets using an 80-20 split.

7. **Model Training**:
   - A Random Forest Regressor model is initialized with 100 estimators and trained on the training data.
   - The model's performance is evaluated using the R-squared metric on both the training and testing datasets.

8. **Results**:
   - The model achieves an R-squared score of approximately 0.999 on the training dataset and 0.989 on the testing dataset, indicating a very good fit to the data.

## Usage

To use this code, ensure you have the necessary libraries installed and the dataset available at the specified path. You can modify the dataset or model parameters to explore different scenarios and improve prediction accuracy.

This project provides a foundation for further exploration and improvement, such as feature engineering, hyperparameter tuning, or using different regression models to enhance prediction performance.
