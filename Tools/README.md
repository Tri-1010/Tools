# Tools

This folder contains trading-related notebooks and utilities.

## trade_tool.ipynb (Backtrader + vnstock)
- Data: fetch VN stock OHLCV via `vnstock`.
- Features: SMA20/50, RSI, ATR, OBV with `pandas_ta`.
- Strategy: Backtrader SMA/RSI crossover.
- Backtest: run in Backtrader with configurable cash/commission.
- Alerts: optional Telegram message with price move and backtest return.
- Stubs: broker adapter placeholder for future auto-trade; AI/ML placeholder.

### Usage
1) Open the notebook and run the install cell (first cell) to pull dependencies:
   - `vnstock`, `pandas`, `pandas_ta`, `backtrader`, `matplotlib`, `requests`
2) Set config in the config cell (ticker, dates, cash, commission, alert threshold).
3) If using Telegram alerts, export `TELEGRAM_BOT_TOKEN` and `TELEGRAM_CHAT_ID`.
4) Run cells top to bottom to fetch data, compute features, backtest, and (optionally) send an alert.
