# Historical Gold Prices Comparison Using Regression Method 

This project aims to develop a model to predict the price of gold based on the date, volume, and the open and close price of gold between the years 2000-2022. Generally, investors invest in gold as it plays an important role in stabilizing investment portfolios. In this study, we compare four regression methods—Linear Regression, Logistic Regression, Lasso Regression, and Ridge Regression—using the R language and data mining techniques. Based on experimental results, Lasso Regression was concluded to be the best method among the four. This project can be further developed to simulate and compare predictions in the context of global monetary crises. Future work could explore the impact of gold mining fluctuations, stock market returns, and inflation rates on gold prices.

## Dataset Overview
- **Data Source:** [gold.csv](https://www.kaggle.com/datasets/faisaljanjua0555/daily-gold-price-historical-dataset)
- **Number of Rows:** 5,703
- **Features:**
    - **Date:** The specific trading date for the gold prices.
    - **Volume:** The total trading volume for the respective date.
    - **Open price:** The gold price at market opening.
    - **Close price:** The gold price at market close.

## Objectives
The key objectives of this project are:
- To explore the relationship between historical data and gold price fluctuations.
- To compare multiple regression techniques for predicting future gold prices.
- To identify the most accurate model for forecasting gold prices.
- To lay the foundation for future work that incorporates global economic factors into price predictions.

## Methods and Models
Four regression models were applied to predict gold prices:
- **Linear Regression:** A basic model that assumes a linear relationship between the independent variables (volume, open price, close price) and the dependent variable (gold price).
- **Logistic Regression:** While primarily a classification model, Logistic Regression was included for comparison. It predicts binary outcomes and was less suited for this continuous prediction task.
- **Lasso Regression:** Lasso Regression adds a regularization term (L1 penalty) to linear regression, which reduces overfitting by shrinking less important feature coefficients to zero. It is useful for feature selection and provides more robust predictions in this context.
- **Ridge Regression:** Ridge Regression is another regularized version of linear regression, but it uses an L2 penalty that minimizes large coefficient values. This helps handle multicollinearity and stabilizes predictions in the presence of correlated features.

## Model Evaluation Metrics
The models were evaluated using the following metrics:
- **Mean Squared Error (MSE):** Measures the average squared difference between actual and predicted values. A lower value indicates better predictive accuracy.
- **R-squared:** Represents the proportion of variance in the dependent variable explained by the independent variables. A higher R-squared indicates a better fit.
- **Root Mean Squared Error (RMSE):** The square root of MSE, RMSE provides a measure of prediction error in the same units as the predicted variable (i.e., gold price).uated based on precision, recall, confusion matrix, and other key metrics to determine their predictive performance.

## Model Comparison
- **Lasso Regression** emerged as the most accurate model, achieving the lowest MSE and highest R-squared score. Its ability to reduce the influence of irrelevant features made it particularly effective for this dataset.
- **Ridge Regression** performed well but did not surpass Lasso Regression in terms of predictive accuracy.
- **Linear Regression** showed decent performance but struggled with overfitting when dealing with complex relationships in the data.
- **Logistic Regression** was not suitable for predicting continuous values and performed the worst among the models.

## Conclusion
The results of this project indicate that Lasso Regression is the most effective model for predicting gold prices. Its ability to regularize and eliminate unimportant features led to superior performance compared to other models. This model can be further developed to handle more complex scenarios, such as the effects of economic crises, inflation, and geopolitical events on gold prices.

## Technical Requirements
To run the analysis, the following R libraries are required:

- `ggplot2 `
- `glmnet `
- `caret`
- `dplyr`


You can install the required R packages by running the following command:

`install.packages(c("ggplot2", "glmnet", "caret", "dplyr"))`

## How to Run the Project
1. **Preprocessing**: Load the dataset, preprocess it to handle missing data, and normalize the features.
2. **Modeling**: Apply the four regression techniques (Linear, Logistic, Lasso, Ridge) to the preprocessed data.
3. **Evaluation**: Use metrics like MSE, R-squared, and RMSE to compare the performance of the models.
4. **Visualization**: Plot the actual vs predicted gold prices to visualize model performance.

## Contributors

2501971742 - Alisha Zahra Saadiya

2540124021 - Edrick Setiawan

2540123044 - Kevin Laurent Oktavian Putra

2540121322 - Lovina Anabelle Citra
