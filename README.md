# 01_-Pair_Trading
This project implements a simple pairs trading strategy using two highly correlated stocks (e.g., GOOGL and MSFT). It uses z-score-based signals to identify long/short entry points and evaluates performance with a backtested equity curve.

#About me 
After developing an interest into financial python, I thought I'd make this my first project and showcase my interest to the wider community. This project was very fun and challenging and to those who view the code, feel free to give me some advice!


##Pairs Trading Strategy Backtest

This project implements a simple mean reversion strategy using z-score signals between two correlated assets, in my example such Google and Microsoft. It includes full backtesting logic and a visualization of cumulative returns to evaluate performance. As mentioned in the code, due to invalid cointegration in the middle sector, my graph went flat, so hopefully with your stocks etc., it performs better.

---

##Strategy Overview

- **Long Entry**: z-score < -0.8  
  → Buy GOOGL, short MSFT
- **Short Entry**: z-score > 0.8  
  → Short GOOGL, buy MSFT
- **Exit Trade**: |z-score| < 0.05  
  → Close all positions

The assumption is that the spread between two cointegrated assets will revert to the mean, and profits can be made from that convergence.

---

## Features

- ✅ Z-score based trading signal logic  
- ✅ Dynamic long/short position allocation  
- ✅ Backtesting with cumulative equity curve  
- ✅ Visual performance plotting  
- ✅ Extendable to SPY 500 tickers

---

