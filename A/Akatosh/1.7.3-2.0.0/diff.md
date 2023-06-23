# Comparing `tmp/Akatosh-1.7.3.tar.gz` & `tmp/Akatosh-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-1.7.3.tar", last modified: Wed Jun 21 13:17:54 2023, max compression
+gzip compressed data, was "Akatosh-2.0.0.tar", last modified: Fri Jun 23 11:22:21 2023, max compression
```

## Comparing `Akatosh-1.7.3.tar` & `Akatosh-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.529914 Akatosh-1.7.3/
-drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.509910 Akatosh-1.7.3/Akatosh/
--rw-rw-rw-   0        0        0      129 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/__init__.py
--rw-rw-rw-   0        0        0    16093 2023-06-21 13:15:43.000000 Akatosh-1.7.3/Akatosh/actor.py
--rw-rw-rw-   0        0        0     1073 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/event.py
--rw-rw-rw-   0        0        0     6678 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/producer.py
--rw-rw-rw-   0        0        0    11540 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/resource.py
--rw-rw-rw-   0        0        0     1443 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/timeline.py
--rw-rw-rw-   0        0        0     2443 2023-06-21 04:34:02.000000 Akatosh-1.7.3/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.518911 Akatosh-1.7.3/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2011 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 13:17:54.000000 Akatosh-1.7.3/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2011 2023-06-21 13:17:54.528915 Akatosh-1.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     1482 2023-06-21 04:34:02.000000 Akatosh-1.7.3/README.md
--rw-rw-rw-   0        0        0      669 2023-06-21 13:16:13.000000 Akatosh-1.7.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 13:17:54.529914 Akatosh-1.7.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-21 13:17:54.525910 Akatosh-1.7.3/test/
--rw-rw-rw-   0        0        0      169 2023-06-21 04:34:02.000000 Akatosh-1.7.3/test/test_actor.py
--rw-rw-rw-   0        0        0      245 2023-06-21 04:34:02.000000 Akatosh-1.7.3/test/test_decorator.py
--rw-rw-rw-   0        0        0      298 2023-06-21 04:34:02.000000 Akatosh-1.7.3/test/test_resource.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:22:21.813570 Akatosh-2.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-23 11:22:21.799563 Akatosh-2.0.0/Akatosh/
+-rw-rw-rw-   0        0        0      120 2023-06-23 07:41:14.000000 Akatosh-2.0.0/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0     4324 2023-06-23 11:20:36.000000 Akatosh-2.0.0/Akatosh/event.py
+-rw-rw-rw-   0        0        0      387 2023-06-23 07:55:30.000000 Akatosh-2.0.0/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     6178 2023-06-23 08:29:24.000000 Akatosh-2.0.0/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      172 2023-06-22 11:35:11.000000 Akatosh-2.0.0/Akatosh/states.py
+-rw-rw-rw-   0        0        0     2362 2023-06-23 05:37:35.000000 Akatosh-2.0.0/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:22:21.809568 Akatosh-2.0.0/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2011 2023-06-23 11:22:21.000000 Akatosh-2.0.0/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-23 11:22:21.000000 Akatosh-2.0.0/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 11:22:21.000000 Akatosh-2.0.0/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 11:22:21.000000 Akatosh-2.0.0/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2011 2023-06-23 11:22:21.811569 Akatosh-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1482 2023-06-21 04:34:02.000000 Akatosh-2.0.0/README.md
+-rw-rw-rw-   0        0        0      669 2023-06-23 11:21:48.000000 Akatosh-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 11:22:21.813570 Akatosh-2.0.0/setup.cfg
```

### Comparing `Akatosh-1.7.3/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.0.0/Akatosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 1.7.3
+Version: 2.0.0
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Akatosh-1.7.3/PKG-INFO` & `Akatosh-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 1.7.3
+Version: 2.0.0
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Akatosh-1.7.3/README.md` & `Akatosh-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.3/pyproject.toml` & `Akatosh-2.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "1.7.3"
+version = "2.0.0"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

