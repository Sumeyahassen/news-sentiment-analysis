# news-sentiment-analysis
# Task 1: Exploratory Data Analysis (EDA)

**Project:** News Sentiment Analysis for Stock Prediction  
**Author:** Sumeya Hassen 
**Date:** May, 2026

## 1. Executive Summary

This report presents the exploratory analysis of the Financial News dataset containing **1,407,328** news headlines. The goal was to understand the structure, quality, and key patterns in the data before performing sentiment and correlation analysis.

## 2. Data Loading & Cleaning

- Dataset: `raw_analyst_ratings.csv`
- Total Rows: 1,407,328
- Total Columns: 6
- Removed `Unnamed: 0` column
- Converted `date` column to proper datetime format (handled mixed formats)

**Missing Values:** None in important columns.

## 3. Key Findings

### 3.1 Basic Statistics
- Unique Stocks: **6204**
- Unique Publishers: **1034**
- Date Range:2009-02-14 00:00:00 → 2020-06-11 21:12:35

### 3.2 Most Active Publishers

![Top 10 Publishers](../images/top_publishers.png)

**Observation:** Benzinga Insights is by far the most active publisher.

### 3.3 Stocks with Most News Coverage

![Top 10 Stocks](../images/top_stocks.png)

**Observation:** Stocks like [TSLA, AAPL, AMZN, etc.] receive the highest news volume.

### 3.4 Headline Length Distribution

![Headline Length](../images/headline_length.png)

- Average headline length: **7.312051e+01**
- Most headlines are between 7.700000e+01 Words.

### 3.5 News Publication Frequency

![Daily News Volume](../images/daily_volume.png)

![Weekly News Volume](../images/weekly_volume.png)

**Observation:** Clear spikes in news volume during certain periods (earnings season, market events).

### 3.6 Most Common Words in Headlines

![Top Words](../images/top_words.png)

**Top Keywords:** upgrade, downgrade, price target, earnings, beat, miss, etc.

## 4. Insights & Business Implications

- News volume is highly concentrated on a few big publishers and popular stocks.
- Headline language is very action-oriented (upgrade/downgrade/beat).
- There are clear temporal patterns in news publication.

## 5. Challenges & Solutions

- Mixed datetime formats → Solved using `format='mixed'`
- Counter name conflict → Solved by aliasing `PyCounter`
- Large dataset → Used efficient pandas operations

## 6. Task 2

# News Sentiment Analysis for Stock Price Prediction

**Project:** Financial News Sentiment Analysis + Technical Indicators  
## Project Overview
This project analyzes the relationship between financial news sentiment and stock price movements using NLP and Technical Analysis.

---

## Task 1: Exploratory Data Analysis (EDA)

**Objective:** Understand the structure and patterns in the financial news dataset.

### Key Findings
- **Total Articles**: 1,407,328
- **Date Range**: 2020 (full year)
- **Most Active Publisher**: Benzinga Insights
- **Stocks with highest coverage**: AAPL, TSLA, AMZN, etc.
- **Average Headline Length**: 7.312051e+01 characters

### Visualizations
- Top 10 Publishers
- Top 10 Stocks by News Volume
- Headline Length Distribution
- Daily & Weekly News Publication Volume
- Top 20 Most Common Words in Headlines

**Notebook**: `notebooks/eda_task1.ipynb`

---

## Task 2: Technical Indicators Analysis

**Objective:** Download historical stock prices and compute technical indicators.

### Stocks Analyzed
- AAPL (Main)
- TSLA, AMZN, MSFT, GOOGL (Optional)

### Technical Indicators Used
- **Trend Indicators**: SMA(20), SMA(50), EMA(20)
- **Momentum**: RSI(14)
- **Trend Momentum**: MACD + Signal Line + Histogram

### Visualizations
- Price Chart with Moving Averages
- RSI with Overbought/Oversold levels
- MACD Indicator

**Notebook**: `notebooks/task2_technical_indicators.ipynb`

**Key Insight**: Technical indicators successfully captured trends and momentum shifts in AAPL and other stocks.

---

## Task 3: Sentiment Analysis & Correlation (In Progress)

- Sentiment scoring using TextBlob / VADER
- Correlation between news sentiment and daily stock returns

---

## Technologies Used
- **Data Analysis**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **NLP**: TextBlob, NLTK
- **Technical Analysis**: TA-Lib, yfinance
- **Environment**: Python 3.12, Virtual Environment, GitHub

## Project Structure
---