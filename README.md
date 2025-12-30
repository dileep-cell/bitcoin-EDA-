# 🪙 Bitcoin Market Analysis: Business-Oriented Exploratory Data Insights

## 📊 Project Overview

**Motto:** *"Exploring volatility, liquidity, and strategic risk factors in Bitcoin markets"*

This project delivers a comprehensive exploratory data analysis (EDA) of cryptocurrency market dynamics, focusing on three major digital assets: **MON**, **BNB**, and **ETH**. The analysis provides actionable insights into market behavior, risk profiles, and investment viability through rigorous quantitative analysis.

---

## 🎯 Data Source

**Primary Source:** [CoinGecko](https://www.coingecko.com/)

CoinGecko is a leading cryptocurrency data aggregator providing reliable, real-time market data including:
- Historical price movements
- Market capitalization trends
- Trading volume metrics
- Comprehensive asset coverage across global exchanges

---

## 📁 Dataset Information

### Dataset Type
**Time-Series Market Data** in CSV format

### Assets Analyzed
1. **MON (MON-usd-max.csv)** - Emerging cryptocurrency
2. **BNB (bnb-usd-max.csv)** - Binance Coin
3. **ETH (eth-usd-max.csv)** - Ethereum

### Key Features
- `snapped_at` - Timestamp of data capture
- `price` - Asset price in USD
- `market_cap` - Total market capitalization
- `total_volume` - 24-hour trading volume
- Engineered features: liquidity ratios, returns, volatility metrics, time components

### Dataset Characteristics
<img width="988" height="547" alt="download" src="https://github.com/user-attachments/assets/cd2e3f23-f6bc-4944-bbb6-fa8cdfd84b9f" />

| Coin | Records | Date Range | Avg Market Cap | Data Quality |
|------|---------|------------|----------------|--------------|
| **ETH** | 3,707 | 2015-08-07 to 2025-09-30 | ~$151B | ✅ Deep & Reliable |
| **BNB** | 2,992 | 2017-09-16 to 2025-11-26 | ~$41.7B | ✅ Strong Coverage |
| **MON** | 3 | 2025-11-24 to 2025-11-26 | ~$0.38B | ⚠️ Thin Liquidity |

---

## 🔍 What Was Done

### 1. **Data Ingestion & Preparation**
- Imported three separate CSV files for MON, BNB, and ETH
- Consolidated datasets with coin labels for comparative analysis
- Performed chronological sorting and data integrity verification
- Converted timestamps to IST (Indian Standard Time) for localized analysis

### 2. **Data Quality Assessment**
- ✅ Verified zero null values across all datasets
- ✅ Confirmed complete data retention after concatenation (6,702 total records)
- ✅ Validated chronological coverage per coin

### 3. **Feature Engineering**
- **Temporal Features:** Extracted date, hour, weekday, and month components
- **Liquidity Ratio:** Calculated as `total_volume / market_cap`
- **Returns:** Computed percentage change in price per coin
- **Volatility:** Measured standard deviation of returns

### 4. **Advanced Financial Metrics**

#### Sharpe Ratio Analysis
Evaluated risk-adjusted returns using a 5% risk-free rate:
- **Daily Sharpe Ratios:** Measure short-term efficiency
- **Annualized Sharpe Ratios:** Assess long-term performance

#### Maximum Drawdown (MDD)
Calculated worst peak-to-trough decline for each asset to quantify downside risk

#### Quarter-over-Quarter (QoQ) Volatility
Assessed growth stability across quarterly periods

### 5. **Comparative Analysis**
- Monthly liquidity ratio trends
- Quarterly volatility patterns
- Market capitalization evolution
- Return distribution across assets
- Executive summary metrics (launch timing, active quarters, best/worst performance periods)

### 6. **Visualization Suite**
<img width="1389" height="590" alt="download" src="https://github.com/user-attachments/assets/ca4c95a7-8577-4a91-8386-ad4bc0e30c80" />
Created comprehensive visual analytics:
- Sharpe ratio comparisons (daily vs annualized)
- Quarterly market cap trends
- Volatility share area charts
- Comparative bar charts for returns, volatility, and market cap
- Time-series analysis of asset evolution
  

---

## 💡 Key Findings & Final Inference
<img width="562" height="435" alt="download" src="https://github.com/user-attachments/assets/06c1e858-86ce-4f31-b465-28e2ababc70f" />



### **ETH (Ethereum) - The Benchmark Asset 🏆**
- **Market Position:** Dominant with deepest liquidity (3,707 records, 41 active quarters)
- **Average Market Cap:** ~$151B with peak at ~$485B (2021Q4)
  <img width="686" height="489" alt="download" src="https://github.com/user-attachments/assets/b0f31451-8053-4e10-9674-9fddb1f4fb93" />

- **Risk Profile:** 
  - Moderate volatility (1.58 QoQ)
  - Maximum Drawdown: -92% (significant historical risk)
  - Sharpe Ratio: 0.95 (annualized) - approaching acceptable risk-adjusted threshold
- **Verdict:** ✅ **Stable, mature asset with reliable liquidity** - best suited for risk-aware portfolios seeking balanced exposure

---

### **BNB (Binance Coin) - The Growth Volatile 📈**
- **Market Position:** Strong mid-tier presence (2,992 records, 34 quarters)
- **Average Market Cap:** ~$41.7B with peak at ~$146B (2025Q4)
- **Risk Profile:**
  - High volatility (3.12 QoQ) - highest among analyzed assets
  - Maximum Drawdown: -85%
  - Sharpe Ratio: 0.42 (annualized) - weak risk-adjusted returns
  - Extreme early volatility (2017-2018) reflecting speculative adoption
- **Verdict:** ⚠️ **High-growth potential but elevated risk** - volatility outweighs gains, suitable only for aggressive risk tolerance

---

### **MON - The Thin Liquidity Anomaly 🚨**
<img width="700" height="470" alt="download" src="https://github.com/user-attachments/assets/69416e43-41ed-4f65-ae87-33528289735f" />

- **Market Position:** Late entrant with minimal history (3 records, 1 quarter)
- **Average Market Cap:** ~$0.38B (negligible compared to peers)
  
**Risk Profile:**
  - Liquidity Ratio: 1.88 (extremely high - signals thin market depth)
  - Sharpe Ratio: 11.2 (annualized) - anomalously high but unreliable
  - Negligible drawdown (~0%) due to data sparsity
  - Zero measurable QoQ volatility
  - Compared to BNB,ETH MON gives high returns( in crypto high returns is not always safe and gaurenteed stability)
    <img width="576" height="474" alt="download" src="https://github.com/user-attachments/assets/fc064344-169d-4f78-8ca4-84c57c1b1f88" />
    
- **Verdict:** ❌ **High-risk outlier with unreliable metrics** - insufficient historical data makes this asset unsuitable for informed investment decisions

---

## 🎓 Business Implications
<img width="691" height="489" alt="download" src="https://github.com/user-attachments/assets/54cef8ab-3859-4088-b8c8-43f7e841a755" />


### Investment Strategy Recommendations

1. **Conservative Portfolios:** Prioritize ETH for stability and liquidity depth
2. **Growth-Oriented Portfolios:** Consider BNB with appropriate risk hedging strategies
3. **Speculative Positions:** Avoid MON until sufficient market maturity is established

### Risk Management Insights
<img width="691" height="489" alt="download" src="https://github.com/user-attachments/assets/3c1fbc0f-4dfe-4de1-9960-ca62e1ccb5c0" />

- **Liquidity Risk:** MON's thin market depth poses significant exit strategy challenges
- **Volatility Exposure:** BNB requires active monitoring and stop-loss mechanisms
- **Drawdown Preparedness:** Both ETH and BNB show substantial historical drawdowns requiring robust risk capital

### Market Maturity Indicators

The analysis reveals three distinct asset profiles:
- **Established Liquidity (ETH):** Deep market, proven resilience
- **Mid-Range Adoption (BNB):** Strong growth trajectory with volatility risk
- **Late Entrant Anomaly (MON):** Insufficient data for reliable assessment

---

## 🛠️ Technical Implementation

### Technologies Used
- **Python 3.11.13**
- **Libraries:** pandas, numpy, matplotlib
- **Platform:** Kaggle Notebooks
- **Data Format:** CSV time-series data

### Key Analytical Techniques
- Time-series decomposition
- Financial risk metrics (Sharpe, MDD)
- Pivot table aggregation
- Rolling window analysis
- Statistical distribution analysis

---

## 📈 Reproducibility

This analysis is fully reproducible with the provided Kaggle dataset. All transformations, calculations, and visualizations are documented in the Jupyter notebook with inline inference statements for transparency.

**Dataset ID:** https://www.kaggle.com/code/dileepp22/bitcoineda

---

## 🤝 Contact & Collaboration

This analysis demonstrates proficiency in:
- Financial data analysis and risk assessment
- Time-series modeling and feature engineering
- Data visualization and business storytelling
- Quantitative investment research methodologies

**Perfect for roles in:** Data Analytics, Financial Engineering, Quantitative Research, Risk Management, Business Intelligence

---

## 📌 Final Takeaway

> **"In cryptocurrency markets, historical depth matters more than headline returns. ETH's decade-long track record provides the reliability that MON's three-day history cannot. Smart investing requires both opportunity recognition and risk discipline."**

---

*Analysis completed: December 8, 2025*  
*Data Source: CoinGecko | Computational Environment: Kaggle Notebooks*
