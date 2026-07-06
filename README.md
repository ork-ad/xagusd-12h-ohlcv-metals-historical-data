# XAGUSD 12h OHLCV Metals Historical Data — Free Sample

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Dataset rows](https://img.shields.io/badge/full_dataset-9_672_rows-blue)](https://ork.ad/) [![Updated](https://img.shields.io/badge/weekly_update-every_Sunday-green)](https://ork.ad/) [![Full data on ork.ad](https://img.shields.io/badge/download-ork.ad-orange)](https://ork.ad/)

### → [**Download the full XAGUSD dataset on ork.ad**](https://ork.ad/)

**XAGUSD 12h OHLCV Precious metals historical data** — ultra high-quality 12h OHLCV for **Silver / US Dollar**. Near-continuous precious-metals liquidity across global sessions. Clean `time, open, high, low, close, volume` CSV for backtesting, algorithmic trading and quantitative research.

## Table of contents

- [Why this dataset?](#why-this-dataset)
- [Download sample CSV](#download-sample)
- [GitHub Pages preview](#github-pages)
- [Sample vs full dataset](#sample-vs-full-dataset)
- [Timeframes on ork.ad](#timeframes-on-orkad)
- [Weekly updates](#weekly-updates)
- [Data preview](#data-preview)
- [Schema](#schema)
- [Code examples](#code-examples)
- [Download full data on ork.ad](#download-full-data)

## Why this dataset?

- **Ultra high-quality 12h OHLCV** for **Silver / US Dollar** (Precious metals)
- **Near-continuous precious-metals liquidity across global sessions**
- **Clean CSV schema** — `time, open, high, low, close, volume` (no gaps in formatting)
- **Free evaluation sample** on GitHub (`12h`) · **13 timeframes** on [ork.ad](https://ork.ad/) · **9,672** `12h` rows in the full archive
- Built for **backtesting**, **algorithmic trading** and **quantitative finance** workflows
- **Weekly refresh** — [ork.ad](https://ork.ad/) every **Sunday**; GitHub `12h` sample updated in sync

> **Sample on GitHub** · `XAGUSD_12h.csv` (425 rows, `2025-10-03` → `2026-07-03`). **Full archive on [ork.ad](https://ork.ad/)** — **9,672** `12h` rows (~0.52 MB), **13 timeframes** (``1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W``), `2009-02-24` → `2026-07-03`.

## Download sample

**[XAGUSD_12h.csv](https://github.com/ork-ad/xagusd-12h-ohlcv-metals-historical-data/blob/main/XAGUSD_12h.csv)** on GitHub ([raw CSV](https://raw.githubusercontent.com/ork-ad/xagusd-12h-ohlcv-metals-historical-data/main/XAGUSD_12h.csv)) · [GitHub Releases](https://github.com/ork-ad/xagusd-12h-ohlcv-metals-historical-data/releases) when the release workflow is active.

## GitHub Pages

Interactive chart & stats: **[https://ork-ad.github.io/xagusd-12h-ohlcv-metals-historical-data/](https://ork-ad.github.io/xagusd-12h-ohlcv-metals-historical-data/)**

## Sample vs full dataset

| | **Sample (this repo)** | **Full dataset ([ork.ad](https://ork.ad/))** |
|---|--:|---|
| Instrument | Silver / US Dollar · Precious metals | Silver / US Dollar · Precious metals |
| Timeframes | `12h` (sample) | **13** — `1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W` |
| 12h rows | 425 | **9,672** |
| Size | 0.02 MB | ~0.52 MB |
| Period | `2025-10-03` → `2026-07-03` | `2009-02-24` → `2026-07-03` |
| File | `XAGUSD_12h.csv` | ZIP on [ork.ad](https://ork.ad/) |
| Updates | Weekly (Sunday) — GitHub sample | Weekly (Sunday) — all timeframes |

## Timeframes on ork.ad

This GitHub repository ships a **`12h` evaluation sample** only. On **[ork.ad](https://ork.ad/)**, each full asset archive is delivered as a ZIP with **13 gap-free OHLCV timeframes** (one CSV per timeframe):

**1m** · **3m** · **5m** · **15m** · **30m** · **1H** · **2H** · **4H** · **8H** · **12H** · **16H** · **1D** · **1W**

GitHub = `12h` sample · [ork.ad](https://ork.ad/) = all **13** timeframes above for the same instrument.

## Weekly updates

- **[ork.ad](https://ork.ad/)** — Full datasets on ork.ad are updated every Sunday.
- **GitHub (this repo)** — GitHub samples are refreshed weekly (every Sunday), in sync with ork.ad.

When a new `12h` sample is published on GitHub, the README, chart preview and CSV reflect the latest week of data.

## Data preview

First and latest rows from the GitHub sample **`XAGUSD_12h.csv`**:

**First rows**

| time | open | high | low | close | volume |
| --- | --- | --- | --- | --- | --- |
| 2025-10-03T12:00:00Z | 47.709 | 48.364 | 47.399 | 47.949 | 201502.0 |
| 2025-10-05T12:00:00Z | 47.949 | 48.336 | 47.946 | 48.33 | 48438.0 |
| 2025-10-06T00:00:00Z | 48.33 | 48.748 | 48.057 | 48.616 | 251624.0 |
| 2025-10-06T12:00:00Z | 48.616 | 48.75 | 48.238 | 48.328 | 182791.0 |
| 2025-10-07T00:00:00Z | 48.328 | 48.639 | 47.723 | 48.309 | 239606.0 |

**Last rows**

| time | open | high | low | close | volume |
| --- | --- | --- | --- | --- | --- |
| time | open | high | low | close | volume |
| 2026-07-01T12:00:00Z | 60.145 | 60.857 | 58.757 | 59.624 | 310589.0 |
| 2026-07-02T00:00:00Z | 59.624 | 61.923 | 59.15 | 61.704 | 384061.0 |
| 2026-07-02T12:00:00Z | 61.704 | 62.313 | 60.201 | 62.061 | 410047.0 |
| 2026-07-03T00:00:00Z | 62.061 | 62.743 | 61.757 | 62.072 | 230627.0 |

## Schema

```text
time,open,high,low,close,volume
```

## Code examples

### pandas

```python
import pandas as pd

df = pd.read_csv('XAGUSD_12h.csv', parse_dates=['time'])
df.set_index('time', inplace=True)
print(df.describe())
print(df.resample('1h').agg({'open': 'first', 'high': 'max',
                              'low': 'min', 'close': 'last', 'volume': 'sum'}).head())
```

### backtrader

```python
import backtrader as bt
import pandas as pd

df = pd.read_csv('XAGUSD_12h.csv', parse_dates=['time'])
df.set_index('time', inplace=True)

class PandasData(bt.feeds.PandasData):
    params = (('datetime', None), ('open', 'open'), ('high', 'high'),
              ('low', 'low'), ('close', 'close'), ('volume', 'volume'))

cerebro = bt.Cerebro()
cerebro.adddata(PandasData(dataname=df))
# cerebro.addstrategy(YourStrategy)
# cerebro.run()
```

### vectorbt

```python
import pandas as pd
import vectorbt as vbt

df = pd.read_csv('XAGUSD_12h.csv', parse_dates=['time'])
close = df.set_index('time')['close']
fast, slow = vbt.MA.run(close, 10), vbt.MA.run(close, 50)
entries = fast.ma_crossed_above(slow)
exits = fast.ma_crossed_below(slow)
pf = vbt.Portfolio.from_signals(close, entries, exits, init_cash=10_000, freq='12h')
print(pf.stats())
```

## Download full data

The complete **XAGUSD** archive on **[ork.ad](https://ork.ad/)** includes **13 OHLCV timeframes** (`1m`, `3m`, `5m`, `15m`, `30m`, `1H`, `2H`, `4H`, `8H`, `12H`, `16H`, `1D`, `1W`) — **9,672** rows at `12h`, plus all other timeframes in the same ZIP.

**[→ Get the full XAGUSD dataset on ork.ad](https://ork.ad/)**

---
*GetData · XAGUSD 12h OHLCV sample on GitHub · Full historical data on [ork.ad](https://ork.ad/) · 2026-07-06 UTC*