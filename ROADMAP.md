# Roadmap

Har session ke baad yahan tick karo. Sunday ko: `journal.md` update → ROADMAP tick → `git push`.
Dates flexible hain, **gates nahi**.

## Legend

**Tags**
- **Core**: zameen se samjho, haath se derive karo, khud code karo.
- **Lib**: formula + intuition samjho, implementation library se.

**"Done" ka matlab** (Core concept ke 4 boxes, Lib concept ke pehle 2 + library use):
`note` Obsidian note, formula ke saath · `prob` 3-5 problems solve · `code` khud ka implementation · `match` library output se match

**Weekly loop (~9 ghante):** Video ~2h · Reading + notes ~1.5h · Problems ~1.5h · Code ~3h · NotebookLM revision ~1h

> Lecture numbers suggestions hain, playlist pe titles verify kar lena.

---

# Phase 1: Foundations (Month 1-3)

## Week 1: Setup + Returns

**Session 1: Setup**
- [x] Repo, folder structure, Python env, `.gitignore`, ROADMAP, CLAUDE.md
- [x] Obsidian installed (vault: `notes/Quant-Lab/`), private GitHub repo pushed
- [ ] VS Code mein `quant-lab` kernel se `import yfinance` chal gaya

**Session 2: Pehla concept**
- [ ] Stat 110 Lecture 1 (Probability and counting)
- [ ] Chan *Quantitative Trading* Ch. 1
- [ ] NotebookLM notebook "Module 1: Returns & Risk" banaya
- [ ] Note: Simple vs Log Returns, Tasks A/B/C ke saath

**Session 3: Pehla code**
- [ ] `notebooks/01_returns.ipynb`: SPY daily log returns histogram vs normal fit
- [ ] Excess kurtosis + worst day kitne σ door, note mein likha

**Session 4: Derive + code**
- [ ] Haath se derive: √252 annualisation
- [ ] Haath se derive: Sharpe ratio
- [ ] `src/metrics.py`: `annualised_return`, `annualised_vol`, `sharpe`, `max_drawdown`
- [ ] SPY pe chala ke sanity check kiya

**Sunday**
- [ ] `journal.md` entry · ROADMAP tick · git push

## Week 2: Volatility, drawdown, multi-ETF

**Padhai**
- [ ] Chan *Quantitative Trading* Ch. 2 (Fishing for Ideas)
- [ ] Note: Drawdown, max drawdown, drawdown duration
- [ ] Note: Sortino, Calmar

**Code**
- [ ] `src/data.py`: ETF list download aur clean (missing days, adjusted prices)
- [ ] Research universe decide kiya (10-15 ETFs: US equity, sectors, bonds, gold, international), list README mein
- [ ] `notebooks/02_risk.ipynb`: 5-6 ETFs pe returns, vol, Sharpe, max DD ki table
- [ ] Drawdown curve (underwater plot) ek ETF ka

**Revision**
- [ ] NotebookLM audio overview + quiz (Module 1)

**Sunday**
- [ ] journal · ROADMAP tick · git push

### ✅ Module 1: Returns & risk
- [ ] Simple vs log returns: [ ] note [ ] prob [ ] code [ ] match
- [ ] Volatility & √252: [ ] note [ ] prob [ ] code [ ] match
- [ ] Drawdown, max drawdown: [ ] note [ ] prob [ ] code [ ] match
- [ ] Sharpe ratio: [ ] note [ ] prob [ ] code [ ] match
- [ ] Sortino, Calmar (Lib): [ ] note [ ] library se compute kiya

---

## Week 3: Probability basics

**Padhai**
- [ ] Stat 110 Lec 4-5 (Conditional probability, LOTP, Bayes)
- [ ] Blitzstein book Ch. 2
- [ ] NotebookLM notebook "Module 2: Probability" banaya
- [ ] Note: Bayes' theorem + ek trading example
- [ ] Problems: Ch. 2 se 3-5

**Code**
- [ ] `notebooks/03_probability.ipynb`: conditional probability empirically ("kal gira toh aaj girne ki probability?" SPY pe)

**Sunday**
- [ ] journal · ROADMAP tick · git push

## Week 4: Random variables, expectation, variance

**Padhai**
- [ ] Stat 110 Lec 7-10 (RVs, distributions, expectation, linearity)
- [ ] Blitzstein Ch. 3-4 (chuninda sections)
- [ ] Note: Expectation, variance, haath se derivations
- [ ] Problems: 3-5

**Code**
- [ ] Mean/variance khud likha, numpy se match kiya
- [ ] Simulation: biased coin "strategy" ka expected P&L vs simulated

**Sunday**
- [ ] journal · ROADMAP tick · git push

## Week 5: Normal, fat tails, covariance

**Padhai**
- [ ] Stat 110 Lec 13-14 (Normal, location-scale)
- [ ] Stat 110 Lec 21 (Covariance and correlation)
- [ ] Note: Normal vs fat tails, skew, kurtosis
- [ ] Note: Covariance, correlation, 2-asset portfolio variance derive kiya
- [ ] Problems: 3-5

**Code**
- [ ] `notebooks/05_tails_corr.ipynb`: ETF universe ka correlation matrix + heatmap
- [ ] Har ETF ka skew/kurtosis, QQ-plot vs normal
- [ ] 2-asset portfolio vol formula vs actual portfolio returns ki vol match

**Sunday**
- [ ] journal · ROADMAP tick · git push

## Week 6: CLT + hypothesis testing (Module 3 shuru)

**Padhai**
- [ ] Stat 110 Lec 29 (LLN, CLT)
- [ ] Hypothesis testing, t-statistic (resource NotebookLM/notes se)
- [ ] Note: CLT, aur "backtest ka Sharpe kitna noisy hai"
- [ ] Note: Strategy ka t-stat, t ≈ Sharpe × √(years)
- [ ] Problems: 3-5

**Code**
- [ ] Bootstrap: SPY Sharpe ka distribution (resampling), confidence interval
- [ ] Random-signal strategies ka t-stat distribution ("luck kaisa dikhta hai")

**Start Module 3**
- [ ] MIT 18.S096 regression lecture (Lec 6, verify)

**Sunday**
- [ ] journal · ROADMAP tick · git push

### ✅ Module 2: Probability & statistics
- [ ] Expectation, variance, covariance, correlation: [ ] note [ ] prob [ ] code [ ] match
- [ ] Normal vs fat tails, skew, kurtosis: [ ] note [ ] prob [ ] concept clear [ ] library calc
- [ ] Central Limit Theorem: [ ] note [ ] prob [ ] code [ ] match
- [ ] Hypothesis testing, strategy t-stat: [ ] note [ ] prob [ ] code [ ] match
- [ ] Bayes' theorem (Lib): [ ] note [ ] example
- Skip: MGFs, measure theory

---

## Week 7: Regression + stationarity

**Padhai**
- [ ] MIT 18.S096 Time Series lecture (Lec 8, verify)
- [ ] NotebookLM notebook "Module 3: Time Series" banaya
- [ ] Note: OLS, beta, hedge ratio (normal equations derive kiye)
- [ ] Note: Stationarity, autocorrelation
- [ ] Problems: 3-5

**Code**
- [ ] OLS khud likha (numpy, normal equations), `statsmodels` se match
- [ ] Har ETF ka beta vs SPY
- [ ] Prices vs returns ka ACF plot: kaun stationary hai?

**Sunday**
- [ ] journal · ROADMAP tick · git push

## Week 8: ADF + cointegration (Module 4 shuru)

**Padhai**
- [ ] MIT 18.S096 Time Series II (Lec 11, verify)
- [ ] Chan *Quantitative Trading* Ch. 7: stationarity aur cointegration section
- [ ] Note: ADF test (kya test karta hai, null hypothesis)
- [ ] Note: Cointegration vs correlation

**Code**
- [ ] `statsmodels` ADF: prices vs returns vs spread
- [ ] Ek pair (jaise GLD/GDX ya similar) pe cointegration test

**Start Module 4**
- [ ] Chan *Quantitative Trading* Ch. 3 (Backtesting) padhna shuru

**Sunday**
- [ ] journal · ROADMAP tick · git push

### ✅ Module 3: Time series
- [ ] Stationarity, autocorrelation: [ ] note [ ] prob [ ] code [ ] match
- [ ] Linear regression (OLS): [ ] note [ ] prob [ ] code [ ] match
- [ ] ADF test (Lib): [ ] note [ ] statsmodels se chalaya
- [ ] Cointegration (Lib): [ ] note [ ] statsmodels se chalaya
- Skip: ARIMA, GARCH (baad mein, `arch` library)

---

## Week 9: Apna backtester

**Padhai**
- [ ] Chan Ch. 3 poora
- [ ] NotebookLM notebook "Chan Strategies" banaya
- [ ] Note: Lookahead bias, `shift(1)` kyun
- [ ] Note: Survivorship bias, yfinance ki limitation
- [ ] Note: Transaction costs, slippage model

**Code**
- [ ] `src/backtest.py`: vectorised backtester (signal → position → returns), **no library**
- [ ] Costs + slippage parameter
- [ ] Test: buy-and-hold SPY ka result direct returns se match
- [ ] Test: jaan-boojh ke lookahead daala, dekha Sharpe kitna fake badha

**Sunday**
- [ ] journal · ROADMAP tick · git push

## Week 10: Validation (Module 5 shuru)

**Padhai**
- [ ] Note: Overfitting, data snooping, multiple testing
- [ ] Note: Walk-forward testing, parameter sensitivity

**Code**
- [ ] Walk-forward split function (train/test windows)
- [ ] Parameter sensitivity heatmap (jaise MA lookback × threshold)
- [ ] vectorbt ya backtrader install, ek strategy pe apne backtester se compare

**Start Module 5**
- [ ] Note: Time-series momentum (trend following)

**Sunday**
- [ ] journal · ROADMAP tick · git push

### ✅ Module 4: Backtesting
- [ ] Vectorised backtester: [ ] note [ ] code [ ] buy-and-hold match [ ] tests
- [ ] Transaction costs, slippage: [ ] note [ ] code
- [ ] Lookahead, survivorship, overfitting bias: [ ] note [ ] lookahead demo
- [ ] Walk-forward, parameter sensitivity: [ ] note [ ] code
- [ ] Event-driven frameworks (Lib): [ ] note [ ] ek library se result match

---

## Week 11: Momentum strategies

**Padhai**
- [ ] Note: Cross-sectional momentum (ETF rotation)
- [ ] Chan Ch. 7: mean reversion vs momentum section

**Code**
- [ ] `research/` ya notebook: time-series momentum on ETF universe, costs ke saath
- [ ] Cross-sectional momentum: top-N ETFs monthly rotation
- [ ] Dono ka walk-forward result + t-stat

**Sunday**
- [ ] journal · ROADMAP tick · git push

## Week 12: Mean reversion + pairs (Module 6 shuru)

**Padhai**
- [ ] Note: Mean reversion (z-score)
- [ ] Note: Pairs trading (cointegration se hedge ratio)
- [ ] Chan Ch. 6 (Money and Risk Management) shuru

**Code**
- [ ] Z-score mean reversion strategy, costs ke saath
- [ ] Pairs trading: ek cointegrated pair pe
- [ ] Saari strategies ki comparison table (Sharpe, DD, turnover, t-stat)

**Start Module 6**
- [ ] Note: Volatility targeting

**Sunday**
- [ ] journal · ROADMAP tick · git push

### ✅ Module 5: Strategies
- [ ] Time-series momentum: [ ] note [ ] code [ ] walk-forward [ ] costs
- [ ] Cross-sectional momentum: [ ] note [ ] code [ ] walk-forward [ ] costs
- [ ] Mean reversion (z-score): [ ] note [ ] code [ ] walk-forward [ ] costs
- [ ] Pairs trading (Lib): [ ] note [ ] cointegration library se

---

## Week 13: Risk, sizing + research report

**Padhai**
- [ ] Chan Ch. 6 poora
- [ ] NotebookLM notebook "Validation & Risk" banaya
- [ ] Note: Kelly criterion derive kiya, fractional Kelly kyun
- [ ] Note: Markowitz (intuition), stop-loss rules, kill switch

**Code**
- [ ] Volatility targeting best strategy pe lagaya
- [ ] Kelly fraction compute kiya, half-Kelly vs full-Kelly simulation
- [ ] PyPortfolioOpt se ETF universe ka min-variance portfolio
- [ ] Kill switch rule backtest mein (max monthly DD pe band)

**Report**
- [ ] `research/01_<strategy>.md`: 2-3 pages (idea, data, results, weaknesses)
- [ ] NotebookLM mein "skeptical quant reviewer" prompt se review karwaya
- [ ] Claude Code se bias check (lookahead, survivorship, costs)

**Sunday**
- [ ] journal · ROADMAP tick · git push

### ✅ Module 6: Risk & position sizing
- [ ] Volatility targeting: [ ] note [ ] prob [ ] code [ ] match
- [ ] Kelly criterion: [ ] note [ ] prob [ ] code [ ] match
- [ ] Markowitz (Lib): [ ] note [ ] PyPortfolioOpt se chalaya
- [ ] Stop-loss rules, kill switch: [ ] note [ ] code

---

## 🚧 Gate 1: Report written
- [ ] Modules 1-6 ke saare Core concepts "done"
- [ ] Apna backtester tested aur `src/` mein
- [ ] Research report `research/` mein, weaknesses honestly likhe

---

# Phase 2: Better research (Month 4-6)
- [ ] Chan *Algorithmic Trading*
- [ ] Better data source (survivorship-free), yfinance se upgrade
- [ ] 2-3 uncorrelated strategies, validated
- [ ] Pending decisions: broker (API access, jaise IBKR + `ib_async`), final market (US stocks vs LSE UCITS), live capital amount
- [ ] Paper trading account open

## 🚧 Gate 2: Strategies validated, paper account open

# Phase 3: Paper trading (Month 7-9)
- [ ] Automated paper trading (daily signal after close → next-day order)
- [ ] Har hafte backtest vs paper results compare
- [ ] López de Prado *Advances in Financial ML*: chuninda chapters (purged CV, meta-labeling)
- [ ] NotebookLM notebook "Financial ML"

## 🚧 Gate 3: 2-3 months consistent paper results

# Phase 4: Small live (Month 10-12)
- [ ] Sirf utna capital jo poora doob jaaye toh bhi farq na pade
- [ ] Pehle se likhe rules: max loss per trade, max monthly DD kill switch
- [ ] Har trade ka journal
- [ ] Tax records (CGT, HMRC guidance check)

---

## Ground rules (har waqt)
- No real money jab tak Gate 3 clear na ho
- No leverage, options, CFDs, spread betting
- Learning code khud likhna; Claude sirf review aur explain karega
