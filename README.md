# Housing Price Prediction with Exploratory Data Analysis and Linear Regression

## Project Overview

This project explores and analyzes a dataset of housing prices (housing.csv) to build a machine learning model for predicting prices.

## Dependencies:

- pandas (for data manipulation)
- numpy (for numerical computations)
- seaborn (for data visualization)
- scikit-learn (for machine learning)

## Data Exploration:

1. Import libraries: The code begins by importing necessary libraries: pandas (pd), numpy (np), seaborn (sns), and from sklearn.linear_model import LinearRegression for linear regression and from sklearn.model_selection import train_test_split for splitting data.
2. Read data: The pd.read_csv("housing.csv") line loads the housing data into a pandas DataFrame named df.
3. Examine data: df.head() displays the first few rows of the DataFrame to get a glimpse of the data.
  - df.shape reveals the dimensions (number of rows and columns) of the DataFrame.
  - df.describe() provides summary statistics for numerical columns (mean, standard deviation, quartiles, etc.).
  - df.isnull().sum() checks for missing values in each column.

## Visualization:

- The code employs seaborn's relplot function to create three relational plots:
- 1st visualizes the relationship between Price, Avg. Area House Age, and Avg. Area Number of Bedrooms with color-coding for different bedroom counts.
- 2nd explores the relationship between Price and Avg. Area Number of Bedrooms.
- 3rd examines the relationship between Price and Avg. Area Number of Rooms.
- These visualizations can help identify potential correlations between features and price.


## Model Building:

- The code prepares features (dropping Price and Address) and splits data for training and testing.
- A linear regression model is created, trained, and used to make predictions on unseen data.
 - Model performance (R-squared) is evaluated on the testing set.
   
