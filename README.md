# Predicting-stock-prices
Predicting stock prices with a Recurrent Neural Network (RNN) with a Long Short-Term Memory (LSTM)
Berlin AirBnB Analysis

Libaries

Phyton 3.6.5

Numpy 1.12.1

Pandas 0.23.1

Matplotlib 2.2.2

Required data

Historic stock market data for has to been downloaded (e.g. from Yahoo Finance) and stored into csv file.

Motivation

Based on historic data, predictions for the future adjusted closing price of the Standard & Poor's 500 (S&P 500) stock market index will be made. The stock price predictor should solve a classical time series prediction problem. To learn the sequential patterns in the data and under consideration of long-term dependencies of the data points, a Recurrent Neural Network (RNN) with a Long Short-Term Memory should be used. The solution should be
The solution of the problem follow this steps:
1. Gathering and exploration of the stock price data
2. Preparation of data for training and testing
3. Creation of a benchmark model (linear regression) to evaluate the solution
4. Design of the architecture of the LSTM-network in Keras with a Tensorflow backend
5. Training and fitting of the network with training data
6. Prediction of stock prices and evaluating the model with test data
7. Improvement of the model and tuning of parameters
8. Visualization and discussion of results
The final solution of the stock price predictor should make predictions for the adjusted stock price of the S&P 500 for multiple days in the future (e.g. 50 days) using a sequence of past stock prices.?

Files

Capstone_final.ipynb: Jupiter Notebook with analysis

Capstone Proposal: Project Report

Summary

I started to downloading the Data for the S&P500 and exploring it. It was interesting to see the characteristics of the data, especially how noisy the stock market data is, what make predictions so difficult.
 
The challenges of the preprocessing step were to bring the data in the right 3D-shape for the LSTM algorithm and generating sequences of multiple time steps for each data point. Normalization and smoothing of the data was also conducted.
The most time I spent with the configuration of the LSTM-network and the tuning of the parameters. I was surprised by the big impact of the batch size and the length of sequences of time steps feed into the network on the prediction performance.
The performance of the one day ahead predictions exceeded my prior expectations, but I think the use of these for real stock investment decisions is limited, because the changes of stock prices between two days are usually not so big.
To find an algorithm to predict and visualize multiday ahead predictions was a quite laborious task. But the reliability of the predictions is limited, I would not put my money on these. But it is a good demonstration of the challenges to predict the stock market. And it could be a starting point to develop a predictor, which combines different methods of prediction and different sources of input data.

Acknowledgements

http://udacity.com

