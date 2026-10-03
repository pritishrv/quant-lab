# Roadmap (Month 1-3, Modules 1-6)

A concept is **done** when: Obsidian note with formula · 3-5 problems solved · own implementation · matches library output.

## Week 1 action plan
- [x] Session 1: repo, folder structure, Python env, `.gitignore`, ROADMAP, CLAUDE.md
- [x] Session 1: Obsidian installed (vault: `notes/Quant-Lab/`); private GitHub repo `quant-lab` pushed
- [ ] Session 2: Stat 110 Lecture 1
- [ ] Session 2: Chan "Quantitative Trading" Ch. 1
- [ ] Session 2: NotebookLM notebook "Module 1: Returns & Risk"
- [ ] Session 2: Obsidian note — simple vs log returns, with derivation
- [ ] Session 3: `notebooks/01_returns.ipynb` — SPY returns histogram vs normal fit
- [ ] Session 3: excess kurtosis + worst day in std devs, written in note
- [ ] Session 4: hand-derive √252 annualisation and Sharpe
- [ ] Session 4: `src/metrics.py` — `annualised_return`, `annualised_vol`, `sharpe`, `max_drawdown`; checked on SPY
- [ ] Session 4: journal entry, ROADMAP tick, git push

## Module 1: Returns & risk (Week 1-2)
- [ ] Simple vs log returns — Core
- [ ] Volatility & annualisation (√252) — Core
- [ ] Drawdown, max drawdown — Core
- [ ] Sharpe ratio — Core
- [ ] Sortino, Calmar — Understand + library
- [ ] Week 2: same analysis on 5-6 ETFs

## Module 2: Probability & statistics (Week 3-6)
- [ ] Expectation, variance, covariance, correlation — Core
- [ ] Normal vs fat tails, skew, kurtosis — Core concept, library calc
- [ ] Central Limit Theorem — Core
- [ ] Hypothesis testing, t-stat of a strategy — Core
- [ ] Bayes' theorem — Understand + library

## Module 3: Time series (Week 6-8)
- [ ] Stationarity, autocorrelation — Core
- [ ] Linear regression (OLS) in finance — Core
- [ ] ADF test — Understand + library
- [ ] Cointegration — Understand + library

## Module 4: Backtesting (Week 8-10)
- [ ] Vectorised backtester (pandas, no library) — Core
- [ ] Transaction costs, slippage — Core
- [ ] Lookahead, survivorship, overfitting bias — Core
- [ ] Walk-forward testing, parameter sensitivity — Core
- [ ] Event-driven frameworks (vectorbt / backtrader) — Understand + library

## Module 5: Strategies (Week 10-12)
- [ ] Time-series momentum — Core
- [ ] Cross-sectional momentum (ETF rotation) — Core
- [ ] Mean reversion (z-score) — Core
- [ ] Pairs trading — Understand + library

## Module 6: Risk & position sizing (Week 12-13)
- [ ] Volatility targeting — Core
- [ ] Kelly criterion (fractional) — Core
- [ ] Markowitz optimisation (PyPortfolioOpt) — Understand + library
- [ ] Stop-loss rules, kill switch — Core

## Gate: end of Week 13
- [ ] 2-3 page research report on best strategy in `research/`
