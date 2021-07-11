## Buy Apple


The world’s economy is based on stock market trading actions, every day, every second of the day the stock market is changing, people is buying, selling, checking prices trends, making money, losing money, these actions affect the course of the world and people lives. For stockbrokers this is their entire life, and for investors trends and prices are vital, this project intends to analysis the Apple Stock Prices in time and predict an action to buy or not a single stock depending on its price, based on the price of the stock that will be minor or equal the third
quartile of the rolling mean (12-month period). The features used for this prediction would be values of stocks of Apple closer competitors: Google, Microsoft, and Samsung, and other companies that are not considered competitors or related to the Apple line of business like, Disney Stock prices, Gold and Oil prices. This analysis is based on closing prices from 2014 to 2021. All Companies’ stock prices were highly correlated with the Apple Stock prices. Random Forest, KNeightbors and Logistic Regression were used to predict the buying action for Apple Stocks, the results for each of the models were similar, having an accuracy value of 0.98. These models will be reviewed.

Question: May I know when to buy or not in a future an Apple Stock, based prices of closest competitors, oil prices, gold process, and Disney stock price?

This project is made as a personal project to create an strategy for stock trading for the family and to complete the school work for the DSC680 All code is based on Jupyter Notebook and using Ptyhon as a main language



## Code Details

For more details please refer to my github repostory

# Results

### The Data

The majority of the data was collected from Yahoo Finance, and the data for oil, prices was collected from Macro trends. The analysis was made using Python language. Each company stock price was analyzed and tested stationarity, using ADF (Augmented Dickey-Fuller) Test [2]. Data was obtained on csv files, read using pandas, cleaned, and organized to then merge all the data sets on final data set that only contains closing prices and data, rolling mean of the closing apple stock price was calculated to determine the third quartile to set a buying price. Correlation using Pearson method was calculated for the whole data set, finding in most of the feature high positive correlation, but the Oil Prices

The price to use for this study is the closing price. The final data set used to feed the models looked as shown: 

![image](https://user-images.githubusercontent.com/58094203/125209204-47da5f80-e265-11eb-90a0-d8c39325fe2a.png)

## The Graph Analysis

Line graphs and Hitograms were used to analyize the distribution of the data, Time sieres analysis was mde for the Apple Stock Prices:

![image](https://user-images.githubusercontent.com/58094203/125209521-4a3db900-e267-11eb-83a2-460d8f0b0da6.png)

![image](https://user-images.githubusercontent.com/58094203/125209524-51fd5d80-e267-11eb-9b10-b1467e9117d5.png)


This analysis shows that to make predictions for future values of this stock prices, a decomposition of the trend and seasonality of this data set, should be made to reach accurate results. Prediction using time series decomposition requires the separation of trend and seasonality, and in this case, this technique would have to be used for each of the companies in this study, as mentioned, this will be a second part of this project

![image](https://user-images.githubusercontent.com/58094203/125209542-65102d80-e267-11eb-8eff-0c33a3a2048d.png)

## The Models

Based on the analysis presented before either of the three models presented can be used based on their accuracy, Logistic regression model has the higher accuracy 0.985, based on this metric, this model should be used, however the deployment of this model to predict daily buying actions based on the price of the stock it is not a realistic option, the stock market prices depends on several factors that are not being taking in consideration on this analysis, most important of all would be the time series and the factors of trends and seasonality, these factors affect the data points and it is not correct to predict values without taking in consideration this analysis, please see Appendix 1 for more details about ADF stationarity test for all the stock market by companies. Other factors like political and social factors must being taking in consideration but these are not within the scope of this project.

![image](https://user-images.githubusercontent.com/58094203/125209647-4494a300-e268-11eb-9553-1842edac6734.png)


### Linear regression Apple Stock Prices Resutls

![image](https://user-images.githubusercontent.com/58094203/125209656-537b5580-e268-11eb-89bb-c07f257c4b3b.png)

Mean Absolute Error: 3.919973133612361
Mean Squared Error: 25.375839022592544
Root Mean Squared Error: 5.037443699198289






### References

[Yahoo Finance](https://finance.yahoo.com/)

[MacroTrends](https://www.macrotrends.net/)

[Kaggle](https://www.kaggle.com/search?q=janet+street)


### Author

Gloria Moore
