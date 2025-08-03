# Market Sentiment and Hyperliquid Trading Behavior Analysis

**Author:** Nivesh Kumar Gupta  
**Date:** August 3, 2025

---

## 📑 Project Overview

This project analyzes the interplay between **market sentiment** (Bitcoin Fear & Greed Index) and **trading behavior** (profitability, risk, volume) on the Hyperliquid platform. Using real trading data and sentiment classifications, the analysis uncovers how trader results shift as markets transition from fear to greed, providing actionable insights for smarter trading strategies.

---

## 🗂️ Data Sources

- **Bitcoin Fear & Greed Index**:  
  Daily sentiment scores and categories (Extreme Fear → Extreme Greed), 2018–2025.  
  - *File:* `fear_greed_index.csv`
  - *Key columns:* `date`, `value`, `classification`

- **Hyperliquid Historical Trader Data:**  
  Records of executed trades including account, coin, side, size, profit/loss, and timestamp.  
  - *File:* `historical_data.csv`
  - *Key columns:* `Account`, `Coin`, `Execution Price`, `Size Tokens`, `Size USD`, `Side`, `Timestamp IST`, `Closed PnL`

---

## 🚀 How to Run the Analysis

1. **Environment Setup**
   - Recommended: Google Colab (no local setup needed)
   - Required: `pandas`, `numpy`, `matplotlib`, `seaborn`
   - Upload both CSV files to your working directory or Colab session.

2. **Run the Notebook**
   - Open `sentiment_trader_analysis.ipynb` (or follow cell-by-cell script in this repo).
   - Cells include: data loading, cleaning & merging, EDA (exploratory data analysis), feature relationships, advanced charts, and actionable insights.

3. **Outputs**
   - Merged analysis file: `merged_trades_sentiment.csv`
   - Key plots: PNGs (violin plots, correlation heatmaps, bar charts)
   - LaTeX report: Compile `sentiment_report.tex` to PDF for polished presentation.

---

## 📊 Project Structure

.
├── fear_greed_index.csv # Sentiment data
├── historical_data.csv # Trader transaction data
├── sentiment_trader_analysis.ipynb# Main analysis notebook
├── merged_trades_sentiment.csv # Output: merged, clean dataset
├── plots/ # All exported charts (PNG, PDF)
│ ├── pnl_by_sentiment.png
│ ├── violin_pnl_sentiment.png
│ └── correlation_heatmap.png
├── sentiment_report.tex # Professional report in LaTeX
├── sentiment_report.pdf # PDF version of report
└── README.md # This file


---

## 🧭 Key Results and Insights

- **Profitability and risk are highest in 'Extreme Greed' sentiment.**
- **Most trades are break-even or slight losers** across regimes; large winners drive profits in greed periods.
- **Trade volume spikes in fearful regimes,** indicating aggressive risk-taking under stress.
- **Direction (Buy/Sell) matters less than market regime—** sentiment is the chief driver of risk and reward.

For full interpretation, see `sentiment_report.pdf` or the `Conclusion` and `Key Insights` sections in the notebook.

---

## 🏆 Recommendations

- **Maximize position size only in strong Greed/Extreme Greed regimes."
- "Reduce risk and exposure during Fear,** as large trades are less rewarded.
- **Monitor ongoing sentiment signals as a primary trading input.**
- *See the full report for institutional-grade recommendations and future research ideas.*

---

## 📬 Submission

Prepared by: **Nivesh Kumar Gupta**  
Date: August 3, 2025

For any queries, reach me at `your.email@example.com` or via LinkedIn.

---

> “Market sentiment is not noise—it's the regime switch. Use it, measure it, but always respect it.”  
