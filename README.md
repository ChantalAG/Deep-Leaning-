# Deep-Leaning:
# LSTM Stock Predictor

![image](https://user-images.githubusercontent.com/99493522/172638704-2de716b6-c7b0-48f6-8659-c657d37f6fc4.png)

## Background

Due to the volatility of cryptocurrency speculation, investors will often try to incorporate sentiment from social media and news articles to help guide their trading strategies. One such indicator is the Crypto Fear and Greed Index (FNG) which attempts to use a variety of data sources to produce a daily FNG value for cryptocurrency. 

This project will build and evaluate deep learning models using both the FNG values and simple closing prices to determine if the FNG indicator provides a better signal for cryptocurrencies than the normal closing price data.
Deep learning recurrent neural networks will be used to model bitcoin closing prices. One model will use the FNG indicators to predict the closing price while the second model will use a window of closing prices to predict the nth closing price.

## Files

[LSTM Stock Predictor Using Fear and Greed Index:](https://github.com/ChantalAG/Deep-Leaning-/blob/main/lstm_stock_predictor_fng.ipynb)
In this notebook, a custom LSTM RNN was built and trained that uses a 10 day window of Bitcoin fear and greed index values to predict the 11th day closing price.

[LSTM Stock Predictor Using Closing Prices:](https://github.com/ChantalAG/Deep-Leaning-/blob/main/lstm_stock_predictor_closing.ipynb)
In this notebook, a custom LSTM RNN was built and trained that uses a 10 day window of Bitcoin closing prices to predict the 11th day closing price.



## Instructions
### Prepare the data for training and testing
* Each model will use 70% of the data for training and 30% of the data for testing.
* MinMaxScaler was applied to the X and y values to scale the data for the model.
* The X_train and X_test values were reshaped to fit the model's requirement of samples, time steps, and features. 
    

### Build and train custom LSTM RNNs
The same parameters and training steps were used for each model.
* epochs = 20
* batch size = 1
* dropout_fraction = 0.2
* number_units = 30

### Evaluate the performance of each model
* The testing data was used to evaluate each model and compare the performance.
* The first graph shows the prediction using the FNG index and the second graph uses the closing price. 

![image](https://user-images.githubusercontent.com/99493522/172665230-59146cb4-a08e-410d-91fe-366acf63af82.png)
![image](https://user-images.githubusercontent.com/99493522/172665067-3abacb6a-1fb1-4b7d-8008-43fc1e5114ec.png)



## Findings
#### Which model has a lower loss?

#### Which model tracks the actual values better over time?
#### Which window size works best for the model?

## Contributors
Chantal Garnett
