## Buy Apple

Predicting Apple Stock Buying Action The following project intends to predict apple stock buying action based on prices predicted using different variables like: closest competitors stock prices, gold prices, crude oil prices, CPI and disney stock prices. The action predicted will be by day This project is made as a personal project to create an strategy for stock trading for the family and to complete the school work for the DSC680 All code is based on Jupyter Notebook and using Ptyhon as a main language

Question: May I know when to buy or not in a future an Apple Stock, based prices of closest competitors, oil prices, gold process, temperature of the day and Disney stock price?
My proposal consists of to analyze prices of the closest Apple Tech Competitors, like Samsung, Google, Dell and Microsoft, if these prices affect the Apple stock prices, can I predict Apple prices in the future? I will introduce some different features as temperature of the day for Florida, and Disney Stock Prices, is Disney is always on the race for latest technology, for Disney is more oriented to entertainment, however, I can’t imagine going to Disney without my iPhone, Air Pods and iWatch.
Introducing some more economic indicators features, I will use gold prices and crude oil prices to predict apple stock prices.
I am analyzing the possibility to add cryptocurrency like the Bitcoin into this list as a suggestion of one of my peers on the Teams channel.



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
