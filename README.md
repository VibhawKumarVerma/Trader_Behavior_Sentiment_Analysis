# 📊 Trader Behavior vs Market Sentiment Analysis

## 🔍 Overview

This project analyzes how Bitcoin market sentiment (Fear vs Greed) influences trader behavior and performance on Hyperliquid.

The goal is to uncover patterns that can inform sentiment-aware trading strategies.

---

## 📁 Dataset

1. Bitcoin Fear & Greed Index  
2. Historical Trader Data (Hyperliquid)

---

## ⚙️ Methodology

### 1️⃣ Data Preparation
- Cleaned missing values and duplicates
- Converted timestamps to daily level
- Merged trader data with sentiment classification

### 2️⃣ Feature Engineering
Created key behavioral metrics:
- Daily PnL per trader
- Win rate
- Average trade size
- Leverage usage
- Trade frequency
- Long/Short ratio

### 3️⃣ Analysis
- Compared performance across Fear vs Greed days
- Segmented traders:
  - High vs Low leverage
  - Frequent vs Infrequent
  - Consistent vs Volatile
- Identified behavioral shifts under different sentiment regimes

---

## 📊 Key Visualizations

### 📌 Market Sentiment Distribution

![Sentiment Distribution](outputs/sentiment_distribution.png)

---

### 📌 PnL Distribution

![PnL Distribution](outputs/pnl_distribution.png)

---

### 📌 Leverage Distribution

![Leverage Distribution](outputs/leverage_distribution.png)

---

### 📌 Long vs Short Ratio

![Long Short Ratio](outputs/long_short_ratio.png)

---

## 🧠 Key Insights

1️⃣ Traders increase leverage and trade frequency during Greed days.

2️⃣ High-leverage traders experience larger drawdowns during Fear periods.

3️⃣ Trade performance variance is significantly higher during Fear regimes.

4️⃣ Consistent traders outperform volatile traders across both sentiment states.

---

## 🎯 Strategy Recommendations

### ✅ Strategy 1: Sentiment-Based Risk Control
- Reduce leverage exposure during Fear days.
- Allow higher leverage only for high win-rate traders during Greed.

### ✅ Strategy 2: Behavioral Segmentation
- Restrict high leverage for volatile traders.
- Encourage disciplined trading during high volatility periods.

### ✅ Strategy 3: Trade Frequency Adjustment
- Reduce trade frequency during Fear.
- Increase participation selectively during Greed.

---

## 🤖 Optional Predictive Modeling

Built a basic Random Forest model to predict next-day profitability using:
- Leverage
- Trade size
- Win rate
- Sentiment

Model demonstrates that trader behavior + sentiment can partially predict profitability buckets.

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
jupyter notebook Trader_Analysis.ipynb
