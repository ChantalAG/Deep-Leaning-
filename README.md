# Deep-Leaning:
# LSTM Stock Predictor

![image](https://user-images.githubusercontent.com/99493522/172638704-2de716b6-c7b0-48f6-8659-c657d37f6fc4.png)

## Background

Due to the volatility of cryptocurrency speculation, investors will often try to incorporate sentiment from social media and news articles to help guide their trading strategies. One such indicator is the Crypto Fear and Greed Index (FNG) which attempts to use a variety of data sources to produce a daily FNG value for cryptocurrency. 

This project will build and evaluate deep learning models using both the FNG values and simple closing prices to determine if the FNG indicator provides a better signal for cryptocurrencies than the normal closing price data.
Deep learning recurrent neural networks will be used to model bitcoin closing prices. One model will use the FNG indicators to predict the closing price while the second model will use a window of closing prices to predict the nth closing price.

## Files

LSTM Stock Predictor Using Fear and Greed Index:

In this notebook, a custom LSTM RNN was built and trained that uses a 10 day window of Bitcoin fear and greed index values to predict the 11th day closing price.

LSTM Stock Predictor Using Closing Prices:

In this notebook, a custom LSTM RNN was built and trained that uses a 10 day window of Bitcoin closing prices to predict the 11th day closing price.



## Instructions
### Prepare the data for training and testing
* Each model will use 70% of the data for training and 30% of the data for testing.
* MinMaxScaler was applied to the X and y values to scale the data for the model.
* Reshape the X_train and X_test values to fit the model's requirement of samples, time steps, and features. (example: X_train = X_train.reshape((X_train.shape[0], X_train.shape[1], 1)))

### Build and train custom LSTM RNNs
* The same parameters and training steps were used for each model.

### Evaluate the performance of each model
* The testing data was used to evaluate each model and compare the performance.

## Findings
Which model has a lower loss?
Which model tracks the actual values better over time?
Which window size works best for the model?

## Contributors
Chantal Garnett
