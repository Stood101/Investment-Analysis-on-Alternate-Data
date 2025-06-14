# Reddit + Google Trends Investment Strategy using XGBoost

An experimental machine learning pipeline that uses sentiment signals from Reddit and public search interest from Google Trends to forecast short-term stock price movements.

🔍 Overview

This project investigates whether social sentiment and trend awareness can be quantified into signals that consistently offer trading insights. The focus is on retail-influenced equities and the short-horizon volatility they exhibit.

📊 Features

Sentiment extraction from Reddit titles (VADER)

Mention volume per ticker

Google search trend data (via pytrends)

Price movement classification from Yahoo Finance

XGBoost-based classifier for predicting bullish/bearish movement

📊 Results

Accuracy: ~76%

Bullish F1-Score: ~0.82

Sentiment Distribution: Balanced positive/negative

Notable Signals: Stocks like NVDA and UNH showed sentiment-price alignment

⚖️ Investment Strategy

Long Entry: Sentiment > 0.4, Trend > 50, Volume > 5 mentions

Hold Period: 2 to 4 days

Exit Trigger: Profit > 3%, or sentiment reversal

Caution with Shorts due to Reddit bullish bias

⚠️ Limitations

Sentiment magnitude is often subtle; signal enhancement needed for thin sentiment cases
