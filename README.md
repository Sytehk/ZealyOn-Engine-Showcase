# ZealyOn Engine

**Rust strategy research, backtesting, replay, and live monitoring**

ZealyOn Engine powers the strategy research and signal workflows used by ZealyOn. It connects historical market-data analysis with the live monitoring that maintains shared strategy records and produces signals for alerts and supported external account routes.

## The problem it addresses

A strategy can look convincing in a single historical chart and still be fragile. Useful evaluation needs repeatable datasets, explicit test assumptions, trade-level records, and a clear distinction between simulated performance and what happens in a connected broker account.

The engine supports a workflow that moves from research candidates to repeatable evaluation and ongoing monitoring. It is designed to make those stages comparable, while preserving the fact that a backtest and a live fill are not the same event.

## Core capabilities

- **Strategy search and screening:** evaluate rule-based crypto and forex candidates against historical market data.
- **Backtesting:** replay historical periods and review trades, performance, and risk measures.
- **Replay workflows:** rerun strategy logic against recorded data to investigate behavior and improve consistency.
- **Live monitoring:** process incoming market data and maintain a forward-tracked record for each monitored strategy.
- **Signal delivery:** provide the signal source used by alerts and supported External Live routes.
- **Research tools:** support command-line and desktop workflows for data preparation, analysis, and review.

## Shared strategy logic

The active strategy search, backtesting, replay, and live engine is written in Rust. Shared Rust libraries are used across evaluation and monitoring so the same strategy rules can be applied consistently across those workflows. Alerts and supported external execution use signals from the same engine and closed-candle decisions.

A shared strategy record is separate from each user's execution route. Each connected account has its own provider conditions and fill results. Fees, slippage, timing, market data, broker rules, sizing constraints, or software defects can make account results differ from a historical test or shared strategy record.

<p align="center">
  <img src="https://raw.githubusercontent.com/Sytehk/ZealyOn-Showcase/main/assets/strategy-discovery-example.jpg" width="340" alt="ZealyOn Discover interface preview powered by the strategy engine">
</p>
<p align="center"><sub>Product interface example showing strategy search criteria. It is not an engine benchmark or a performance result.</sub></p>

## Engineering scope

The project includes Rust services, shared libraries, market-data workflows, replay and simulation components, plus command-line and desktop research tools. This showcase describes the current Rust engine direction without publishing strategy implementations or live operating details.

## Technology

Rust, historical market-data processing, backtesting, replay, and command-line and desktop tooling.

## This repository

This is a documentation-only project summary. It contains no strategy source, proprietary entry and exit rules, credentials, account details, or live deployment instructions.

[Explore AceNetics](https://acenetics.dev)
