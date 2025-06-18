##About me 
Hello github, after developing an interest into financial python, I thought it was time to make a project. With a background in finance, I found it enjoyeable to contrast my knowledge and interest in finance to challenge myself to try and build something in python, something I haven't done before. Please feel free to drop improvements to my code, it'd be great to hear feedback.

##Description

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

