# Comparing `tmp/tradingview_defi_strategy-0.1.0.tar.gz` & `tmp/tradingview_defi_strategy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingview_defi_strategy-0.1.0.tar", max compression
+gzip compressed data, was "tradingview_defi_strategy-0.2.0.tar", max compression
```

## Comparing `tradingview_defi_strategy-0.1.0.tar` & `tradingview_defi_strategy-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    18030 2023-04-29 18:28:04.651339 tradingview_defi_strategy-0.1.0/README.md
--rw-r--r--   0        0        0      827 2023-04-29 18:54:12.480145 tradingview_defi_strategy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       54 2023-04-29 18:23:46.621779 tradingview_defi_strategy-0.1.0/tradingview_defi_strategy/__init__.py
--rw-r--r--   0        0        0    19288 1970-01-01 00:00:00.000000 tradingview_defi_strategy-0.1.0/setup.py
--rw-r--r--   0        0        0    18946 1970-01-01 00:00:00.000000 tradingview_defi_strategy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    18751 2023-06-23 10:57:57.037292 tradingview_defi_strategy-0.2.0/README.md
+-rw-r--r--   0        0        0     1024 2023-06-23 11:03:10.923793 tradingview_defi_strategy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-04-29 18:23:46.621779 tradingview_defi_strategy-0.2.0/tradingview_defi_strategy/__init__.py
+-rw-r--r--   0        0        0     7700 2023-05-01 23:06:09.682971 tradingview_defi_strategy-0.2.0/tradingview_defi_strategy/trader_joe_grid_search.py
+-rw-r--r--   0        0        0     7671 2023-05-01 12:28:04.364657 tradingview_defi_strategy-0.2.0/tradingview_defi_strategy/uniswap_grid_search.py
+-rw-r--r--   0        0        0    19667 1970-01-01 00:00:00.000000 tradingview_defi_strategy-0.2.0/PKG-INFO
```

### Comparing `tradingview_defi_strategy-0.1.0/README.md` & `tradingview_defi_strategy-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,16 @@
- # TradingView to TradingStrategy.ai algorithmic DeFi trading strategy conversion
+ # TradingView and Coinbase to DeFi and Trader Joe algorithmic trading strategy porting
 
 This is an example Python project on how to convert TradingView-based PineScript algorithmic 
 trading strategies to [TradingStrategy.ai](https://tradingstrategy.ai) [Python format](https://tradingstrategy.ai/docs/).
 
+[![Watch the recorded workshop session for this project](https://img.youtube.com/vi/Pwst54BGCEM/maxresdefault.jpg)](https://www.youtube.com/watch?v=Pwst54BGCEM)
+
+**[Watch the recorded workshop session on YouTube](https://www.youtube.com/watch?v=Pwst54BGCEM)**
+
 This example repository was made for [Avalanche Summit II workshop](https://tradingstrategy.ai/blog/avalanche-summit-ii-workshop).
 [See the example Github repository here](https://github.com/tradingstrategy-ai/tradingview-defi-strategy).
 
    * [Benefits of DeFi for algorithmic traders](#benefits-of-defi-for-algorithmic-traders)
    * [Prerequisites](#prerequisites)
       * [Your skills](#your-skills)
       * [Software](#software)
@@ -47,24 +51,26 @@
 ### Your skills
 
 To work with this example, you need to have
 
 - Basic experience in cryptocurrencies
 - Basic experience in trading
 - Experience in TradingView's PineScript
-- Junior software developer level experience in Python
+- Junior level experience in Python
 
 ### Software 
 
 - Python 3.10
-- [Poetry package manager for Python](https://tradingstrategy.ai/community)
+- [Poetry package manager for Python](https://python-poetry.org/docs/#installing-with-the-official-installer)
 - Git
 
 ## About the example strategy
 
+The example strategy backtest is in  [bollinger_band_example_defi_strategy.ipynb](.bollinger_band_example_defi_strategy.ipynb) notebook.
+
 The example strategy is a simple [Bollinger band](https://tradingstrategy.ai/glossary/bollinger-bands) strategy.
 **Whether it makes profit or not is outside the scope of the example.** The strategy is not optimised at all and parameters
 are picked more or less by a gut feeling. Please use this example as learning material and base for your own strategies. 
 
 - Use [Bollinger Band's](https://tradingstrategy.ai/glossary/bollinger-bands) and [RSI](https://tradingstrategy.ai/glossary/relative-strength-index-(rsi)) to determine position entries
 - Long only - suitable for [DEX spot markets](https://tradingstrategy.ai/glossary/spot-market) like Trader Joe
 - 4 hours timeframe for candles
@@ -356,14 +362,19 @@
 
 - [Trailing stop loss](/delayed_trailing_stop_loss.ipynb) - Annual return 18%, max drawdown 7%
 - [All in](./all_in.ipynb): Use 90% of cash instead of 50% of cash when entering a position. Realised profit $300 -> $600.
 - [Multipair](./multipair.ipynb): Trade more than single pair
 - [Uniswap full history](/uniswap_v2_full_history.ipynb): Trade on ETH-USD pair based on Uniswap v2, so we get max DEX 2020-2023 backtesting history
 - [Uniswap 1h candles](./uniswap_v2_1h_candle_stddev_1.ipynb): Same as above, but trade very frequently
 
+Grid searches
+
+- [Grid search - basic](./grid_search.ipynb): Automatically search through strategy parameters for an optional combination
+- [Grid search - multiprocessing](./uniswao_grid_search.ipynb): Optimise strategy parameters over larger dataset and parameter space using Python multiprocessing
+
 ## Next steps
 
 - [Join the Trading Strategy community Discord for discussion and questions](https://tradingstrategy.ai/docs/)
 - [View our learning material for algorithmic trading](https://tradingstrategy.ai/docs/learn/index.html)
 - [Study other strategy backtesting examples and code samples](https://tradingstrategy.ai/docs/programming/index.html)
 
 Links
```

### Comparing `tradingview_defi_strategy-0.1.0/pyproject.toml` & `tradingview_defi_strategy-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "tradingview-defi-strategy"
-version = "0.1.0"
+version = "0.2.0"
 description = "Convert TradingView and PineScript based algorithmig trading strategies for DeFi. An example repository."
 authors = ["Mikko Ohtamaa <mikko@opensourcehacker.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["algorithmic trading", "ethereum", "cryptocurrency", "tradingview", "quantitative finance", "binance", "coinbase", "uniswap"]
 homepage = "https://tradingstrategy.ai"
 repository = "https://github.com/tradingstrategy-ai/tradingview-defi-strategy"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 pytest = "^7.3.0"
 trade-executor = {version = "0.3", extras = ["web-server", "execution", "quantstats", "data"]}
+#  rade-executor = {git = "https://github.com/tradingstrategy-ai/trade-executor.git", extras = ["web-server", "execution", "quantstats", "data"], rev = "82d353fcdffe8647f0a04790040e4ca177c726a3" }
 ipython = "^8.12.0"
 ipdb = "^0.13.13"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tradingview_defi_strategy-0.1.0/setup.py` & `tradingview_defi_strategy-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,408 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tradingview-defi-strategy
+Version: 0.2.0
+Summary: Convert TradingView and PineScript based algorithmig trading strategies for DeFi. An example repository.
+Home-page: https://tradingstrategy.ai
+License: MIT
+Keywords: algorithmic trading,ethereum,cryptocurrency,tradingview,quantitative finance,binance,coinbase,uniswap
+Author: Mikko Ohtamaa
+Author-email: mikko@opensourcehacker.com
+Requires-Python: >=3.10,<3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: ipdb (>=0.13.13,<0.14.0)
+Requires-Dist: ipython (>=8.12.0,<9.0.0)
+Requires-Dist: pytest (>=7.3.0,<8.0.0)
+Requires-Dist: trade-executor[data,execution,quantstats,web-server] (==0.3)
+Project-URL: Repository, https://github.com/tradingstrategy-ai/tradingview-defi-strategy
+Description-Content-Type: text/markdown
 
-packages = \
-['tradingview_defi_strategy']
+ # TradingView and Coinbase to DeFi and Trader Joe algorithmic trading strategy porting
 
-package_data = \
-{'': ['*']}
+This is an example Python project on how to convert TradingView-based PineScript algorithmic 
+trading strategies to [TradingStrategy.ai](https://tradingstrategy.ai) [Python format](https://tradingstrategy.ai/docs/).
 
-install_requires = \
-['ipdb>=0.13.13,<0.14.0',
- 'ipython>=8.12.0,<9.0.0',
- 'pytest>=7.3.0,<8.0.0',
- 'trade-executor[data,execution,quantstats,web-server]==0.3']
-
-setup_kwargs = {
-    'name': 'tradingview-defi-strategy',
-    'version': '0.1.0',
-    'description': 'Convert TradingView and PineScript based algorithmig trading strategies for DeFi. An example repository.',
-    'long_description': ' # TradingView to TradingStrategy.ai algorithmic DeFi trading strategy conversion\n\nThis is an example Python project on how to convert TradingView-based PineScript algorithmic \ntrading strategies to [TradingStrategy.ai](https://tradingstrategy.ai) [Python format](https://tradingstrategy.ai/docs/).\n\nThis example repository was made for [Avalanche Summit II workshop](https://tradingstrategy.ai/blog/avalanche-summit-ii-workshop).\n[See the example Github repository here](https://github.com/tradingstrategy-ai/tradingview-defi-strategy).\n\n   * [Benefits of DeFi for algorithmic traders](#benefits-of-defi-for-algorithmic-traders)\n   * [Prerequisites](#prerequisites)\n      * [Your skills](#your-skills)\n      * [Software](#software)\n   * [About the example strategy](#about-the-example-strategy)\n      * [Technical indicator documentation](#technical-indicator-documentation)\n   * [Strategy performance results and algorithm porting notes](#strategy-performance-results-and-algorithm-porting-notes)\n      * [Equity curve](#equity-curve)\n      * [Price action and positions](#price-action-and-positions)\n      * [Trading summary](#trading-summary)\n      * [Position timeline](#position-timeline)\n   * [Example code](#example-code)\n   * [Notable differences between Python and PineScript](#notable-differences-between-python-and-pinescript)\n   * [About trading on decentralised finance](#about-trading-on-decentralised-finance)\n      * [DEX trading fees](#dex-trading-fees)\n   * [Installation](#installation)\n      * [API key](#api-key)\n   * [Running backtests](#running-backtests)\n      * [Running backtest notebooks from terminal](#running-backtest-notebooks-from-terminal)\n      * [Running backtest notebooks with Visual Studio Code](#running-backtest-notebooks-with-visual-studio-code)\n      * [Running backtest notebooks Jupyter](#running-backtest-notebooks-jupyter)\n   * [Variations of the backtest example](#variations-of-the-backtest-example)\n   * [Next steps](#next-steps)\n\n\n## Benefits of DeFi for algorithmic traders\n\nRunning your trading strategy on [decentralised exchanges](https://tradingstrategy.ai/glossary/decentralised-exchange) instead of centralised exchanges have several benefits:\n\n- Execute your strategy in a counterparty risk free manner \n- Broker free, direct to exchange\n- Have 100% control of your strategy market data and live execution\n- [Low trading fees on efficient decentralised markets](https://tradingstrategy.ai/blog/most-efficient-market-is-on-a-public-blockchain-and-decentralised)\n- Convert your trading algorithm to a on-chain fund\n  - Benefits of rich Python quant finance libraries like [pandas_ta](https://github.com/twopirllc/pandas-ta) and [quantstats](https://github.com/ranaroussi/quantstats).\n\n## Prerequisites\n\n### Your skills\n\nTo work with this example, you need to have\n\n- Basic experience in cryptocurrencies\n- Basic experience in trading\n- Experience in TradingView\'s PineScript\n- Junior software developer level experience in Python\n\n### Software \n\n- Python 3.10\n- [Poetry package manager for Python](https://tradingstrategy.ai/community)\n- Git\n\n## About the example strategy\n\nThe example strategy is a simple [Bollinger band](https://tradingstrategy.ai/glossary/bollinger-bands) strategy.\n**Whether it makes profit or not is outside the scope of the example.** The strategy is not optimised at all and parameters\nare picked more or less by a gut feeling. Please use this example as learning material and base for your own strategies. \n\n- Use [Bollinger Band\'s](https://tradingstrategy.ai/glossary/bollinger-bands) and [RSI](https://tradingstrategy.ai/glossary/relative-strength-index-(rsi)) to determine position entries\n- Long only - suitable for [DEX spot markets](https://tradingstrategy.ai/glossary/spot-market) like Trader Joe\n- 4 hours timeframe for candles\n- Backtesting period of 2024-04-01 - 2023-04-01\n- Use a tight stop loss when entering a position\n  - This will result multiple positions closed for stop loss and few profitable positions during market rallies\n\n- We target the following live trading pairs \n  - [EAVAXTH/USDC pair on Trader Joe on Avalanche with 20 BPS fee tier](https://tradingstrategy.ai/trading-view/polygon/uniswap-v3/eth-usdc-fee-5).\n    See a note about this in `decide_trades()` Python code.\n  - [Coinbase ETH/USDC with 60 BPS market taker fee](https://help.coinbase.com/en/exchange/trading-and-funding/exchange-fees) (12x more expensive than DeFi)\n \n**Note**: Long only strategies are challenging in a descending or sideways cryptocurrencies market like 2021-2023. Furthermore, this strategy was handpicked\nfor an overly short backtesting period, to better illustrate the features of the backtesting framework.\n\n### Technical indicator documentation\n\nFind documentation for technical indicators used in the example\n\n- [Exponential Moving Average (EMA)](https://tradingstrategy.ai/docs/programming/api/technical-analysis/overlap/help/pandas_ta.overlap.ema.html#ema):\n  The Exponential Moving Average is a more responsive moving average compared to the Simple Moving Average (SMA). The weights are determined by alpha which is proportional to it’s length. \n\n- [Relative Strength Index (RSI)](https://tradingstrategy.ai/docs/programming/api/technical-analysis/momentum/help/pandas_ta.momentum.rsi.html#rsi):\n  The Relative Strength Index is a popular momentum oscillator used to measure the velocity as well as the magnitude of directional price movements.\n\n- [Bollinger Bands (BB)](https://tradingstrategy.ai/docs/programming/api/technical-analysis/volatility/help/pandas_ta.volatility.bbands.html#bbands):\n  A popular volatility indicator by John Bollinger.\n\n## Strategy performance results and algorithm porting notes\n\nBoth TradingView and Trading Strategy strategies open positions in a similar fashion, so they are more or less comparable.\n\n**Note**. Because of the different price feeds and other subtle differences you cannot have the same strategy backtest\n    result on two different markets: Coinbase and Trader Joe.**. If you carefully examine the price chart, RSI and other indicators,\n    you will see the results vary a bit. In such a small backtesting timeframe, this strategy is prone to small fluxuations\n    and is not robust. The goal of this example, however, is not robustness, but easily demonstrable data.\n\nIf you examine, some of positions like ~March 17th are opened around the same time, \nso we do see that the strategy is following the same pattern.\n\nBoth strategy implementations make a low number of trades, 10-20, for the backtesting period.\nThis makes it easier to demonstrate the example.\n\n### Equity curve\n\nHow well the strategy would have historically performed on AVAX-USDC pair on Trader Joe on Avalanche (20 BPS fee).\n\n![equity curve trading strategy](./screenshots/equity-curve.png)\n\nHow well the strategy would have historically performed on AVAX-USD on Coinbase (no fees).\n\n![equity curve coinbase](./screenshots/equity-curve-coinbase.png)\n\nHowever, if we switch on 50 BPS taker fee on Coinbase we can see it destroys the strategy performance,\ngoing to loss (vs. 20 BPS fee on Trader Joe).\n\n![equity curve coinbase with fee](./screenshots/equity-curve-coinbase-with-fees.png)\n\n### Positions taken\n\nHere is a screenshot of individual won/lost positions in Python strategy.\nYou can see we have few profitable long duration positions, and very short duration\nunprofitable positions.\n\n![positions](./screenshots/positions.png)\n\n\n### Price action and indicators\n\nHere is a screenshot of the price action and technical indicators of the strategy.\n\n![price action and positions](./screenshots/price-action-and-positions.png)\n\n### Trading summary\n\nSummary statistics are calculated as follow:\n\n```                                                \nTrading period length                     145 days\nReturn %                                    11.90%\nAnnualised return %                         29.88%\nCash at start                            $5,000.00\nValue at end                             $5,594.84\nTrade volume                            $47,387.00\nPosition win percent                        55.56%\nTotal positions                                  9\nWon positions                                    5\nLost positions                                   4\nStop losses triggered                            4\nStop loss % of all                          44.44%\nStop loss % of lost                        100.00%\nWinning stop losses                              0\nWinning stop losses percent                  0.00%\nLosing stop losses                               4\nLosing stop losses percent                 100.00%\nTake profits triggered                           0\nTake profit % of all                         0.00%\nTake profit % of won                         0.00%\nZero profit positions                            0\nPositions open at the end                        0\nRealised profit and loss                   $594.84\nPortfolio unrealised value                   $0.00\nExtra returns on lending pool interest       $0.00\nCash left at the end                     $5,594.84\nAverage winning position profit %            6.72%\nAverage losing position loss %              -2.57%\nBiggest winning position %                  12.12%\nBiggest losing position %                   -2.76%\nAverage duration of winning positions       3 days\nAverage duration of losing positions        0 days\nLP fees paid                                $94.87\nLP fees paid % of volume                     0.20%\nAverage position:                            2.59%\nMedian position:                             1.65%\nMost consecutive wins                            2\nMost consecutive losses                          3\nBiggest realized risk                       -1.38%\nAvg realised risk                           -1.28%\nMax pullback of total capital               -4.00%\nMax loss risk at opening of position         1.10%\n```\n\n### Position timeline\n\nHere are individual positions.\n\n![position timeline](./screenshots/timeline.png)\n\n## Example code\n\nThe example strategy is presented as  \n\n- [PineScript source file](./bollinger_band_example_tradingview_strategy.pine) \n- [Backtesting Jupyter Notebook for Trading Strategy](./bollinger_band_example_defi_strategy.ipynb)\n\nStrategy core:\n\n```python\nrsi_series = rsi(close_prices, length=RSI_LENGTH)\n\n# Calculate Bollinger Bands with a 20-day SMA and 2 standard deviations using pandas_ta\n# See documentation here https://tradingstrategy.ai/docs/programming/api/technical-analysis/volatility/help/pandas_ta.volatility.bbands.html#bbands\nbollinger_bands = bbands(close_prices, length=MOVING_AVERAGE_LENGTH, std=STDDEV)\n\n# bbands() returns a dictionary of items with different name mangling\nbb_upper = bollinger_bands[f"BBU_{MOVING_AVERAGE_LENGTH}_{STDDEV}"]\nbb_lower = bollinger_bands[f"BBL_{MOVING_AVERAGE_LENGTH}_{STDDEV}"]\nbb_mid = bollinger_bands[f"BBM_{MOVING_AVERAGE_LENGTH}_{STDDEV}"]  # Moving average\n\nif not position_manager.is_any_open():\n    # No open positions, decide if BUY in this cycle.\n    # We buy if the price on the daily chart closes above the upper Bollinger Band.\n    if price_latest > bb_upper.iloc[-1] and rsi_series[-1] >= RSI_THRESHOLD:\n        buy_amount = cash * POSITION_SIZE\n        trades += position_manager.open_1x_long(\n            pair, \n            buy_amount, \n            stop_loss_pct=STOP_LOSS_PCT)\n\nelse:\n    # We have an open position, decide if SELL in this cycle.\n    # We close the position when the price closes below the 20-day moving average.        \n    if price_latest < bb_mid.iloc[-1]:\n        trades += position_manager.close_all()\n```            \n\n## Notable differences between Python and PineScript\n\nSome major differences between Python and PineScript:\n\n- Python is a general-purpose programming language, making a vast number of tutorials, books and courses available for it.\n- Python is open source - making a vast number of software libraries like technical indicators and statistics available for it.\n- TradingView\'s PineScript is optimised to be used with their service only. It is streamlined, easier to work with,\n  but inflexible.\n- PineScript is fast: backtests complete fast as it is simplified what PineScript can do. \n- Python data is presented as Pandas DataFrame\'s - the de facto core unit of any data science,\n  whereas TradingView uses its own data format.\n- Trading Strategy\'s `decide_trades()` function is designed to suit all kind of strategies, including portfolio construction, lending strategies,\n  liquidity provider positions and such. Thus, it will return a list of trades to be executed on a blockchain to enter a new position\n  and you have more finer-grained control than PineScript\'s entry/exit that has been designed for traditional stock markets.\n\nSome differences traders should note:\n\n- Trading Strategy use a term [position](https://tradingstrategy.ai/glossary/position) to cover a trading position with entry and exit,\n  where as TradingView is using a term *trade*. This might be confusing because a single position consists of multiple trades.\n- Because the price feed is not 1:1 same (different exchanges),\n  different trades will be taken at a different time\n- Depending on a blockchain and DEX, the assets use wrapped token notation.\n  E.g. `ETH` becomes `WETH`. This is due to the technical limitations of [EVM-compatible blockchains](https://tradingstrategy.ai/glossary/evm-compatible).\n\nSome differences programmer\'s should note:\n\n- Python use the zero indexed arrays unlike PineScript that uses reverse arrays. In Python, like in most programming languages,\n  the latest value of time series is in the last index of an array, noted by `-1` and the oldest value is in zero index `0`.\n  In PineScript, this is the opposite, where the latest value is noted without index or index 0.\n\n## About trading on decentralised finance\n\n### DEX trading fees\n\nYou have four elements of fees\n\n- Blockchain transaction costs or [gas fees](https://tradingstrategy.ai/glossary/gas-fee)\n  - Going towards zero and neglible in the future\n- Trading fee, which consists of\n  - [Liquidity provider fee](https://tradingstrategy.ai/glossary/liquidity-provider) \n  - ...and [protocol fee](https://tradingstrategy.ai/glossary/protocol-fee) \n  - Usually 0.05% for large Uniswap v3 pools, otherwise 0.25% - 0.30% on [AMMs](https://tradingstrategy.ai/glossary/amm)\n  - [Compares to 0.60% taker fee on Coinbase, others]()\n- [Price impact](https://tradingstrategy.ai/glossary/price-impact)\n  - Unlike on order book exchanges, this is very easy to historically backtest on AMMs due to deterministic nature of the price\n    based on liquidity\n- [Slippage](https://tradingstrategy.ai/glossary/slippage)\n  - Price change between signing your transction and having a block producer to include it in a block \n  - Also important for [MEV protection](https://tradingstrategy.ai/glossary/mev)\n  - Usually orders are signed with maximum slippage\n- AMM and [CLMM](https://tradingstrategy.ai/glossary/clmm) based DEXes do not have slippage\n\n## Installation\n\nMake a git clone of this repository and then run `poetry` to create a Python environment for your project.\n\n```shell\npoetry shell\npoetry install\n```\n\n### API key\n\nWhen you run the notebook for the first time, you will be prompted to register to give an API key to download Trading Strategy datasets.\n\n## Running backtests\n\n### Running backtest notebooks from terminal\n\nRunning the backtesting notebook in a terminal is the most robust, though not that useful method \n\n- Works always - you see if your code works\n- Opens any charts separate windows in a web browser\n- But it\'s very hard to work with notebooks in a terminal\n- Using shell for notebooks allows e.g. you to use `ipdb` breakpoints in Python code.\n\nHow to run:\n\n```shell\nipython bollinger_band_example_defi_strategy.ipynb \n```\n\nThis will open a couple of browser tabs and print out the trading summary as\n\n### Running backtest notebooks with Visual Studio Code\n\nVisual Studio Code is the recommended tool for the backtest development.\n\nFirst start Poetry environment in a terminal:\n\n```shell\npoetry shell\n```\n\n**Within this shell session**, start Visual Studio Code.\n\n```shell\ncode \n```\n\nOpen a notebook in Visual Studio Code.\n\nUse `Select Kernel` at the top right of the screen. Visual Studio Code should recommend you the same Python virtual environment\nthat is installed with Poetry.\n\nRun the notebook.\n\n### Running backtest notebooks Jupyter\n\nYou can start Jupyter by:\n\n```shell\npoetry shell\njupyter notebook\n```\nThen choose a notebook from the file explorer and run it\n\n## Variations of the backtest example\n\nWe have created some alternatives on the notebook to show how it affects profit and loss\n\nBaseline: Annual return 14%, max drawdown 7%.\n\n- [Trailing stop loss](/delayed_trailing_stop_loss.ipynb) - Annual return 18%, max drawdown 7%\n- [All in](./all_in.ipynb): Use 90% of cash instead of 50% of cash when entering a position. Realised profit $300 -> $600.\n- [Multipair](./multipair.ipynb): Trade more than single pair\n- [Uniswap full history](/uniswap_v2_full_history.ipynb): Trade on ETH-USD pair based on Uniswap v2, so we get max DEX 2020-2023 backtesting history\n- [Uniswap 1h candles](./uniswap_v2_1h_candle_stddev_1.ipynb): Same as above, but trade very frequently\n\n## Next steps\n\n- [Join the Trading Strategy community Discord for discussion and questions](https://tradingstrategy.ai/docs/)\n- [View our learning material for algorithmic trading](https://tradingstrategy.ai/docs/learn/index.html)\n- [Study other strategy backtesting examples and code samples](https://tradingstrategy.ai/docs/programming/index.html)\n\nLinks \n\n- [Trading Strategy website](https://tradingstrategy.ai)\n- [Blog](https://tradingstrategy.ai/blog)\n- [Twitter](https://twitter.com/TradingProtocol)\n- [Discord](https://tradingstrategy.ai/community#discord) \n- [Telegram channel](https://t.me/trading_protocol)\n- [Changelog and version history](https://github.com/tradingstrategy-ai/trading-strategy/blob/master/CHANGELOG.md)\n',
-    'author': 'Mikko Ohtamaa',
-    'author_email': 'mikko@opensourcehacker.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://tradingstrategy.ai',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<3.11',
-}
+[![Watch the recorded workshop session for this project](https://img.youtube.com/vi/Pwst54BGCEM/maxresdefault.jpg)](https://www.youtube.com/watch?v=Pwst54BGCEM)
 
+**[Watch the recorded workshop session on YouTube](https://www.youtube.com/watch?v=Pwst54BGCEM)**
+
+This example repository was made for [Avalanche Summit II workshop](https://tradingstrategy.ai/blog/avalanche-summit-ii-workshop).
+[See the example Github repository here](https://github.com/tradingstrategy-ai/tradingview-defi-strategy).
+
+   * [Benefits of DeFi for algorithmic traders](#benefits-of-defi-for-algorithmic-traders)
+   * [Prerequisites](#prerequisites)
+      * [Your skills](#your-skills)
+      * [Software](#software)
+   * [About the example strategy](#about-the-example-strategy)
+      * [Technical indicator documentation](#technical-indicator-documentation)
+   * [Strategy performance results and algorithm porting notes](#strategy-performance-results-and-algorithm-porting-notes)
+      * [Equity curve](#equity-curve)
+      * [Price action and positions](#price-action-and-positions)
+      * [Trading summary](#trading-summary)
+      * [Position timeline](#position-timeline)
+   * [Example code](#example-code)
+   * [Notable differences between Python and PineScript](#notable-differences-between-python-and-pinescript)
+   * [About trading on decentralised finance](#about-trading-on-decentralised-finance)
+      * [DEX trading fees](#dex-trading-fees)
+   * [Installation](#installation)
+      * [API key](#api-key)
+   * [Running backtests](#running-backtests)
+      * [Running backtest notebooks from terminal](#running-backtest-notebooks-from-terminal)
+      * [Running backtest notebooks with Visual Studio Code](#running-backtest-notebooks-with-visual-studio-code)
+      * [Running backtest notebooks Jupyter](#running-backtest-notebooks-jupyter)
+   * [Variations of the backtest example](#variations-of-the-backtest-example)
+   * [Next steps](#next-steps)
+
+
+## Benefits of DeFi for algorithmic traders
+
+Running your trading strategy on [decentralised exchanges](https://tradingstrategy.ai/glossary/decentralised-exchange) instead of centralised exchanges have several benefits:
+
+- Execute your strategy in a counterparty risk free manner 
+- Broker free, direct to exchange
+- Have 100% control of your strategy market data and live execution
+- [Low trading fees on efficient decentralised markets](https://tradingstrategy.ai/blog/most-efficient-market-is-on-a-public-blockchain-and-decentralised)
+- Convert your trading algorithm to a on-chain fund
+  - Benefits of rich Python quant finance libraries like [pandas_ta](https://github.com/twopirllc/pandas-ta) and [quantstats](https://github.com/ranaroussi/quantstats).
+
+## Prerequisites
+
+### Your skills
+
+To work with this example, you need to have
+
+- Basic experience in cryptocurrencies
+- Basic experience in trading
+- Experience in TradingView's PineScript
+- Junior level experience in Python
+
+### Software 
+
+- Python 3.10
+- [Poetry package manager for Python](https://python-poetry.org/docs/#installing-with-the-official-installer)
+- Git
+
+## About the example strategy
+
+The example strategy backtest is in  [bollinger_band_example_defi_strategy.ipynb](.bollinger_band_example_defi_strategy.ipynb) notebook.
+
+The example strategy is a simple [Bollinger band](https://tradingstrategy.ai/glossary/bollinger-bands) strategy.
+**Whether it makes profit or not is outside the scope of the example.** The strategy is not optimised at all and parameters
+are picked more or less by a gut feeling. Please use this example as learning material and base for your own strategies. 
+
+- Use [Bollinger Band's](https://tradingstrategy.ai/glossary/bollinger-bands) and [RSI](https://tradingstrategy.ai/glossary/relative-strength-index-(rsi)) to determine position entries
+- Long only - suitable for [DEX spot markets](https://tradingstrategy.ai/glossary/spot-market) like Trader Joe
+- 4 hours timeframe for candles
+- Backtesting period of 2024-04-01 - 2023-04-01
+- Use a tight stop loss when entering a position
+  - This will result multiple positions closed for stop loss and few profitable positions during market rallies
+
+- We target the following live trading pairs 
+  - [EAVAXTH/USDC pair on Trader Joe on Avalanche with 20 BPS fee tier](https://tradingstrategy.ai/trading-view/polygon/uniswap-v3/eth-usdc-fee-5).
+    See a note about this in `decide_trades()` Python code.
+  - [Coinbase ETH/USDC with 60 BPS market taker fee](https://help.coinbase.com/en/exchange/trading-and-funding/exchange-fees) (12x more expensive than DeFi)
+ 
+**Note**: Long only strategies are challenging in a descending or sideways cryptocurrencies market like 2021-2023. Furthermore, this strategy was handpicked
+for an overly short backtesting period, to better illustrate the features of the backtesting framework.
+
+### Technical indicator documentation
+
+Find documentation for technical indicators used in the example
+
+- [Exponential Moving Average (EMA)](https://tradingstrategy.ai/docs/programming/api/technical-analysis/overlap/help/pandas_ta.overlap.ema.html#ema):
+  The Exponential Moving Average is a more responsive moving average compared to the Simple Moving Average (SMA). The weights are determined by alpha which is proportional to it’s length. 
+
+- [Relative Strength Index (RSI)](https://tradingstrategy.ai/docs/programming/api/technical-analysis/momentum/help/pandas_ta.momentum.rsi.html#rsi):
+  The Relative Strength Index is a popular momentum oscillator used to measure the velocity as well as the magnitude of directional price movements.
+
+- [Bollinger Bands (BB)](https://tradingstrategy.ai/docs/programming/api/technical-analysis/volatility/help/pandas_ta.volatility.bbands.html#bbands):
+  A popular volatility indicator by John Bollinger.
+
+## Strategy performance results and algorithm porting notes
+
+Both TradingView and Trading Strategy strategies open positions in a similar fashion, so they are more or less comparable.
+
+**Note**. Because of the different price feeds and other subtle differences you cannot have the same strategy backtest
+    result on two different markets: Coinbase and Trader Joe.**. If you carefully examine the price chart, RSI and other indicators,
+    you will see the results vary a bit. In such a small backtesting timeframe, this strategy is prone to small fluxuations
+    and is not robust. The goal of this example, however, is not robustness, but easily demonstrable data.
+
+If you examine, some of positions like ~March 17th are opened around the same time, 
+so we do see that the strategy is following the same pattern.
+
+Both strategy implementations make a low number of trades, 10-20, for the backtesting period.
+This makes it easier to demonstrate the example.
+
+### Equity curve
+
+How well the strategy would have historically performed on AVAX-USDC pair on Trader Joe on Avalanche (20 BPS fee).
+
+![equity curve trading strategy](./screenshots/equity-curve.png)
+
+How well the strategy would have historically performed on AVAX-USD on Coinbase (no fees).
+
+![equity curve coinbase](./screenshots/equity-curve-coinbase.png)
+
+However, if we switch on 50 BPS taker fee on Coinbase we can see it destroys the strategy performance,
+going to loss (vs. 20 BPS fee on Trader Joe).
+
+![equity curve coinbase with fee](./screenshots/equity-curve-coinbase-with-fees.png)
+
+### Positions taken
+
+Here is a screenshot of individual won/lost positions in Python strategy.
+You can see we have few profitable long duration positions, and very short duration
+unprofitable positions.
+
+![positions](./screenshots/positions.png)
+
+
+### Price action and indicators
+
+Here is a screenshot of the price action and technical indicators of the strategy.
+
+![price action and positions](./screenshots/price-action-and-positions.png)
+
+### Trading summary
+
+Summary statistics are calculated as follow:
+
+```                                                
+Trading period length                     145 days
+Return %                                    11.90%
+Annualised return %                         29.88%
+Cash at start                            $5,000.00
+Value at end                             $5,594.84
+Trade volume                            $47,387.00
+Position win percent                        55.56%
+Total positions                                  9
+Won positions                                    5
+Lost positions                                   4
+Stop losses triggered                            4
+Stop loss % of all                          44.44%
+Stop loss % of lost                        100.00%
+Winning stop losses                              0
+Winning stop losses percent                  0.00%
+Losing stop losses                               4
+Losing stop losses percent                 100.00%
+Take profits triggered                           0
+Take profit % of all                         0.00%
+Take profit % of won                         0.00%
+Zero profit positions                            0
+Positions open at the end                        0
+Realised profit and loss                   $594.84
+Portfolio unrealised value                   $0.00
+Extra returns on lending pool interest       $0.00
+Cash left at the end                     $5,594.84
+Average winning position profit %            6.72%
+Average losing position loss %              -2.57%
+Biggest winning position %                  12.12%
+Biggest losing position %                   -2.76%
+Average duration of winning positions       3 days
+Average duration of losing positions        0 days
+LP fees paid                                $94.87
+LP fees paid % of volume                     0.20%
+Average position:                            2.59%
+Median position:                             1.65%
+Most consecutive wins                            2
+Most consecutive losses                          3
+Biggest realized risk                       -1.38%
+Avg realised risk                           -1.28%
+Max pullback of total capital               -4.00%
+Max loss risk at opening of position         1.10%
+```
+
+### Position timeline
+
+Here are individual positions.
+
+![position timeline](./screenshots/timeline.png)
+
+## Example code
+
+The example strategy is presented as  
+
+- [PineScript source file](./bollinger_band_example_tradingview_strategy.pine) 
+- [Backtesting Jupyter Notebook for Trading Strategy](./bollinger_band_example_defi_strategy.ipynb)
+
+Strategy core:
+
+```python
+rsi_series = rsi(close_prices, length=RSI_LENGTH)
+
+# Calculate Bollinger Bands with a 20-day SMA and 2 standard deviations using pandas_ta
+# See documentation here https://tradingstrategy.ai/docs/programming/api/technical-analysis/volatility/help/pandas_ta.volatility.bbands.html#bbands
+bollinger_bands = bbands(close_prices, length=MOVING_AVERAGE_LENGTH, std=STDDEV)
+
+# bbands() returns a dictionary of items with different name mangling
+bb_upper = bollinger_bands[f"BBU_{MOVING_AVERAGE_LENGTH}_{STDDEV}"]
+bb_lower = bollinger_bands[f"BBL_{MOVING_AVERAGE_LENGTH}_{STDDEV}"]
+bb_mid = bollinger_bands[f"BBM_{MOVING_AVERAGE_LENGTH}_{STDDEV}"]  # Moving average
+
+if not position_manager.is_any_open():
+    # No open positions, decide if BUY in this cycle.
+    # We buy if the price on the daily chart closes above the upper Bollinger Band.
+    if price_latest > bb_upper.iloc[-1] and rsi_series[-1] >= RSI_THRESHOLD:
+        buy_amount = cash * POSITION_SIZE
+        trades += position_manager.open_1x_long(
+            pair, 
+            buy_amount, 
+            stop_loss_pct=STOP_LOSS_PCT)
+
+else:
+    # We have an open position, decide if SELL in this cycle.
+    # We close the position when the price closes below the 20-day moving average.        
+    if price_latest < bb_mid.iloc[-1]:
+        trades += position_manager.close_all()
+```            
+
+## Notable differences between Python and PineScript
+
+Some major differences between Python and PineScript:
+
+- Python is a general-purpose programming language, making a vast number of tutorials, books and courses available for it.
+- Python is open source - making a vast number of software libraries like technical indicators and statistics available for it.
+- TradingView's PineScript is optimised to be used with their service only. It is streamlined, easier to work with,
+  but inflexible.
+- PineScript is fast: backtests complete fast as it is simplified what PineScript can do. 
+- Python data is presented as Pandas DataFrame's - the de facto core unit of any data science,
+  whereas TradingView uses its own data format.
+- Trading Strategy's `decide_trades()` function is designed to suit all kind of strategies, including portfolio construction, lending strategies,
+  liquidity provider positions and such. Thus, it will return a list of trades to be executed on a blockchain to enter a new position
+  and you have more finer-grained control than PineScript's entry/exit that has been designed for traditional stock markets.
+
+Some differences traders should note:
+
+- Trading Strategy use a term [position](https://tradingstrategy.ai/glossary/position) to cover a trading position with entry and exit,
+  where as TradingView is using a term *trade*. This might be confusing because a single position consists of multiple trades.
+- Because the price feed is not 1:1 same (different exchanges),
+  different trades will be taken at a different time
+- Depending on a blockchain and DEX, the assets use wrapped token notation.
+  E.g. `ETH` becomes `WETH`. This is due to the technical limitations of [EVM-compatible blockchains](https://tradingstrategy.ai/glossary/evm-compatible).
+
+Some differences programmer's should note:
+
+- Python use the zero indexed arrays unlike PineScript that uses reverse arrays. In Python, like in most programming languages,
+  the latest value of time series is in the last index of an array, noted by `-1` and the oldest value is in zero index `0`.
+  In PineScript, this is the opposite, where the latest value is noted without index or index 0.
+
+## About trading on decentralised finance
+
+### DEX trading fees
+
+You have four elements of fees
+
+- Blockchain transaction costs or [gas fees](https://tradingstrategy.ai/glossary/gas-fee)
+  - Going towards zero and neglible in the future
+- Trading fee, which consists of
+  - [Liquidity provider fee](https://tradingstrategy.ai/glossary/liquidity-provider) 
+  - ...and [protocol fee](https://tradingstrategy.ai/glossary/protocol-fee) 
+  - Usually 0.05% for large Uniswap v3 pools, otherwise 0.25% - 0.30% on [AMMs](https://tradingstrategy.ai/glossary/amm)
+  - [Compares to 0.60% taker fee on Coinbase, others]()
+- [Price impact](https://tradingstrategy.ai/glossary/price-impact)
+  - Unlike on order book exchanges, this is very easy to historically backtest on AMMs due to deterministic nature of the price
+    based on liquidity
+- [Slippage](https://tradingstrategy.ai/glossary/slippage)
+  - Price change between signing your transction and having a block producer to include it in a block 
+  - Also important for [MEV protection](https://tradingstrategy.ai/glossary/mev)
+  - Usually orders are signed with maximum slippage
+- AMM and [CLMM](https://tradingstrategy.ai/glossary/clmm) based DEXes do not have slippage
+
+## Installation
+
+Make a git clone of this repository and then run `poetry` to create a Python environment for your project.
+
+```shell
+poetry shell
+poetry install
+```
+
+### API key
+
+When you run the notebook for the first time, you will be prompted to register to give an API key to download Trading Strategy datasets.
+
+## Running backtests
+
+### Running backtest notebooks from terminal
+
+Running the backtesting notebook in a terminal is the most robust, though not that useful method 
+
+- Works always - you see if your code works
+- Opens any charts separate windows in a web browser
+- But it's very hard to work with notebooks in a terminal
+- Using shell for notebooks allows e.g. you to use `ipdb` breakpoints in Python code.
+
+How to run:
+
+```shell
+ipython bollinger_band_example_defi_strategy.ipynb 
+```
+
+This will open a couple of browser tabs and print out the trading summary as
+
+### Running backtest notebooks with Visual Studio Code
+
+Visual Studio Code is the recommended tool for the backtest development.
+
+First start Poetry environment in a terminal:
+
+```shell
+poetry shell
+```
+
+**Within this shell session**, start Visual Studio Code.
+
+```shell
+code 
+```
+
+Open a notebook in Visual Studio Code.
+
+Use `Select Kernel` at the top right of the screen. Visual Studio Code should recommend you the same Python virtual environment
+that is installed with Poetry.
+
+Run the notebook.
+
+### Running backtest notebooks Jupyter
+
+You can start Jupyter by:
+
+```shell
+poetry shell
+jupyter notebook
+```
+Then choose a notebook from the file explorer and run it
+
+## Variations of the backtest example
+
+We have created some alternatives on the notebook to show how it affects profit and loss
+
+Baseline: Annual return 14%, max drawdown 7%.
+
+- [Trailing stop loss](/delayed_trailing_stop_loss.ipynb) - Annual return 18%, max drawdown 7%
+- [All in](./all_in.ipynb): Use 90% of cash instead of 50% of cash when entering a position. Realised profit $300 -> $600.
+- [Multipair](./multipair.ipynb): Trade more than single pair
+- [Uniswap full history](/uniswap_v2_full_history.ipynb): Trade on ETH-USD pair based on Uniswap v2, so we get max DEX 2020-2023 backtesting history
+- [Uniswap 1h candles](./uniswap_v2_1h_candle_stddev_1.ipynb): Same as above, but trade very frequently
+
+Grid searches
+
+- [Grid search - basic](./grid_search.ipynb): Automatically search through strategy parameters for an optional combination
+- [Grid search - multiprocessing](./uniswao_grid_search.ipynb): Optimise strategy parameters over larger dataset and parameter space using Python multiprocessing
+
+## Next steps
+
+- [Join the Trading Strategy community Discord for discussion and questions](https://tradingstrategy.ai/docs/)
+- [View our learning material for algorithmic trading](https://tradingstrategy.ai/docs/learn/index.html)
+- [Study other strategy backtesting examples and code samples](https://tradingstrategy.ai/docs/programming/index.html)
+
+Links 
+
+- [Trading Strategy website](https://tradingstrategy.ai)
+- [Blog](https://tradingstrategy.ai/blog)
+- [Twitter](https://twitter.com/TradingProtocol)
+- [Discord](https://tradingstrategy.ai/community#discord) 
+- [Telegram channel](https://t.me/trading_protocol)
+- [Changelog and version history](https://github.com/tradingstrategy-ai/trading-strategy/blob/master/CHANGELOG.md)
 
-setup(**setup_kwargs)
```

