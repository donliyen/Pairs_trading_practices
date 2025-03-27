# Pair Trading Strategy

This repository contains Jupyter notebooks for implementing and analyzing a pairs trading strategy. The strategy leverages statistical methods such as cointegration and the Ornstein-Uhlenbeck process to identify and trade mean-reverting asset pairs.

## Contents

### Notebooks
1. **pair_selection.ipynb** - Identifies suitable asset pairs for trading using statistical tests.
2. **pairs_trading_ou_process.ipynb** - Models the spread between pairs using the Ornstein-Uhlenbeck process to assess mean reversion.
3. **pairs_trading_zscore.ipynb** - Implements a trading strategy based on Z-score thresholds for entry and exit signals.

## Strategy Overview
Pairs trading is a market-neutral strategy that involves:
- Selecting two assets that move together historically.
- Establishing a long position in the underperforming asset and a short position in the outperforming asset when the spread deviates from its mean.
- Closing the positions when the spread reverts.

## Requirements
To run the notebooks, install the required libraries:
```bash
pip install numpy pandas statsmodels matplotlib scikit-learn
```

## Usage
1. Open the notebooks in Jupyter:
   ```bash
   jupyter notebook
   ```
2. Run each cell to perform pair selection, spread modeling, and backtesting.
