# MF821-high-freq-trading

# High-Frequency Statistical Arbitrage using ETF Pairs

This project implements a statistical arbitrage strategy by identifying and exploiting price inefficiencies between highly correlated ETF pairs. Using historical price data and statistical techniques such as Kendall's Tau and Sum of Squared Differences (SSD), the model identifies candidate pairs and simulates a simple high-frequency trading strategy based on their divergence and convergence behavior.

## Overview

We analyze 30+ ETFs across various sectors (Technology, Health Care, Financial Services, Energy) and evaluate their daily returns to compute statistical distances. The top-scoring pairs are selected for further signal generation and performance evaluation.

## Techniques Used

- **Data Cleaning and Transformation**:
  - Daily adjusted close, high, and low prices
  - Log-based daily range computation
- **Pair Selection Metrics**:
  - **Sum of Squared Differences (SSD)**: Measures co-movement similarity
  - **Kendall Tau Correlation**: Captures monotonic relationships
- **Monthly Aggregation**:
  - Resampling daily returns to monthly for robustness testing
- *(Further sections likely include trading signal generation and backtesting – to be added if available)*

## Key Components

- `Team6_Trade_Final.ipynb`: Main notebook containing all processing, metric computation, and pair analysis logic
- Data includes ETF prices such as SPY, QQQ, XLK, XLF, etc., categorized by sector
