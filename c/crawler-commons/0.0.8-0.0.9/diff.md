# Comparing `tmp/crawler_commons-0.0.8.tar.gz` & `tmp/crawler_commons-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crawler_commons-0.0.8.tar", last modified: Mon May 15 10:10:59 2023, max compression
+gzip compressed data, was "dist/crawler_commons-0.0.9.tar", last modified: Mon May 15 10:18:18 2023, max compression
```

## Comparing `crawler_commons-0.0.8.tar` & `crawler_commons-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-15 10:10:59.000000 crawler_commons-0.0.8/
--rw-r--r--   0 nezah      (501) staff       (20)      419 2023-05-15 10:10:59.000000 crawler_commons-0.0.8/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-15 10:10:59.000000 crawler_commons-0.0.8/crawlutils/
--rw-r--r--   0 nezah      (501) staff       (20)     1556 2023-05-06 07:27:29.000000 crawler_commons-0.0.8/crawlutils/text_utils.py
--rw-r--r--   0 nezah      (501) staff       (20)      273 2023-05-12 10:44:28.000000 crawler_commons-0.0.8/crawlutils/log.py
--rw-r--r--   0 nezah      (501) staff       (20)     1150 2022-12-27 06:40:36.000000 crawler_commons-0.0.8/crawlutils/date_utils.py
--rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.8/crawlutils/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1503 2023-05-15 10:10:57.000000 crawler_commons-0.0.8/crawlutils/num_utils.py
--rw-r--r--   0 nezah      (501) staff       (20)     1007 2023-05-06 07:56:32.000000 crawler_commons-0.0.8/crawlutils/soup_traversal.py
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.8/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-15 10:10:59.000000 crawler_commons-0.0.8/crawapi/
--rw-r--r--   0 nezah      (501) staff       (20)     2634 2023-05-06 07:54:17.000000 crawler_commons-0.0.8/crawapi/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.8/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      569 2023-05-15 10:10:57.000000 crawler_commons-0.0.8/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-15 10:10:59.000000 crawler_commons-0.0.8/crawler_commons.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      419 2023-05-15 10:10:59.000000 crawler_commons-0.0.8/crawler_commons.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      346 2023-05-15 10:10:59.000000 crawler_commons-0.0.8/crawler_commons.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       19 2023-05-15 10:10:59.000000 crawler_commons-0.0.8/crawler_commons.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-15 10:10:59.000000 crawler_commons-0.0.8/crawler_commons.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-15 10:10:59.000000 crawler_commons-0.0.8/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-15 10:18:18.000000 crawler_commons-0.0.9/
+-rw-r--r--   0 nezah      (501) staff       (20)      419 2023-05-15 10:18:18.000000 crawler_commons-0.0.9/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-15 10:18:18.000000 crawler_commons-0.0.9/crawlutils/
+-rw-r--r--   0 nezah      (501) staff       (20)     1556 2023-05-06 07:27:29.000000 crawler_commons-0.0.9/crawlutils/text_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)      273 2023-05-12 10:44:28.000000 crawler_commons-0.0.9/crawlutils/log.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1150 2022-12-27 06:40:36.000000 crawler_commons-0.0.9/crawlutils/date_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.9/crawlutils/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1540 2023-05-15 10:18:16.000000 crawler_commons-0.0.9/crawlutils/num_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1007 2023-05-06 07:56:32.000000 crawler_commons-0.0.9/crawlutils/soup_traversal.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.9/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-15 10:18:18.000000 crawler_commons-0.0.9/crawapi/
+-rw-r--r--   0 nezah      (501) staff       (20)     2634 2023-05-06 07:54:17.000000 crawler_commons-0.0.9/crawapi/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.9/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      569 2023-05-15 10:18:16.000000 crawler_commons-0.0.9/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-15 10:18:18.000000 crawler_commons-0.0.9/crawler_commons.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      419 2023-05-15 10:18:18.000000 crawler_commons-0.0.9/crawler_commons.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      346 2023-05-15 10:18:18.000000 crawler_commons-0.0.9/crawler_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       19 2023-05-15 10:18:18.000000 crawler_commons-0.0.9/crawler_commons.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-15 10:18:18.000000 crawler_commons-0.0.9/crawler_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-15 10:18:18.000000 crawler_commons-0.0.9/setup.cfg
```

### Comparing `crawler_commons-0.0.8/crawlutils/text_utils.py` & `crawler_commons-0.0.9/crawlutils/text_utils.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.8/crawlutils/date_utils.py` & `crawler_commons-0.0.9/crawlutils/date_utils.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.8/crawlutils/__init__.py` & `crawler_commons-0.0.9/crawlutils/__init__.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.8/crawlutils/num_utils.py` & `crawler_commons-0.0.9/crawlutils/num_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 def defaultIfNumber(text, unit_multiplier, default="-"):
     op_num = make_num(text)
     op = default if op_num == '-' or op_num == '' else round(float(op_num) * unit_multiplier)
     return op
 
 def to_int(text) -> int:
     try:
-        return int(text.replace(",", "").replace(" ", ""))
+        t = text.replace(",", "").replace(" ", "")
+        return np.nan if t == '' else int(t)
     except Exception as ex:
         logging.exception(ex)
         return np.nan
 
 def to_float(text) -> float:
     try:
         return float(text.replace(",", "").replace(" ", ""))
```

### Comparing `crawler_commons-0.0.8/crawlutils/soup_traversal.py` & `crawler_commons-0.0.9/crawlutils/soup_traversal.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.8/LICENSE` & `crawler_commons-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.8/crawapi/__init__.py` & `crawler_commons-0.0.9/crawapi/__init__.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.8/setup.py` & `crawler_commons-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="crawler_commons",
-    version="0.0.8",
+    version="0.0.9",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="crawler commons",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/crawler_commons",
     packages=setuptools.find_packages(exclude=("test",)),
```

