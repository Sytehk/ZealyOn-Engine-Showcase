# ZealyOn Engine

**Rust strategy research, backtesting, and live monitoring**

ZealyOn Engine powers strategy search and evaluation for the ZealyOn product. It supports systematic research on historical market data and the ongoing monitoring that produces shared strategy records and user signals.

## What it covers

- **Strategy research:** search and screen rule-based crypto and forex strategy candidates against historical data.
- **Backtesting and replay:** run repeatable simulations and inspect trade-by-trade results and performance over time.
- **Live monitoring:** evaluate strategy signals as market data arrives and maintain a shared forward-tracked record.
- **Alerts and execution signals:** alerts and supported External Live routes use the same strategy signal engine and completed-candle decisions.
- **Shared behavior:** reuse strategy and replay logic across research and monitoring to keep their results comparable.

A historical simulation, the shared forward-tracked record, and a user's broker fills describe different things. Fees, slippage, timing, market data, broker rules, and execution details can cause outcomes to differ. Historical performance is not a promise of future results.

## Engineering scope

The active strategy search, backtesting, replay, and live engine is written in Rust. The project includes shared Rust libraries and command-line and desktop research tools. Per-user execution routes are kept separate from the shared strategy record.

## Technology

Rust, market-data processing, backtesting and replay workflows, command-line and desktop tooling.

## About this repository

This is a documentation-only public showcase. It does not include trading strategies, proprietary rules, source code, account information, credentials, or live operating instructions.

[Explore AceNetics](https://acenetics.dev)
