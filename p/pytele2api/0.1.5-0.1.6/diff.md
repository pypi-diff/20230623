# Comparing `tmp/pytele2api-0.1.5.tar.gz` & `tmp/pytele2api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytele2api-0.1.5.tar", last modified: Sun Jun  4 21:30:07 2023, max compression
+gzip compressed data, was "pytele2api-0.1.6.tar", last modified: Fri Jun 23 06:54:46 2023, max compression
```

## Comparing `pytele2api-0.1.5.tar` & `pytele2api-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-04 21:30:07.395653 pytele2api-0.1.5/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1062 2023-06-01 07:29:48.000000 pytele2api-0.1.5/LICENSE
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       16 2023-06-01 06:30:04.000000 pytele2api-0.1.5/MANIFEST.in
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-04 21:30:07.395702 pytele2api-0.1.5/PKG-INFO
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       65 2023-06-01 06:25:52.000000 pytele2api-0.1.5/README.md
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-04 21:30:07.394888 pytele2api-0.1.5/pytele2api/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     4396 2023-06-04 21:21:07.000000 pytele2api-0.1.5/pytele2api/Tele2Api.py
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       31 2023-06-01 07:21:21.000000 pytele2api-0.1.5/pytele2api/__init__.py
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      504 2023-06-04 21:19:17.000000 pytele2api-0.1.5/pytele2api/const.py
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-04 21:30:07.395546 pytele2api-0.1.5/pytele2api.egg-info/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-04 21:30:07.000000 pytele2api-0.1.5/pytele2api.egg-info/PKG-INFO
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      283 2023-06-04 21:30:07.000000 pytele2api-0.1.5/pytele2api.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)        1 2023-06-04 21:30:07.000000 pytele2api-0.1.5/pytele2api.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       18 2023-06-04 21:30:07.000000 pytele2api-0.1.5/pytele2api.egg-info/requires.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       11 2023-06-04 21:30:07.000000 pytele2api-0.1.5/pytele2api.egg-info/top_level.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       79 2023-06-04 21:30:07.395884 pytele2api-0.1.5/setup.cfg
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1045 2023-06-04 21:15:13.000000 pytele2api-0.1.5/setup.py
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-23 06:54:46.354145 pytele2api-0.1.6/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1062 2023-06-01 07:29:48.000000 pytele2api-0.1.6/LICENSE
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       16 2023-06-01 06:30:04.000000 pytele2api-0.1.6/MANIFEST.in
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-23 06:54:46.354191 pytele2api-0.1.6/PKG-INFO
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       65 2023-06-01 06:25:52.000000 pytele2api-0.1.6/README.md
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-23 06:54:46.353215 pytele2api-0.1.6/pytele2api/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     5026 2023-06-23 06:50:00.000000 pytele2api-0.1.6/pytele2api/Tele2Api.py
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       31 2023-06-01 07:21:21.000000 pytele2api-0.1.6/pytele2api/__init__.py
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      538 2023-06-23 06:47:10.000000 pytele2api-0.1.6/pytele2api/const.py
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-23 06:54:46.354048 pytele2api-0.1.6/pytele2api.egg-info/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-23 06:54:46.000000 pytele2api-0.1.6/pytele2api.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      283 2023-06-23 06:54:46.000000 pytele2api-0.1.6/pytele2api.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)        1 2023-06-23 06:54:46.000000 pytele2api-0.1.6/pytele2api.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       18 2023-06-23 06:54:46.000000 pytele2api-0.1.6/pytele2api.egg-info/requires.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       11 2023-06-23 06:54:46.000000 pytele2api-0.1.6/pytele2api.egg-info/top_level.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       79 2023-06-23 06:54:46.354362 pytele2api-0.1.6/setup.cfg
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1045 2023-06-23 06:50:48.000000 pytele2api-0.1.6/setup.py
```

### Comparing `pytele2api-0.1.5/LICENSE` & `pytele2api-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytele2api-0.1.5/PKG-INFO` & `pytele2api-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytele2api
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python library for communication with Tele2 My TSO
 Home-page: https://github.com/fredrikhaggbom/pytele2
 Author: Fredrik Häggbom
 Author-email: fredrik.haggbom@gmail.com
 License: MIT
-Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.5.tar.gz
+Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.6.tar.gz
 Keywords: tele2
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pytele2api-0.1.5/pytele2api/Tele2Api.py` & `pytele2api-0.1.6/pytele2api/Tele2Api.py`

 * *Files 18% similar despite different names*

```diff
@@ -93,25 +93,34 @@
                 )
                 self._data[RES_ERROR] = None
 
                 if Tele2ApiResult.unlimitedData in data:
                     self._data[RES_UNLIMITED] = data[Tele2ApiResult.unlimitedData]
 
                 if Tele2ApiResult.buckets in data and len(data["buckets"]) > 0:
-                    bucket = data["buckets"][0]
-                    if Tele2ApiResult.startDate in bucket:
-                        startDate = datetime.datetime.strptime(
-                            bucket[Tele2ApiResult.startDate], "%Y-%m-%d"
-                        ).date()
-                        self._data[RES_PERIOD_START] = startDate
-                    if Tele2ApiResult.endDate in bucket:
-                        endDate = datetime.datetime.strptime(
-                            bucket[Tele2ApiResult.endDate], "%Y-%m-%d"
-                        ).date()
-                        self._data[RES_PERIOD_END] = endDate
+                    for bucket in data["buckets"]:
+                        if bucket["status"] == "active":
+                            if Tele2ApiResult.startDate in bucket:
+                                startDate = datetime.datetime.strptime(
+                                    bucket[Tele2ApiResult.startDate], "%Y-%m-%d"
+                                ).date()
+                                self._data[RES_PERIOD_START] = startDate
+                            if Tele2ApiResult.endDate in bucket:
+                                endDate = datetime.datetime.strptime(
+                                    bucket[Tele2ApiResult.endDate], "%Y-%m-%d"
+                                ).date()
+                                self._data[RES_PERIOD_END] = endDate
+                            if Tele2ApiResult.remaining in bucket:
+                                if bucket[Tele2ApiResult.remaining] is None:
+                                    remaining = limit
+                                if Tele2ApiResult.unlimitedBucket in bucket:
+                                    self._data[RES_UNLIMITED] = bucket[
+                                        Tele2ApiResult.unlimitedBucket
+                                    ]
+                            break
 
                 self.tries = 0
                 self._data[RES_LIMIT] = limit
                 self._data[RES_USAGE] = usage
                 self._data[RES_DATA_LEFT] = remaining
                 self.log("Setting native value to: %d", remaining)
                 return self._data
```

### Comparing `pytele2api-0.1.5/pytele2api.egg-info/PKG-INFO` & `pytele2api-0.1.6/pytele2api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytele2api
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python library for communication with Tele2 My TSO
 Home-page: https://github.com/fredrikhaggbom/pytele2
 Author: Fredrik Häggbom
 Author-email: fredrik.haggbom@gmail.com
 License: MIT
-Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.5.tar.gz
+Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.6.tar.gz
 Keywords: tele2
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pytele2api-0.1.5/setup.py` & `pytele2api-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytele2api",
-    version="0.1.5",
+    version="0.1.6",
     author="Fredrik Häggbom",
     author_email="fredrik.haggbom@gmail.com",
     description="Python library for communication with Tele2 My TSO",
-    download_url="https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.5.tar.gz",
+    download_url="https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.6.tar.gz",
     keywords=["tele2"],
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fredrikhaggbom/pytele2",
     packages=setuptools.find_packages(),
     install_requires=["requests", "datetime"],
```

