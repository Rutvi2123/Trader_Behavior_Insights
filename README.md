# Trader Behavior Insights

## 📌 Problem Statement
The goal of this project is to explore the relationship between **trader performance** and **market sentiment**, uncover hidden patterns, and deliver insights that can drive **smarter trading strategies**.


## 📂 Data Sources

### 1. Historical Trader Data from Hyperliquid
- **Description:** Contains detailed trading history such as account, execution price, size, side (BUY/SELL), and closed PnL.
- **Key Columns:** `account`, `symbol`, `execution price`, `size`, `side`, `time`, `start position`, `event`, `closedPnL`, `leverage`, etc.
- **Download Link:** [Historical Data](https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing)

### 2. Bitcoin Market Sentiment Dataset (Fear & Greed Index)
- **Description:** Provides daily sentiment data including a numerical score and a categorical classification (Fear, Greed, Extreme Fear, Extreme Greed).
- **Key Columns:** `date`, `value`, `classification`
- **Download Link:** [Fear & Greed Index](https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing)


## 🔍 Key Insights
1. **Weak Negative Correlation:**  
   A weak negative correlation exists between overall daily profitability and the market sentiment score.  
   → Traders tend to be **less profitable during high optimism** periods.

2. **Contrarian Behavior in Top Traders:**  
   Top 10% PnL traders often **BUY during Extreme Fear** and **SELL during Extreme Greed**, contrasting with the majority.

3. **Volume & Volatility Patterns:**  
   - Trading volume spikes during periods of **Fear**.  
   - Both **Extreme Fear** and **Extreme Greed** show **larger PnL swings**, reflecting heightened market volatility.

## ▶️ How to Run the Project

### **1. Download Datasets**
Download both files and place them in the same directory as the Jupyter Notebook:
- `historical_data.csv`
- `fear_greed_index.csv`

### **2. Install Dependencies**
Run the following command:
```bash
pip install pandas matplotlib
