# Unit-14-LSTM-Stock-Predictor

In this assignment, we used deep learning recurrent neural networks to model bitcoin closing prices. One of the models used the FNG indicators to predict the closing price while the second model used a window of closing prices to predict the nth closing price.

We were required to:

1. Prepare the data for training and testing
2. Build and train custom LSTM RNNs
3. Evaluate the performance of each model

To prepare the data for training and testing purpose:

1. We used the FNG values to try and predict the closing price for the Fear and Greed model.
2. And for the closing price model, we used previous closing prices to try and predict the next closing price.

For the next step we created the same custom LSTM RNN architecture. In one notebook, we fit the data using the FNG values. In the second notebook, we fit the data using only closing prices.

For the purposes of evaluation, we used the testing data to evaluate each model and compare the performance on the following basis:

1. Which model has a lower loss? _The closing price model had the lower loss at 0.0443 compared to the FNG model's loss of 0.1591_
2. Which model tracks the actual values better over time? _The closing price model tracks the actual values better over time_
3. Which window size works best for the model? _Based on test runs, a smaller window size between 2 - 3 works better for the model_
