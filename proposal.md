# Machine Learning Engineer Nanodegree
## Capstone Proposal
Marcos Wada  
June 24th, 2020

## Proposal

### Bitcoin
Bitcoin is a decentralized digital currency without a central bank or single administrator that can be sent from user to user on the peer-to-peer bitcoin network without the need for intermediaries.
Transactions are verified by network nodes through cryptography and recorded in a public distributed ledger called a blockchain. Bitcoin was invented in 2008 by an unknown person or group of people using the name Satoshi Nakamoto and started in 2009 when its source code was released as open-source software. Bitcoins are created as a reward for a process known as mining. They can be exchanged for other currencies, products, and services.

### Bitcoin Price Forecasting
The goal of this project is to create a model that forecast bitcoin time series, predicting a sequence of prices that will happen at specific times using deep learning approaches.
I'll use dataset from two bitcoin exchanges for the time period of Jan 2012 to April 2020, with minute to minute updates of OHLC (Open, High, Low, Close), Volume in BTC and indicated currency, and weighted bitcoin price. (https://www.kaggle.com/mczielinski/bitcoin-historical-data)

### Implementation
I'll try to implement Long short-term memory (LSTM) network, an artificial recurrent neural network (RNN) architecture used in the field of deep learning. 
After developing the model, I'll benchmark performance with DeepAR, a built-in time series forecasting method based on RNN provided by Samemaker.
Finally, I'll provide an service endpoint using Sagemaker, Lambda and API Gateway that predict if you should buy or sell bitcoin.