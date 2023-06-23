# Comparing `tmp/hkfdb-3.5.2.tar.gz` & `tmp/hkfdb-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.5.2.tar", last modified: Thu Jun 22 23:40:43 2023, max compression
+gzip compressed data, was "hkfdb-3.5.5.tar", last modified: Fri Jun 23 00:20:31 2023, max compression
```

## Comparing `hkfdb-3.5.2.tar` & `hkfdb-3.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-22 23:40:43.027787 hkfdb-3.5.2/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.5.2/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-06-22 23:40:43.027634 hkfdb-3.5.2/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.5.2/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-22 23:40:43.026656 hkfdb-3.5.2/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   108708 2023-06-22 23:25:56.000000 hkfdb-3.5.2/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.5.2/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-22 23:40:43.027444 hkfdb-3.5.2/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-06-22 23:40:42.000000 hkfdb-3.5.2/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-22 23:40:42.000000 hkfdb-3.5.2/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-22 23:40:42.000000 hkfdb-3.5.2/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-06-22 23:40:42.000000 hkfdb-3.5.2/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-22 23:40:42.000000 hkfdb-3.5.2/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-22 23:40:43.027833 hkfdb-3.5.2/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-06-22 23:39:59.000000 hkfdb-3.5.2/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-23 00:20:31.040716 hkfdb-3.5.5/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.5.5/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-06-23 00:20:31.040496 hkfdb-3.5.5/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.5.5/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-23 00:20:31.039079 hkfdb-3.5.5/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   108712 2023-06-23 00:19:39.000000 hkfdb-3.5.5/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.5.5/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-23 00:20:31.040186 hkfdb-3.5.5/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-06-23 00:20:30.000000 hkfdb-3.5.5/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-23 00:20:30.000000 hkfdb-3.5.5/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-23 00:20:30.000000 hkfdb-3.5.5/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-06-23 00:20:30.000000 hkfdb-3.5.5/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-23 00:20:30.000000 hkfdb-3.5.5/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-23 00:20:31.040785 hkfdb-3.5.5/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-06-23 00:20:18.000000 hkfdb-3.5.5/setup.py
```

### Comparing `hkfdb-3.5.2/LICENSE` & `hkfdb-3.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.5.2/PKG-INFO` & `hkfdb-3.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.5.2
+Version: 3.5.5
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.5.2/README.md` & `hkfdb-3.5.5/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.5.2/hkfdb/Database.py` & `hkfdb-3.5.5/hkfdb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,17 +286,17 @@
             link_url = 'http://www.hkfdb.net/data_api?'
             token = str(self.authToken)
             start_date_str = str(start_date)
             end_date_str = str(end_date)
             # end_date_str = str(end_date)[:4], str(end_date)[4:6]
             # _, last_day = calendar.monthrange( int(str(end_date)[:4]), int(str(end_date)[4:6]))
             # end_date_str = f'{str(end_date)[:4]}{str(end_date)[4:6]}{last_day}'
-            print(start_date_str, end_date_str)
+            # print(start_date_str, end_date_str)
             link_str = f'{link_url}token={token}&database=hk_futures_ohlc&index={index}&freq={freq}&start_date={start_date_str}&end_date={end_date_str}'
-            print(link_str)
+            # print(link_str)
 
             response = requests.get(link_str)
             response_ok = response_check(response)
 
 
             if response_ok == True:
```

### Comparing `hkfdb-3.5.2/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.5.5/hkfdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.5.2
+Version: 3.5.5
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.5.2/setup.py` & `hkfdb-3.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.5.2",
+    version="3.5.5",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

