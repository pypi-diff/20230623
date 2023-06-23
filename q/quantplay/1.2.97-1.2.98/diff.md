# Comparing `tmp/quantplay-1.2.97.tar.gz` & `tmp/quantplay-1.2.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.2.97.tar", last modified: Fri Jun  9 05:01:11 2023, max compression
+gzip compressed data, was "quantplay-1.2.98.tar", last modified: Fri Jun 23 06:50:58 2023, max compression
```

## Comparing `quantplay-1.2.97.tar` & `quantplay-1.2.98.tar`

### file list

```diff
@@ -1,139 +1,140 @@
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.673107 quantplay-1.2.97/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-09 05:01:11.673187 quantplay-1.2.97/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.2.97/README.md
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.649835 quantplay-1.2.97/quantplay/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.650754 quantplay-1.2.97/quantplay/backtest/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/backtest/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.2.97/quantplay/backtest/backtest_trades.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.653565 quantplay-1.2.97/quantplay/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/broker/angelone.py
--rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/broker/broker_client.py
--rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/broker/client.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.654031 quantplay-1.2.97/quantplay/broker/finvasia_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/broker/finvasia_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.2.97/quantplay/broker/finvasia_utils/shoonya.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.654410 quantplay-1.2.97/quantplay/broker/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/broker/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.2.97/quantplay/broker/generics/broker.py
--rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.2.97/quantplay/broker/iifl.py
--rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.2.97/quantplay/broker/iifl_xts.py
--rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/broker/kite_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/broker/motilal.py
--rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.2.97/quantplay/broker/shoonya.py
--rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.2.97/quantplay/broker/symphony.py
--rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-09 05:00:32.000000 quantplay-1.2.97/quantplay/broker/xts.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.656312 quantplay-1.2.97/quantplay/broker/xts_utils/
--rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.2.97/quantplay/broker/xts_utils/Connect.py
--rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/broker/xts_utils/Exception.py
--rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.2.97/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/broker/xts_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17192 2023-05-23 09:41:25.000000 quantplay-1.2.97/quantplay/broker/zerodha.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.656754 quantplay-1.2.97/quantplay/brokerage/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/brokerage/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.657474 quantplay-1.2.97/quantplay/brokerage/angelone/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/brokerage/angelone/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/brokerage/angelone/angel_broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.658299 quantplay-1.2.97/quantplay/brokerage/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/brokerage/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28081 2023-04-26 18:39:03.000000 quantplay-1.2.97/quantplay/brokerage/generics/broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.659072 quantplay-1.2.97/quantplay/brokerage/zerodha/
--rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.2.97/quantplay/brokerage/zerodha/ZBroker.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/brokerage/zerodha/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.659281 quantplay-1.2.97/quantplay/config/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/config/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/config/qplay_config.py
--rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/create_sample_data.py
--rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.2.97/quantplay/data_modify_script.py
--rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-04-19 06:37:00.000000 quantplay-1.2.97/quantplay/date_fix.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.659600 quantplay-1.2.97/quantplay/exception/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/exception/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/exception/exceptions.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.659871 quantplay-1.2.97/quantplay/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.660483 quantplay-1.2.97/quantplay/indicators/
--rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/indicators/Indicator.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/indicators/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/indicators/atr.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.660750 quantplay-1.2.97/quantplay/model/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/model/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.662253 quantplay-1.2.97/quantplay/model/exchange/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/model/exchange/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/model/exchange/instrument.py
--rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.2.97/quantplay/model/exchange/order.py
--rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/model/exchange/tick.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.662492 quantplay-1.2.97/quantplay/model/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/model/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/model/strategy/strategy_response.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.662657 quantplay-1.2.97/quantplay/oms/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/oms/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.663470 quantplay-1.2.97/quantplay/order_execution/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/order_execution/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/order_execution/execution_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/order_execution/mean_price.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.664214 quantplay-1.2.97/quantplay/reporting/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/reporting/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10780 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/reporting/strategy_report.py
--rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.2.97/quantplay/reporting/visuals.py
--rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.2.97/quantplay/service.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.665179 quantplay-1.2.97/quantplay/services/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/services/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.2.97/quantplay/services/market.py
--rw-r--r--   0 ashok      (502) staff       (20)    10889 2023-06-05 16:09:13.000000 quantplay-1.2.97/quantplay/services/tradelens.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.665469 quantplay-1.2.97/quantplay/strategies/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.2.97/quantplay/strategies/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.665613 quantplay-1.2.97/quantplay/strategies/equities/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.2.97/quantplay/strategies/equities/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.665741 quantplay-1.2.97/quantplay/strategies/equities/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.2.97/quantplay/strategies/equities/intraday/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.665863 quantplay-1.2.97/quantplay/strategies/equities/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.2.97/quantplay/strategies/equities/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.666043 quantplay-1.2.97/quantplay/strategies/futures/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.2.97/quantplay/strategies/futures/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.666500 quantplay-1.2.97/quantplay/strategies/futures/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.2.97/quantplay/strategies/futures/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.666639 quantplay-1.2.97/quantplay/strategies/options/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.2.97/quantplay/strategies/options/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.667691 quantplay-1.2.97/quantplay/strategies/options/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.2.97/quantplay/strategies/options/intraday/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.2.97/quantplay/strategies/options/intraday/ladder.py
--rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.2.97/quantplay/strategies/options/intraday/musk.py
--rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.2.97/quantplay/strategies/options/intraday/short_straddle.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.668093 quantplay-1.2.97/quantplay/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.2.97/quantplay/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.2.97/quantplay/strategy_run.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.670741 quantplay-1.2.97/quantplay/utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/utils/config_util.py
--rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.2.97/quantplay/utils/constant.py
--rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.2.97/quantplay/utils/data_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/utils/exchange.py
--rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/utils/number_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/utils/pickle_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/utils/selenium_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.2.97/quantplay/utils/transaction_utils.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.650541 quantplay-1.2.97/quantplay.egg-info/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-09 05:01:11.000000 quantplay-1.2.97/quantplay.egg-info/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-06-09 05:01:11.000000 quantplay-1.2.97/quantplay.egg-info/SOURCES.txt
--rw-r--r--   0 ashok      (502) staff       (20)        1 2023-06-09 05:01:11.000000 quantplay-1.2.97/quantplay.egg-info/dependency_links.txt
--rw-r--r--   0 ashok      (502) staff       (20)      221 2023-06-09 05:01:11.000000 quantplay-1.2.97/quantplay.egg-info/requires.txt
--rw-r--r--   0 ashok      (502) staff       (20)       15 2023-06-09 05:01:11.000000 quantplay-1.2.97/quantplay.egg-info/top_level.txt
--rw-r--r--   0 ashok      (502) staff       (20)       49 2023-06-09 05:01:11.673468 quantplay-1.2.97/setup.cfg
--rw-r--r--   0 ashok      (502) staff       (20)      876 2023-06-09 05:01:08.000000 quantplay-1.2.97/setup.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.671053 quantplay-1.2.97/test/
--rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.2.97/test/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.671428 quantplay-1.2.97/test/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/test/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.2.97/test/broker/finvasia.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.671744 quantplay-1.2.97/test/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/test/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.2.97/test/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-09 05:01:11.672884 quantplay-1.2.97/test/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.97/test/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.2.97/test/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.2.97/test/strategy/sample_strategy.py
--rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.2.97/test/test_motilal.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.755872 quantplay-1.2.98/
+-rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-23 06:50:58.755923 quantplay-1.2.98/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.2.98/README.md
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.740078 quantplay-1.2.98/quantplay/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.740951 quantplay-1.2.98/quantplay/backtest/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/backtest/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.2.98/quantplay/backtest/backtest_trades.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.743541 quantplay-1.2.98/quantplay/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/angelone.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/broker_client.py
+-rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/client.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.743968 quantplay-1.2.98/quantplay/broker/finvasia_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/finvasia_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.2.98/quantplay/broker/finvasia_utils/shoonya.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.744307 quantplay-1.2.98/quantplay/broker/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.2.98/quantplay/broker/generics/broker.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.2.98/quantplay/broker/iifl.py
+-rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.2.98/quantplay/broker/iifl_xts.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/kite_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/motilal.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.2.98/quantplay/broker/shoonya.py
+-rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.2.98/quantplay/broker/symphony.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-09 05:00:32.000000 quantplay-1.2.98/quantplay/broker/xts.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.745756 quantplay-1.2.98/quantplay/broker/xts_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.2.98/quantplay/broker/xts_utils/Connect.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/xts_utils/Exception.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.2.98/quantplay/broker/xts_utils/InteractiveSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/xts_utils/MarketDataSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/broker/xts_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17192 2023-05-23 09:41:25.000000 quantplay-1.2.98/quantplay/broker/zerodha.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.745848 quantplay-1.2.98/quantplay/brokerage/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/brokerage/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.746026 quantplay-1.2.98/quantplay/brokerage/angelone/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/brokerage/angelone/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/brokerage/angelone/angel_broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.746425 quantplay-1.2.98/quantplay/brokerage/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/brokerage/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28081 2023-04-26 18:39:03.000000 quantplay-1.2.98/quantplay/brokerage/generics/broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.747161 quantplay-1.2.98/quantplay/brokerage/zerodha/
+-rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.2.98/quantplay/brokerage/zerodha/ZBroker.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/brokerage/zerodha/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.747380 quantplay-1.2.98/quantplay/config/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/config/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/config/qplay_config.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/create_sample_data.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.2.98/quantplay/data_modify_script.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.2.98/quantplay/date_fix.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.747614 quantplay-1.2.98/quantplay/exception/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/exception/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/exception/exceptions.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.747934 quantplay-1.2.98/quantplay/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.748654 quantplay-1.2.98/quantplay/indicators/
+-rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/indicators/Indicator.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/indicators/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/indicators/atr.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.748800 quantplay-1.2.98/quantplay/model/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.749405 quantplay-1.2.98/quantplay/model/exchange/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/exchange/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/exchange/instrument.py
+-rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.2.98/quantplay/model/exchange/order.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/exchange/tick.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.749650 quantplay-1.2.98/quantplay/model/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/model/strategy/strategy_response.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.749789 quantplay-1.2.98/quantplay/oms/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/oms/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.750149 quantplay-1.2.98/quantplay/order_execution/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/order_execution/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/order_execution/execution_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/order_execution/mean_price.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.750496 quantplay-1.2.98/quantplay/reporting/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/reporting/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.2.98/quantplay/reporting/strategy_report.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.2.98/quantplay/reporting/visuals.py
+-rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.2.98/quantplay/service.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751332 quantplay-1.2.98/quantplay/services/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/services/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-06-23 06:49:50.000000 quantplay-1.2.98/quantplay/services/alphawiz.py
+-rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.2.98/quantplay/services/market.py
+-rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.2.98/quantplay/services/tradelens.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751456 quantplay-1.2.98/quantplay/strategies/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.2.98/quantplay/strategies/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751558 quantplay-1.2.98/quantplay/strategies/equities/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.2.98/quantplay/strategies/equities/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751666 quantplay-1.2.98/quantplay/strategies/equities/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.2.98/quantplay/strategies/equities/intraday/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751775 quantplay-1.2.98/quantplay/strategies/equities/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.2.98/quantplay/strategies/equities/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751879 quantplay-1.2.98/quantplay/strategies/futures/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.2.98/quantplay/strategies/futures/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.751977 quantplay-1.2.98/quantplay/strategies/futures/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.2.98/quantplay/strategies/futures/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.752078 quantplay-1.2.98/quantplay/strategies/options/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.2.98/quantplay/strategies/options/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.752819 quantplay-1.2.98/quantplay/strategies/options/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.2.98/quantplay/strategies/options/intraday/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.2.98/quantplay/strategies/options/intraday/ladder.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.2.98/quantplay/strategies/options/intraday/musk.py
+-rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.2.98/quantplay/strategies/options/intraday/short_straddle.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.753078 quantplay-1.2.98/quantplay/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.2.98/quantplay/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.2.98/quantplay/strategy_run.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.754647 quantplay-1.2.98/quantplay/utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/config_util.py
+-rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.2.98/quantplay/utils/constant.py
+-rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.2.98/quantplay/utils/data_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/exchange.py
+-rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/number_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/pickle_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/selenium_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.2.98/quantplay/utils/transaction_utils.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.740740 quantplay-1.2.98/quantplay.egg-info/
+-rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-23 06:50:58.000000 quantplay-1.2.98/quantplay.egg-info/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)     3422 2023-06-23 06:50:58.000000 quantplay-1.2.98/quantplay.egg-info/SOURCES.txt
+-rw-r--r--   0 ashok      (502) staff       (20)        1 2023-06-23 06:50:58.000000 quantplay-1.2.98/quantplay.egg-info/dependency_links.txt
+-rw-r--r--   0 ashok      (502) staff       (20)      221 2023-06-23 06:50:58.000000 quantplay-1.2.98/quantplay.egg-info/requires.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       15 2023-06-23 06:50:58.000000 quantplay-1.2.98/quantplay.egg-info/top_level.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       49 2023-06-23 06:50:58.756115 quantplay-1.2.98/setup.cfg
+-rw-r--r--   0 ashok      (502) staff       (20)      876 2023-06-23 06:50:55.000000 quantplay-1.2.98/setup.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.754904 quantplay-1.2.98/test/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.2.98/test/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.755138 quantplay-1.2.98/test/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/broker/finvasia.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.755374 quantplay-1.2.98/test/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-23 06:50:58.755751 quantplay-1.2.98/test/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/strategy/sample_strategy.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.2.98/test/test_motilal.py
```

### Comparing `quantplay-1.2.97/PKG-INFO` & `quantplay-1.2.98/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.2.97
+Version: 1.2.98
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.97/quantplay/backtest/backtest_trades.py` & `quantplay-1.2.98/quantplay/backtest/backtest_trades.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/angelone.py` & `quantplay-1.2.98/quantplay/broker/angelone.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/broker_client.py` & `quantplay-1.2.98/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/finvasia_utils/shoonya.py` & `quantplay-1.2.98/quantplay/broker/finvasia_utils/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/generics/broker.py` & `quantplay-1.2.98/quantplay/broker/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/iifl.py` & `quantplay-1.2.98/quantplay/broker/iifl.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/iifl_xts.py` & `quantplay-1.2.98/quantplay/broker/iifl_xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/kite_utils.py` & `quantplay-1.2.98/quantplay/broker/kite_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/motilal.py` & `quantplay-1.2.98/quantplay/broker/motilal.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/shoonya.py` & `quantplay-1.2.98/quantplay/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/symphony.py` & `quantplay-1.2.98/quantplay/broker/symphony.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/xts.py` & `quantplay-1.2.98/quantplay/broker/xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/xts_utils/Connect.py` & `quantplay-1.2.98/quantplay/broker/xts_utils/Connect.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/xts_utils/Exception.py` & `quantplay-1.2.98/quantplay/broker/xts_utils/Exception.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/xts_utils/InteractiveSocketClient.py` & `quantplay-1.2.98/quantplay/broker/xts_utils/InteractiveSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/xts_utils/MarketDataSocketClient.py` & `quantplay-1.2.98/quantplay/broker/xts_utils/MarketDataSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/broker/zerodha.py` & `quantplay-1.2.98/quantplay/broker/zerodha.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/brokerage/angelone/angel_broker.py` & `quantplay-1.2.98/quantplay/brokerage/angelone/angel_broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/brokerage/generics/broker.py` & `quantplay-1.2.98/quantplay/brokerage/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.2.98/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/config/qplay_config.py` & `quantplay-1.2.98/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/create_sample_data.py` & `quantplay-1.2.98/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/data_modify_script.py` & `quantplay-1.2.98/quantplay/data_modify_script.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/date_fix.py` & `quantplay-1.2.98/quantplay/date_fix.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/exception/exceptions.py` & `quantplay-1.2.98/quantplay/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/executor/strategy_executor.py` & `quantplay-1.2.98/quantplay/executor/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/indicators/Indicator.py` & `quantplay-1.2.98/quantplay/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/model/exchange/instrument.py` & `quantplay-1.2.98/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/model/exchange/order.py` & `quantplay-1.2.98/quantplay/model/exchange/order.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/model/exchange/tick.py` & `quantplay-1.2.98/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.2.98/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/order_execution/mean_price.py` & `quantplay-1.2.98/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/reporting/strategy_report.py` & `quantplay-1.2.98/quantplay/reporting/strategy_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,16 +126,16 @@
         VisualReport.display_balance_report(portfolio, file_prefix=file_prefix)
 
     @staticmethod
     def add_more_params(portfolio, cm_slippage=0, fno_slippage=0):
         # Basic trade checks
         portfolio = portfolio[portfolio.close_price > 0]
         portfolio = portfolio[portfolio.entry_price > 0]
-
         portfolio.loc[:, "order_timestamp"] = pd.to_datetime(portfolio["order_timestamp"])
+      
         portfolio.loc[:, "order_timestamp"] = portfolio.sort_values("order_timestamp")
 
         portfolio.loc[:, "profit"] = portfolio.exposure * (
             1 - portfolio.close_price / portfolio.entry_price
         )
 
         portfolio.loc[:, Order.profit] = np.where(
@@ -150,14 +150,15 @@
             portfolio.exchange == ExchangeName.nse,
             portfolio.profit - portfolio.exposure * cm_slippage,
             portfolio.profit - portfolio.exposure * fno_slippage,
         )
 
         portfolio.loc[:, "pct_profit"] = portfolio.profit / portfolio.exposure
 
+
         portfolio.loc[:, "day_of_week"] = portfolio.order_timestamp.dt.day_name()
         portfolio.loc[:, "point_diff"] = np.where(
             portfolio[Order.transaction_type] == Order.sell_transaction,
             portfolio.entry_price - portfolio.close_price,
             portfolio.close_price - portfolio.entry_price,
         )
 
@@ -216,16 +217,16 @@
         response["total_profit"] = portfolio["profit"].sum()
 
         portfolio.loc[:, "balance"] = portfolio.profit.cumsum()
 
         portfolio.loc[:, "date"] = portfolio.order_timestamp.dt.date
 
         # unique stock count
-        t_df = portfolio.groupby("date").symbol.nunique().reset_index()
-        response[StrategyMetricsTableColumns.unique_stocks] = int(t_df.symbol.mean())
+        t_df = portfolio.groupby("date").tradingsymbol.nunique().reset_index()
+        response[StrategyMetricsTableColumns.unique_stocks] = int(t_df.tradingsymbol.mean())
 
         day_wise_pnl = portfolio.groupby(["date"])["profit"].sum().reset_index()
         day_wise_pnl = day_wise_pnl.sort_values("date")
 
         day_wise_pnl.loc[:, "is_loss"] = np.where(day_wise_pnl.profit > 0, 0, 1)
         m = day_wise_pnl.is_loss.astype(bool)
         day_wise_pnl.loc[:, "loss_streak"] = (
```

### Comparing `quantplay-1.2.97/quantplay/reporting/visuals.py` & `quantplay-1.2.98/quantplay/reporting/visuals.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/services/market.py` & `quantplay-1.2.98/quantplay/services/market.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/services/tradelens.py` & `quantplay-1.2.98/quantplay/services/tradelens.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import plotly.graph_objects as go
 import pandas as pd
 from quantplay.reporting.visuals import VisualReport
 from quantplay.services.market import Market
 import matplotlib.pyplot as plt
 import inspect
 import typing
+from quantplay.reporting.strategy_report import StrategyReport
 
 market = Market()
 
 
 class TradeLens:
 
     @staticmethod
@@ -22,17 +23,33 @@
                                      high=df['high'],
                                      low=df['low'],
                                      close=df['close']))
         fig.update(layout_xaxis_rangeslider_visible=False)
         fig.show()
 
     @staticmethod
+    def generate_report(trades, columns=None):
+        response = StrategyReport.generate_report(trades)
+        result = pd.DataFrame(response)
+
+        if columns:
+            result = result[columns]
+        with pd.option_context('display.max_rows', None, 'display.max_columns',
+                               None):  # more options can be specified also
+            print(result)
+    @staticmethod
     def max_drawdowns(trades):
         trades = trades.sort_values("order_timestamp")
         temp_df = trades[['order_timestamp', 'profit']]
+        
+        temp_df.loc[:,'order_timestamp'] = pd.to_datetime(temp_df['order_timestamp'])
+        temp_df.loc[:, "date_only"] = trades.order_timestamp.dt.date
+        temp_df = temp_df.groupby(["date_only"])["profit"].sum().reset_index()
+        temp_df = temp_df.sort_values("date_only")
+        
 
         for j in range(0, 5):
             temp_df.loc[:, 'balance'] = temp_df.profit.cumsum()
             temp_df.loc[:, 'running_max_balance'] = np.maximum.accumulate(
                 temp_df.balance)
             temp_df.loc[:, 'drawdowns'] = temp_df.running_max_balance - \
                 temp_df.balance
@@ -46,19 +63,19 @@
 
                 start_index = end_index
                 while temp_df.iloc[start_index - 1]['running_max_balance'] == temp_df.iloc[start_index][
                         'running_max_balance']:
                     start_index = start_index - 1
 
                 print("Max drawdown {} from {} till {} amount {}".format(j,
-                                                                         temp_df.iloc[start_index]['order_timestamp'],
-                                                                         temp_df.iloc[end_index]['order_timestamp'],
+                                                                         temp_df.iloc[start_index]['date_only'],
+                                                                         temp_df.iloc[end_index]['date_only'],
                                                                          max_drawdown))
 
-                temp_df = temp_df.drop(temp_df.index[start_index:end_index])
+                temp_df = temp_df.drop(temp_df.index[start_index:end_index+1])
                 break
 
     @staticmethod
     def analyse(trades, disable_metrics=[]):
         trades.loc[:, 'date'] = pd.to_datetime(trades.date)
         exchanges = list(trades.exchange.unique())
         trades.loc[:, 'segment'] = np.where(
```

### Comparing `quantplay-1.2.97/quantplay/strategies/options/intraday/ladder.py` & `quantplay-1.2.98/quantplay/strategies/options/intraday/ladder.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/strategies/options/intraday/musk.py` & `quantplay-1.2.98/quantplay/strategies/options/intraday/musk.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/strategy/base.py` & `quantplay-1.2.98/quantplay/strategy/base.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/utils/config_util.py` & `quantplay-1.2.98/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/utils/constant.py` & `quantplay-1.2.98/quantplay/utils/constant.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/utils/data_utils.py` & `quantplay-1.2.98/quantplay/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/utils/exchange.py` & `quantplay-1.2.98/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/utils/number_utils.py` & `quantplay-1.2.98/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/utils/selenium_utils.py` & `quantplay-1.2.98/quantplay/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay/utils/transaction_utils.py` & `quantplay-1.2.98/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/quantplay.egg-info/PKG-INFO` & `quantplay-1.2.98/quantplay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.2.97
+Version: 1.2.98
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.97/quantplay.egg-info/SOURCES.txt` & `quantplay-1.2.98/quantplay.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 quantplay/order_execution/__init__.py
 quantplay/order_execution/execution_algorithm.py
 quantplay/order_execution/mean_price.py
 quantplay/reporting/__init__.py
 quantplay/reporting/strategy_report.py
 quantplay/reporting/visuals.py
 quantplay/services/__init__.py
+quantplay/services/alphawiz.py
 quantplay/services/market.py
 quantplay/services/tradelens.py
 quantplay/strategies/__init__.py
 quantplay/strategies/equities/__init__.py
 quantplay/strategies/equities/intraday/__init__.py
 quantplay/strategies/equities/overnight/__init__.py
 quantplay/strategies/futures/__init__.py
```

### Comparing `quantplay-1.2.97/setup.py` & `quantplay-1.2.98/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.2.97",
+    version="1.2.98",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.2.97/test/strategy/sample_strategy.py` & `quantplay-1.2.98/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.97/test/test_motilal.py` & `quantplay-1.2.98/test/test_motilal.py`

 * *Files identical despite different names*

