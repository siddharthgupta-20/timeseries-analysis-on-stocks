# Stock-price-prediction

Importing libraries
Adding 3 new features :
change(closing_price-opening_price)
Percent change(how much stock lost or gained during the day
Decline (whether particular stock declined during day)

Moving averages help us to see the stock prices in the long term by smoothing the graph and showing the general trend of the graph.(calculated moving averages for a week, bi-week, and 60 days)

Taking similar types of stock under the same label,for example, tata motors and tata steel, I presume that both the stocks are related somehow.(correlation: +0.49)

Then we spend Rs10000 at each stock to determine the risk in each stock

Pre-processing:
Converting the date_time format into columns of dataframe as month, week, day
Making other dataframes with rolling window of 3, 7 and 30 days and adding them to original dataset

Applying the prophet model on TCS stocks

Applying ARIMA model on Bajaj stocks

Applying RRN on TATASTEEL (using 50 previous values to predict 1 next value)(loss='mean_squared_error',optimizer='adam')

Trying early stopping to get better results( rmse = 19.73)

Applying LSTM ( rmse = 27.53)

Checking effect of Ukraine war on the stocks which started on 24 th feb,2022 on 3 example stocks APPLE,HDFC and TATAMOTORS.
Defining average directional movement(ADX)
ADX <=25 no trend
25 < ADX <50 trending
ADX> 50 strongly trending

we can see that in the start of 2022 hdfc stock pricing has been decreasing and had a gradual decrease till june 2022, we  can see a slight rise in the stock pricing at the end of  june to july,2022. The ADX values have been below 25 for almost all the time since 2022-02 showing no trending of these stocks
