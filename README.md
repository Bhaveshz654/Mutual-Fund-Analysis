# Mutual Fund Analysis 

In this project, we conducted a comprehensive analysis of a Axis Small Cap mutual fund using historical NAV data over a three-year period. We computed key performance and risk metrics—including daily returns, 
cumulative returns, absolute returns, CAGR, Sharpe ratio, and Sortino ratio—to assess the fund's overall performance. These metrics were then benchmarked against a set of peer funds to evaluate relative performance on a risk-adjusted basis.

---

## Table of Contents

1. [Source of Data](#source-of-data)
2. [Main Libraries Used](#Main-Libraries-Used)
3. [Disclaimer](#Disclaimer)
4. [Pre-Processing](#pre-processing)
5. [Analysing Single Mutual Fund](#analysing-single-mutual-fund)
6. [Portfolio Analysis](#portfolio-analysis)
7. [Growth Analysis](#growth-analysis)
8. [Volatility Analysis](#volatility-analysis)
9. [Peer Comparison](#peer-comparison)

---

## Source of Data

The primary data source for this analysis is the NSE historical data, which provides detailed daily NAVs and other market information for mutual funds and indices.

---

## Main Libraries Used

- **Mftool:**  
  A Python library that retrieves mutual fund data directly from the AMFI API. It allows fetching historical NAV data and scheme details, which forms the backbone of our fund performance analysis.

- **Yfinance:**  
  A powerful library for downloading market data from Yahoo Finance. It is used to obtain indices and stock market information, making it easier to benchmark mutual fund performance against market indices.

- **Matplotlib:**  
  A widely-used plotting library in Python that provides flexible tools for creating static, animated, and interactive visualizations. In this project, it is used for generating comparative line charts and other performance visualizations.

- **Dash (Jupyter):**  
  An interactive web application framework built on top of Flask, Plotly, and React.js. The Jupyter integration allows for the creation of interactive dashboards directly within Jupyter Notebook, enabling dynamic filtering and visualization of the mutual fund performance data.

---

## Disclaimer

The analysis presented in this project is for educational and informational purposes only and should not be construed as investment advice. The data, calculations, and visualizations are based on historical information and are intended solely to illustrate various analytical techniques. Investors are encouraged to perform their own research and consult with professional financial advisors before making any investment decisions.

---

## Pre-Processing

The pre-processing section involves fetching and transforming raw data from multiple sources into a uniform format ready for analysis. This includes:
- Converting date columns to datetime objects.
- Sorting the data in chronological order.
- Filtering datasets to a consistent three-year period.
- Calculating key metrics such as daily returns and cumulative returns to normalize the data.

---

## Analysing Single Mutual Fund

In this section, we focus on a detailed analysis of a single mutual fund—Axis Small Cap Fund—using its historical NAV data. The process involves:
- Preparing the NAV data by converting dates and sorting chronologically.
- Computing key performance metrics like daily returns and cumulative returns.
- Building an interactive Jupyter Dash dashboard to allow users to filter and visualize the fund’s performance over various time periods (e.g., 1 month, 6 months, 1 year, etc.), providing valuable insights into its return dynamics and risk profile.

---

## Portfolio Analysis

This section examines the composition of the Axis Small Cap Mutual Fund's portfolio by analyzing its stock holdings and sector weightings. Using the fund’s ticker, data is retrieved on individual stock holdings and their distribution across various industry sectors. This analysis helps assess the fund’s diversification and understand any concentration risks present in its portfolio.

---

## Growth Analysis

Growth Analysis assesses the fund's performance by calculating its absolute returns and Compound Annual Growth Rate (CAGR) over different time horizons. These metrics provide a clear picture of the fund’s overall capital appreciation. Additionally, the fund’s growth is benchmarked against the NIFTY Smallcap 100 index, a key indicator of the small-cap market, to evaluate relative performance.

---

## Volatility Analysis

Volatility Analysis evaluates the risk profile of the Axis Small Cap Mutual Fund by measuring its volatility through metrics such as standard deviation and maximum drawdown. These metrics are then compared with those of the Nifty 50 (a safer, large-cap benchmark) and the Nifty Smallcap 100 (representing the small-cap market). This comparative analysis highlights the impact of active management on the fund’s risk relative to its benchmarks.

---

## Peer Comparison

In the peer comparison section, the performance of Axis Small Cap Mutual Fund is benchmarked against a set of peer funds. The analysis includes:
- Growth Analysis (using absolute returns and CAGR).
- Risk and Return Analysis (using Sharpe ratio and Sortino ratio).
**Sharpe Ratio:**
The Sharpe ratio measures the excess return of an investment (the return above a risk-free rate) relative to its total volatility. A higher Sharpe ratio indicates that the fund delivers better risk-adjusted returns.

**Sortino Ratio:**
The Sortino ratio is a variation of the Sharpe ratio that focuses solely on downside risk by considering only the negative deviations from the risk-free rate. This ratio provides a more accurate measure of an investment’s risk-adjusted performance when returns are skewed or when investors are particularly concerned with losses.

By comparing these metrics across funds, investors can identify which funds offer superior risk-adjusted returns and determine the overall efficiency of each fund's performance strategy.
