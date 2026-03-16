# Energy Sector Ichimoku Strategy Backtest

This project evaluates an Ichimoku Cloud trading strategy applied to major US energy stocks and compares its performance against standard benchmarks, inspired by https://www.quantconnect.com/research/9031/ichimoku-clouds-in-the-energy-sector/p1

## Assets

The strategy is tested on ten large U.S. energy companies:

- Exxon Mobil (XOM)
- Chevron (CVX)
- ConocoPhillips (COP)
- EOG Resources (EOG)
- Schlumberger (SLB)
- Phillips 66 (PSX)
- Valero Energy (VLO)
- Marathon Petroleum (MPC)
- Kinder Morgan (KMI)
- Williams Companies (WMB)

## Benchmarks

Two benchmarks are used for comparison:

1. **XLE ETF** — Energy Select Sector SPDR Fund  
2. **Equal-weight portfolio** of the ten energy stocks

## Strategy

The strategy uses **Ichimoku Cloud indicators** to generate trading signals based on the relationship between price and the **Chikou Span**.

Signals are shifted forward to avoid **look-ahead bias** in the backtest.

## Data

Market data is downloaded from **Yahoo Finance** using the `yfinance` Python library.

Backtest period:
2015 – Present

## Performance Metrics

The strategy is evaluated using standard portfolio metrics:

- Total Return
- Annualized Return
- Annualized Volatility
- Sharpe Ratio
- Maximum Drawdown

## Technologies

- Python
- pandas
- numpy
- matplotlib
- yfinance
- Jupyter Notebook

## File
ichimoku_energy_backtest.ipynb contains the full data pipeline, indicator computation, and backtesting framework.

---

## Disclaimer

This project is for research and educational purposes only and does not constitute financial advice.

