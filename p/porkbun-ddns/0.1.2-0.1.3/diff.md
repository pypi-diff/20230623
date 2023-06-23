# Comparing `tmp/porkbun-ddns-0.1.2.tar.gz` & `tmp/porkbun-ddns-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porkbun-ddns-0.1.2.tar", last modified: Fri Jun 23 13:01:00 2023, max compression
+gzip compressed data, was "porkbun-ddns-0.1.3.tar", last modified: Fri Jun 23 13:26:55 2023, max compression
```

## Comparing `porkbun-ddns-0.1.2.tar` & `porkbun-ddns-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:01:00.012397 porkbun-ddns-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-23 13:01:00.012397 porkbun-ddns-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:01:00.012397 porkbun-ddns-0.1.2/porkbun_ddns/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/porkbun_ddns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/porkbun_ddns/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/porkbun_ddns/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/porkbun_ddns/porkbun_ddns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:01:00.012397 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-23 13:01:00.000000 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 13:01:00.000000 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:01:00.000000 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 13:01:00.000000 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 13:01:00.000000 porkbun-ddns-0.1.2/porkbun_ddns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 13:01:00.012397 porkbun-ddns-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-23 13:00:47.000000 porkbun-ddns-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:26:55.271616 porkbun-ddns-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-23 13:26:44.000000 porkbun-ddns-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-23 13:26:55.271616 porkbun-ddns-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-23 13:26:44.000000 porkbun-ddns-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:26:55.271616 porkbun-ddns-0.1.3/porkbun_ddns/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 13:26:44.000000 porkbun-ddns-0.1.3/porkbun_ddns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-23 13:26:44.000000 porkbun-ddns-0.1.3/porkbun_ddns/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-23 13:26:44.000000 porkbun-ddns-0.1.3/porkbun_ddns/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-06-23 13:26:44.000000 porkbun-ddns-0.1.3/porkbun_ddns/porkbun_ddns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:26:55.271616 porkbun-ddns-0.1.3/porkbun_ddns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-23 13:26:55.000000 porkbun-ddns-0.1.3/porkbun_ddns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 13:26:55.000000 porkbun-ddns-0.1.3/porkbun_ddns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:26:55.000000 porkbun-ddns-0.1.3/porkbun_ddns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-23 13:26:55.000000 porkbun-ddns-0.1.3/porkbun_ddns.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 13:26:55.000000 porkbun-ddns-0.1.3/porkbun_ddns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 13:26:55.271616 porkbun-ddns-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-23 13:26:44.000000 porkbun-ddns-0.1.3/setup.py
```

### Comparing `porkbun-ddns-0.1.2/LICENSE` & `porkbun-ddns-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.1.2/PKG-INFO` & `porkbun-ddns-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porkbun-ddns
-Version: 0.1.2
+Version: 0.1.3
 Summary: A unofficial DDNS-Client for Porkbun domains
 Home-page: https://github.com/mietzen/porkbun-ddns
 Author: Nils Stein
 Author-email: github.nstein@mailbox.org
 License: MIT
 Keywords: porkbun ddns
 Classifier: Development Status :: 4 - Beta
```

### Comparing `porkbun-ddns-0.1.2/README.md` & `porkbun-ddns-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.1.2/porkbun_ddns/cli.py` & `porkbun-ddns-0.1.3/porkbun_ddns/cli.py`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.1.2/porkbun_ddns/helpers.py` & `porkbun-ddns-0.1.3/porkbun_ddns/helpers.py`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.1.2/porkbun_ddns/porkbun_ddns.py` & `porkbun-ddns-0.1.3/porkbun_ddns/porkbun_ddns.py`

 * *Files identical despite different names*

### Comparing `porkbun-ddns-0.1.2/porkbun_ddns.egg-info/PKG-INFO` & `porkbun-ddns-0.1.3/porkbun_ddns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porkbun-ddns
-Version: 0.1.2
+Version: 0.1.3
 Summary: A unofficial DDNS-Client for Porkbun domains
 Home-page: https://github.com/mietzen/porkbun-ddns
 Author: Nils Stein
 Author-email: github.nstein@mailbox.org
 License: MIT
 Keywords: porkbun ddns
 Classifier: Development Status :: 4 - Beta
```

### Comparing `porkbun-ddns-0.1.2/setup.py` & `porkbun-ddns-0.1.3/setup.py`

 * *Files identical despite different names*

