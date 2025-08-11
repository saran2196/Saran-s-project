Project Overview
This project analyzes the relationship between Bitcoin market sentiment and trader performance using two primary datasets:

Bitcoin Market Sentiment Dataset
Contains daily sentiment data labeled as Fear, Greed, or Neutral.

Historical Trader Data from Hyperliquid
Includes trade-level data such as account ID, coin symbol, execution price, trade size, side (buy/sell), timestamp, closed profit and loss (PnL), and more.

The objective is to uncover patterns and insights that reveal how market sentiment impacts trading outcomes, helping to inform smarter trading strategies.


Data Preparation
Loaded and cleaned both datasets.

Normalized column names and converted timestamps to datetime.

Merged the datasets on date fields to associate each trade with the corresponding market sentiment.

Key Analyses
Performance by Sentiment: Aggregate closed PnL and win rates analyzed by Fear, Greed, Neutral, etc.

Statistical Significance: Tested differences between Fear and Greed periods using Mann-Whitney U test.

Risk-Adjusted Metrics: Computed volatility and Sharpe-like metrics using winsorized PnL.

Trader Cohorts: Identified top traders per sentiment and analyzed consistency in win rates.

Leverage & Sizing: Analyzed average trade size and leverage behavior with correlation and binning approaches.

Time-Based Effects: Explored whether previous-day sentiment predicts current PnL and time-of-day effects.

Predictive Modeling: Built logistic regression models to predict trade success based on sentiment and trade features.

Interactive Visualizations: Created both static and interactive plots (Plotly) for clearer insights.

How to Run
Load the datasets:

historical_data.csv (trades data)

fear_greed_index.csv (sentiment data)

Run data preprocessing and merging scripts.

Execute analysis notebooks or scripts for visualizations and statistical tests.

Run predictive modeling scripts if needed.

Deliverables
Merged dataset file: merged_trades_with_sentiment.csv

Summary statistics and analysis outputs (CSV files)

Visualizations (static images and interactive HTML files)

Predictive model code and performance metrics
