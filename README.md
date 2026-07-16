# FX & Rates Macro Statistical Arbitrage

> Status: Work in progress

This project aims to build a quantitative research framework for macro-driven foreign exchange strategies using interest rate differentials, momentum, volatility regimes and statistical analysis.

The objective is to study whether simple and interpretable macro signals can help explain or generate systematic trading signals across major currency pairs.

## Project Overview

Foreign exchange markets are strongly influenced by macroeconomic variables such as interest rates, inflation expectations, monetary policy and global risk appetite.

This project focuses on the relationship between FX markets and interest rates. The idea is to analyze whether variables such as rate differentials, FX momentum and volatility regimes can be used to construct simple long/short signals.

The purpose is not to build a production-ready trading strategy, but to develop a clean and disciplined quantitative research process.

## Objectives

The project focuses on:

- collecting FX and interest rate time series;
- cleaning and aligning macro-financial data;
- computing FX returns and interest rate differentials;
- building momentum and carry-inspired signals;
- analyzing rolling correlations and volatility regimes;
- testing stationarity and possible cointegration relationships;
- backtesting simple long/short FX strategies;
- including transaction costs;
- evaluating risk-adjusted performance;
- analyzing robustness and limitations.

## Motivation

FX and rates are central markets for macro trading and systematic strategies.

A quantitative approach can help study:

- the role of interest rate differentials in currency movements;
- momentum effects in FX markets;
- changes in relationships across market regimes;
- the stability of macro signals;
- the risk-adjusted performance of simple systematic strategies.

This project is designed to connect macroeconomic intuition, statistical analysis and practical backtesting.

## Planned Repository Structure

```text
notebooks/
  01_fx_rates_data_exploration.ipynb
  02_macro_signal_construction.ipynb
  03_strategy_backtest.ipynb

src/
  data.py
  features.py
  signals.py
  backtest.py
  risk_metrics.py

references/
  README.md

README.md
```

## Research Questions

The project will be guided by the following questions:

- Do interest rate differentials help explain FX movements?
- Are FX momentum signals stable across different market regimes?
- Can volatility regimes improve risk management?
- Are some FX pairs more sensitive to rate differentials than others?
- Can simple macro signals generate robust long/short strategies?
- How much do transaction costs affect the results?
- What are the limitations of a simplified macro statistical arbitrage framework?

## Roadmap

### Step 1 — Data Collection

- Collect FX time series such as EUR/USD, GBP/USD, EUR/GBP and USD/JPY.
- Collect interest rate series for the US, euro area and UK.
- Align data frequencies.
- Handle missing values.
- Convert all series into a consistent format.

### Step 2 — Data Exploration

- Plot FX levels and returns.
- Plot interest rate series.
- Analyze rate differentials.
- Compute descriptive statistics.
- Identify major market regimes and stress periods.

### Step 3 — Feature Engineering

- Compute FX log returns.
- Compute interest rate differentials.
- Compute momentum signals over different horizons.
- Compute rolling volatility.
- Compute rolling correlations.
- Build carry-inspired indicators.

### Step 4 — Statistical Analysis

- Study the relationship between FX returns and rate differentials.
- Run simple regressions.
- Test stationarity of selected spreads.
- Explore possible cointegration relationships where relevant.
- Analyze the stability of signals over time.

### Step 5 — Signal Construction

- Build simple long/short FX signals.
- Combine macro indicators with momentum features.
- Add volatility filters.
- Avoid excessive model complexity.
- Keep the signals interpretable.

### Step 6 — Backtesting Framework

- Backtest simple FX strategies.
- Include transaction costs.
- Avoid look-ahead bias.
- Compute daily or weekly PnL.
- Track positions and turnover.
- Add volatility targeting.

### Step 7 — Risk and Performance Analysis

- Compute cumulative returns.
- Compute annualized return and volatility.
- Compute Sharpe ratio.
- Compute maximum drawdown.
- Compute hit ratio.
- Analyze performance by market regime.

### Step 8 — Robustness and Limitations

- Discuss regime instability.
- Analyze sensitivity to transaction costs.
- Study the risk of overfitting.
- Discuss the limits of simple macro signals.
- Propose possible improvements.

## References

- Academic literature on currency carry and FX momentum.
- Moskowitz, Ooi and Pedersen, *Time Series Momentum*.
- Research on statistical arbitrage and pairs trading.
- Research on cointegration and macro-financial time series.

## Tech Stack

- Python
- pandas
- NumPy
- scipy
- statsmodels
- matplotlib
- scikit-learn
- Time series analysis
- Statistical testing
- Backtesting
- Risk metrics

## Current Status

The project is currently in progress.

The first development phase focuses on reviewing FX and rates market basics, collecting clean macro-financial data and building exploratory analysis tools before implementing trading signals and backtests.

## Disclaimer

This project is for academic and educational purposes only. It does not constitute financial advice or a production-ready trading strategy.
