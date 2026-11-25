# Backtest Engine

A moving-average crossover backtester that runs entirely in the browser, with real trading costs.
Part of a set of four quant projects; this one answers: does a simple trend rule beat buy and hold
once fees and slippage are charged?

Live: https://mjanthony819.github.io/backtest-engine/

## What it does

- Ships with 12 years of real S&P 500 daily closes (Nov 2014 - Nov 2026) embedded in the page, so it works offline
- Fast/slow simple moving average crossover, long-only, all-in/all-out, executed at close with no lookahead
- Configurable fee per trade and slippage; every entry and exit pays both
- Equity curve vs buy and hold, drawdown chart, Sharpe / CAGR / max drawdown / win rate
- Full trade log with CSV export
- Load your own data: any CSV with Date,Close rows

## Stack

Single `index.html`. No frameworks, no build step, no API keys. Charts are hand-drawn on canvas.

## Honest note

At the default 20/100 settings the strategy underperforms buy and hold over this window. That is the
point of the project: most simple rules do, once costs are real.

Built with AI assistance (Claude).
