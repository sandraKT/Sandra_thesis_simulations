# Sandra_thesis_simulations
In this implementation part of our master research, we present two trading algorithms to find optimal selling strategies to fill large execution orders.  The algorithms we propose are derived using discrete stochastic optimal control. The simulations in the notebooks are performed with historical financial market data.

Our working environment is Jupyter on Python and we provide FOUR files detailed as follows: 

FILE 1: Financial data
We import the three data in .csv format from the companies we will use to implement our algorithms. These are the 2017 intraday data of companies like google (GOOGIntradayOf5-23-2017.csv), Apple (AAPLIntradayOf10-12-2017.csv) and ExxonMobil (XOMIntradayOf9-7-2017.csv).

FILE 2 : This implementation represents the market indices of the Google company as captured by trading volume and stock price. we observe that the volume of transactions is not constant, it varies according to the set of financial operations carried out by the market players. The volumes represented here are those of the digital giant Google’s share price observed on 23 May 2017, we observe a first wave before noon, just before the lunch break and a second wave just after 1pm.

FILE 3 : Optimal VWAP Algorithm
This trading algorithm returns the recommended trading volume (sell) and stock price to optimise the overall VWAP (volume weighted average price) of the trade. The return and volatility are dynamically calibrated using finite differences in time series. The example we present shows how this algorithm can be implemented with Apple's historical intraday data for October 12, 2027.

FILE 4 : Minimal Shortfall
The main goal of this algorithm is to return a trading startegy that minimizes the overall execution shortfall at the end of the trade. This sort of strategies are extremely useful if you have a large position. Roughly speaking the execution shortfall is difference between the value of the large position before and after the trade. Given that the share price follows a random path, the algorithm will minimize the expected execution shortfall. The example we present shows how this algorithm can be implemented with ExxonMobil's historical intraday data for September 7, 2027.

These are the terms on which our implementations end.
