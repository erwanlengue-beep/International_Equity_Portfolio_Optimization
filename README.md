# International Equity Portfolio Optimization

## Overview

This project develops an international equity portfolio analysis and optimization framework using Python.

The objective is to evaluate individual stocks, measure portfolio risk and performance, and compare different asset-allocation strategies using quantitative portfolio-management techniques.

The project is designed as an educational application of concepts relevant to **Asset Management, Portfolio Management, and Financial Markets**.

## Investment Universe

The portfolio includes seven listed companies across different countries and sectors:

| Company | Country | Sector | Ticker |
|---|---|---|---|
| LVMH | France | Luxury Goods | `MC.PA` |
| ASML | Netherlands | Semiconductors | `ASML` |
| Microsoft | United States | Technology | `MSFT` |
| JPMorgan Chase | United States | Banking | `JPM` |
| Toyota | Japan | Automotive | `TM` |
| Nestlé | Switzerland | Consumer Staples | `NESN.SW` |
| SAP | Germany | Enterprise Software | `SAP` |

## Methodology

The analysis is based on historical adjusted price data retrieved through Yahoo Finance using `yfinance`.

Main steps:

1. Data collection and preparation
2. Calculation of daily returns
3. Individual stock performance and volatility analysis
4. Correlation and covariance analysis
5. Equal-weight portfolio construction
6. Minimum-volatility portfolio optimization
7. Maximum-Sharpe-ratio portfolio optimization
8. Efficient frontier construction
9. Portfolio optimization with a 25% maximum allocation constraint
10. Risk analysis using:
   - Maximum drawdown
   - Historical Value at Risk (VaR)
   - Historical Conditional Value at Risk (CVaR)

A simplified **2% risk-free rate** is used for Sharpe ratio calculations.

## Portfolio Strategies

The project compares the following allocation approaches:

- Equal-weight portfolio
- Minimum-volatility portfolio
- Maximum-Sharpe-ratio portfolio
- Constrained maximum-Sharpe-ratio portfolio

The constrained strategy applies a maximum allocation of 25% per asset to reduce concentration.

## Technologies and Libraries

- Python
- pandas
- NumPy
- yfinance
- Matplotlib
- SciPy

## Project Structure

```text
International_Equity_Portfolio_Optimization/
│
├── International_Equity_Portfolio_Optimization_Junior_L.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── images/
```

## Key Learning Outcomes

This project helped develop practical skills in:

- Quantitative portfolio analysis
- Asset allocation
- Portfolio optimization
- Risk measurement
- Financial data analysis
- Python programming for finance
- Interpretation of portfolio performance indicators

## Limitations

The results should be interpreted as an educational quantitative analysis rather than investment advice.

Key limitations include:

- Historical data does not guarantee future performance.
- The optimization uses historical estimates of returns and risk.
- The risk-free rate is simplified and does not reflect every currency in the investment universe.
- Currency movements and foreign-exchange hedging are not modeled separately.
- Transaction costs, taxes, liquidity constraints, and market impact are not included.
- The optimization is based on historical data and does not represent an out-of-sample backtest.

## Disclaimer

This project is for educational and portfolio-analysis purposes only. It does not constitute financial advice or a recommendation to buy or sell any security.
