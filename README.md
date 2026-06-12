
# primetrade.ai
# Bitcoin Market Sentiment vs Trader Performance Analysis

## Overview

This project analyzes the relationship between Bitcoin market sentiment and trader performance using the Fear & Greed Index and Hyperliquid historical trading data.

The objective is to understand how market sentiment influences profitability, win rates, trading activity, trade sizing, and trader behavior, and to derive insights that can support smarter trading strategies.

---

## Dataset Information

### 1. Historical Trader Data

* Total Records: 211,224
* Features:

  * Account
  * Coin
  * Execution Price
  * Size USD
  * Direction
  * Closed PnL
  * Fee
  * Timestamp
  * Transaction Information

### 2. Bitcoin Fear & Greed Index

* Total Records: 2,644
* Features:

  * Sentiment Classification
  * Sentiment Score
  * Date

---

## Project Workflow

### Data Preprocessing

* Loaded trading and sentiment datasets using Pandas.
* Checked for missing values.
* Converted timestamps into datetime format.
* Created common date fields for integration.

### Data Integration

* Merged trader data with sentiment data using trading date.

### Feature Engineering

* Profitability Indicator
* Trade Size Metrics
* Sentiment-Based Grouping

### Exploratory Data Analysis

* Average PnL by Sentiment
* Win Rate Analysis
* Trade Activity Analysis
* Trade Size Analysis
* Direction Analysis
* Top Trader Analysis
* PnL Distribution Analysis

---

## Key Findings

### Profitability by Sentiment

| Sentiment     | Average PnL |
| ------------- | ----------: |
| Extreme Greed |       67.89 |
| Fear          |       54.29 |
| Greed         |       42.74 |
| Extreme Fear  |       34.54 |
| Neutral       |       34.31 |

Observation:
Extreme Greed periods generated the highest average profitability.

---

### Win Rate Analysis

| Sentiment     | Win Rate (%) |
| ------------- | -----------: |
| Extreme Greed |        46.49 |
| Fear          |        42.08 |
| Neutral       |        39.70 |
| Greed         |        38.48 |
| Extreme Fear  |        37.06 |

Observation:
Win rates remained below 50% across all sentiment categories, indicating that profitability is driven by larger winning trades rather than frequent wins.

---

### Trading Activity

| Sentiment     | Trade Count |
| ------------- | ----------: |
| Fear          |      61,837 |
| Greed         |      50,303 |
| Extreme Greed |      39,992 |
| Neutral       |      37,686 |
| Extreme Fear  |      21,400 |

Observation:
Traders were most active during Fear periods, likely due to increased market volatility.

---

### Average Trade Size

| Sentiment     | Avg Trade Size (USD) |
| ------------- | -------------------: |
| Fear          |                7,816 |
| Greed         |                5,737 |
| Extreme Fear  |                5,350 |
| Neutral       |                4,783 |
| Extreme Greed |                3,112 |

Observation:
Capital deployment was highest during Fear periods.

---

### Top Trader Analysis

Top-performing traders consistently outperformed the overall trader population across all sentiment regimes.

Observation:
Trader skill and risk management appear to be stronger drivers of profitability than sentiment alone.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Project Structure

```text
TraderSentimentAnalysis
│
├── data
│   ├── historical_data.csv
│   └── fear_greed_index.csv
│
├── notebooks
│   └── analysis.ipynb
│
├── outputs
│   ├── avg_pnl_by_sentiment.png
│   ├── win_rate_by_sentiment.png
│   ├── trade_count_by_sentiment.png
│   ├── trade_size_by_sentiment.png
│   ├── pnl_distribution_boxplot.png
│   ├── sentiment_summary.csv
│   └── top_traders.csv
│
├── report
│   └── Trader_Sentiment_Analysis_Report.pdf
│
└── README.md
```

---

## Conclusion

The analysis demonstrates a measurable relationship between market sentiment and trading outcomes. While profitability peaks during Extreme Greed conditions, trading activity and capital deployment are highest during Fear periods.

The results suggest that market sentiment can provide useful context for trading decisions, but successful performance depends more heavily on execution quality, position sizing, and risk management.

---

## Author

D Sai

B.Tech CSE (AI & ML)

Data Analytics | Machine Learning | Full Stack Development

Data Analytics | Machine Learning | Full Stack Development
