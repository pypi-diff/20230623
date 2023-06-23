# Comparing `tmp/fmpsdk-20230522.0.tar.gz` & `tmp/fmpsdk-20230623.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmpsdk-20230522.0.tar", last modified: Mon May 22 14:13:32 2023, max compression
+gzip compressed data, was "fmpsdk-20230623.0.tar", last modified: Fri Jun 23 14:11:11 2023, max compression
```

## Comparing `fmpsdk-20230522.0.tar` & `fmpsdk-20230623.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-05-22 14:13:32.449701 fmpsdk-20230522.0/
--rw-r--r--   0 dmickelson   (503) staff       (20)     1500 2022-12-05 15:16:07.000000 fmpsdk-20230522.0/LICENSE.md
--rw-r--r--   0 dmickelson   (503) staff       (20)      877 2023-05-22 14:13:32.449768 fmpsdk-20230522.0/PKG-INFO
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-05-22 14:13:32.448870 fmpsdk-20230522.0/fmpsdk/
--rw-r--r--   0 dmickelson   (503) staff       (20)     5730 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/__init__.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     2607 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/alternative_data.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     4117 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/calendar.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      728 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/commodities.py
--rw-r--r--   0 dmickelson   (503) staff       (20)    28897 2023-05-22 14:07:52.000000 fmpsdk-20230522.0/fmpsdk/company_valuation.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      749 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/cryptocurrencies.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1561 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/etf.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      714 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/euronext.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1022 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/forex.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     3076 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/general.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     3053 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/insider_trading.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     5203 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/institutional_fund.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     4410 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/market_indexes.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      735 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/mutual_funds.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1782 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/senate.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     8572 2023-05-22 14:07:52.000000 fmpsdk-20230522.0/fmpsdk/settings.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1774 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/stock_market.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     2186 2023-05-22 14:07:52.000000 fmpsdk-20230522.0/fmpsdk/stock_time_series.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      949 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/technical_indicators.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      684 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/tsx.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     6361 2023-05-22 14:07:52.000000 fmpsdk-20230522.0/fmpsdk/url_methods.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-05-22 14:13:32.449602 fmpsdk-20230522.0/fmpsdk.egg-info/
--rw-r--r--   0 dmickelson   (503) staff       (20)      877 2023-05-22 14:13:32.000000 fmpsdk-20230522.0/fmpsdk.egg-info/PKG-INFO
--rw-r--r--   0 dmickelson   (503) staff       (20)      659 2023-05-22 14:13:32.000000 fmpsdk-20230522.0/fmpsdk.egg-info/SOURCES.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)        1 2023-05-22 14:13:32.000000 fmpsdk-20230522.0/fmpsdk.egg-info/dependency_links.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)       23 2023-05-22 14:13:32.000000 fmpsdk-20230522.0/fmpsdk.egg-info/requires.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)        7 2023-05-22 14:13:32.000000 fmpsdk-20230522.0/fmpsdk.egg-info/top_level.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)      222 2022-12-05 15:16:06.000000 fmpsdk-20230522.0/pyproject.toml
--rw-r--r--   0 dmickelson   (503) staff       (20)       91 2023-05-22 14:13:32.450072 fmpsdk-20230522.0/setup.cfg
--rw-r--r--   0 dmickelson   (503) staff       (20)     1369 2023-05-22 14:11:30.000000 fmpsdk-20230522.0/setup.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-06-23 14:11:11.295433 fmpsdk-20230623.0/
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1500 2022-12-05 15:16:07.000000 fmpsdk-20230623.0/LICENSE.md
+-rw-r--r--   0 dmickelson   (503) staff       (20)      877 2023-06-23 14:11:11.295489 fmpsdk-20230623.0/PKG-INFO
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-06-23 14:11:11.294878 fmpsdk-20230623.0/fmpsdk/
+-rw-r--r--   0 dmickelson   (503) staff       (20)     5730 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/__init__.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     2607 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/alternative_data.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     4117 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/calendar.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      728 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/commodities.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)    28897 2023-05-22 14:07:52.000000 fmpsdk-20230623.0/fmpsdk/company_valuation.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      749 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/cryptocurrencies.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1561 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/etf.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      714 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/euronext.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1022 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/forex.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     3063 2023-06-23 13:54:50.000000 fmpsdk-20230623.0/fmpsdk/general.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     3053 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/insider_trading.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     5203 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/institutional_fund.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     4410 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/market_indexes.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      735 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/mutual_funds.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1782 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/senate.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     8572 2023-05-22 14:07:52.000000 fmpsdk-20230623.0/fmpsdk/settings.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1774 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/stock_market.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     2186 2023-05-22 14:07:52.000000 fmpsdk-20230623.0/fmpsdk/stock_time_series.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      949 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/technical_indicators.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      684 2022-12-05 15:16:05.000000 fmpsdk-20230623.0/fmpsdk/tsx.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     6361 2023-05-22 14:07:52.000000 fmpsdk-20230623.0/fmpsdk/url_methods.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-06-23 14:11:11.295342 fmpsdk-20230623.0/fmpsdk.egg-info/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      877 2023-06-23 14:11:11.000000 fmpsdk-20230623.0/fmpsdk.egg-info/PKG-INFO
+-rw-r--r--   0 dmickelson   (503) staff       (20)      659 2023-06-23 14:11:11.000000 fmpsdk-20230623.0/fmpsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)        1 2023-06-23 14:11:11.000000 fmpsdk-20230623.0/fmpsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)       23 2023-06-23 14:11:11.000000 fmpsdk-20230623.0/fmpsdk.egg-info/requires.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)        7 2023-06-23 14:11:11.000000 fmpsdk-20230623.0/fmpsdk.egg-info/top_level.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)      305 2023-06-23 14:04:44.000000 fmpsdk-20230623.0/pyproject.toml
+-rw-r--r--   0 dmickelson   (503) staff       (20)       91 2023-06-23 14:11:11.295750 fmpsdk-20230623.0/setup.cfg
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1369 2023-06-23 14:10:46.000000 fmpsdk-20230623.0/setup.py
```

### Comparing `fmpsdk-20230522.0/LICENSE.md` & `fmpsdk-20230623.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/PKG-INFO` & `fmpsdk-20230623.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpsdk
-Version: 20230522.0
+Version: 20230623.0
 Summary: SDK for interacting with FMP's APIs.
 Home-page: https://github.com/daxm/fmpsdk
 Author: Dax Mickelson
 Author-email: fmp@daxm.net
 License: BSD
 Keywords: fmpsdk financial stock valuation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fmpsdk-20230522.0/fmpsdk/__init__.py` & `fmpsdk-20230623.0/fmpsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/alternative_data.py` & `fmpsdk-20230623.0/fmpsdk/alternative_data.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/calendar.py` & `fmpsdk-20230623.0/fmpsdk/calendar.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/commodities.py` & `fmpsdk-20230623.0/fmpsdk/commodities.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/company_valuation.py` & `fmpsdk-20230623.0/fmpsdk/company_valuation.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/cryptocurrencies.py` & `fmpsdk-20230623.0/fmpsdk/cryptocurrencies.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/etf.py` & `fmpsdk-20230623.0/fmpsdk/etf.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/euronext.py` & `fmpsdk-20230623.0/fmpsdk/euronext.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/forex.py` & `fmpsdk-20230623.0/fmpsdk/forex.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/general.py` & `fmpsdk-20230623.0/fmpsdk/general.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,10 +87,9 @@
         query_vars["serietype"] = __validate_series_type(series_type)
     if from_date:
         query_vars["from"] = from_date
     if to_date:
         query_vars["to"] = to_date
 
     res = __return_json_v3(path=path, query_vars=query_vars)
-    if res is None or len(res) == 0:
-        return res
-    return res["historical"]
+
+    return res.get("historicalStockList", res.get('historical', None))
```

### Comparing `fmpsdk-20230522.0/fmpsdk/insider_trading.py` & `fmpsdk-20230623.0/fmpsdk/insider_trading.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/institutional_fund.py` & `fmpsdk-20230623.0/fmpsdk/institutional_fund.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/market_indexes.py` & `fmpsdk-20230623.0/fmpsdk/market_indexes.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/mutual_funds.py` & `fmpsdk-20230623.0/fmpsdk/mutual_funds.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/senate.py` & `fmpsdk-20230623.0/fmpsdk/senate.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/settings.py` & `fmpsdk-20230623.0/fmpsdk/settings.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/stock_market.py` & `fmpsdk-20230623.0/fmpsdk/stock_market.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/stock_time_series.py` & `fmpsdk-20230623.0/fmpsdk/stock_time_series.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/technical_indicators.py` & `fmpsdk-20230623.0/fmpsdk/technical_indicators.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/tsx.py` & `fmpsdk-20230623.0/fmpsdk/tsx.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk/url_methods.py` & `fmpsdk-20230623.0/fmpsdk/url_methods.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/fmpsdk.egg-info/PKG-INFO` & `fmpsdk-20230623.0/fmpsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpsdk
-Version: 20230522.0
+Version: 20230623.0
 Summary: SDK for interacting with FMP's APIs.
 Home-page: https://github.com/daxm/fmpsdk
 Author: Dax Mickelson
 Author-email: fmp@daxm.net
 License: BSD
 Keywords: fmpsdk financial stock valuation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fmpsdk-20230522.0/fmpsdk.egg-info/SOURCES.txt` & `fmpsdk-20230623.0/fmpsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230522.0/setup.py` & `fmpsdk-20230623.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = "20230522.0"
+__version__ = "20230623.0"
 __author__ = "Dax Mickelson"
 __author_email__ = "fmp@daxm.net"
 __license__ = "BSD"
 __package_name__ = "fmpsdk"
 __description__ = "SDK for interacting with FMP's APIs."
 __long_description__ = """Interact with Financial Modeling Prep's APIs."""
 __url__ = "https://github.com/daxm/fmpsdk"
```

