# Transformer for time series forecasting

A neural network model for time series forecasting with a transformer encoder.

The model is applied to forecast a bivariate timeseries of daily currency exchange rates: euro (EUR) against US dollar (USD), and sterling pound (GBP) against US dollar.

<p align="center">
  <img src="https://github.com/paulbuiqg/transformer4timeseries/blob/main/viz/EUR.png" />
</p>

<p align="center">
  <img src="https://github.com/paulbuiqg/transformer4timeseries/blob/main/viz/GBP.png" />
</p>

The model inputs the last 128 daily values of the two univariate timeseries (EUR/USD and GBP/USD), and outputs the values for EUR/USD and GBP/USD for the next day.

[Work in progress...]
