# Comparing `tmp/PyEmailExtractor-0.1.tar.gz` & `tmp/PyEmailExtractor-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEmailExtractor-0.1.tar", last modified: Thu Jun 22 13:11:24 2023, max compression
+gzip compressed data, was "PyEmailExtractor-0.2.tar", last modified: Fri Jun 23 08:40:11 2023, max compression
```

## Comparing `PyEmailExtractor-0.1.tar` & `PyEmailExtractor-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 13:11:24.532441 PyEmailExtractor-0.1/
--rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 13:11:24.532441 PyEmailExtractor-0.1/PKG-INFO
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 13:11:24.532441 PyEmailExtractor-0.1/PyEmailExtractor/
--rw-rw-r--   0 karki     (1000) karki     (1000)      132 2023-06-22 10:33:58.000000 PyEmailExtractor-0.1/PyEmailExtractor/__init__.py
--rw-rw-r--   0 karki     (1000) karki     (1000)      958 2023-06-22 10:33:25.000000 PyEmailExtractor-0.1/PyEmailExtractor/driver.py
--rw-rw-r--   0 karki     (1000) karki     (1000)     1898 2023-06-22 10:33:31.000000 PyEmailExtractor-0.1/PyEmailExtractor/helper.py
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 13:11:24.532441 PyEmailExtractor-0.1/PyEmailExtractor.egg-info/
--rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 13:11:24.000000 PyEmailExtractor-0.1/PyEmailExtractor.egg-info/PKG-INFO
--rw-rw-r--   0 karki     (1000) karki     (1000)      300 2023-06-22 13:11:24.000000 PyEmailExtractor-0.1/PyEmailExtractor.egg-info/SOURCES.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)        1 2023-06-22 13:11:24.000000 PyEmailExtractor-0.1/PyEmailExtractor.egg-info/dependency_links.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)       76 2023-06-22 13:11:24.000000 PyEmailExtractor-0.1/PyEmailExtractor.egg-info/requires.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)       17 2023-06-22 13:11:24.000000 PyEmailExtractor-0.1/PyEmailExtractor.egg-info/top_level.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)        0 2023-06-22 09:26:17.000000 PyEmailExtractor-0.1/README.md
--rw-rw-r--   0 karki     (1000) karki     (1000)       38 2023-06-22 13:11:24.532441 PyEmailExtractor-0.1/setup.cfg
--rw-rw-r--   0 karki     (1000) karki     (1000)      473 2023-06-22 13:11:12.000000 PyEmailExtractor-0.1/setup.py
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-23 08:40:11.400879 PyEmailExtractor-0.2/
+-rw-rw-r--   0 karki     (1000) karki     (1000)     1525 2023-06-23 08:40:11.400879 PyEmailExtractor-0.2/PKG-INFO
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-23 08:40:11.396879 PyEmailExtractor-0.2/PyEmailExtractor/
+-rw-rw-r--   0 karki     (1000) karki     (1000)      132 2023-06-22 10:33:58.000000 PyEmailExtractor-0.2/PyEmailExtractor/__init__.py
+-rw-rw-r--   0 karki     (1000) karki     (1000)      958 2023-06-22 10:33:25.000000 PyEmailExtractor-0.2/PyEmailExtractor/driver.py
+-rw-rw-r--   0 karki     (1000) karki     (1000)     1898 2023-06-22 10:33:31.000000 PyEmailExtractor-0.2/PyEmailExtractor/helper.py
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-23 08:40:11.400879 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/
+-rw-rw-r--   0 karki     (1000) karki     (1000)     1525 2023-06-23 08:40:11.000000 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/PKG-INFO
+-rw-rw-r--   0 karki     (1000) karki     (1000)      300 2023-06-23 08:40:11.000000 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/SOURCES.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)        1 2023-06-23 08:40:11.000000 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/dependency_links.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)       76 2023-06-23 08:40:11.000000 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/requires.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)       17 2023-06-23 08:40:11.000000 PyEmailExtractor-0.2/PyEmailExtractor.egg-info/top_level.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)     1275 2023-06-23 08:39:32.000000 PyEmailExtractor-0.2/README.md
+-rw-rw-r--   0 karki     (1000) karki     (1000)       38 2023-06-23 08:40:11.400879 PyEmailExtractor-0.2/setup.cfg
+-rw-rw-r--   0 karki     (1000) karki     (1000)      648 2023-06-23 08:40:09.000000 PyEmailExtractor-0.2/setup.py
```

### Comparing `PyEmailExtractor-0.1/PyEmailExtractor/driver.py` & `PyEmailExtractor-0.2/PyEmailExtractor/driver.py`

 * *Files identical despite different names*

### Comparing `PyEmailExtractor-0.1/PyEmailExtractor/helper.py` & `PyEmailExtractor-0.2/PyEmailExtractor/helper.py`

 * *Files identical despite different names*

