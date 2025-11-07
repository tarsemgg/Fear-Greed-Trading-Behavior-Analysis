# Sentiment-Aware Trading Strategy

This project analyzes the relationship between Bitcoin market sentiment (Fear vs Greed) and trader behavior/performance. Using historical trading execution data and the Bitcoin Fear & Greed Index, the analysis uncovers how sentiment influences trade size, profitability, and direction preference.

## Objective

* Understand how trader performance changes during different sentiment phases.
* Identify behavioral patterns such as BUY vs SELL preferences.
* Generate data-driven trading strategies based on sentiment.

## Datasets

**1. Trader Execution Dataset**
Contains individual trade records including price, position, PnL, and side.

**2. Bitcoin Sentiment Dataset**
Contains daily sentiment scores and sentiment classification labels.

The datasets were merged on the `Date` column to align trading activity with daily sentiment.

## Key Insights

* **Fear Periods:** BUY trades tend to perform better as prices are discounted.
* **Greed Periods:** SELL trades tend to perform better due to market overextension.
* **Neutral Sentiment:** Market direction is unclear; high leverage becomes risky.
* **Extreme Greed:** May signal trend exhaustion—wait for confirmation before entering.

## Strategy Recommendations

* Accumulate or enter long positions during **Fear dips**.
* Reduce long exposure or consider shorts during **Greed peaks**.
* Avoid high leverage in **Neutral** sentiment conditions.
* During **Extreme Greed**, monitor for reversal signals.

## Project Structure

```
├── DS_Task_Final.ipynb                # Final cleaned analysis notebook
├── Trader_Sentiment_Analysis_Presentation.pptx  # Summary presentation
├── data/                               # Folder for datasets (not included here)
│   ├── trader_data.csv
│   └── sentiment_data.csv
└── README.md                           # Project documentation
```

## How to Run

1. Open `DS_Task_Final.ipynb` in Jupyter Notebook or Google Colab.
2. Place your datasets inside the `data/` folder.
3. Update file paths in the notebook where indicated.
4. Run all cells to reproduce the analysis.

## Tools Used

* Python (Pandas, NumPy, Matplotlib, Seaborn)
* Jupyter Notebook
* PowerPoint for presentation formatting

## Author

**Tarsem Kumar**

---
