# 📊 Trader Performance vs Market Sentiment  
### Data Science Intern Assignment – Primetrade.ai  

---

## 📌 Project Overview  

This project analyzes the relationship between **Bitcoin Market Sentiment (Fear/Greed Index)** and **trader behavior & performance** on Hyperliquid.

The objective is to uncover behavioral patterns that can inform smarter trading strategies by answering:

- Does trader performance differ during Fear vs Greed market conditions?
- Do traders adjust leverage, frequency, or bias based on sentiment?
- Can we derive actionable trading rules from behavioral segments?

---

## 🎯 Business Objective  

Understanding how traders react to market sentiment can help:

- Improve risk management  
- Optimize leverage usage  
- Adjust trade frequency dynamically  
- Identify profitable trader archetypes  

This analysis aims to convert behavioral insights into actionable strategy ideas.

---

## 📂 Dataset Description  

### 1️⃣ Bitcoin Market Sentiment Dataset  
- Columns: `Date`, `Classification (Fear/Greed)`  
- Daily sentiment classification (Fear / Greed)

### 2️⃣ Historical Trader Data (Hyperliquid)  
Includes fields such as:
- `account`
- `symbol`
- `execution_price`
- `size`
- `side` (Long / Short)
- `time`
- `closedPnL`
- `leverage`
- `event`
- `start_position`
- etc.

---

## 🧹 Part A – Data Preparation  

### ✔ Data Cleaning & Validation  

- Checked row & column counts  
- Identified and handled missing values  
- Removed duplicates  
- Converted timestamps to datetime format  
- Standardized date format  
- Aggregated trader data at daily level  
- Merged datasets on Date  

### ✔ Key Metrics Created  

- 📈 Daily PnL per trader  
- 🎯 Win rate  
- 📊 Average trade size  
- ⚖ Leverage distribution  
- 🔁 Number of trades per day  
- 📉 Long/Short ratio  
- 📊 PnL volatility (drawdown proxy)  

---

## 📊 Part B – Analysis & Findings  

### 1️⃣ Performance Comparison: Fear vs Greed  

Compared the following across sentiment regimes:

- Average Daily PnL  
- Win Rate  
- PnL Volatility  

**Observation:** Trader performance and volatility differed significantly between Fear and Greed days.

---

### 2️⃣ Behavioral Changes by Sentiment  

Analyzed changes in:

- Trade frequency  
- Leverage usage  
- Position size  
- Long vs Short bias  

**Finding:** Traders exhibit more aggressive behavior during Greed periods and more volatile outcomes during Fear phases.

---

### 3️⃣ Trader Segmentation  

Identified key behavioral segments:

- 🔥 High Leverage vs Low Leverage Traders  
- ⚡ Frequent vs Infrequent Traders  
- 🏆 Consistent Winners vs Inconsistent Traders  

Segment-wise sentiment sensitivity was evaluated to identify risk exposure patterns.

---

## 💡 Key Insights  

1. High leverage traders experienced significantly higher volatility during Fear days.  
2. Trade frequency increased during Greed periods, indicating higher speculative activity.  
3. Consistent performers maintained moderate leverage and stable win rates across sentiment regimes.  

(All insights are supported by visualizations and tables in the notebook.)

---

## 🚀 Part C – Actionable Strategy Recommendations  

### Strategy 1: Sentiment-Based Leverage Control  
- Reduce leverage during Fear periods for high-risk segments.  
- Maintain moderate leverage during Greed phases to optimize risk-adjusted returns.

### Strategy 2: Segment-Based Capital Allocation  
- Allocate more capital to consistent performers during volatile Fear periods.  
- Allow controlled risk expansion for high win-rate traders during Greed periods.

These strategies aim to reduce drawdowns while preserving upside potential.

---

## 📈 (Optional Extension) Predictive Framework  

A lightweight predictive framework can be developed to:

- Predict next-day trader profitability bucket  
- Forecast volatility using:
  - Market sentiment  
  - Leverage usage  
  - Trade frequency  
  - Historical win rate  

---

## 🛠 Tech Stack  

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

## ▶ How to Run  

```bash
# Clone repository
git clone <your-repo-link>

# Navigate to project folder
cd trader-sentiment-analysis

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook
```

Open the main notebook and run cells sequentially.

---

## 📁 Repository Structure  

```
├── notebook.ipynb
├── data/
│   ├── sentiment_data.csv
│   ├── trader_data.csv
├── outputs/
│   ├── charts/
│   ├── tables/
├── README.md
└── requirements.txt
```

---

## 📌 Evaluation Alignment  

This submission focuses on:

✔ Correct data cleaning and alignment  
✔ Strong reasoning backed by evidence  
✔ Actionable, non-generic insights  
✔ Structured communication  
✔ Reproducibility and clarity  

---

## 👩‍💻 Author  

**Mallika Goyal**
Aspiring Data Analyst | Python | SQL | Data Visualization  

---

