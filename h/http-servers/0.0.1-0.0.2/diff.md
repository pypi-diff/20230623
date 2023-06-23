# Comparing `tmp/http_servers-0.0.1.tar.gz` & `tmp/http_servers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_servers-0.0.1.tar", last modified: Fri Jun 23 12:25:38 2023, max compression
+gzip compressed data, was "http_servers-0.0.2.tar", last modified: Fri Jun 23 12:29:06 2023, max compression
```

## Comparing `http_servers-0.0.1.tar` & `http_servers-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sledeunf  (1001) ovh       (1001)        0 2023-06-23 12:25:38.579317 http_servers-0.0.1/
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)       56 2023-06-23 12:25:38.579317 http_servers-0.0.1/PKG-INFO
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)      844 2023-06-23 12:25:20.000000 http_servers-0.0.1/README.md
-drwxr-xr-x   0 sledeunf  (1001) ovh       (1001)        0 2023-06-23 12:25:38.579317 http_servers-0.0.1/http_servers/
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)        0 2023-06-22 16:44:44.000000 http_servers-0.0.1/http_servers/__init__.py
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)       90 2023-06-23 12:24:10.000000 http_servers-0.0.1/http_servers/__main__.py
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)     1127 2023-06-23 12:25:00.000000 http_servers-0.0.1/http_servers/commands.py
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)      147 2023-06-23 12:24:38.000000 http_servers-0.0.1/http_servers/options.py
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)     1233 2023-06-23 12:25:00.000000 http_servers-0.0.1/http_servers/parser.py
-drwxr-xr-x   0 sledeunf  (1001) ovh       (1001)        0 2023-06-23 12:25:38.579317 http_servers-0.0.1/http_servers.egg-info/
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)       56 2023-06-23 12:25:38.000000 http_servers-0.0.1/http_servers.egg-info/PKG-INFO
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)      329 2023-06-23 12:25:38.000000 http_servers-0.0.1/http_servers.egg-info/SOURCES.txt
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)        1 2023-06-23 12:25:38.000000 http_servers-0.0.1/http_servers.egg-info/dependency_links.txt
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)       64 2023-06-23 12:25:38.000000 http_servers-0.0.1/http_servers.egg-info/entry_points.txt
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)       13 2023-06-23 12:25:38.000000 http_servers-0.0.1/http_servers.egg-info/top_level.txt
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)      135 2023-06-23 12:23:53.000000 http_servers-0.0.1/pyproject.toml
--rw-r--r--   0 sledeunf  (1001) ovh       (1001)       38 2023-06-23 12:25:38.579317 http_servers-0.0.1/setup.cfg
+drwxr-xr-x   0 sledeunf  (1001) ovh       (1001)        0 2023-06-23 12:29:06.444806 http_servers-0.0.2/
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)     1026 2023-06-23 12:29:06.444806 http_servers-0.0.2/PKG-INFO
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)      845 2023-06-23 12:26:41.000000 http_servers-0.0.2/README.md
+drwxr-xr-x   0 sledeunf  (1001) ovh       (1001)        0 2023-06-23 12:29:06.444806 http_servers-0.0.2/http_servers/
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)        0 2023-06-22 16:44:44.000000 http_servers-0.0.2/http_servers/__init__.py
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)       90 2023-06-23 12:24:10.000000 http_servers-0.0.2/http_servers/__main__.py
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)     1127 2023-06-23 12:25:00.000000 http_servers-0.0.2/http_servers/commands.py
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)      147 2023-06-23 12:24:38.000000 http_servers-0.0.2/http_servers/options.py
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)     1233 2023-06-23 12:25:00.000000 http_servers-0.0.2/http_servers/parser.py
+drwxr-xr-x   0 sledeunf  (1001) ovh       (1001)        0 2023-06-23 12:29:06.444806 http_servers-0.0.2/http_servers.egg-info/
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)     1026 2023-06-23 12:29:06.000000 http_servers-0.0.2/http_servers.egg-info/PKG-INFO
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)      329 2023-06-23 12:29:06.000000 http_servers-0.0.2/http_servers.egg-info/SOURCES.txt
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)        1 2023-06-23 12:29:06.000000 http_servers-0.0.2/http_servers.egg-info/dependency_links.txt
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)       64 2023-06-23 12:29:06.000000 http_servers-0.0.2/http_servers.egg-info/entry_points.txt
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)       13 2023-06-23 12:29:06.000000 http_servers-0.0.2/http_servers.egg-info/top_level.txt
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)      247 2023-06-23 12:28:57.000000 http_servers-0.0.2/pyproject.toml
+-rw-r--r--   0 sledeunf  (1001) ovh       (1001)       38 2023-06-23 12:29:06.444806 http_servers-0.0.2/setup.cfg
```

### Comparing `http_servers-0.0.1/README.md` & `http_servers-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 * Similar to node.js http-server, but without the need to install node
 * This package doesn't bring additional dependencies
 
 ## Installation
 
 ```python
-pip install http-server
+pip install http-servers
 ```
 
 ## Documentation - RTF(riendly)M
 
 ```
 $ http-server --help
 usage: http-server [--cors] [-h HOST] [-p PORT] [-d SOURCE_DIR] [--cache] [--help]
```

### Comparing `http_servers-0.0.1/http_servers/commands.py` & `http_servers-0.0.2/http_servers/commands.py`

 * *Files identical despite different names*

### Comparing `http_servers-0.0.1/http_servers/parser.py` & `http_servers-0.0.2/http_servers/parser.py`

 * *Files identical despite different names*

