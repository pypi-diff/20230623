# Comparing `tmp/tarn-0.7.0.tar.gz` & `tmp/tarn-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.7.0.tar", last modified: Tue Jun 20 16:08:05 2023, max compression
+gzip compressed data, was "tarn-0.7.1.tar", last modified: Fri Jun 23 12:54:03 2023, max compression
```

## Comparing `tarn-0.7.0.tar` & `tarn-0.7.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.920478 tarn-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-20 16:08:03.000000 tarn-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-20 16:08:03.000000 tarn-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-20 16:08:05.920478 tarn-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-20 16:08:03.000000 tarn-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-20 16:08:03.000000 tarn-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 16:08:03.000000 tarn-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:08:05.920478 tarn-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-20 16:08:03.000000 tarn-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.920478 tarn-0.7.0/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/tools/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-20 16:08:05.000000 tarn-0.7.0/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 16:08:05.000000 tarn-0.7.0/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:08:05.000000 tarn-0.7.0/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 16:08:05.000000 tarn-0.7.0/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 16:08:05.000000 tarn-0.7.0/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.651293 tarn-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-23 12:53:58.000000 tarn-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 12:53:58.000000 tarn-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-23 12:54:03.651293 tarn-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-23 12:53:58.000000 tarn-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-23 12:53:58.000000 tarn-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 12:53:58.000000 tarn-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 12:54:03.651293 tarn-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-23 12:53:58.000000 tarn-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.643293 tarn-0.7.1/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.647293 tarn-0.7.1/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.651293 tarn-0.7.1/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/tools/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-23 12:53:58.000000 tarn-0.7.1/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:54:03.643293 tarn-0.7.1/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-23 12:54:03.000000 tarn-0.7.1/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 12:54:03.000000 tarn-0.7.1/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:54:03.000000 tarn-0.7.1/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 12:54:03.000000 tarn-0.7.1/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 12:54:03.000000 tarn-0.7.1/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.7.0/LICENSE` & `tarn-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/PKG-INFO` & `tarn-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.7.0
+Version: 0.7.1
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.7.0.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.7.1.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.7.0/README.md` & `tarn-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/pyproject.toml` & `tarn-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/setup.py` & `tarn-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/cache/storage.py` & `tarn-0.7.1/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/compat.py` & `tarn-0.7.1/tarn/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/config.py` & `tarn-0.7.1/tarn/config.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/digest.py` & `tarn-0.7.1/tarn/digest.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/interface.py` & `tarn-0.7.1/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/local/storage.py` & `tarn-0.7.1/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/location/disk_dict.py` & `tarn-0.7.1/tarn/location/disk_dict.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/location/fanout.py` & `tarn-0.7.1/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/location/interface.py` & `tarn-0.7.1/tarn/location/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/location/levels.py` & `tarn-0.7.1/tarn/location/levels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/location/nginx.py` & `tarn-0.7.1/tarn/location/nginx.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/location/scp.py` & `tarn-0.7.1/tarn/location/scp.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/pickler/compat.py` & `tarn-0.7.1/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/pickler/interface.py` & `tarn-0.7.1/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/pool/hash_key.py` & `tarn-0.7.1/tarn/pool/hash_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/pool/pickle_key.py` & `tarn-0.7.1/tarn/pool/pickle_key.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/serializers.py` & `tarn-0.7.1/tarn/serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,22 @@
         for serializer in self.serializers:
             with suppress(SerializerError):
                 return list(serializer.save(value, write))
 
         raise SerializerError(f'No serializer was able to save the value of type {type(value).__name__!r}.')
 
     def load(self, contents: ContentsIn, read: Callable) -> Any:
+        # TODO: old style
+        if isinstance(contents, (str, Path)):
+            contents = [
+                (str(file.relative_to(contents)), bytes.fromhex(file.read_text())) 
+                for file in contents.glob('**/*') if not file.is_dir()
+            ]
+            read = read.read
+
         contents = list(contents)
         for serializer in self.serializers:
             with suppress(SerializerError):
                 # TODO: old style
                 if list(inspect.signature(serializer.load).parameters)[0] == 'folder':
                     with TemporaryDirectory() as folder:
                         folder = Path(folder)
```

### Comparing `tarn-0.7.0/tarn/tools/labels.py` & `tarn-0.7.1/tarn/tools/labels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/tools/locker.py` & `tarn-0.7.1/tarn/tools/locker.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/tools/size.py` & `tarn-0.7.1/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/tools/usage.py` & `tarn-0.7.1/tarn/tools/usage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn/utils.py` & `tarn-0.7.1/tarn/utils.py`

 * *Files identical despite different names*

### Comparing `tarn-0.7.0/tarn.egg-info/PKG-INFO` & `tarn-0.7.1/tarn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.7.0
+Version: 0.7.1
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.7.0.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.7.1.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.7.0/tarn.egg-info/SOURCES.txt` & `tarn-0.7.1/tarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

