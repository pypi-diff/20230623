# Comparing `tmp/graphreduce-0.1.tar.gz` & `tmp/graphreduce-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-0.1.tar", last modified: Thu Jun 22 22:04:53 2023, max compression
+gzip compressed data, was "graphreduce-0.2.tar", last modified: Thu Jun 22 22:12:01 2023, max compression
```

## Comparing `graphreduce-0.1.tar` & `graphreduce-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-22 22:04:53.617168 graphreduce-0.1/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     4571 2023-06-22 22:04:53.617051 graphreduce-0.1/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     3597 2023-06-21 15:12:22.000000 graphreduce-0.1/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-22 22:04:53.615908 graphreduce-0.1/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-0.1/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-15 15:13:54.000000 graphreduce-0.1/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    13186 2023-06-22 21:54:31.000000 graphreduce-0.1/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     8891 2023-06-20 22:32:11.000000 graphreduce-0.1/graphreduce/node.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-22 22:04:53.616901 graphreduce-0.1/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     4571 2023-06-22 22:04:53.000000 graphreduce-0.1/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-06-22 22:04:53.000000 graphreduce-0.1/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-22 22:04:53.000000 graphreduce-0.1/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-0.1/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      106 2023-06-22 22:04:53.000000 graphreduce-0.1/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-06-22 22:04:53.000000 graphreduce-0.1/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-06-22 22:04:53.617203 graphreduce-0.1/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1801 2023-06-22 22:04:40.000000 graphreduce-0.1/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-22 22:12:01.963112 graphreduce-0.2/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     4571 2023-06-22 22:12:01.963000 graphreduce-0.2/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     3597 2023-06-21 15:12:22.000000 graphreduce-0.2/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-22 22:12:01.961976 graphreduce-0.2/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-0.2/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      290 2023-06-15 15:13:54.000000 graphreduce-0.2/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    13186 2023-06-22 21:54:31.000000 graphreduce-0.2/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     8891 2023-06-20 22:32:11.000000 graphreduce-0.2/graphreduce/node.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-06-22 22:12:01.962850 graphreduce-0.2/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     4571 2023-06-22 22:12:01.000000 graphreduce-0.2/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      318 2023-06-22 22:12:01.000000 graphreduce-0.2/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-22 22:12:01.000000 graphreduce-0.2/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-0.2/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      106 2023-06-22 22:12:01.000000 graphreduce-0.2/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-06-22 22:12:01.000000 graphreduce-0.2/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-06-22 22:12:01.963146 graphreduce-0.2/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1801 2023-06-22 22:11:30.000000 graphreduce-0.2/setup.py
```

### Comparing `graphreduce-0.1/PKG-INFO` & `graphreduce-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 0.1
+Version: 0.2
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-0.1/README.md` & `graphreduce-0.2/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-0.1/graphreduce/graph_reduce.py` & `graphreduce-0.2/graphreduce/graph_reduce.py`

 * *Files identical despite different names*

### Comparing `graphreduce-0.1/graphreduce/node.py` & `graphreduce-0.2/graphreduce/node.py`

 * *Files identical despite different names*

### Comparing `graphreduce-0.1/graphreduce.egg-info/PKG-INFO` & `graphreduce-0.2/graphreduce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 0.1
+Version: 0.2
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-0.1/setup.py` & `graphreduce-0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = 0.1,
+        version = 0.2,
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "structlog >= 22.3.0",
             "dask >= 2023.1.1",
             "networkx >= 2.8.2",
-            "pyvis >= 0.3.1",
-            "pandas >= 1.4.2",
-            "pyarrow >= 8.0.0",
-            "pyspark >= 3.4.0"
+            "pyvis >= 0.2.1",
+            "pandas >= 1.3.2",
+            "pyarrow >= 7.0.0",
+            "pyspark >= 3.2.0"
             ],
         author="Wes Madrigal",
         author_email="wes@madconsulting.ai",
         license="MIT",
 
         description="Leveraging graph data structures for complex feature engineering pipelines.",
         long_description = pathlib.Path("README.md").read_text(),
```

