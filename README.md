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

![Top 10 Publishers]
<img width="987" height="590" alt="image" src="https://github.com/user-attachments/assets/630cbe84-584e-4184-9d99-a836f1e7c869" />


**Observation:** Benzinga Insights is by far the most active publisher.

### 3.3 Stocks with Most News Coverage

![Top 10 Stock]
<img width="989" height="590" alt="image" src="https://github.com/user-attachments/assets/5f9e6711-1e55-4334-8ee5-c98d25df44ea" />


**Observation:** Stocks like [TSLA, AAPL, AMZN, etc.] receive the highest news volume.

### 3.4 Headline Length Distribution

![Headline Length]
<img width="876" height="547" alt="image" src="https://github.com/user-attachments/assets/4f3bbca4-d619-40e5-b4db-a7676c5061cd" />


- Average headline length: **7.312051e+01**
- Most headlines are between 7.700000e+01 Words.

### 3.5 News Publication Frequency

![Daily News Volume]
<img width="1389" height="689" alt="image" src="https://github.com/user-attachments/assets/edd63ee4-117b-4b94-8659-e5da9ec35086" />


![Weekly News Volume]
<img width="1389" height="690" alt="image" src="https://github.com/user-attachments/assets/06d14b65-b964-4c02-9a72-3ce9b777c5b5" />


**Observation:** Clear spikes in news volume during certain periods (earnings season, market events).

### 3.6 Most Common Words in Headlines

![Top Words]
<img width="1389" height="690" alt="image" src="https://github.com/user-attachments/assets/b3caa501-375c-40e2-a6fe-da8464bbbfcc" />


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
