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

The analysis compares four portfolio allocation strategies
based on historical return, volatility and risk-adjusted performance.

| Strategy | Annualized Return (%) | Volatility (%) | Sharpe Ratio | Maximum Drawdown (%) | VaR 95% (%) | CVaR 95% (%) |
|---|---:|---:|---:|---:|---:|---:|
| Equal Weight | 16.09 | 18.13 | 0.78 | -30.89 | -1.73 | -2.46 |
| Minimum Volatility | 8.32 | 13.14 | 0.48 | -23.80 | -1.32 | -1.89 |
| Maximum Sharpe | 23.14 | 20.11 | 1.05 | -36.36 | -1.96 | -2.81 |
| Constrained Maximum Sharpe | 19.66 | 18.94 | 0.93 | -33.75 | -1.85 | -2.56 |

### Key Observations

- The Minimum Volatility strategy exhibits the lowest historical volatility and maximum drawdown.
- The Maximum Sharpe strategy achieves the highest historical Sharpe ratio.
- The Constrained Maximum Sharpe strategy incorporates position limits to improve diversification.
- The results highlight the trade-off between return potential, portfolio risk and diversification.
