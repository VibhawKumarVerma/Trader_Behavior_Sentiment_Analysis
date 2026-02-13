# Trader_Behavior_Sentiment_Analysis

## Objective
Analyze how market sentiment (Fear/Greed) influences trader performance and behavior on Hyperliquid.

## Dataset
- Bitcoin Fear & Greed Index
- Historical Trader Data (Hyperliquid)

## Methodology
1. Cleaned and aligned datasets on daily level.
2. Engineered behavioral features:
   - Daily PnL
   - Win rate
   - Trade frequency
   - Leverage usage
   - Long/Short ratio
3. Compared performance metrics across sentiment regimes.
4. Segmented traders by leverage, frequency, and consistency.

## Key Insights
1. Performance differs significantly between Fear and Greed days.
2. High leverage traders show higher volatility during Fear days.
3. Trade frequency increases during Greed periods.

## Strategy Recommendations
1. Reduce leverage exposure during Fear regimes.
2. Allow aggressive positioning only for consistent high win-rate traders.
3. Adjust trade frequency based on sentiment state.

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook Trader_Analysis.ipynb
