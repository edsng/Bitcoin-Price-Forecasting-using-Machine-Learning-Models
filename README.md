# Bitcoin-Price-Forecasting-using-Machine-Learning-Models
Bitcoin Price Forecasting using k-Nearest Neighbors and Long Short Term Memory

## Purpose
My father and I have been interested in the crypto markets since the start of the crypto boom. I was interested in seeing if we could run a model on the historic Bitcoin price data in order to predict future price trends. The models I will be testing are the k-Nearest Neighbors and Long Short Term Memory Models.

## Data Preparation
Most of the data obtained from yahoo finance were clean with no nan values. Therefore the most we had to do was account for potential invalid data when feature engineering or lagging.

## Feature Engineering
We used a variety of features but most prominently our Tenchical Analysis features. We implemented TA indicators such as SMA, EMA, RSI, MACD, Stochastic Oscillator, and Bollinger Bands which were lagged to prevent future bias. While we have created a large amount of extra features, we make sure to limit our use through feature selection later on.

## k-Nearest Neighbors
![image](https://github.com/user-attachments/assets/31beade9-a334-4929-9e03-7d6bbbe1e3b5)
Root Mean Squared Error (RMSE): An RMSE of $3430 indicate that, on average, accounting for squared differences, the model's predictions are off by $3430.

Percent Error: A percent error of 6.73% indicates that, on average, the model's predictions are off by 6.73%.

r2: An r2 value of 95.93% indicates that this model captures 95.93% of the variability in BTC prices. This suggests that the model fits the data well.

Mean Absolute Error (MAE): A Mean Absolute Error of $2538.27 indicate that, on averaeg, the model's predictions are off by $2538.27. We did not implement cross-validation since our data is a time-series using lagged features requiring it to use other methods of cross-validation.

## Long Short Terrm Memory
