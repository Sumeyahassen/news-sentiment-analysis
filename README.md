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


---