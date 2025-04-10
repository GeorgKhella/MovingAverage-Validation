# Moving Average Crossover Strategy – Statistical Validation

**Author:** Georg Khella  
**Year:** 2025

## 📈 Overview

This project rigorously evaluates a **moving average crossover trading strategy**, assessing its profitability and robustness across different market regimes.  
Key focus areas include:
- Sharpe ratio analysis
- Cross-validation to mitigate data snooping bias
- Evaluation during **COVID-19 Crash Recovery** and **Quantitative Easing Bull Market**

## 🧠 Methodology

- Define short-term and long-term moving averages:
  - Buy signal: Short MA > Long MA
  - Sell signal: Short MA < Long MA
- Compute portfolio returns and **Sharpe ratio**
- Apply **rolling cross-validation** for parameter tuning (short/long window)
- Test strategy across SPY and QQQ ETFs

## 📊 Results Summary

| Market Regime                 | Asset | Total Return | Sharpe Ratio |
|------------------------------|-------|--------------|--------------|
| COVID-19 Crash Recovery      | SPY   | 59.99%       | 1.98         |
|                              | QQQ   | 65.36%       | 1.53         |
| Quantitative Easing Bull Run | SPY   | 79.46%       | 0.78         |
|                              | QQQ   | 140.94%      | 0.93         |

- Strategy performed well across **bull and bear** conditions
- **Cross-validation** improved generalization and reduced overfitting
- **Transaction costs not included** – results are optimistic

## 🔍 Future Improvements

- Include **trading commissions** and **borrowing costs**
- Test **Superior Predictive Ability (SPA)** for model comparison
- Apply strategy to **cryptocurrencies** and other asset classes

## 📁 Files

- `Moving_Average_Crossover_Strategy.pdf`: Full report with strategy formulation, performance charts, and market regime testing

## 📚 References

- White (2000). *A Reality Check for Data Snooping*, Econometrica  
- Hansen (2005). *A Test for Superior Predictive Ability*, JBES
