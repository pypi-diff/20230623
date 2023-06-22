# Comparing `tmp/sqscraper-0.4.0.tar.gz` & `tmp/sqscraper-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqscraper-0.4.0.tar", last modified: Tue Jun 20 22:48:12 2023, max compression
+gzip compressed data, was "sqscraper-0.4.1.tar", last modified: Thu Jun 22 23:15:28 2023, max compression
```

## Comparing `sqscraper-0.4.0.tar` & `sqscraper-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 22:48:12.786126 sqscraper-0.4.0/
--rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     2312 2023-06-20 22:48:12.786126 sqscraper-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-06-15 19:52:45.000000 sqscraper-0.4.0/README.md
--rw-rw-rw-   0        0        0     2197 2023-06-20 22:47:00.000000 sqscraper-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 22:48:12.786126 sqscraper-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 22:48:12.765165 sqscraper-0.4.0/sqscraper/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.4.0/sqscraper/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.4.0/sqscraper/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 22:48:12.786126 sqscraper-0.4.0/sqscraper/cnbc/
--rw-rw-rw-   0        0        0       84 2023-06-17 17:45:03.000000 sqscraper-0.4.0/sqscraper/cnbc/__init__.py
--rw-rw-rw-   0        0        0      931 2023-06-18 02:02:54.000000 sqscraper-0.4.0/sqscraper/cnbc/_apps.py
--rw-rw-rw-   0        0        0    13045 2023-06-20 18:44:13.000000 sqscraper-0.4.0/sqscraper/cnbc/quote_page.py
--rw-rw-rw-   0        0        0    11780 2023-06-20 22:32:19.000000 sqscraper-0.4.0/sqscraper/cnbc/summary.py
--rw-rw-rw-   0        0        0      592 2023-06-20 18:30:10.000000 sqscraper-0.4.0/sqscraper/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 22:48:12.775511 sqscraper-0.4.0/sqscraper.egg-info/
--rw-rw-rw-   0        0        0     2312 2023-06-20 22:48:12.000000 sqscraper-0.4.0/sqscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-06-20 22:48:12.000000 sqscraper-0.4.0/sqscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 22:48:12.000000 sqscraper-0.4.0/sqscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      635 2023-06-20 22:48:12.000000 sqscraper-0.4.0/sqscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-20 22:48:12.000000 sqscraper-0.4.0/sqscraper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 23:15:28.391802 sqscraper-0.4.1/
+-rw-rw-rw-   0        0        0     1087 2023-06-13 17:25:03.000000 sqscraper-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     2312 2023-06-22 23:15:28.389803 sqscraper-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-06-15 19:52:45.000000 sqscraper-0.4.1/README.md
+-rw-rw-rw-   0        0        0     1989 2023-06-22 23:14:09.000000 sqscraper-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 23:15:28.391802 sqscraper-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 23:15:28.222716 sqscraper-0.4.1/sqscraper/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.4.1/sqscraper/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:52:45.000000 sqscraper-0.4.1/sqscraper/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:15:28.343213 sqscraper-0.4.1/sqscraper/cnbc/
+-rw-rw-rw-   0        0        0       84 2023-06-21 17:43:19.000000 sqscraper-0.4.1/sqscraper/cnbc/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-06-20 22:50:22.000000 sqscraper-0.4.1/sqscraper/cnbc/_apps.py
+-rw-rw-rw-   0        0        0    12837 2023-06-22 23:13:54.000000 sqscraper-0.4.1/sqscraper/cnbc/_serializer.py
+-rw-rw-rw-   0        0        0    13041 2023-06-22 23:13:54.000000 sqscraper-0.4.1/sqscraper/cnbc/quote_page.py
+-rw-rw-rw-   0        0        0    15339 2023-06-22 23:13:54.000000 sqscraper-0.4.1/sqscraper/cnbc/summary.py
+-rw-rw-rw-   0        0        0      592 2023-06-22 05:52:27.000000 sqscraper-0.4.1/sqscraper/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:15:28.233355 sqscraper-0.4.1/sqscraper.egg-info/
+-rw-rw-rw-   0        0        0     2312 2023-06-22 23:15:28.000000 sqscraper-0.4.1/sqscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-06-22 23:15:28.000000 sqscraper-0.4.1/sqscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 23:15:28.000000 sqscraper-0.4.1/sqscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      483 2023-06-22 23:15:28.000000 sqscraper-0.4.1/sqscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-22 23:15:28.000000 sqscraper-0.4.1/sqscraper.egg-info/top_level.txt
```

### Comparing `sqscraper-0.4.0/LICENSE` & `sqscraper-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqscraper-0.4.0/PKG-INFO` & `sqscraper-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.4.0
+Version: 0.4.1
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sqscraper-0.4.0/pyproject.toml` & `sqscraper-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqscraper"
-version = "0.4.0"
+version = "0.4.1"
 description = "API wrapper and web scraper for select stock quote websites."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Financial and Insurance Industry",
@@ -26,28 +26,24 @@
     "Topic :: Software Development"
 ]
 requires-python = ">=3.6"
 dependencies = [
     "beautifulsoup4==4.12.2",
     "certifi==2023.5.7 ; python_version >= '3.6'",
     "charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'",
-    "greenlet==2.0.2 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
     "html5lib==1.1",
     "idna==3.4 ; python_version >= '3.5'",
     "lxml==4.9.2",
     "numpy==1.24.3",
     "pandas==2.0.2",
-    "playwright==1.35.0",
-    "pyee==9.0.4",
     "python-dateutil==2.8.2 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
     "pytz==2023.3",
     "requests==2.31.0",
     "six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
     "soupsieve==2.4.1 ; python_version >= '3.7'",
-    "typing-extensions==4.6.3 ; python_version >= '3.7'",
     "tzdata==2023.3 ; python_version >= '2'",
     "urllib3==2.0.3 ; python_version >= '3.7'",
     "webencodings==0.5.1"
 ]
 
 [project.urls]
 homepage = "https://github.com/JacobLee23/SQScraper"
```

### Comparing `sqscraper-0.4.0/sqscraper/cnbc/_apps.py` & `sqscraper-0.4.1/sqscraper/cnbc/_apps.py`

 * *Files identical despite different names*

### Comparing `sqscraper-0.4.0/sqscraper/cnbc/quote_page.py` & `sqscraper-0.4.1/sqscraper/cnbc/quote_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
             "52 Week High": self.fiftytwo_week_high,
             "52 Week High Date": self.fiftytwo_week_high_date,
             "52 Week Low": self.fiftytwo_week_low,
             "52 Week Low Date": self.fiftytwo_week_low_date,
             "Beta": self.beta,
             "Shares Out": self.shares_out,
             "Dividend": self.dividend,
-            "Dividend Yield (%)": self.dividend_yield,
+            "Dividend Yield": self.dividend_yield,
             "YTD % Change": self.ytd_pct_change
         }
         return pd.Series(data, name="Key Stats")
 
     @property
     @QuotePageSection.quote_data
     def open(self) -> float:
```

### Comparing `sqscraper-0.4.0/sqscraper/cnbc/summary.py` & `sqscraper-0.4.1/sqscraper/cnbc/_serializer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,376 +1,441 @@
 """
 """
 
-import datetime
-import decimal
-import operator
+import json
 import re
 import typing
-import urllib.parse
 
-import bs4
-import numpy as np
-import pandas as pd
-from playwright import sync_api
-from playwright._impl import _api_types
 
-from ._apps import Apps
-from ._apps import PageSection
-from sqscraper.utils import expand_value
-from sqscraper.utils import normalize_value
-
-
-class StockSummary(Apps):
+class Serializer:
     """
     """
-    def __init__(self, symbol: str):
-        super().__init__(symbol, "stocks/summary")
+    _sbase64 = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/"
 
-        with sync_api.sync_playwright() as play:
-            browser = play.chromium.launch()
-            page = browser.new_page()
-            page.goto(self._url)
-
-            self.pricing_momentum = _PricingMomentum(self.symbol, self._soup, page)
-            self.growth_rates = _GrowthRates(self.symbol, self._soup, page)
-            self.key_measures = _KeyMeasures(self.symbol, self._soup, page)
+    def __init__(self):
+        self._name_exclusions = {}
+        self._type_exclusions = {}
+        self._encode = True
+        self._strict_json = False
+        self._safe_deserialize = False
 
-            browser.close()
+        self._data = []
 
     @property
-    def shares(self) -> pd.Series:
+    def require_strict_json(self) -> bool:
         """
+        Specifies whether to follow strict JSON serialization.
         """
-        data = {
-            "Shares Outstanding": self.shares_outstanding,
-            "Institutional Ownership (%)": self.institutional_ownership,
-            "Market Cap": self.market_cap,
-            "Last Stock Split (Date)": self.last_stock_split_date,
-            "Last Stock Split (Ratio)": self.last_stock_split_ratio
-        }
-        return pd.Series(data, name="Shares")
-
-    @property
-    def shares_outstanding(self) -> int:
+        return self._strict_json
+    
+    @require_strict_json.setter
+    def require_strict_json(self, value: bool) -> None:
         """
+        :param value:
         """
-        element = self._soup.select_one("table#shares tr:nth-child(1) > td:nth-child(2)")
-        return expand_value(element.text)
+        self._strict_json = value
 
     @property
-    def institutional_ownership(self) -> float:
+    def require_safe_deserialize(self) -> bool:
         """
+        Specifies whether to check for well-formedness before deserializing.
         """
-        element = self._soup.select_one("table#shares tr:nth-child(2) > td:nth-child(2)")
-        return float(element.text.strip("%"))
+        return self._safe_deserialize
     
-    @property
-    def market_cap(self) -> int:
+    @require_safe_deserialize.setter
+    def require_safe_deserialize(self, value: bool) -> None:
         """
+        :param value:
         """
-        element = self._soup.select_one("table#shares tr:nth-child(3) > td:nth-child(2)")
-        return expand_value(element.text)
-    
+        self._safe_deserialize = value
+
     @property
-    def last_stock_split_date(self) -> typing.Optional[datetime.datetime]:
+    def allow_encoding(self) -> bool:
         """
+        Specifies whether results should be encoded.
         """
-        element = self._soup.select_one("table#shares tr:nth-child(4) > td:nth-child(1)")
-        try:
-            return datetime.datetime.strptime(element.text, "Last Stock Split %m/%d/%Y")
-        except ValueError:
-            return np.nan
-        
-    @property
-    def last_stock_split_ratio(self) -> typing.Optional[float]:
+        return self._encode
+    
+    @allow_encoding.setter
+    def allow_encoding(self, value: bool) -> None:
         """
+        :param value:
         """
-        element = self._soup.select_one("table#sharestr:nth-child(4) > td:nth-child(2)")
-        regex = re.compile(r"^(.*):(.*)$")
-        try:
-            return float(
-                operator.truediv(
-                    *[decimal.Decimal(x) for x in regex.search(element.text).groups()]
-                )
-            )
-        except AttributeError:
-            return np.nan
-        
-    @property
-    def analyst_consensus(self) -> typing.Optional[pd.Series]:
+        self._encode = value
+    
+    def add_name_exclusion(self, *args: str) -> None:
         """
+        Exclude certain named elements from seralization.
+        
+        :param args:
         """
-        element = self._soup.select_one("div#trends > img")
-        if element is None:
-            return
-
-        url_components = urllib.parse.urlparse(element.attrs.get("desturl"))
-        query_parameters = dict(x.split("=") for x in url_components.query.split("&"))
-
-        ratings = ("Strong Buy", "Buy", "Hold", "Sell", "Underperform")
-        return pd.Series(dict(zip(ratings, map(int, query_parameters["data"].split(",")))))
-
-
-class _PricingMomentum(PageSection):
-    """
-    :param page:
-    :type page: sync_api._generated.Page
-    """
-    def __init__(self, symbol: str, soup: bs4.BeautifulSoup, page):
-        super().__init__(symbol, soup)
+        for argument in args:
+            self._name_exclusions[argument] = True
 
-        self._performance = self._scrape_performance(page)
-
-    @property
-    def quote(self) -> pd.Series:
+    def remove_name_exclusion(self, *args: str) -> None:
         """
+        Remove exclusion of named elements.
+        
+        :param args:
         """
-        data = {
-            "Last": self.last,
-            "Change": self.change,
-            "Change (%)": self.change_pct,
-            "Open": self.open,
-            "Day High": self.day_high,
-            "Day Low": self.day_low,
-            "Volume": self.volume
-        }
-        return pd.Series(data, name="Quote")
+        for argument in args:
+            self._name_exclusions[argument] = False
 
-    @property
-    def last(self) -> float:
+    def add_type_exclusion(self, *args: type) -> None:
         """
+        Exclude certain data types from serialization.
+        
+        :param args:
         """
-        element = self._soup.select_one("span#quoteTable_last")
-        return float(element.text)
+        for argument in args:
+            self._type_exclusions[argument] = True
 
-    @property
-    def change(self) -> float:
+    def remove_type_exclusion(self, *args: type) -> None:
         """
+        Remove exclusion of data types.
+        
+        :param args:
         """
-        element = self._soup.select_one("span#quoteTable_chg > span")
-        if "colUnch" in element.attrs.get("class"):
-            return np.nan
-        elif "colPos" in element.attrs.get("class"):
-            return float(element.text)
-        elif "colNeg" in element.attrs.get("class"):
-            return -float(element.text)
-        else:
-            raise ValueError
+        for argument in args:
+            self._type_exclusions[argument] = False
 
-    @property
-    def change_pct(self) -> float:
+    def seralize(self, obj: object) -> str:
+        self._data = []
+        self._seralize_node([obj], obj, 0, None)
+
+        sdata = "".join(self._data).replace(",}", "}").replace(",]", "]")[:-1]
+        return self.base64encode(sdata) if self.allow_encoding else sdata
+
+    def _seralize_node(self, objects: typing.List[object], start_object: object, depth: int, parent_type: type) -> None:
+        """
+        :param objects:
+        :param start_object:
+        :param depth:
+        :param parent_type:
+        """
+        for i in (list(objects) if isinstance(objects, dict) else range(len(objects))):
+            if (
+                type(objects[i]) not in self._type_exclusions
+                and i not in self._name_exclusions
+                and not (self._strict_json and isinstance(objects[i], function))
+            ):
+                if isinstance(objects[i], str):
+                    delimiters = ["\"", "\""]
+                elif isinstance(objects[i], dict):
+                    delimiters = ["{", "}"]
+                elif isinstance(objects[i], list):
+                    delimiters = ["[", "]"]
+                else:
+                    delimiters = ["", ""]
+
+                if not (parent_type == dict):
+                    self._data.append(delimiters[0])
+                else:
+                    n = f"\"{i}\"" if isinstance(i, str) else i
+                    self._data.append(f"{n}:{delimiters[0]}")
+
+                if isinstance(objects[i], dict):
+                    if depth == 0 or objects[i] is not start_object:
+                        self._seralize_node(objects[i], None, None, type(objects[i]))
+                else:
+                    if isinstance(objects[i], str):
+                        self._data.append(objects[i].replace("\"", "\\\""))
+                    elif isinstance(objects[i], None):
+                        self._data.append("null")
+                    else:
+                        self._data.append(objects[i])
+
+            self._data.append(f"{delimiters[1]},")
+
+    def deserialize(self, obj) -> dict:
         """
+        :param obj:
+        :return:
         """
-        element = self._soup.select_one("span#quoteTable_chgPct > span")
-        if "colUnch" in element.attrs.get("class"):
-            return np.nan
-        return float(element.text.strip("%"))
+        try:
+            if self.has_encoding_leader(obj):
+                obj = self.base64decode(obj)
 
-    @property
-    def open(self) -> float:
+            if self._safe_deserialize:
+                return self.safe_deserialize(obj)
+            else:
+                return self.unsafe_deserialize(obj)
+        except json.JSONDecodeError:
+            return {}
+    
+    def safe_deserialize(self, obj) -> str:
         """
+        :param obj:
+        :return:
         """
-        element = self._soup.select_one("span#quoteTable_open")
-        return float(element.text)
+        try:
+            parser = JSONParser()
+            parser.parse(obj)
+            return eval(obj)
+        except json.JSONDecodeError:
+            return ""
 
-    @property
-    def day_high(self) -> float:
+    def unsafe_deserialize(self, obj):
         """
+        :param obj:
+        :return:
         """
-        element = self._soup.select_one("span#quoteTable_high")
-        return float(element.text)
+        try:
+            return eval(obj)
+        except json.JSONDecodeError:
+            return ""
 
-    @property
-    def day_low(self) -> float:
+    def has_encoding_leader(self, string: str) -> bool:
         """
+        :param string:
+        :return:
         """
-        element = self._soup.select_one("span#quoteTable_low")
-        return float(element.text)
-
-    @property
-    def volume(self) -> int:
+        return string.find("B64ENC") == 0
+    
+    def strip_leader(self, string: str) -> str:
         """
+        :param string:
+        :return:
         """
-        element = self._soup.select_one("span#quoteTable_volume")
-        return int("".join(element.text.split(",")))
-
-    @property
-    def performance(self) -> typing.Dict[str, str]:
+        return string.replace("B64ENC", "")
+    
+    def prepend_leader(self, string: str) -> str:
         """
+        :param string:
+        :return:
         """
-        return self._performance
-
-    def _scrape_performance(self, page) -> typing.Dict[str, str]:
+        return f"B64ENC{string}"
+    
+    def base64decode(self, string: str) -> str:
         """
-        :param page:
-        :type page: sync_api._generated.Page
+        :param string:
         :return:
         """
-        urls = {}
+        if self.has_encoding_leader(string):
+            str_in = self.strip_leader(string)
+        else:
+            return string
+        
+        str_in = str_in.replace("=", "")
+        str_out = []
+
+        for i in range(0, len(str_in), 4):
+            ibits = (
+                self._sbase64.index(str_in[i]) << 18
+            ) | (
+                (self._sbase64.index(str_in[i + 1]) << 12) if (i + 1 < len(str_in)) else 0
+            ) | (
+                ((self._sbase64.index(str_in[i + 2]) & 0xff) << 6) if (i + 2 < len(str_in)) else 0
+            ) | (
+                (self._sbase64.index(str_in[i + 3]) & 0xff) if (i + 3 < len(str_in)) else 0
+            )
 
-        element_loading = page.locator("div#divLoading")
-        element_chart = page.locator("img#performanceChartImg")
-        element_checkbox = page.locator("div#chk0")
+            str_out.append(chr(ibits >> 16 & 0xff))
+            str_out.append("" if (i > len(str_in) - 3) else chr(ibits >> 8 & 0xff))
+            str_out.append("" if (i > len(str_in) - 4) else chr(ibits & 0xff))
 
-        element_loading.wait_for(state="detached")
+        return "".join(str_out)
+    
+    def base64encode(self, string: str) -> str:
+        """
+        :param string:
+        :return:
+        """
+        str_out = []
 
-        urls.setdefault("spx-on", element_chart.get_attribute("src"))
-        element_checkbox.click()
-        element_loading.wait_for(state="detached")
+        for i in range(0, len(string), 3):
+            ibits = (
+                ord(string[i]) << 16
+            ) + (
+                ((ord(string[i + 1]) & 0xff) << 8) if (i + 1 < len(string)) else 0
+            ) + (
+                (ord(string[i + 2]) & 0xff) if (i + 2 < len(string)) else 0
+            )
 
-        urls.setdefault("spx-off", element_chart.get_attribute("src"))
-        element_checkbox.click()
-        element_loading.wait_for(state="detached")
+            str_out.append(self._sbase64[ibits >> 18 & 0x3f])
+            str_out.append(self._sbase64[ibits >> 12 & 0x3f])
+            str_out.append("=" if (i > len(string) - 2) else self._sbase64[ibits >> 6 & 0x3f])
+            str_out.append("=" if (i > len(string) - 3) else self._sbase64[ibits & 0x3f])
 
-        return {k: f"https://apps.cnbc.com{v}" for k, v in urls.items()}
+        return self.prepend_leader("".join(str_out))
 
 
-class _GrowthRates(PageSection):
+class JSONParser:
     """
     """
-    def __init__(self, symbol: str, soup: bs4.BeautifulSoup, page):
-        super().__init__(symbol, soup)
-
-        self._earnings_per_share = self._scrape_chart(page, "div#rollMapImg0")
-        self._revenue = self._scrape_chart(page, "div#rollMapImg1")
-        self._dividend = self._scrape_chart(page, "div#rollMapImg2")
+    def __init__(self):
+        self.lexer = None
+        self.tokens: typing.List[JSONToken] = []
 
-    @property
-    def earnings_per_share(self) -> typing.Optional[pd.DataFrame]:
+    def parse(self, string: str) -> str:
         """
+        :param string:
+        :return:
         """
-        dataframe = self._earnings_per_share.copy()
-        if dataframe.empty:
-            return None
-
-        dataframe.iloc[:2, :] = dataframe.iloc[:2, :].applymap(
-            lambda x: float(normalize_value(x)) if isinstance(x, str) else x
-        )
-        dataframe.iloc[2, :] = pd.Series(dataframe.iloc[2, :], dtype="Int64")
-        dataframe.iloc[3:, :] = dataframe.iloc[3:, :].applymap(
-            lambda x: float(normalize_value(x)) if isinstance(x, str) else x
-        )
-
-        return dataframe
+        self.lexer = JSONLexer(string)
 
-    @property
-    def revenue(self) -> typing.Optional[pd.DataFrame]:
+        return self._json()
+    
+    def look_ahead(self, k: int = 0) -> str:
         """
+        :param k:
+        :return:
         """
-        dataframe = self._revenue.copy()
-        if dataframe.empty:
-            return None
-
-        dataframe.iloc[:2, :] = dataframe.iloc[:2, :].applymap(
-            lambda x: float(normalize_value(x)) if isinstance(x, str) else x
-        )
-        dataframe.iloc[2, :] = pd.Series(dataframe.iloc[2, :], dtype="Int64")
-        dataframe.iloc[3:, :] = dataframe.iloc[3:, :].applymap(
-            lambda x: float(normalize_value(x)) if isinstance(x, str) else x
-        )
-
-        return dataframe
-
-    @property
-    def dividend(self) -> typing.Optional[pd.DataFrame]:
+        while len(self.tokens <= k):
+            self.tokens.append(self.lexer.next_token())
+        return self.tokens[k].typeof
+    
+    def consume(self, typeof: str) -> None:
         """
+        :param typeof:
+        :raise json.JSONDecodeError:
         """
-        dataframe = self._dividend.copy()
-        if dataframe.empty:
-            return None
-
-        dataframe = dataframe.applymap(
-            lambda x: float(normalize_value(x)) if isinstance(x, str) else x
-        )
+        if len(self.tokens) == 0:
+            self.tokens.append(self.lexer.next_token())
 
-        return dataframe
-
-    def _scrape_chart(self, page, selector: str) -> typing.Optional[pd.DataFrame]:
+        if self.tokens[0].typeof == typeof:
+            self.tokens.pop(0)
+        else:
+            raise json.JSONDecodeError(
+                f"invalid token encountered while validating string (expected {typeof}, got {self.tokens[0].typeof})"
+            )
+        
+    def _json(self) -> None:
         """
-        :param page:
-        :type page: sync_api._generated.Page
-        :param selector:
-        :return:
         """
-        regex = re.compile(r"^(\d{4}) (EPS|Revenue|Dividend) Analysis$")
-
-        chart = page.locator(selector)
-        chart.hover()
-        chart_bars = chart.locator("map > area[shape='rect']")
-
-        popup_heading = page.locator("div#popContent > h1")
-        popup_body = page.locator("div#popBody")
-
-        data = {}
-        for bar in chart_bars.all():
-            bar.dispatch_event("mouseover")
-
-            popup_heading.wait_for(state="visible", timeout=5000)
-            year = int(regex.search(popup_heading.text_content()).group(1))
-            items =  dict(x.split(": ") for x in popup_body.inner_text().split("\n"))
-            data.setdefault(int(year), dict(items))
-
-            bar.dispatch_event("mouseout")
-
-        return pd.DataFrame(data).replace("--", np.nan)
+        self._value()
+        self.consume("_EOF")
 
+    def _value(self) -> None:
+        """
+        """
+        typeof = self.look_ahead()
 
-class _KeyMeasures(PageSection):
-    """
-    """
-    def __init__(self, symbol: str, soup: bs4.BeautifulSoup, page):
-        super().__init__(symbol, soup)
+        if typeof == "_OBJ_OPEN":
+            self._object()
+        elif typeof == "_ARR_OPEN":
+            self._array()
+        elif typeof == "_DIGITS" or typeof == "_NEG":
+            self._number()
+        elif typeof == "_STRING":
+            self.consume("_STRING")
+        elif typeof == "_TRUE":
+            self.consume("_TRUE")
+        elif typeof == "_FALSE":
+            self.consume("_FALSE")
+        elif typeof == "_NULL":
+            self.consume("_NULL")
 
-        self._dataframe = pd.read_html(page.locator("div#keyMeasResults").inner_html())[0]
-        self._dataframe.replace("--", np.nan, inplace=True)
+    def _object(self) -> None:
+        """
+        """
+        self.consume("_OBJ_OPEN")
+        
+        if self.look_ahead() != "_OBJ_CLOSE":
+            self._member()
+        while self.look_ahead() != "_OBJ_CLOSE":
+            self.consume("_SEP")
+            self._member()
+        
+        self.consume("_OBJ_CLOSE")
 
-    @property
-    def valuation(self) -> pd.DataFrame:
+    def _member(self) -> None:
         """
         """
-        dataframe = self._dataframe.iloc[1:5, 1:5].copy()
-        dataframe.index = list(self._dataframe.iloc[1:5, 0])
-        dataframe.columns = list(self._dataframe.iloc[0, 1:5])
+        self.consume("_STRING")
+        self.consume("_ASSIGN")
+        self._value()
 
-        return dataframe
-    
-    @property
-    def financial_strength(self) -> pd.DataFrame:
+    def _array(self) -> None:
         """
         """
-        dataframe = self._dataframe.iloc[6:13, 1:5].copy()
-        dataframe.index = list(self._dataframe.iloc[6:13, 0])
-        dataframe.columns = list(self._dataframe.iloc[0, 1:5])
+        self.consume("_ARR_OPEN")
+        
+        if self.look_ahead() != "_ARR_CLOSE":
+            self._member()
+        while self.look_ahead() != "_ARR_CLOSE":
+            self.consume("_SEP")
+            self._member()
+        
+        self.consume("_ARR_CLOSE")
 
-        return dataframe
-    
-    @property
-    def assets(self) -> pd.DataFrame:
+    def _number(self) -> None:
         """
         """
-        dataframe = self._dataframe.iloc[14:17, 1:5].copy()
-        dataframe.index = list(self._dataframe.iloc[14:17, 0])
-        dataframe.columns = list(self._dataframe.iloc[0, 1:15])
+        if self.look_ahead() == "_NEG":
+            self.consume("_NEG")
 
-        dataframe.iloc[1, :] = dataframe.iloc[1, :].map(
-            lambda x: expand_value(x.strip("$"))
-        )
+        self.consume("_DIGITS")
 
-        return dataframe
+        if self.look_ahead() == "_DOT":
+            self.consume("_DOT")
+            self.consume("_DIGITS")
 
-    @property
-    def profitability(self) -> pd.DataFrame:
+        if self.look_ahead() == "_EXP":
+            self.consume("_EXP")
+            if self.look_ahead() == "_POS":
+                self.consume("_POS")
+            elif self.look_ahead() == "_NEG":
+                self.consume("_NEG")
+            self.consume("_DIGITS")
+
+
+class JSONLexer:
+    """
+    """
+    def __init__(self, input: str):
+        input = re.sub(r"\"([^\"\\]|\\\"|\\)*\"", "S", input)
+        input = re.sub(r"[0-9]+", "0", input)
+
+        self.input = input
+        self.char_tokens = {
+            '{': '_OBJ_OPEN',
+            '}': '_OBJ_CLOSE',
+            '[': '_ARR_OPEN',
+            ']': '_ARR_CLOSE',
+            ':': '_ASSIGN',
+            ',': '_SEP',
+            '.': '_DOT',
+            '-': '_NEG',
+            '+': '_POS',
+            'e': '_EXP',
+            'E': '_EXP',
+            'S': '_STRING',
+            '0': '_DIGITS'
+        }
+    
+    def next_token(self) -> "JSONToken":
         """
+        :return:
+        :raise json.JSONDecodeError:
         """
-        dataframe = pd.DataFrame(self._dataframe.iloc[18:22, 1:5].copy())
-        dataframe.index = list(self._dataframe.iloc[18:22, 0])
-        dataframe.columns = list(self._dataframe.iloc[0, 1:5])
-
-        dataframe.iloc[0, :] = dataframe.iloc[0, :].map(
-            lambda x: expand_value(x.strip("$"))
-        )
-        dataframe.iloc[1:5, :] = dataframe.iloc[1:5, :].applymap(
-            lambda x: float(x.strip("%"))
+        if len(self.input) == 0:
+            return JSONToken("_EOF", None)
+        
+        first = self.input[0]
+        if first in self.char_tokens:
+            self.input = self.input[1:]
+            return JSONToken(self.char_tokens[first], first)
+        
+        if self.input[:4].lower() == "true":
+            self.input = self.input[4:]
+            return JSONToken("_TRUE", True)
+            
+        if self.input[:5].lower() == "false":
+            self.input = self.input[:5]
+            return JSONToken("_FALSE", True)
+        
+        if self.input[:4].lower() == "null":
+            self.input = self.input[:4]
+            return JSONToken("_NULL", True)
+        
+        raise json.JSONDecodeError(
+            f"unexpected character ({first}) encountered while validating string"
         )
 
-        return dataframe
+
+class JSONToken:
+    """
+    """
+    def __init__(self, typeof: str, value: typing.Any):
+        self.typeof = typeof
+        self.value = value
```

### Comparing `sqscraper-0.4.0/sqscraper/utils.py` & `sqscraper-0.4.1/sqscraper/utils.py`

 * *Files identical despite different names*

### Comparing `sqscraper-0.4.0/sqscraper.egg-info/PKG-INFO` & `sqscraper-0.4.1/sqscraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqscraper
-Version: 0.4.0
+Version: 0.4.1
 Summary: API wrapper and web scraper for select stock quote websites.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

