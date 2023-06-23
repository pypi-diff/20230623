# Comparing `tmp/amazon-scraper-toolkit-1.1.0.tar.gz` & `tmp/amazon-scraper-toolkit-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-scraper-toolkit-1.1.0.tar", last modified: Tue Jun 20 12:35:43 2023, max compression
+gzip compressed data, was "amazon-scraper-toolkit-2.0.0.tar", last modified: Fri Jun 23 14:24:12 2023, max compression
```

## Comparing `amazon-scraper-toolkit-1.1.0.tar` & `amazon-scraper-toolkit-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 12:35:43.824874 amazon-scraper-toolkit-1.1.0/
--rw-rw-rw-   0        0        0     1100 2023-06-05 04:51:21.000000 amazon-scraper-toolkit-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2026 2023-06-20 12:35:43.823874 amazon-scraper-toolkit-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-04 02:35:50.000000 amazon-scraper-toolkit-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 12:35:43.805393 amazon-scraper-toolkit-1.1.0/amazon_scrape_toolkit/
--rw-rw-rw-   0        0        0      138 2023-06-04 02:23:01.000000 amazon-scraper-toolkit-1.1.0/amazon_scrape_toolkit/__init__.py
--rw-rw-rw-   0        0        0    12537 2023-06-20 12:30:23.000000 amazon-scraper-toolkit-1.1.0/amazon_scrape_toolkit/main.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:35:43.821874 amazon-scraper-toolkit-1.1.0/amazon_scraper_toolkit.egg-info/
--rw-rw-rw-   0        0        0     2026 2023-06-20 12:35:43.000000 amazon-scraper-toolkit-1.1.0/amazon_scraper_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-06-20 12:35:43.000000 amazon-scraper-toolkit-1.1.0/amazon_scraper_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 12:35:43.000000 amazon-scraper-toolkit-1.1.0/amazon_scraper_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-20 12:35:43.000000 amazon-scraper-toolkit-1.1.0/amazon_scraper_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-20 12:35:43.000000 amazon-scraper-toolkit-1.1.0/amazon_scraper_toolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1353 2023-06-20 12:35:19.000000 amazon-scraper-toolkit-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-20 12:35:43.825870 amazon-scraper-toolkit-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 14:24:12.859105 amazon-scraper-toolkit-2.0.0/
+-rw-rw-rw-   0        0        0     1100 2023-06-05 04:51:21.000000 amazon-scraper-toolkit-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2026 2023-06-23 14:24:12.857195 amazon-scraper-toolkit-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-04 02:35:50.000000 amazon-scraper-toolkit-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 14:24:12.837148 amazon-scraper-toolkit-2.0.0/amazon_scrape_toolkit/
+-rw-rw-rw-   0        0        0      138 2023-06-04 02:23:01.000000 amazon-scraper-toolkit-2.0.0/amazon_scrape_toolkit/__init__.py
+-rw-rw-rw-   0        0        0    12947 2023-06-23 14:05:22.000000 amazon-scraper-toolkit-2.0.0/amazon_scrape_toolkit/main.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:24:12.854835 amazon-scraper-toolkit-2.0.0/amazon_scraper_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     2026 2023-06-23 14:24:12.000000 amazon-scraper-toolkit-2.0.0/amazon_scraper_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-06-23 14:24:12.000000 amazon-scraper-toolkit-2.0.0/amazon_scraper_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 14:24:12.000000 amazon-scraper-toolkit-2.0.0/amazon_scraper_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-23 14:24:12.000000 amazon-scraper-toolkit-2.0.0/amazon_scraper_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-23 14:24:12.000000 amazon-scraper-toolkit-2.0.0/amazon_scraper_toolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1353 2023-06-23 14:22:44.000000 amazon-scraper-toolkit-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:24:12.859105 amazon-scraper-toolkit-2.0.0/setup.cfg
```

### Comparing `amazon-scraper-toolkit-1.1.0/LICENSE` & `amazon-scraper-toolkit-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-scraper-toolkit-1.1.0/PKG-INFO` & `amazon-scraper-toolkit-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scraper-toolkit
-Version: 1.1.0
+Version: 2.0.0
 Summary: Some Helpful Classes and Functions for Scraping Amazon Data
 Author: Tejas
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `amazon-scraper-toolkit-1.1.0/amazon_scrape_toolkit/main.py` & `amazon-scraper-toolkit-2.0.0/amazon_scrape_toolkit/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
-from typing import Optional
 import bs4
 import time
-import json
 import logging
+from typing import Optional
 from functools import wraps
 from dataclasses import dataclass
 import requests
 
 logger = logging.getLogger()
 
 
@@ -35,16 +34,16 @@
         }
 
 
 @dataclass
 class ProductInfo:
     """Data class representing the information of a product"""
 
-    other_products: list[str]
-    ratings: dict[str, int]
+    other_products: list[str] | None
+    ratings: dict[str, int] | None
     data: dict
     custom_scraper_time_taken: float
     ratings_scraper_time_taken: float
     more_phones_scraper_time_taken: float
 
 
 def timer():
@@ -151,50 +150,57 @@
     logger.debug(f"avg page half scrape time: {sum(scrape_times) / len(scrape_times)}")
     logger.debug(f"max page half scrape time: {max(scrape_times)}")
     logger.debug(f"min page half scrape time: {min(scrape_times)}")
 
     return set(all_product_ids)
 
 
-def product_scraper(fetch_ratings: bool = True, get_others: bool = True):
+def product_scraper(
+    fetch_ratings: bool = True, get_others: bool = True, should_raise: bool = False
+):
     """
     Decorator to mark a function as a product scraper.
 
     Args:
         fetch_ratings (bool, optional): Whether to fetch the ratings. Defaults to True.
         get_others (bool, optional): Whether to fetch information about other related products. Defaults to True.
 
     Returns:
         function: The decorated function.
     """
 
     def inner_decorator(func):
         @wraps(func)
         def _wrapper(soup: bs4.BeautifulSoup, product_id: str, *args, **kwargs):
+            logger.info("\nSCRAPING DATA FROM PRODUCT [%s] -------", product_id)
+
             data_func_timer = timer()
             next(data_func_timer)
+
             try:
                 data = func(soup, product_id, *args, **kwargs)
-            except Exception:
+                assert isinstance(data, dict), "Output Can Only Be A Dictionary"
+                logger.info("STATUS: \033[31mSUCCESS\003[42m")
+            except AssertionError as e:
+                assert not should_raise, e
+                logger.info("STATUS: \033[31mFAILED\003[39m")
                 data = None
 
-            assert data is None or isinstance(
-                data, dict
-            ), "Output should be Dict or None!"
+            data_func_timer = next(data_func_timer)
+            logger.info("FUNC SCRAPER TOOK: [%s]", data_func_timer)
 
             if data is None:
-                logger.info(f"page_failed [{product_id}]")
                 return None
 
-            data_func_timer = next(data_func_timer)
+            # Scraping New Phones
             new_phones_to_add = [] if get_others else None
-
             other_phones_fetch_timer = timer()
             next(other_phones_fetch_timer)
-            if get_others:
+
+            if get_others and isinstance(new_phones_to_add, list):
                 compare_table = soup.find("table", {"id": "HLCXComparisonTable"})
 
                 if isinstance(compare_table, bs4.Tag):
                     compare_table_trs = compare_table.find(
                         "tr", class_="comparison_table_image_row"
                     )
                     assert isinstance(
@@ -219,17 +225,18 @@
                 new_phones_to_add.extend(
                     filter(
                         lambda x: x not in ["", product_id],
                         [div["data-asin"] for div in soup.select("div[data-asin]")],
                     )
                 )
                 new_phones_to_add = list(set(new_phones_to_add))
+
             other_phones_fetch_timer = next(other_phones_fetch_timer)
 
-            # get ratings
+            # Scraping Ratings
             stared_ratings = None
             ratings_fetch_timer = timer()
             next(ratings_fetch_timer)
 
             if fetch_ratings:
                 rating_histogram_div = soup.find(
                     "span",
@@ -242,17 +249,15 @@
                 if not isinstance(rating_histogram_div, bs4.Tag):
                     rating_histogram_div = soup.find(
                         "div", {"id": "cm_cr_dp_d_rating_histogram"}
                     )
 
                 no_of_ratings_div = rating_histogram_div.find(
                     "div",
-                    {
-                        "class": "a-row a-spacing-medium averageStarRatingNumerical",
-                    },
+                    {"class": "a-row a-spacing-medium averageStarRatingNumerical"},
                 )
 
                 if isinstance(no_of_ratings_div, bs4.Tag):
                     no_of_ratings_span = no_of_ratings_div.find("span")
                     assert isinstance(
                         no_of_ratings_span, bs4.Tag
                     ), "Ratings Span Not Found"
@@ -286,15 +291,18 @@
                         for key, value in individual_star_ratings
                     }
                 else:
                     stared_ratings = {f"no of {key} star": 0 for key in range(1, 6)}
             ratings_fetch_timer = next(ratings_fetch_timer)
 
             # log success in fetching thing
-            logger.info(f"fetched_everything [{product_id}]")
+            logger.info(
+                "TOOLKIT SCRAPER TOOK: [%s]",
+                ratings_fetch_timer + other_phones_fetch_timer,
+            )
 
             return ProductInfo(
                 new_phones_to_add,
                 stared_ratings,
                 data,
                 data_func_timer,
                 ratings_fetch_timer,
@@ -343,17 +351,20 @@
     while len(product_ids_to_scrape) > 0 and len(scraped_ids) < max_products:
         id_to_scrape = product_ids_to_scrape.pop()
         logger.info(f"Scraping product with ID: {id_to_scrape}")
 
         if id_to_scrape in scraped_ids:
             continue
 
-        link = f"https://www.amazon.in/dp/{id_to_scrape}"
-        soup = bs4.BeautifulSoup(fetch_webpage(link), "lxml")
-        output: Optional[ProductInfo] = function(soup, id_to_scrape)
+        try:
+            link = f"https://www.amazon.in/dp/{id_to_scrape}"
+            soup = bs4.BeautifulSoup(fetch_webpage(link), "lxml")
+            output: Optional[ProductInfo] = function(soup, id_to_scrape)
+        except:
+            continue
 
         if output is None:
             continue
 
         product_data = dict()
         product_data.update(output.data)
 
@@ -361,16 +372,17 @@
             product_ids_to_scrape.update(output.other_products)
 
         if output.ratings is not None:
             product_data.update(output.ratings)
 
         if product_data not in data:
             data.append(product_data)
-            logger.info(f"product_scraped and saved [{id_to_scrape}]")
+            logger.info(f"ADDED?: YES")
         else:
-            logger.info(f"product data not new and so not saved [{id_to_scrape}]")
+            logger.info(f"ADDED?: NO")
 
-        logger.info(f"Remaining products to scrape: {len(product_ids_to_scrape)}")
+        logger.info(f"REMAINING: {len(product_ids_to_scrape)}")
+        logger.info(f"SCRAPED: {len(data)}")
         logger.info("-------")
 
     logger.info(f"DONE - TIME TAKEN: {next(code_timer)}")
     return data
```

### Comparing `amazon-scraper-toolkit-1.1.0/amazon_scraper_toolkit.egg-info/PKG-INFO` & `amazon-scraper-toolkit-2.0.0/amazon_scraper_toolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-scraper-toolkit
-Version: 1.1.0
+Version: 2.0.0
 Summary: Some Helpful Classes and Functions for Scraping Amazon Data
 Author: Tejas
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `amazon-scraper-toolkit-1.1.0/pyproject.toml` & `amazon-scraper-toolkit-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amazon-scraper-toolkit"
-version = "1.1.0"
+version = "2.0.0"
 description = "Some Helpful Classes and Functions for Scraping Amazon Data"
 readme = "README.md"
 authors = [{ name = "Tejas" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
@@ -32,15 +32,15 @@
 [project.optional-dependencies]
 dev = ["black", "pylint", "pep8"]
 
 [project.urls]
 Homepage = "https://github.com/KidCoderT/amazon-scraper"
 
 [tool.bumpver]
-current_version = "1.0.1"
+current_version = "2.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

