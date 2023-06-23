# Comparing `tmp/Akatosh-1.7.3.tar.gz` & `tmp/Akatosh-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-1.7.3.tar", last modified: Wed Jun 21 13:17:54 2023, max compression
+gzip compressed data, was "Akatosh-2.0.5.tar", last modified: Fri Jun 23 15:17:06 2023, max compression
```

## Comparing `Akatosh-1.7.3.tar` & `Akatosh-2.0.5.tar`

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
+drwxrwxrwx   0        0        0        0 2023-06-23 15:17:06.182309 Akatosh-2.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-23 15:17:06.170313 Akatosh-2.0.5/Akatosh/
+-rw-rw-rw-   0        0        0      120 2023-06-23 07:41:14.000000 Akatosh-2.0.5/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0     4449 2023-06-23 15:13:28.000000 Akatosh-2.0.5/Akatosh/event.py
+-rw-rw-rw-   0        0        0      387 2023-06-23 07:55:30.000000 Akatosh-2.0.5/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     6178 2023-06-23 08:29:24.000000 Akatosh-2.0.5/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      172 2023-06-22 11:35:11.000000 Akatosh-2.0.5/Akatosh/states.py
+-rw-rw-rw-   0        0        0     2816 2023-06-23 15:12:05.000000 Akatosh-2.0.5/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-06-23 15:17:06.179313 Akatosh-2.0.5/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2011 2023-06-23 15:17:06.000000 Akatosh-2.0.5/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-23 15:17:06.000000 Akatosh-2.0.5/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 15:17:06.000000 Akatosh-2.0.5/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 15:17:06.000000 Akatosh-2.0.5/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2011 2023-06-23 15:17:06.181309 Akatosh-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1482 2023-06-21 04:34:02.000000 Akatosh-2.0.5/README.md
+-rw-rw-rw-   0        0        0      580 2023-06-23 15:16:41.000000 Akatosh-2.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 15:17:06.182309 Akatosh-2.0.5/setup.cfg
```

### Comparing `Akatosh-1.7.3/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.0.5/Akatosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 1.7.3
+Version: 2.0.5
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Akatosh-1.7.3/PKG-INFO` & `Akatosh-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 1.7.3
+Version: 2.0.5
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Akatosh-1.7.3/README.md` & `Akatosh-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-1.7.3/pyproject.toml` & `Akatosh-2.0.5/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "1.7.3"
+version = "2.0.5"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -14,11 +14,7 @@
 [project.urls]
 "Homepage" = "https://github.com/ulfaric/Akatosh"
 "Bug Tracker" = "https://github.com/ulfaric/Akatosh/issues"
 
 [tool.setuptools]
 packages = ["Akatosh"]
 
-[tool.pytest.ini_options]
-minversion = "6.0"
-addopts = "-ra -q"
-testpaths = ["test"]
```

