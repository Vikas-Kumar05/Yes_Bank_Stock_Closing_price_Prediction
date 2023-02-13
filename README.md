# Yes_Bank_Stock_Closing_price_Prediction
Project Summary -
This project is done by Vikas Kumar. We received a single CSV file for this project's input. Data YesBank StockPrices.csv, one of the CSV files, has around 185 rows and 5 columns. Since we only have one data collection, we opt to collaborate with other team members. First, we imported all necessary libraries for a later assessment. A well-known bank in the Indian financial industry is Yes Bank. The Rana Kapoor fraud case has been in the headlines since 2018 as a result of it. Due to this, it was intriguing to observe how it affected the company's stock prices and whether Time series models or other prediction models could adequately account for such circumstances.Since the bank's foundation, this dataset has included closing, starting, highest, and lowest stock values for each month. Predicting the stock's monthly closing price is the primary goal.

Second, we have reviewed the data that has been provided and done data interpretation. Only one column has data of the string (object) type, whereas the majority of the data are of the int data type. After using pandas to load the supplied data set into the colab environment, we performed some data cleaning by adding more necessary columns, eliminating undesirable columns, renaming columns, and so on. After data cleaning, we performed data wrangling, which involves running a programme to extract particular results from the supplied data set. Next, we visualized the processed data for graphical representation. The following task is feature engineering, which we completed in this step. The pre-processing stage in machine learning known as feature engineering is used to turn raw data into features that may be utilised to build a prediction model using either machine learning or statistical modelling. Machine learning feature engineering seeks to enhance model performance. Four operations make up the majority of feature engineering in machine learning: feature creation, transformations, feature extraction, and feature selection. The machine learning portion is the most crucial and challenging since we must choose two variables. both the independent and dependent variables. employing an alternative regression technique, such as Linear Regression, Lasso Regression, and Ridge Regression model.

1. Linear Regression- One of the most fundamental kinds of regression in machine learning is linear regression. A predictor variable and a dependent variable that are linearly related to one another make up the linear regression model. A multiple linear regression model is what is used when there are numerous independent variables in the data.

2. Ridge Regression- Another regression type utilised in machine learning, this one is typically applied when the correlation between the independent variables is large. This is so that the least square estimations for multi-collinear data provide unbiased values. But there might be some bias value if the collinearity is really high. As a result, the Ridge Regression equation includes a bias matrix. With this effective regression technique, the model is less prone to overfitting.

3. Lasso Regression- One of the regression models used in machine learning that combines feature selection and regularisation is called Lasso Regression. It forbids the regression coefficient's maximum absolute value. As a result, unlike in the case of Ridge Regression, the coefficient value approaches zero.

We will measure the accuracy of the model's predictions after it has learned from the training data using the Mean Squared Error, Root Mean Squared Error, Mean Absolute Error, R square, Adjusted R squared, and R2 score following Hyper parameter tuning using GridSearch CV. Finally, based on how successfully it forecasts future stock values, we'll come to the conclusion that approach is the best of the three.

In the end, we extracted the conclusion after training the model for future prediction.

Dataset description:

Date - Date of record

Open - Opening Price

High - Highest price in the day

Low - Lowest price in the day

Close - Price at the end of the day

Problem Statement
Yes Bank is a well-known bank in the Indian financial domain. Since 2018, it has been in the news because of the fraud case involving Rana Kapoor. Owing to this fact, it was interesting to see how that impacted the stock prices of the company and whether Time series models or any other predictive models can do justice to such situations. This dataset has monthly stock prices of the bank since its inception and includes closing, starting, highest, and lowest stock prices of every month. The main objective is to predict the stock's closing price of the month.

Conclusion:

1. In the EDA section, we draw the following conclusions from our data: After 2018, the stock's closing price declined, primarily as a result of the Rana Kapoor case, which had a negative impact on the stock price. The initial price and closing price on the Yes BANK graph are identical.

2. The fact that after 2018, the stock price of YES BANK drops, making it unwise for investors to place money in the company.

3. We can infer from the scatter plot that the bivariate analysis shows a strong link between closing price and other parameters.

4. Every histogram plot reveals that they are all right-skewed. Because the data was slightly right-skewed, we utilised log transformation to alter it.

5. We may infer from the heatmap that all the features have a significant degree of association with one another.

6. The ridge regression model is the best model for forecasting the closing price of Yes Bank's stock, according to the findings of the prior comparisons.

7. With low mean squared error, root mean squared error, and mean absolute error, as well as a high R2 score, the ridge regression model has consistently demonstrated a high level of prediction accuracy.

8. The Local Interpretable Model-agnostic prediction local values further support the excellent accuracy of the ridge regression model.

9. The linear regression model offers intermediate accuracy, whereas the lasso regression model has a lesser level of accuracy.

10. As a result, the ridge regression model is best suited to forecast the closing price of Yes Bank's shares.

Following that, we visualise the results of our linear regression model, and the graph demonstrates that we almost perfectly fit our dataset with our model.
