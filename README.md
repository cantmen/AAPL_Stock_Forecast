# AAPL_Stock_Forecast
This is an exercise in forcasting time series data. 

## Dependencies
In order to forecast AAPL stock, [prophet](https://facebook.github.io/prophet/docs/quick_start.html) is used.



Matplotlib is used for plotting the forecasted data.

Pandas is used to handle dataframes.

## Included Documents
stocks.csv includes data on price over time on multiple stokcs.

stk_forecast.csv includes the forecasted AAPL stock prices for 365 days.

AAPL.csv shows the real values of stock prices for the forecasted period.

## Explanation

My aim from this analysis is to create a forecast for AAPL stock prices. I used "date" and "AAPL" columns from stocks.csv data frame by fitting it to a new model to do my forecast. By giving the period as 365 days, I got this result:

![](Stock%20Analysis/Images/AAPL_Forecast.png)

To evaluate the forecast, I plotted a new figure showing both the forecasted data and actual AAPL stock prices. Before I adjusted holidays on the data, the relationship between AAPL opening prices and forecasted stock prices are seen as:

![](Stock%20Analysis/Images/Before_Holiday_Adjustment.png)

After adjusting the holiday seasons to data, the new comparison looks like:

![](Stock%20Analysis/Images/Prediction_vs_Opening_Prices.png)

The circles on the images show the difference adjusting Christmas and Black Friday dates make. Adjusting the holidays makes the forecasted stock prices look closer to the real opening prices. 

