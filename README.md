# Yes_Bank_Stock_Closing_price_Prediction

# Introduction -

In today's rapidly evolving world, the banking sector is experiencing unparalleled growth and expansion on a daily basis. The advent of technology has revolutionized the way they operate, granting them unprecedented access to vast markets and an ever-expanding customer base.
Here we talking about the "Yes Bank" which is one of the prominent private-sector banks in India. Established in 2004, it operates as a full-service commercial bank offering a wide range of banking and financial services to individuals, businesses, and corporate clients.
As with any investment, predicting the future price of a stock involves a certain level of uncertainty. However, various approaches and techniques are used to analyze historical data and market trends to estimate future prices.

# Problem Statement

Yes Bank is a well-known bank in the Indian financial domain. Since 2018, it has been in the news because of the fraud case involving Rana Kapoor. Owing to this fact, it was interesting to see how that impacted the stock prices of the company and whether Time series models or any other predictive models can do justice to such situations. This dataset has monthly stock prices of the bank since its inception and includes closing, starting, highest, and lowest stock prices of every month. The main objective is to predict the stock's closing price of the month.

# Dataset description:

Date - Date of record
Open - Opening Price
High - Highest price in the day
Low - Lowest price in the day
Close - Price at the end of the day

# Approach taken

* Data inspection
* EDA
* Data preparation
  
Data YesBank StockPrices.csv, one of the CSV files, has around 185 rows and 5 columns. Since we only have one data collection, we opt to collaborate with other team members. First, we imported all necessary libraries for a later assessment.We have reviewed the data that has been provided and done data interpretation. Only one column has data of the string (object) type, whereas the majority of the data are of the int data type. After using pandas to load the supplied data set into the colab environment, we performed some data cleaning by adding more necessary columns, eliminating undesirable columns, renaming columns, and so on. After data cleaning, we performed data wrangling, which involves running a programme to extract particular results from the supplied data set.
Next, we visualized the processed data for graphical representation. The following task is feature engineering, which we completed in this step. The pre-processing stage in machine learning known as feature engineering is used to turn raw data into features that may be utilized to build a prediction model using either machine learning or statistical modeling. Machine learning feature engineering seeks to enhance model performance. Four operations make up the majority of feature engineering in machine learning: feature creation, transformations, feature extraction, and feature selection. The machine learning portion is the most crucial and challenging since we must choose two variables. both the independent and dependent variables. employing an alternative regression technique, such as Linear Regression, Lasso Regression, and Ridge Regression model.

We will measure the accuracy of the model's predictions after it has learned from the training data using the Mean Squared Error, Root Mean Squared Error, Mean Absolute Error, R square, Adjusted R squared, and R2 score following Hyperparameter tuning using GridSearch CV. Finally, based on how successfully it forecasts future stock values, we'll come to the conclusion that the approach is the best of the three.

In the end, we extracted the conclusion after training the model for future prediction.

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
