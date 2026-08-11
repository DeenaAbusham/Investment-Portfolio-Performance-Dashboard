Investment Portfolio Performance Dashboard

Overview

An interactive Power BI investment portfolio analytics project designed to evaluate the performance, allocation and risk characteristics of a simulated multi-sector equity portfolio.

Objectives:

- Monitor portfolio value over time.
- Calculate current portfolio value and unrealised profit/loss.
- Analyse holding-level returns and portfolio concentration.
- Evaluate sector allocation and diversification.
- Measure annualised portfolio volatility.
- Calculate risk-adjusted performance using the Sharpe Ratio.
- Present investment insights through an interactive Power BI dashboard.

Tools & Technologies:

- Power BI Desktop
- DAX
- Power Query
- Excel / CSV
- Historical equity market data
- Star-schema data modelling

Portfolio:

The simulated portfolio contains 10 publicly traded companies: 
Apple, Amazon, Microsoft, Nvidia, Tesla, Visa, JPMorgan Chase, Coca-Cola, Exxon Mobil and Pfizer.

Data Model

*Fact_StockPrices

Historical market data:

- Date
- Ticker
- Open
- High
- Low
- Close
- Volume

*Fact_Holdings

Portfolio holdings:

- Company
- Ticker
- Shares
- Purchase Price

*Dim_Companies

Reference data:

- Company
- Ticker
- Sector

*Dim_Date

Calendar dimension used for time-series analysis and date filtering.

Key DAX Measures:

- Current Portfolio Value
- Total Investment
- Portfolio Profit
- Portfolio Return %
- Portfolio Value Over Time
- Portfolio Daily Return
- Annualised Return
- Annualised Volatility
- Sharpe Ratio

Portfolio value is calculated dynamically from shares held and the latest available closing price for each holding. 
Daily returns are used to calculate annualised volatility using 252 trading days.

The Sharpe Ratio uses an assumed 4% annual risk-free rate.

Dashboard Pages:

1. Investment Portfolio Performance

- Current Portfolio Value
- Total Investment
- Portfolio Profit
- Portfolio Return %
- Portfolio Value Over Time
- Sector Allocation
- Holding Returns
- Portfolio Value by Holding

2. Risk & Performance Analysis

- Annualised Volatility
- Annualised Return
- Sharpe Ratio
- Daily Portfolio Returns
- Methodology and assumptions

Key Portfolio Results

- Current Portfolio Value: £64.12K
- Total Investment: £56.76K
- Portfolio Profit: £7.36K
- Portfolio Return: 12.97%
- Annualised Volatility: 14.32%
- Annualised Return: 16.60%
- Sharpe Ratio: 0.88

Investment Insights

- The simulated portfolio generated a positive overall return of 12.97%.
- Portfolio value increased from approximately £33K at the beginning of the historical period to approximately £64K at the latest date.
- Technology represents the largest sector allocation, creating meaningful concentration exposure.
- Individual holding performance varies significantly, with Tesla showing the strongest return and Nvidia the weakest return in the simulated portfolio.
- Annualised volatility of 14.32% provides a measure of portfolio return variability.
- A Sharpe Ratio of 0.88 indicates positive risk-adjusted performance under the stated assumptions.

Assumptions & Limitations

- The portfolio is simulated and does not represent personal investment activity.
- Purchase prices and share quantities are project assumptions.
- The Sharpe Ratio uses an assumed 4% annual risk-free rate.
- Volatility is annualised using 252 trading days.
- The analysis does not currently include transaction costs, dividends, taxes or corporate actions.
- Historical performance does not guarantee future performance.

Potential Enhancements

- Benchmark comparison against the S&P 500.
- Beta and alpha analysis.
- Maximum drawdown.
- Value at Risk (VaR).
- Rolling volatility.
- Dividend-adjusted returns.
- Portfolio rebalancing analysis.
- Automated data refresh.

Author

Deena Ali

Focus: Power BI | DAX | Investment Analytics | Portfolio Performance | Risk Analysis
