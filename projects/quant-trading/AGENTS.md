# AGENTS.md — projects/quant-trading

## Project Purpose
`quant-trading` is a Python-based collection of quantitative trading and research example scripts, including:
- Technical indicator backtests (MACD, RSI, Parabolic SAR, Dual Thrust, etc.)
- Options-related scripts (for example, VIX calculation)
- Themed research subprojects (Oil Money, Smart Farmers, Monte Carlo, Ore Money)

This directory is a multi-script workspace, not a single deployable application.

## Entry Files (Minimal Orientation)
- Common entry points: individual strategy scripts that are directly runnable (most include `main()` plus `if __name__ == '__main__':`).
  - Examples:
    - `MACD Oscillator backtest.py`
    - `Pair trading backtest.py`
    - `VIX Calculator.py`
    - `Oil Money project/Oil Money Trading backtest.py`
- Some scripts follow notebook-export style and execute top-level statements in sequence (not all define `main`).
  - Examples:
    - `Smart Farmers project/forecast.py`
    - `Oil Money project/Oil Money NOK.py`

## Common Dependencies
Based on imports used by existing scripts, common dependencies include:
- `pandas`, `numpy`, `matplotlib`
- `statsmodels`, `scipy`, `scikit-learn`
- `yfinance`, `fix_yahoo_finance`
- `seaborn`, `cvxopt`, `imageio`, `python-dateutil`

Note: this directory typically does not include one unified dependency manifest; script imports are the source of truth.

## Default Do-Not-Modify Scope
Unless a task explicitly requires it, do not modify:
- Assets in `data/` and `preview/`
- `LICENSE`
- Unrelated scripts in other themed subprojects

Also:
- Keep edits inside `projects/quant-trading/` only.
- Do not change files in other repository directories.
