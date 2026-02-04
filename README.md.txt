Trader Performance vs Market Sentiment Analysis

--Objective

This project analyzes how Bitcoin market sentiment (Fear vs Greed) impacts trader performance and behavior on Hyperliquid.
The goal is to identify patterns that can inform smarter, sentiment-aware trading strategies.

--Methodology
1. Data Preparation

Loaded trader and sentiment datasets.

Converted timestamps to daily format.

Aligned datasets at daily granularity.

Merged trader data with daily sentiment labels.

Checked missing values and duplicates.

2. Feature Engineering

Created key performance and behavior metrics:

Daily PnL per trader

Win rate

Average position size

Trade frequency

Long/Short ratio

Trader segmentation (Frequent vs Infrequent)

3. Analysis

Compared performance between Fear and Greed days.

Evaluated behavior shifts based on sentiment.

Identified trader segments and analyzed sensitivity to sentiment.

Key Insights

Traders generate higher average PnL during Greed periods compared to Fear periods.

Trade frequency and position sizes increase during Greed days, indicating higher risk appetite.

Frequent traders show stronger performance sensitivity to sentiment shifts.

Strategy Recommendations

Reduce position size during Fear periods to manage downside risk.

Increase trade activity selectively during Greed periods for high-performing trader segments.

Setup & How to Run
1.Clone the repository
git clone https://github.com/yourusername/Trader-Sentiment-Analysis.git
cd Trader-Sentiment-Analysis

2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

3. Run the notebook
jupyter notebook
Open Trader_Sentiment_Analysis.ipynb and run all cells.

Final Summary

Methodology

The analysis was conducted by aligning trader-level transaction data with daily Bitcoin sentiment classification (Fear vs Greed).
All timestamps were converted to daily granularity to ensure consistent merging.

Key performance metrics such as daily PnL, win rate, trade frequency, position size, and long/short bias were computed.
Traders were segmented into frequent and infrequent groups to examine behavioral sensitivity to sentiment shifts.

Insights

Average profitability is higher during Greed periods, suggesting traders benefit from bullish momentum environments.

Traders increase position size and trade frequency during Greed days, reflecting elevated risk appetite.

Frequent traders exhibit amplified performance differences across sentiment regimes, indicating higher exposure to market mood shifts.

Strategic Implications

Incorporating sentiment-aware adjustments to position sizing and trading intensity can improve risk-adjusted returns.
Dynamic strategy rules based on sentiment classification may help reduce drawdowns during Fear periods and capitalize on momentum during Greed periods.