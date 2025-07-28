# 💹 Trader Behavior vs Bitcoin Market Sentiment

This project explores the relationship between **trader performance** and the **Bitcoin Fear & Greed Index** using real trade data from the Hyperliquid platform. We uncover how market sentiment affects trading behavior, profitability, and risk, and build a machine learning model to predict sentiment based on trading actions.

---

## 🧠 Objective

To analyze how trader behavior varies with market sentiment (Fear/Greed), identify hidden behavioral patterns, and deliver actionable insights that can guide smarter, sentiment-aware trading strategies.

---

## 📁 Datasets

1. **Bitcoin Fear & Greed Index**  
   - Columns: `date`, `value`, `classification` (e.g. Fear, Extreme Greed)
   - Source: [Alternative.me API](https://alternative.me/crypto/fear-and-greed-index/)

2. **Hyperliquid Historical Trader Data**  
   - Columns include: `account`, `execution price`, `size`, `side`, `closedPnL`, `start position`, `timestamp`, etc.

---

## 🔍 Analysis Highlights

- Merged trades with daily sentiment data
- Conducted exploratory data analysis (EDA):
  - Bar Plot: Avg PnL under Fear vs Greed
  - Box Plot: Leverage usage by sentiment
  - Line Chart: Trade volume trend by sentiment
  - Heatmap: Correlation among trading features
  - Pie Chart: Profitability under each sentiment

---

## 📊 Key Insights

- Traders are generally **more profitable during Greed** days
- **Leverage and trade volume increase** when sentiment is bullish
- Behavioral patterns (like timing, risk, side) vary clearly across sentiment types

---

## 🤖 Machine Learning

We trained a classification model to **predict market sentiment (Fear/Greed)** based on trader behavior.

- **Features Used:**
  - Execution Price, Size USD, Closed PnL
  - Leverage (proxy), Trade Side, Hour of Day
- **Models:**
  - Logistic Regression
  - Random Forest (higher accuracy)
- **Outcome:**
  - Random Forest revealed leverage and trade timing as top predictors of sentiment

---

## ✅ Conclusion

> Traders adapt their risk-taking and behavior based on market sentiment.  
> Machine learning can detect this shift, offering a foundation for **adaptive trading systems** that react to behavioral signals.

---


