# Comparing `tmp/hkfdb-3.5.1.tar.gz` & `tmp/hkfdb-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-3.5.1.tar", last modified: Mon Jun 19 02:34:31 2023, max compression
+gzip compressed data, was "hkfdb-3.5.2.tar", last modified: Thu Jun 22 23:40:43 2023, max compression
```

## Comparing `hkfdb-3.5.1.tar` & `hkfdb-3.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-19 02:34:31.379424 hkfdb-3.5.1/
--rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.5.1/LICENSE
--rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-06-19 02:34:31.379273 hkfdb-3.5.1/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.5.1/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-19 02:34:31.378342 hkfdb-3.5.1/hkfdb/
--rw-rw-rw-   0 cmw        (501) staff       (20)   108587 2023-06-19 02:29:22.000000 hkfdb-3.5.1/hkfdb/Database.py
--rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.5.1/hkfdb/__init__.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-19 02:34:31.379079 hkfdb-3.5.1/hkfdb.egg-info/
--rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-06-19 02:34:31.000000 hkfdb-3.5.1/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-19 02:34:31.000000 hkfdb-3.5.1/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-19 02:34:31.000000 hkfdb-3.5.1/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-06-19 02:34:31.000000 hkfdb-3.5.1/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-19 02:34:31.000000 hkfdb-3.5.1/hkfdb.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-19 02:34:31.379469 hkfdb-3.5.1/setup.cfg
--rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-06-19 02:33:24.000000 hkfdb-3.5.1/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-22 23:40:43.027787 hkfdb-3.5.2/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-3.5.2/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1620 2023-06-22 23:40:43.027634 hkfdb-3.5.2/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-3.5.2/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-22 23:40:43.026656 hkfdb-3.5.2/hkfdb/
+-rw-rw-rw-   0 cmw        (501) staff       (20)   108708 2023-06-22 23:25:56.000000 hkfdb-3.5.2/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-3.5.2/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-22 23:40:43.027444 hkfdb-3.5.2/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1620 2023-06-22 23:40:42.000000 hkfdb-3.5.2/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-06-22 23:40:42.000000 hkfdb-3.5.2/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-06-22 23:40:42.000000 hkfdb-3.5.2/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       51 2023-06-22 23:40:42.000000 hkfdb-3.5.2/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-06-22 23:40:42.000000 hkfdb-3.5.2/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-22 23:40:43.027833 hkfdb-3.5.2/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      772 2023-06-22 23:39:59.000000 hkfdb-3.5.2/setup.py
```

### Comparing `hkfdb-3.5.1/LICENSE` & `hkfdb-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-3.5.1/PKG-INFO` & `hkfdb-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.5.1
+Version: 3.5.2
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.5.1/README.md` & `hkfdb-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-3.5.1/hkfdb/Database.py` & `hkfdb-3.5.2/hkfdb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,18 +282,21 @@
 
 
         if False not in list(check_bool_dict.values()):
 
             link_url = 'http://www.hkfdb.net/data_api?'
             token = str(self.authToken)
             start_date_str = str(start_date)
+            end_date_str = str(end_date)
             # end_date_str = str(end_date)[:4], str(end_date)[4:6]
-            _, last_day = calendar.monthrange( int(str(end_date)[:4]), int(str(end_date)[4:6]))
-            end_date_str = f'{str(end_date)[:4]}{str(end_date)[4:6]}{last_day}'
+            # _, last_day = calendar.monthrange( int(str(end_date)[:4]), int(str(end_date)[4:6]))
+            # end_date_str = f'{str(end_date)[:4]}{str(end_date)[4:6]}{last_day}'
+            print(start_date_str, end_date_str)
             link_str = f'{link_url}token={token}&database=hk_futures_ohlc&index={index}&freq={freq}&start_date={start_date_str}&end_date={end_date_str}'
+            print(link_str)
 
             response = requests.get(link_str)
             response_ok = response_check(response)
 
 
             if response_ok == True:
```

### Comparing `hkfdb-3.5.1/hkfdb.egg-info/PKG-INFO` & `hkfdb-3.5.2/hkfdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkfdb
-Version: 3.5.1
+Version: 3.5.2
 Summary: Hong Kong Finance Database.
 Home-page: https://www.hkfdb.net
 Author: Hong Kong Finance Database Team
 Author-email: info@hkfdb.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hkfdb-3.5.1/setup.py` & `hkfdb-3.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="3.5.1",
+    version="3.5.2",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

