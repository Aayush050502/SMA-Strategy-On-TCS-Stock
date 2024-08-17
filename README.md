
Moving Average Trading Strategy on TCS Stock
Introduction
This repository presents the development and testing of a simple moving average (SMA) trading strategy applied to TCS stock data. The objective is to determine buy and sell signals based on SMA crossover patterns to optimize returns on an initial investment of ₹1,00,000. This document details the process from gathering stock data to backtesting the strategy, evaluating its performance, and suggesting improvements.

Data Acquisition
Historical stock data for TCS from August 2022 to August 2024 was sourced using Python's yfinance library. The dataset includes daily stock prices such as opening, high, low, and closing prices, as well as volume traded. The TCS stock data was retrieved using the ticker symbol ("TCS.NS") from the National Stock Exchange (NSE) via the yfinance API, ensuring data credibility and accuracy.

Moving Average Trading Strategy
The core of the strategy involves two types of SMAs:

Short-Term SMA (20 days): Calculates the average closing price over the past 20 days, reflecting short-term price trends.
Long-Term SMA (50 days): Calculates the average closing price over the past 50 days, representing long-term trends.
Trading Signals:

Buy Signal: Generated when the short-term SMA crosses above the long-term SMA, indicating an upward trend.
Sell Signal: Triggered when the short-term SMA crosses below the long-term SMA, signaling a downward trend.
Backtesting
Backtesting was performed using the historical TCS stock data with an initial capital of ₹1,00,000. The following metrics were tracked:

Total Return: Final return on investment at the end of the period.
Number of Trades: Total number of buy and sell signals acted upon.
Winning and Losing Trades: Percentage of trades resulting in gains or losses.
Maximum Drawdown: Largest decline from the peak value of the portfolio.
Strategy Performance
Performance Metrics:

Initial Capital: ₹1,00,000
Final Portfolio Value: ₹2,00,639.60
Total Returns: ₹1,00,639.60
Total Trades: 11.0 trades
Winning Trades: 1272.73% of trades were profitable.
Losing Trades: -1172.73%% of trades resulted in losses.
Maximum Drawdown: 53.80% peak-to-trough decline in portfolio value.
A graph illustrating price movements, buy and sell signals, and SMAs is available in the repository.

Observations and Conclusion
The moving average strategy demonstrated potential for profitable trades by capturing momentum shifts. However, performance fluctuated based on market conditions, with some losing trades during periods of consolidation or "whipsaw" movements. The maximum drawdown indicates potential significant losses during prolonged downturns. Risk management techniques such as stop-loss orders could mitigate these risks.

Potential Enhancements
To improve the strategy, consider the following enhancements:

Risk Management: Incorporate stop-loss orders to limit downside risk.
Additional Indicators: Combine SMAs with indicators like the Relative Strength Index (RSI) or Moving Average Convergence Divergence (MACD) to filter out false signals.
Position Sizing: Adjust trade sizes based on the strength of signals to improve returns and manage risk effectively.
Conclusion
This report demonstrates the implementation and backtesting of a simple moving average strategy on TCS stock data. While the strategy showed positive returns under certain conditions, it faced challenges in volatile periods. Future refinements, including additional indicators and risk management protocols, could enhance the strategy's robustness and profitability.

