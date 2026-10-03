# quant-lab

Personal research lab for learning systematic swing trading (daily data, liquid cross-asset ETF universe).
Process: idea → data → backtest → validation → paper trading → small live.

## Setup

```bash
conda env create -f environment.yml
conda activate quant-lab
python -m ipykernel install --user --name quant-lab
```

## Layout

- `notes/` – Obsidian vault, module-wise notes with LaTeX
- `notebooks/` – experiments
- `src/` – reusable code (`data.py`, `metrics.py`, `backtest.py`) — written by me, by hand
- `research/` – strategy write-ups
- `data/` – raw data (git-ignored)
- `journal.md` – weekly log
- `ROADMAP.md` – module tracker

Not financial advice. A learning project.
