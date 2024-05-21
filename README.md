# Yes Bank Stock Price Prediction

## Business Context
Yes Bank is a prominent entity in the Indian financial sector. Since 2018, it has garnered significant attention due to a fraud case involving Rana Kapoor. This project aims to analyze the impact of this event on the bank's stock prices and to determine whether time series or other predictive models can accurately forecast such fluctuations. The dataset includes monthly stock prices from the bank's inception, covering closing, starting, highest, and lowest prices.

## Project Objective
Predict the stock’s closing price for each month.

## Project Summary

### Data Cleaning
- Addressed null values, duplicate data, and outliers.

### Exploratory Data Analysis
- Plotted the dependent variable and distributions of dependent and independent variables.
- Checked and visualized the correlation between our dependent and independent variables.
- Visualized the relationship between each pair of variables.

### Data Preprocessing & Feature Engineering
- Checked for and addressed multicollinearity in the dataset.
- Applied log transformation to handle positively skewed data.
- Scaled the data and split it into training and test sets.

### Model Implementation
- Fitted various models and optimized them via cross-validation.
- Used these models to make predictions on test and train data.
- Implemented Models:
  - Linear Regression
  - Lasso Regression
  - Ridge Regression
  - Elastic Net Regression

### Data Visualization
- Utilized various charts like line charts, scatter plots, heatmaps, pair plots, distplots, and boxplots to visualize data and understand correlations and trends.

### Model Performance Comparison
- Compared all implemented models using regression evaluation metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), R-squared, and Adjusted R-squared.

### Conclusion
- Derived insights from the data and predictions made by various models on unseen (test) data.

## Dataset Information

### Features
- `Date`: The date (Month and Year).
- `Open`: The stock price at the beginning of the period.
- `High`: The peak price during the period.
- `Low`: The lowest price during the period.
- `Close`: The trading price at the end of the month.

## Conclusion
- Data visualization revealed a significant decline in stock prices during the 2018 fraud case involving Rana Kapoor.
- No null values or duplicate data were found in the dataset.
- Outliers were present but were retained to preserve the dataset's integrity given its small size.
- All variables exhibited positive skewness, so log transformation was applied.
- There was a high correlation between dependent and independent variables, indicating strong predictive capabilities.
- Despite high multicollinearity among independent variables, it was tolerated due to the dataset's small size.
- Elastic Net regression outperformed other models, achieving an Adjusted R² score of 0.9932.
- All models performed well, with Adjusted R² values above 99%.
- No heteroscedasticity was detected, ensuring consistent model performance.
- The model's high accuracy allows for confident deployment for future predictive tasks.
