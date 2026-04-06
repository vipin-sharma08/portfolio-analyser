# 💼 Portfolio Analyser

> A Python portfolio analytics tool that tracks P&L, risk-adjusted returns, drawdown, and sector allocation for Indian equity portfolios.

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python) ![License](https://img.shields.io/badge/license-MIT-green)

---

## ✨ Features

- **P&L Dashboard** — Realised & unrealised gains by stock and sector
- **Risk Metrics** — Sharpe ratio, Sortino ratio, Calmar ratio, Max Drawdown
- **Sector Allocation** — Pie chart breakdown of portfolio weights
- **Benchmark Comparison** — Compare portfolio NAV against NIFTY 50
- **Rolling Returns** — 1M, 3M, 6M, 1Y rolling window analysis
- **Interactive Charts** — Plotly-powered equity curves and heatmaps
- **CSV/Excel Import** — Load trades directly from broker export files (Kotak Neo, Zerodha)

---

## 📁 Project Structure

```
portfolio-analyser/
├── analyser.py          # Main analytics engine
├── loader.py            # Broker CSV import (Kotak, Zerodha)
├── metrics.py           # Sharpe, Sortino, Drawdown, CAGR
├── charts.py            # Plotly visualisations
├── sector_map.py        # NSE sector classification
├── benchmark.py         # NIFTY 50 comparison
└── requirements.txt
```

---

## 🚀 Quickstart

```bash
git clone https://github.com/vipin-sharma08/portfolio-analyser.git
cd portfolio-analyser
pip install -r requirements.txt
python analyser.py --input trades.csv
```

---

## 📊 Sample Output

```
Portfolio Summary (as of 06-Apr-2026)
────────────────────────────────────────────
Total Invested   : ₹ 5,00,000
Current Value    : ₹ 6,24,300
Absolute Return  : +24.86%
CAGR             : 18.2%
Sharpe Ratio     : 1.34
Max Drawdown     : -11.2%

Top Holdings: RELIANCE (18%) | INFY (14%) | HDFCBANK (12%)
Sectors     : Financials (32%) | IT (24%) | Energy (18%)
```

---

## 🛠️ Tech Stack

| Library | Purpose |
|---|---|
| `pandas` / `numpy` | Data wrangling & return calculations |
| `plotly` | Interactive charts & sector pie |
| `yfinance` | Live & historical price data |
| `openpyxl` | Excel import/export |

---

## 📝 License

MIT © [Vipin Sharma](https://github.com/vipin-sharma08)
