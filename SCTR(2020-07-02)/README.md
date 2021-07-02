# SCTR Ranking for S&P 500 Tickers and Screener for Potential Stock Picks

![Plot](https://github.com/jinwei-ang/Stock-Market-Analysis-Mini-Projects/blob/main/SCTR(2020-07-02)/SCTR(2021-07-02).png)
## Introduction
The StockCharts Technical Rank (SCTR) is a numerical score that ranks a stock within a group of stocks. The methodology for these rankings comes from the wisdom of John Murphy, author of many books on technical analysis and contributor to the Market Message at StockCharts.com.

Stocks are assigned a score based on six key indicators covering different timeframes. These indicator scores are then sorted and assigned a technical rank. Using SCTR tables, chartists can sort stocks according to their technical rank, making it easy to identify the technical leaders and laggards within a specific group.

As with all technical indicators, SCTRs are designed to be used in conjunction with other indicators and analysis techniques. For example, chartists can use SCTRs as a filter when there are too many signals, weeding out stocks showing relative weakness and providing a manageable subset for further analysis.

```
Long-Term Indicators (weighting)
--------------------------------

  * Percent above/below 200-day EMA (30%)
  * 125-Day Rate-of-Change (30%)

Medium-Term Indicators (weighting)
----------------------------------

  * Percent above/below 50-day EMA (15%)
  * 20-day Rate-of-Change (15%)

Short-Term Indicators (weighting)
---------------------------------

  * 3-day slope of PPO(12,26,9) Histogram/3 (5%)
  * 14-day RSI (5%)
```

## Ranking
In the original SCTR universe, the stocks were grouped into baskets and ranked based on market cap. In this project, the universe considered are stocks in the S&P 500.

## Screener
A screener is built based on the inspiration of '@AboveGreenLine' by Joanne Klein. The rules are:
1. Above the Green Line; above long term moving average.
2. Above 90 Relative Strength; > 90 decile rank for SCTR.
3. Money Wave is coming out of the Green Zone; stochastic crossing over oversold region.

There is a slight modification where the long term moving average is define as 200-day simple moving average as compared to the original 250-day simple moving average.

## Charts
The charts of the potential tickers were downloaded from Finviz.

## Data
* yfinance
* finvizfinance
* Finviz Charts

## Potential Development
* Sorting tickers into baskets based on their market cap
* Re-balancing of market cap
* Depoly as web app (Flask/Streamlit)

#### Credit is where credit due
- John J. Murphy: Technical Analysis of the Financial Markets
- https://school.stockcharts.com/doku.php?id=technical_indicators:sctr
- https://stockcharts.com/public/1107832/chartbook
