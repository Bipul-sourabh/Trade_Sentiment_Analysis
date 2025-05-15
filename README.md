# Trade_Sentiment_Analysis
https://docs.google.com/spreadsheets/d/1N3993gvPVe-RBjmW6QXTQseuilEWKFJq/edit?usp=drive_link&ouid=114224520195623056349&rtpof=true&sd=true



---

## 🧠 Trader Behavior Insights Based on Market Sentiment 📊

This project explores the relationship between **trader performance** and the **Bitcoin market sentiment** (Fear & Greed Index). Using two datasets—**Hyperliquid Trader Data** and **Fear/Greed Index Data**—I performed data cleaning, transformation, and analysis in **Microsoft Excel** to uncover patterns that can drive smarter trading strategies.

---

### 📁 Datasets Used

1. **Trader Historical Data (Hyperliquid)**
   Columns include: `account`, `symbol`, `execution price`, `size (USD)`, `side`, `timestamp`, `event`, `closedPnL`, etc.

2. **Bitcoin Fear/Greed Index**
   Columns: `Date`, `Classification` (Fear, Greed, Neutral, Extreme Fear, Extreme Greed)

---

### ✅ Key Steps Performed

* **Date Transformation**:
  Converted UNIX timestamps into human-readable datetime format in trader data and formatted both datasets to match (YYYY-MM-DD) for merging.

* **Data Merging**:
  Used `XLOOKUP` to match sentiment data to each trade based on date.

* **Loss Flag Column**:
  Created a new column to flag trades as "Loss" or "Profit" based on `closedPnL`.

* **Pivot Table Analysis**:

  * Average Profit/Loss by Sentiment
  * Number of Trades by Sentiment
  * Profit vs Loss distribution under each sentiment

* **Visualizations**:

  * Bar Chart: Avg Profit/Loss by Sentiment
  * Line Chart: Trades over Time by Sentiment
    (Excluded Leverage as it wasn’t available in the dataset)

---

### 📌 Key Questions Answered

1. **Are profits higher on Greed days?**
   ➤ Yes, average closedPnL was higher on Greed days.

2. **Do people trade more on Greed days?**
   ➤ Yes, number of trades is significantly higher during Greed.

3. **Are losses more common on Fear days?**
   ➤ Yes, more negative `closedPnL` entries occurred during Fear days.

---

### 📄 Tools Used

* Microsoft Excel
* Pivot Tables
* Excel Charts
* Data Transformation Functions (`XLOOKUP`, `DATE`, `IF`)

---


