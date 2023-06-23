# Comparing `tmp/wave-venture-0.0.8.tar.gz` & `tmp/wave-venture-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wave-venture-0.0.8.tar", last modified: Tue Sep 27 10:48:47 2022, max compression
+gzip compressed data, was "wave-venture-0.0.9.tar", last modified: Fri Nov 18 16:17:06 2022, max compression
```

## Comparing `wave-venture-0.0.8.tar` & `wave-venture-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 10:48:47.209270 wave-venture-0.0.8/
--rw-r--r--   0 runner    (1000) runner    (1000)       37 2022-09-26 11:17:01.000000 wave-venture-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1000) runner    (1000)     8317 2022-09-27 10:48:47.209270 wave-venture-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     7697 2022-09-26 12:42:10.000000 wave-venture-0.0.8/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2022-09-27 10:48:47.209270 wave-venture-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     2910 2022-09-27 10:44:46.000000 wave-venture-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 10:48:47.201254 wave-venture-0.0.8/wave_venture/
--rw-r--r--   0 runner    (1000) runner    (1000)      179 2022-09-26 11:17:01.000000 wave-venture-0.0.8/wave_venture/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)       63 2022-09-27 10:47:19.000000 wave-venture-0.0.8/wave_venture/__version__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      240 2022-09-26 11:17:01.000000 wave-venture-0.0.8/wave_venture/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5495 2022-09-27 10:44:46.000000 wave-venture-0.0.8/wave_venture/interface.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4014 2022-09-26 11:17:01.000000 wave-venture-0.0.8/wave_venture/plotting.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 10:48:47.205262 wave-venture-0.0.8/wave_venture/resources/
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2022-09-26 11:17:01.000000 wave-venture-0.0.8/wave_venture/resources/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20764 2022-09-26 11:17:01.000000 wave-venture-0.0.8/wave_venture/resources/wave-venture-logo.png
--rw-r--r--   0 runner    (1000) runner    (1000)     4117 2022-09-26 11:17:01.000000 wave-venture-0.0.8/wave_venture/serializer.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4584 2022-09-26 11:17:01.000000 wave-venture-0.0.8/wave_venture/utils.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-09-27 10:48:47.205262 wave-venture-0.0.8/wave_venture.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     8317 2022-09-27 10:48:47.000000 wave-venture-0.0.8/wave_venture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      465 2022-09-27 10:48:47.000000 wave-venture-0.0.8/wave_venture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2022-09-27 10:48:47.000000 wave-venture-0.0.8/wave_venture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       78 2022-09-27 10:48:47.000000 wave-venture-0.0.8/wave_venture.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2022-09-27 10:48:47.000000 wave-venture-0.0.8/wave_venture.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-11-18 16:17:06.287944 wave-venture-0.0.9/
+-rw-r--r--   0 runner    (1000) runner    (1000)       37 2022-09-26 11:17:01.000000 wave-venture-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1000) runner    (1000)     8317 2022-11-18 16:17:06.283946 wave-venture-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     7697 2022-09-26 12:42:10.000000 wave-venture-0.0.9/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2022-11-18 16:17:06.287944 wave-venture-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     2910 2022-09-27 10:44:46.000000 wave-venture-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-11-18 16:17:06.275949 wave-venture-0.0.9/wave_venture/
+-rw-r--r--   0 runner    (1000) runner    (1000)      179 2022-09-26 11:17:01.000000 wave-venture-0.0.9/wave_venture/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       63 2022-11-18 16:15:10.000000 wave-venture-0.0.9/wave_venture/__version__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      240 2022-09-26 11:17:01.000000 wave-venture-0.0.9/wave_venture/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5495 2022-09-27 10:44:46.000000 wave-venture-0.0.9/wave_venture/interface.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4014 2022-09-26 11:17:01.000000 wave-venture-0.0.9/wave_venture/plotting.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-11-18 16:17:06.283946 wave-venture-0.0.9/wave_venture/resources/
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2022-09-26 11:17:01.000000 wave-venture-0.0.9/wave_venture/resources/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20764 2022-09-26 11:17:01.000000 wave-venture-0.0.9/wave_venture/resources/wave-venture-logo.png
+-rw-r--r--   0 runner    (1000) runner    (1000)     5208 2022-11-18 16:15:10.000000 wave-venture-0.0.9/wave_venture/serializer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4584 2022-09-26 11:17:01.000000 wave-venture-0.0.9/wave_venture/utils.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2022-11-18 16:17:06.279947 wave-venture-0.0.9/wave_venture.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     8317 2022-11-18 16:17:06.000000 wave-venture-0.0.9/wave_venture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      465 2022-11-18 16:17:06.000000 wave-venture-0.0.9/wave_venture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2022-11-18 16:17:06.000000 wave-venture-0.0.9/wave_venture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       78 2022-11-18 16:17:06.000000 wave-venture-0.0.9/wave_venture.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2022-11-18 16:17:06.000000 wave-venture-0.0.9/wave_venture.egg-info/top_level.txt
```

### Comparing `wave-venture-0.0.8/PKG-INFO` & `wave-venture-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wave-venture
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wave Venture's Python interface to TE Software API.
 Home-page: https://github.com/waveventure/wv_py
 Author: Wave Venture
 Author-email: admin@wave-venture.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wave-venture-0.0.8/README.md` & `wave-venture-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wave-venture-0.0.8/setup.py` & `wave-venture-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `wave-venture-0.0.8/wave_venture/interface.py` & `wave-venture-0.0.9/wave_venture/interface.py`

 * *Files identical despite different names*

### Comparing `wave-venture-0.0.8/wave_venture/plotting.py` & `wave-venture-0.0.9/wave_venture/plotting.py`

 * *Files identical despite different names*

### Comparing `wave-venture-0.0.8/wave_venture/resources/wave-venture-logo.png` & `wave-venture-0.0.9/wave_venture/resources/wave-venture-logo.png`

 * *Files identical despite different names*

### Comparing `wave-venture-0.0.8/wave_venture/utils.py` & `wave-venture-0.0.9/wave_venture/utils.py`

 * *Files identical despite different names*

### Comparing `wave-venture-0.0.8/wave_venture.egg-info/PKG-INFO` & `wave-venture-0.0.9/wave_venture.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wave-venture
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wave Venture's Python interface to TE Software API.
 Home-page: https://github.com/waveventure/wv_py
 Author: Wave Venture
 Author-email: admin@wave-venture.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

