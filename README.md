# Transformer for time series forecasting

A neural network model for time series forecasting with a transformer encoder.

The model is applied to forecast a time series of daily currency exchange rates: euro (EUR) against US dollar (USD).

<p align="center">
  <img src="https://github.com/paulbuiqg/transformer_forecaster/blob/main/viz/timeseries.png" />
</p>

The model inputs the last 64 daily values of the time series and outputs the predicted value for the next day. It is composed of a transformer sequence encoder and a linear layer, and has ~3.6M parameters.

The (L1) loss converges quite fast.

<p align="center">
  <img src="https://github.com/paulbuiqg/transformer_forecaster/blob/main/viz/training.png" />
</p>

The predictions match well the actual values in terms of variation. But it is biased: the model systematically underestimates the ground truth.

<p align="center">
  <img src="https://github.com/paulbuiqg/transformer_forecaster/blob/main/viz/prediction.png" />
</p>

For a better assessment, the model should be updated daily by adding the last observation to the training data.
