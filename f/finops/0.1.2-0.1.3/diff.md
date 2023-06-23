# Comparing `tmp/finops-0.1.2.tar.gz` & `tmp/finops-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.1.2.tar", last modified: Sat Jun 17 12:20:03 2023, max compression
+gzip compressed data, was "finops-0.1.3.tar", last modified: Fri Jun 23 13:56:50 2023, max compression
```

## Comparing `finops-0.1.2.tar` & `finops-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-17 12:19:51.000000 finops-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-17 12:20:03.773547 finops-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-17 12:19:51.000000 finops-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/finops/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-17 12:19:51.000000 finops-0.1.2/finops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-17 12:19:51.000000 finops-0.1.2/finops/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 12:19:51.000000 finops-0.1.2/finops/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-17 12:19:51.000000 finops-0.1.2/finops/tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-17 12:19:51.000000 finops-0.1.2/finops/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/finops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 12:19:51.000000 finops-0.1.2/finops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-17 12:19:51.000000 finops-0.1.2/finops/utils/base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-17 12:19:51.000000 finops-0.1.2/finops/utils/base_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 12:19:51.000000 finops-0.1.2/finops/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/finops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-17 12:20:03.000000 finops-0.1.2/finops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-17 12:20:03.000000 finops-0.1.2/finops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 12:20:03.000000 finops-0.1.2/finops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-17 12:20:03.000000 finops-0.1.2/finops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 12:20:03.000000 finops-0.1.2/finops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 12:20:03.773547 finops-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-17 12:19:51.000000 finops-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 12:19:51.000000 finops-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-17 12:19:51.000000 finops-0.1.2/tests/test_tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-17 12:19:51.000000 finops-0.1.2/tests/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 12:19:51.000000 finops-0.1.2/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-17 12:19:51.000000 finops-0.1.2/tests/test_utils/test_base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-17 12:19:51.000000 finops-0.1.2/tests/test_utils/test_base_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-23 13:56:40.000000 finops-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-23 13:56:50.060248 finops-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-23 13:56:40.000000 finops-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 13:56:40.000000 finops-0.1.3/finops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-23 13:56:40.000000 finops-0.1.3/finops/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-23 13:56:40.000000 finops-0.1.3/finops/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-23 13:56:40.000000 finops-0.1.3/finops/tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-23 13:56:40.000000 finops-0.1.3/finops/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/finops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:40.000000 finops-0.1.3/finops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-23 13:56:40.000000 finops-0.1.3/finops/utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-23 13:56:40.000000 finops-0.1.3/finops/utils/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-23 13:56:40.000000 finops-0.1.3/finops/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-23 13:56:50.000000 finops-0.1.3/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-23 13:56:50.000000 finops-0.1.3/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:56:50.000000 finops-0.1.3/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 13:56:50.000000 finops-0.1.3/finops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 13:56:50.000000 finops-0.1.3/finops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 13:56:50.060248 finops-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-23 13:56:40.000000 finops-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:40.000000 finops-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-23 13:56:40.000000 finops-0.1.3/tests/test_tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-06-23 13:56:40.000000 finops-0.1.3/tests/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:50.060248 finops-0.1.3/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 13:56:40.000000 finops-0.1.3/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-23 13:56:40.000000 finops-0.1.3/tests/test_utils/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-23 13:56:40.000000 finops-0.1.3/tests/test_utils/test_scraper.py
```

### Comparing `finops-0.1.2/LICENSE` & `finops-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `finops-0.1.2/PKG-INFO` & `finops-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.1.2
-Summary: Financial tools for the rest of us.
+Version: 0.1.3
+Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `finops-0.1.2/README.md` & `finops-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `finops-0.1.2/finops/config.py` & `finops-0.1.3/finops/config.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.2/finops/utils/base_downloader.py` & `finops-0.1.3/finops/utils/downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import requests
 import pandas as pd
 from .wrappers import lock
 from bs4 import BeautifulSoup
 
 
-class BaseDownloader:
+class Downloader:
     @staticmethod
     def _create_csv_file(path, columns):
         if os.path.isfile(path):
             existing_columns = pd.read_csv(path, nrows=0).columns.tolist()
             if existing_columns != columns:
                 raise ValueError(
                     f"Columns in the {path} do not match the specified columns."
@@ -45,10 +45,9 @@
         return BeautifulSoup(response.text, "html.parser")
 
     def _load_or_create_csv(self, path, columns, **kwargs):
         self._create_csv_file(path, columns=columns)
         return pd.read_csv(path, **kwargs)
 
     @staticmethod
-    @lock
     def _save_csv(data, path):
         data.to_csv(path, index=False, mode="a", header=False)
```

### Comparing `finops-0.1.2/finops/utils/base_scraper.py` & `finops-0.1.3/finops/utils/scraper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
-from .base_downloader import BaseDownloader
+from .downloader import Downloader
 
 
-class BaseScraper(BaseDownloader):
+class Scraper(Downloader):
     @staticmethod
     def _filter_scraped_dates(traded_dates, scraped_dates):
         not_scraped_dates = list(set(traded_dates) - set(scraped_dates))
         return not_scraped_dates
 
     @staticmethod
     def _filter_dates_range(dates, start_date, end_date):
```

### Comparing `finops-0.1.2/finops.egg-info/PKG-INFO` & `finops-0.1.3/finops.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.1.2
-Summary: Financial tools for the rest of us.
+Version: 0.1.3
+Summary: A Python package for financial operations.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `finops-0.1.2/setup.py` & `finops-0.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='finops',
-    version='0.1.2',
-    description='Financial tools for the rest of us.',
+    version='0.1.3',
+    description='A Python package for financial operations.',
     author='Alireza Nilgaran',
     author_email='alireza.nilgaran@gmail.com',
     url='https://github.com/nixuri/FinOps',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='BSD (3-clause)',
```

### Comparing `finops-0.1.2/tests/test_tehran_stock_exchange.py` & `finops-0.1.3/tests/test_tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.2/tests/test_ticker.py` & `finops-0.1.3/tests/test_ticker.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from datetime import datetime
 import pandas as pd
 from finops.ticker import Ticker
 from finops.config import (
     SHAREHOLDER_URL,
     PRICE_HISTORY_URL,
     PRICE_HISTORY_DATA_COLUMNS,
-    SHAREHOLDER_DATA_COLUMNS,PRICE_HISTORY_FIELD_MAP, SHAREHOLDER_FIELD_MAP
+    SHAREHOLDER_DATA_COLUMNS,
+    PRICE_HISTORY_FIELD_MAP,
+    SHAREHOLDER_FIELD_MAP,
 )
 
 
 class TestTicker(unittest.TestCase):
     def setUp(self):
         self.ticker_index = "2400322364771558"
         self.ticker = Ticker(self.ticker_index)
@@ -52,17 +54,15 @@
                 "n_shares": [1000, 2000],
                 "per_shares": [10.5, 15.25],
                 "ticker_index": self.ticker_index,
                 "req_date": datetime(2021, 6, 1),
             }
         )
 
-        result = self.ticker._preprocess_shareholder_data(
-            parsed_response, date
-        )
+        result = self.ticker._preprocess_shareholder_data(parsed_response, date)
         pd.testing.assert_frame_equal(result, expected_result)
 
     def test_get_price_history(self):
         price_history = self.ticker.get_price_history()
         self.assertIsInstance(price_history, pd.DataFrame)
         expected_columns = [
             "en_ticker",
@@ -79,15 +79,15 @@
             "ticker_index",
         ]
         self.assertListEqual(list(price_history.columns), expected_columns)
         self.assertEqual(price_history["ticker_index"].unique(), [self.ticker_index])
 
     def test_get_shareholder_data_one_day(self):
         date = datetime(2023, 5, 22)
-        result = self.ticker.get_shareholder_data_one_day(date)
+        result = self.ticker._get_shareholder_data_one_day(date)
         expected_result = pd.DataFrame(
             [
                 {
                     "shareholder_id": 99,
                     "shareholder_name": "سازمان تامين اجتماعي",
                     "isin": "IRO1TAMN0006",
                     "date": datetime(2023, 5, 23),
@@ -130,8 +130,8 @@
         )
         self.assertIsInstance(result, pd.DataFrame)
         pd.testing.assert_frame_equal(result, expected_result)
 
     def test_get_traded_dates(self):
         traded_dates = self.ticker.get_traded_dates()
         self.assertIsInstance(traded_dates, list)
-        self.assertTrue(all(isinstance(date, datetime) for date in traded_dates))
+        self.assertTrue(all(isinstance(date, datetime) for date in traded_dates))
```

### Comparing `finops-0.1.2/tests/test_utils/test_base_downloader.py` & `finops-0.1.3/tests/test_utils/test_downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import pandas as pd
 import requests
 import unittest
 from unittest.mock import patch, Mock
 from io import StringIO
-from finops.utils.base_downloader import BaseDownloader
+from finops.utils.downloader import Downloader
 
 
 class TestBaseDownloader(unittest.TestCase):
     def setUp(self):
         self.columns = ["col1", "col2", "col3"]
         self.path = "test.csv"
         self.url = "http://cdn.tsetmc.com/api/Shareholder/65883838195688438/20230522"
@@ -19,52 +19,50 @@
         if os.path.exists(self.path):
             os.remove(self.path)
 
     def test_create_csv_file_existing_file(self):
         pd.DataFrame(columns=self.columns).to_csv(self.path, index=False)
         with patch("pandas.read_csv") as mock_read_csv:
             mock_read_csv.return_value.columns.tolist.return_value = self.columns
-            BaseDownloader._create_csv_file(self.path, self.columns)
+            Downloader._create_csv_file(self.path, self.columns)
             mock_read_csv.assert_called_once_with(self.path, nrows=0)
         self.assertTrue(os.path.exists(self.path))
 
     def test_create_csv_file_new_file(self):
-        BaseDownloader._create_csv_file(self.path, self.columns)
+        Downloader._create_csv_file(self.path, self.columns)
         self.assertTrue(os.path.exists(self.path))
         df = pd.read_csv(self.path)
         self.assertListEqual(df.columns.tolist(), self.columns)
 
     @patch("requests.get")
     def test_download(self, mock_get):
         mock_response = Mock()
         mock_response.raise_for_status.return_value = None
         mock_get.return_value = mock_response
-        response = BaseDownloader._download(self.url, self.user_agent, self.timeout)
+        response = Downloader._download(self.url, self.user_agent, self.timeout)
         mock_get.assert_called_once_with(
             self.url, headers={"user-agent": self.user_agent}, timeout=self.timeout
         )
         mock_response.raise_for_status.assert_called_once_with()
         self.assertEqual(response, mock_response)
 
     def test_parse_json_response(self):
         response = Mock()
         response.content.decode.return_value = '{"key": "value"}'
-        parsed_response = BaseDownloader._parse_json_response(response)
+        parsed_response = Downloader._parse_json_response(response)
         self.assertDictEqual(parsed_response, {"key": "value"})
 
     def test_parse_csv_response(self):
         response = Mock()
         response.content.decode.return_value = "col1,col2,col3\n1,2,3\n4,5,6\n"
-        parsed_response = BaseDownloader._parse_csv_response(response)
+        parsed_response = Downloader._parse_csv_response(response)
         expected_df = pd.DataFrame({"col1": [1, 4], "col2": [2, 5], "col3": [3, 6]})
         pd.testing.assert_frame_equal(parsed_response, expected_df)
 
     def test_store_existing_file(self):
         existing_df = pd.DataFrame({"col1": [1, 2], "col2": [3, 4], "col3": [5, 6]})
-        existing_df.to_csv(
-            self.path, index=False, mode="w", header=True
-        )
+        existing_df.to_csv(self.path, index=False, mode="w", header=True)
         new_df = pd.DataFrame({"col1": [7, 8], "col2": [9, 10], "col3": [11, 12]})
-        BaseDownloader._save_csv(new_df, self.path)
+        Downloader._save_csv(new_df, self.path)
         stored_df = pd.read_csv(self.path)
         expected_df = pd.concat([existing_df, new_df], ignore_index=True)
         pd.testing.assert_frame_equal(stored_df, expected_df)
```

### Comparing `finops-0.1.2/tests/test_utils/test_base_scraper.py` & `finops-0.1.3/tests/test_utils/test_scraper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 import pandas as pd
 from datetime import date
-from finops.utils.base_scraper import BaseScraper
+from finops.utils.scraper import Scraper
 
 
 class TestBaseScraper(unittest.TestCase):
     def setUp(self):
         self.traded_dates = [
             date(2022, 1, 1),
             date(2022, 1, 2),
@@ -31,27 +31,25 @@
                     date(2022, 1, 3),
                     date(2022, 1, 4),
                 ],
             }
         )
 
     def test_filter_scraped_dates(self):
-        not_scraped_dates = BaseScraper._filter_scraped_dates(
+        not_scraped_dates = Scraper._filter_scraped_dates(
             self.traded_dates, self.scraped_dates
         )
         expected_dates = [date(2022, 1, 2), date(2022, 1, 4)]
         self.assertListEqual(not_scraped_dates, expected_dates)
 
     def test_filter_dates_range(self):
-        filtered_dates = BaseScraper._filter_dates_range(
+        filtered_dates = Scraper._filter_dates_range(
             self.traded_dates, self.start_date, self.end_date
         )
         expected_dates = [date(2022, 1, 3)]
         self.assertListEqual(filtered_dates, expected_dates)
 
     def test_get_ticker_scraped_dates(self):
         ticker_index = 0
-        scraped_dates = BaseScraper._get_ticker_scraped_dates(
-            self.log, ticker_index
-        )
+        scraped_dates = Scraper._get_ticker_scraped_dates(self.log, ticker_index)
         expected_dates = [date(2022, 1, 1), date(2022, 1, 2), date(2022, 1, 3)]
-        self.assertListEqual(list(scraped_dates), expected_dates)
+        self.assertListEqual(list(scraped_dates), expected_dates)
```

