# Walmart Sales Prediction Model Report

## Problem Statement
Walmart aims to predict their sales and demand accurately. Certain events and holidays impact daily sales. Sales data for 45 Walmart stores is available in the `Walmart.csv` file. The business faces challenges due to unforeseen demands and stockouts, attributed to inadequate machine learning algorithms.

## Goal
Develop an ideal machine learning algorithm to predict weekly sales accurately, incorporating factors like economic conditions, CPI, and the Unemployment Index.

## Report

### Model Selection
The objective is to predict weekly sales, a continuous variable, indicating the use of regression models. Given the multiple features influencing the prediction, we tested the following models:

- Multiple Linear Regression
- Support Vector Regression (SVR)
- Decision Tree Regression
- Random Forest Regression

### Evaluation Metrics
The models were evaluated using the following metrics:

- **R² Score**: Indicates the proportion of variance in the dependent variable predictable from the independent variables.
- **Mean Absolute Error (MAE)**: The average absolute difference between predicted and actual values.
- **Mean Squared Error (MSE)**: The average of the squared differences between predicted and actual values.

### Results
After training each model, they were tested with the same test set, yielding the following results:

| Metric      | Multiple Linear | SVR          | Decision Tree | Random Forest |
|-------------|-----------------|--------------|---------------|---------------|
| **R² Score** | 0.13            | -0.04        | 0.69          | 0.93          |
| **MAE**     | 438,460.78      | 460,891.17   | 214,397.51    | 77,228.69     |
| **MSE**     | 291,515,759,979.30 | 327,198,488,157.92 | 317,939.26    | 150,949.20    |

### Conclusion
The Random Forest model exhibited the best prediction performance with the highest R² Score and the lowest MAE and MSE. Therefore, the Random Forest model is considered the best for predicting weekly sales for Walmart.