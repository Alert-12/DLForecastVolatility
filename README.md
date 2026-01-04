# DLForecastVolatility — Volatility Forecasting in Crypto: HAR/HAR-X vs GARCH vs LSTM

This repository contains code and materials for the working paper:

**Can Deep Learning Exploit Nonlinear Market Signals for Volatility Forecasting? Evidence from Cryptocurrency Markets**

- **Paper (Zenodo, Working Paper):** https://doi.org/10.5281/zenodo.18148216  
- **Status:** Working paper (not peer-reviewed)

## What this project does
We study whether deep learning models can improve **out-of-sample volatility forecasting** in cryptocurrency markets compared with strong econometric benchmarks.

Using **Bitcoin (BTC-USD)** daily OHLCV data, we:
- Construct realized volatility proxies (e.g., close-to-close, Parkinson, Garman–Klass).
- Build HAR-style features (daily/weekly/monthly volatility components) and optional exogenous indicators.
- Compare:
  - **HAR / HAR-X** (linear regression baseline)
  - **GARCH(1,1)** (ARCH package, walk-forward refit)
  - **LSTM** (TensorFlow/Keras)
- Evaluate multi-step-ahead forecasts (e.g., 7-day-ahead) under a rolling/expanding out-of-sample scheme.
- Report metrics such as **RMSE, MAE, QLIKE**.

> Note: Results depend on data period, forecasting horizon, and modeling choices. This repository is intended for research/replication purposes.
