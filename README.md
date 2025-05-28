# Adaptive Factor Alpha – A Machine Learning Driven Quant Equity Strategy

This project implements a dynamic long/short equity trading strategy that uses multi-factor modeling enhanced with machine learning to predict future stock returns. The strategy constructs a portfolio based on factor exposures like momentum, value, and volatility, and allocates capital by ranking predictions from a Gradient Boosting Regressor.

## Features
* Factor construction for:

    * Momentum (3-month price return)

    * Value (inverse of price)

    * Volatility (20-day standard deviation)

* NForward return prediction using scikit-learn machine learning models

* Dynamic long-short portfolio construction based on predicted ranks

* Backtesting and performance evaluation

* Simple and extendable codebase


## Technologies Used
* Python 3

* ```pandas```, ```numpy``` for data manipulation

* ```yfinance``` for historical stock price data

* ```scikit-learn``` for model training

* ```matplotlib``` for performance visualization


## Results
The strategy ranks stocks based on predicted 1-month returns and creates an equal-weighted portfolio:

Long top N stocks, Short bottom N stocks

Monthly rebalancing

Backtest performance visualized via cumulative returns
