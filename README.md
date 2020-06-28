# Stock-Prediction-using-Prophet

## INTRODUCTION
"The stock market is like a beauty contest where you make money not by selecting which face you think is the prettiest, but by guessing who others will think the prettiest" - Anonymous

Financial theorists, and data scientists for the better part of the last 50 years, have been employed to make sense of the marketplace in order to increase return on investment. However, due to the multidimensional nature of the problem, the scale of the system, and inherent variation with time, it has been an overwhelmingly tough challenge for humans to solve, even with the assistance of conventional data analytics tools. With recent developments in forecasting including Facebook's Prophet model or Amazon's DeepAR these issues have been addressed to some extent. Here we look at predicting a particular company's stock prices using Facebook's Prophet model.


## APPROACH AND CONCEPTS
* **Data Description** - The dataset contains 5 years of stock data for some major and other smaller companies.  All the files have the following columns:
            
            Date - in format: yy-mm-dd

            Open - price of the stock at market open (this is NYSE data so all in USD)

            High - Highest price reached in the day

            Low Close - Lowest price reached in the day

            Volume - Number of shares traded

            Name - the stock's ticker name


## **Modeling** - 
The following steps were taken for using Prophet:
  * Replace closing price for y and date for ds.
  * Fit that dataframe to Prophet in order to detect future patterns.
  * Predict the upper and lower prices of the closing price.

## **Observations** - 
Trends:
  * Amazon's stock price is showing signs of upper trend yearly.
  * Amazon's stock price show upper trend signs during January (December Sales tend to give a boost to Amazon's stock price)
  * There is no weekly trend for stock prices.
  * First major decline after 10-d crosses 50-d moving average
  * Upward trend after 10-day crosses 200-day moving average


## References
* https://www.kaggle.com/janiobachmann/s-p-500-time-series-forecasting-with-prophet
* https://towardsdatascience.com/time-series-analysis-in-python-an-introduction-70d5a5b1d52a

## REPOSITORY DETAILS
Access -
1. [Data](https://www.kaggle.com/camnugent/sandp500)
2. [Code](https://github.com/arnavd17/Stock-Prediction-using-Prophet/blob/master/Stock_Prediction_using_Prophet.ipynb)
