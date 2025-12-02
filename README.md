Bitcoin Sentiment vs. Trader Behavior Analysis 
Candidate Name: Akshat Jain 

Project Overview This project explores the relationship between market sentiment (Fear vs. Greed) and trader behavior. By merging the Fear & Greed Index with historical trade data, I aimed to identify how trading habits—such as risk appetite, volume, and profitability—change as market emotions shift.

The core goal was to answer: Does the "Smart Money" (top profitable traders) behave differently than the retail crowd during emotional extremes?

Repository Structure notebook_1.ipynb: The main analysis notebook containing data cleaning, metric calculations, and visualization code.

csv_files/:

fear_greed_index.csv: Daily sentiment data.

historical_data.csv: Transaction-level trader data.

outputs/: Generated charts and visualizations used in this report.

ds_report.pdf: A PDF version of the final insights.

Key Findings

General Market Behavior Profitability: Traders are, on average, most profitable during Extreme Greed ($130 Avg PnL) and Fear ($112 Avg PnL).

Risk Management: Surprisingly, position sizes are largest during Fear ($7,800) and smallest during Extreme Greed ($3,100). This suggests that while traders aggressively "buy the dip," they become cautious and size down when the market overheats.

Volume: Activity peaks during Fear, indicating high volatility and hand-changing during corrections.

The "Smart Money" Signal (Hidden Trend) I isolated the top 10% of traders by total profit ("Smart Money") and compared their buying behavior to the rest of the market ("Retail").

The Signal: During Extreme Greed, a clear divergence appears.

Retail Behavior: Continues to buy aggressively (Accounting for ~51% of their volume).

Smart Money Behavior: Aggressively reduces buying (Dropping to ~32% of their volume).

Actionable Insight: When sentiment hits "Extreme Greed" and retail buying remains high, the "Smart Money" is already selling into that liquidity. A smarter strategy would be to follow the Smart Money: take profits or open short positions when sentiment hits Extreme Greed.

Asset Preference Most Traded Asset: The coin HYPE dominates trading volume (68k+ trades), followed by @107 and BTC. This indicates a heavy focus on high-beta/meme assets over traditional majors in this specific dataset.

Setup & Instructions To reproduce the analysis:

Upload the csv_files folder to your Google Drive or local environment.

Open notebook_1.ipynb in Google Colab.

Ensure the file paths in the first cell match your directory structure.

Run all cells to generate the metrics and visualizations found in the outputs/ folder.

