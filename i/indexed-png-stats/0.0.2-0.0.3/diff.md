# Comparing `tmp/indexed-png-stats-0.0.2.tar.gz` & `tmp/indexed-png-stats-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexed-png-stats-0.0.2.tar", last modified: Thu Jun 15 00:27:00 2023, max compression
+gzip compressed data, was "indexed-png-stats-0.0.3.tar", last modified: Thu Jun 22 22:50:58 2023, max compression
```

## Comparing `indexed-png-stats-0.0.2.tar` & `indexed-png-stats-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      198 2023-06-15 00:25:51.000000 indexed-png-stats-0.0.2/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       48 2023-06-14 03:58:06.000000 indexed-png-stats-0.0.2/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 indexed-png-stats-0.0.2/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      860 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1159 2023-06-15 00:25:51.000000 indexed-png-stats-0.0.2/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1154 2023-06-15 00:26:16.000000 indexed-png-stats-0.0.2/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/src/indexed_png_stats/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-06-14 03:58:34.000000 indexed-png-stats-0.0.2/src/indexed_png_stats/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     6014 2023-06-15 00:24:47.000000 indexed-png-stats-0.0.2/src/indexed_png_stats/generate.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-15 00:27:00.141223 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      860 2023-06-15 00:26:59.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      398 2023-06-15 00:27:00.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-06-15 00:26:59.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       75 2023-06-15 00:26:59.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/entry_points.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       13 2023-06-15 00:26:59.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       18 2023-06-15 00:26:59.000000 indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-22 22:50:58.798411 indexed-png-stats-0.0.3/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      350 2023-06-22 22:48:06.000000 indexed-png-stats-0.0.3/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      219 2023-06-22 22:49:52.000000 indexed-png-stats-0.0.3/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 indexed-png-stats-0.0.3/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1263 2023-06-22 22:50:58.798411 indexed-png-stats-0.0.3/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1332 2023-06-22 22:49:52.000000 indexed-png-stats-0.0.3/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-06-22 22:50:58.798411 indexed-png-stats-0.0.3/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1154 2023-06-22 22:48:06.000000 indexed-png-stats-0.0.3/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-22 22:50:58.794411 indexed-png-stats-0.0.3/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-22 22:50:58.794411 indexed-png-stats-0.0.3/src/indexed_png_stats/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        0 2023-06-14 03:58:34.000000 indexed-png-stats-0.0.3/src/indexed_png_stats/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     6098 2023-06-22 22:45:41.000000 indexed-png-stats-0.0.3/src/indexed_png_stats/generate.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-06-22 22:50:58.798411 indexed-png-stats-0.0.3/src/indexed_png_stats.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1263 2023-06-22 22:50:58.000000 indexed-png-stats-0.0.3/src/indexed_png_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      398 2023-06-22 22:50:58.000000 indexed-png-stats-0.0.3/src/indexed_png_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-06-22 22:50:58.000000 indexed-png-stats-0.0.3/src/indexed_png_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       75 2023-06-22 22:50:58.000000 indexed-png-stats-0.0.3/src/indexed_png_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       13 2023-06-22 22:50:58.000000 indexed-png-stats-0.0.3/src/indexed_png_stats.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       18 2023-06-22 22:50:58.000000 indexed-png-stats-0.0.3/src/indexed_png_stats.egg-info/top_level.txt
```

### Comparing `indexed-png-stats-0.0.2/PKG-INFO` & `indexed-png-stats-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Metadata-Version: 1.1
 Name: indexed-png-stats
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library that inspects indexed PNG files.
 Home-page: https://github.com/waikato-datamining/indexed-png-stats
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT
-Description: Python library that inspects indexed PNG files.
+Description: Python library that inspects indexed PNG files and outputs the pixel counts
+        per palette entry.
+        Can inspect multiple directories and work recursively as well.
+        Output can be as summary or per file, in plain-text or JSON.
         
         Changelog
         =========
         
+        0.0.3 (2023-06-23)
+        ------------------
+        
+        - fixed recursive analysis, no longer iterates through characters of path,
+          verbose flag is passed on now too
+        
+        
         0.0.2 (2023-06-15)
         ------------------
         
         - added missing MANIFEST.in
         - `--image_dir` supports multiple directories now
```

### Comparing `indexed-png-stats-0.0.2/README.md` & `indexed-png-stats-0.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # indexed-png-stats
-Python library that inspects indexed PNG files.
+Python library that inspects indexed PNG files and outputs the pixel counts
+per palette entry.
+Can inspect multiple directories and work recursively as well.
+Output can be as summary or per file, in plain-text or JSON.  
 
 ## Installation
 
 ```
 pip install indexed-png-stats
 ```
```

### Comparing `indexed-png-stats-0.0.2/setup.py` & `indexed-png-stats-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     },
     packages=find_namespace_packages(where='src'),
     entry_points={
         "console_scripts": [
             "indexed-png-stats=indexed_png_stats.generate:sys_main",
         ]
     },
-    version="0.0.2",
+    version="0.0.3",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
     install_requires=[
         "pillow",
         "numpy",
     ]
 )
```

### Comparing `indexed-png-stats-0.0.2/src/indexed_png_stats/generate.py` & `indexed-png-stats-0.0.3/src/indexed_png_stats/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,31 +28,34 @@
 def collect(stats, image_dirs, recursive=False, stats_type=STATS_TYPE_SUMMARY, verbose=False):
     """
     Collects the statistics from the indexed PNG files.
 
     :param stats: the stats to append to
     :type stats: dict
     :param image_dirs: the directory to look for PNG files
-    :type image_dirs: str
+    :type image_dirs: list
     :param recursive: whether to search recursively for PNG files
     :type recursive: bool
     :param stats_type: the type of stats to generate
     :type stats_type: str
     :param verbose: whether to output some logging information
     :type verbose: bool
     """
     for image_dir in image_dirs:
         if verbose:
             print("Entering: %s" % image_dir)
         for f in os.listdir(image_dir):
+            if f == "." or f == "..":
+                continue
+
             full = os.path.join(image_dir, f)
 
             # recurse?
             if recursive and os.path.isdir(full):
-                collect(stats, full, recursive=True, stats_type=stats_type)
+                collect(stats, [full], recursive=True, stats_type=stats_type, verbose=verbose)
                 print("Back in: %s" % image_dir)
 
             # png?
             if f.lower().endswith(".png"):
                 if verbose:
                     print("%s" % f)
```

### Comparing `indexed-png-stats-0.0.2/src/indexed_png_stats.egg-info/PKG-INFO` & `indexed-png-stats-0.0.3/src/indexed_png_stats.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Metadata-Version: 1.1
 Name: indexed-png-stats
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library that inspects indexed PNG files.
 Home-page: https://github.com/waikato-datamining/indexed-png-stats
 Author: Peter Reutemann
 Author-email: fracpete@waikato.ac.nz
 License: MIT
-Description: Python library that inspects indexed PNG files.
+Description: Python library that inspects indexed PNG files and outputs the pixel counts
+        per palette entry.
+        Can inspect multiple directories and work recursively as well.
+        Output can be as summary or per file, in plain-text or JSON.
         
         Changelog
         =========
         
+        0.0.3 (2023-06-23)
+        ------------------
+        
+        - fixed recursive analysis, no longer iterates through characters of path,
+          verbose flag is passed on now too
+        
+        
         0.0.2 (2023-06-15)
         ------------------
         
         - added missing MANIFEST.in
         - `--image_dir` supports multiple directories now
```

