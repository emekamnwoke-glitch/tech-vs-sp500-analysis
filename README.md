# Tech Stocks vs S&P 500 — Performance Analysis (2020–2023)

> **Exploratory data analysis comparing the performance of major tech stocks against the S&P 500 benchmark across a full market cycle: boom, crash, and recovery.**

---

## Overview

This project analyses the behaviour of five major tech stocks — **Apple, Microsoft, Google (Alphabet), Amazon, and Meta** — relative to the **S&P 500 index** over the 2020–2023 period. The analysis covers a complete and turbulent market cycle including the post-COVID bull run, the 2022 rate-hike-driven selloff, and the subsequent AI-driven recovery.

The project is built entirely in Python and presented as a Jupyter Notebook, making it easy to follow the analysis step by step with annotated charts and commentary.

---

## Key Questions Explored

- Did tech stocks outperform the broader market over this period?
- How did individual tech stocks compare to each other year by year?
- Were investors adequately compensated for the extra risk of holding tech?
- How did volatility evolve during the 2022 market crash vs. calmer periods?

---

## Key Findings

| Insight | Detail |
|---|---|
| **Tech dominated 2020–2021** | The Tech Index significantly outpaced the S&P 500 during the pandemic-era bull run |
| **2022 was a brutal year** | Tech stocks fell harder than the broader market during the Fed's rate hike cycle — Meta particularly so |
| **Recovery was strong in 2023** | The AI boom (ChatGPT, LLMs) drove a sharp rebound, with tech reclaiming ground |
| **Sharpe Ratios were mixed** | Not all tech stocks justified their added volatility — some delivered poor risk-adjusted returns |

---

## Project Structure

```
tech-vs-sp500-analysis/
│
├── tech_vs_sp500_analysis.ipynb   # Main analysis notebook
├── README.md                      # Project documentation
└── charts/                        # Exported chart images
    ├── chart1_cumulative_performance.png
    ├── chart2_annual_returns.png
    ├── chart3_volatility.png
    └── chart4_risk_return.png
```

---

## Charts Produced

1. **Cumulative Performance** — Growth of $1 invested across all assets from Jan 2020
2. **Annual Returns by Year** — Side-by-side bar charts breaking down each calendar year
3. **Volatility Analysis** — Rolling 30-day volatility over time + annualised vol per asset
4. **Risk vs Return Scatter** — Sharpe Ratio comparison: was the extra tech risk worth it?

---

## Tech Stack

| Tool | Purpose |
|---|---|
| `Python 3.12` | Core language |
| `pandas` | Data manipulation and returns calculation |
| `numpy` | Numerical simulation and statistics |
| `matplotlib` | Chart generation and formatting |
| `seaborn` | Visual styling |
| `yfinance` *(optional)* | Pull real market data instead of simulated data |

---

## Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/emekamnwoke-glitch/tech-vs-sp500-analysis.git
cd tech-vs-sp500-analysis
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn
```

To use **real market data** instead of simulated data, also install:
```bash
pip install yfinance
```

### 3. Run the notebook
```bash
jupyter notebook tech_vs_sp500_analysis.ipynb
```

> The notebook runs on **simulated data by default** (no internet required). To switch to live data, uncomment **Option A** and comment out **Option B** in Cell 3.

---

## Notes

- Simulated data is calibrated to reflect realistic 2020–2023 market behaviour (returns, volatility, and crash sensitivity per asset)
- Risk-free rate assumed at **2%** for Sharpe Ratio calculations
- All returns are price-based; dividends are not included

---

## Author

**Chukwuemeka Nwoke**  
[LinkedIn](https://linkedin.com/in/emekamnwoke) · [GitHub](https://github.com/emekamnwoke-glitch)

---

*This project was built for portfolio and educational purposes.*
