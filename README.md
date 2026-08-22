# TradingView Futures Pine Script Strategy

An automated quantitative trading strategy designed in Pine Script v5 for TradingView, optimized for NASDAQ-100 E-mini (`NQ`) and Micro E-mini (`MNQ`) futures contracts.

---

## Strategy Specifications

| Parameter | Configuration |
| :--- | :--- |
| **Asset Class** | Index Futures (`CME:NQ`, `CME:MNQ`) |
| **Primary Timeframe** | 5-Minute / 15-Minute |
| **Trading Session** | Regular Trading Hours (RTH: 09:30 - 16:00 EST) |
| **Pine Script Version** | v6 |
| **Order Execution** | Market on Close / Limit with Slippage modeling |

---

## Core Logic & Features

* **Trend & Momentum Filters:** Multi-timeframe trend alignment using exponential moving averages and volatility bands.
* **Session & News Timing:** Built-in session time windows to restrict entries around high-impact economic releases (CPI, FOMC, NFP).
* **Risk Management:**
  * Fixed risk per trade (e.g., 1–2% account equity / fixed dollar risk).
  * Dynamic ATR-based Stop Loss and Trailing Take Profit targets.
  * Hard daily max-loss circuit breaker.

---

## Setup & Installation

1. Open **TradingView** in your browser or desktop app.
2. Open the **Pine Editor** tab at the bottom of the screen.
3. Click **Open** > **New blank strategy**.
4. Copy the code from `NQ_Strategy.pine` and paste it into the editor.
5. Click **Save**, then click **Add to chart**.
6. Adjust inputs (stop loss ATR multiplier, trading hours, contract size) under the strategy settings gear icon.

---

## Risk Disclaimer

> **Disclaimer:** Futures trading involves substantial risk of loss and is not suitable for all investors. Past performance of this script or its backtest results do not guarantee future returns. This code is provided for educational and research purposes only. Always test thoroughly in paper trading before deploying capital.
EOF# trading-futures-cme
