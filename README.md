# Trader Performance vs Market Sentiment Analysis

## 📌 Project Overview
This project analyzes how **market sentiment (Fear vs Greed)** relates to **trader behavior and performance** on the Hyperliquid platform.  
The objective is to uncover behavioral patterns, evaluate performance differences, and propose **actionable trading strategies**.

This analysis was completed as part of the **Data Science / Analytics Intern – Round‑0 Assignment**.

---

## 📂 Datasets Used

### 1. Bitcoin Market Sentiment (Fear & Greed Index)
- Columns: `date`, `classification` (Fear / Greed)
- Granularity: Daily

### 2. Historical Trader Data (Hyperliquid)
- Trade‑level dataset containing:
  - Account
  - Coin
  - Trade size
  - Direction (Buy/Sell)
  - Closed PnL
  - Timestamps

---

## 🧠 Methodology

### Data Preparation
- Inspected datasets for shape, missing values, and inconsistencies
- Normalized timestamps and aggregated data at **daily trader (account) level**

### Feature Engineering
- Daily PnL
- Win rate
- Trades per day
- Average trade size
- Leverage proxy
- Long/Short ratio

### Sentiment Integration
- Market sentiment was mapped to daily trader metrics using **date-based lookup**
- A merge was intentionally avoided to prevent timestamp alignment issues

### Analysis
- Performance comparison across Fear vs Greed days
- Behavioral analysis based on sentiment
- Trader segmentation analysis

### Strategy Design
- Translated analytical insights into actionable trading rules

---

## 🛠️ Setup Instructions

### 1️⃣ Clone the Repository
```bash
git clone <your-repository-link>
cd primetrade-sentiment-analysis
## 2️⃣ Create a Virtual Environment

Create a virtual environment named `venv`:

```bash
python -m venv venv

## 3️⃣ Install Dependencies

Install all required Python libraries using the `requirements.txt` file:

```bash
pip install -r requirements.txt

## 📦 requirements.txt

```txt
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
seaborn>=0.12.0
scikit-learn>=1.2.0
jupyter>=1.0.0
notebook>=6.5.0



