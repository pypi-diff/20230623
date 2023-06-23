# Comparing `tmp/recurtx-0.0.1.tar.gz` & `tmp/recurtx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurtx-0.0.1.tar", last modified: Mon Jun 19 15:46:13 2023, max compression
+gzip compressed data, was "dist/recurtx-0.0.2.tar", last modified: Fri Jun 23 14:45:36 2023, max compression
```

## Comparing `recurtx-0.0.1.tar` & `recurtx-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 15:46:13.460000 recurtx-0.0.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-18 12:28:09.000000 recurtx-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-19 15:46:13.460000 recurtx-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1918 2023-06-19 15:38:24.000000 recurtx-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-18 14:06:24.000000 recurtx-0.0.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 15:46:13.460000 recurtx-0.0.1/recurtx/
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-18 14:06:36.000000 recurtx-0.0.1/recurtx/__init__.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-19 15:10:52.000000 recurtx-0.0.1/recurtx/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1231 2023-06-19 15:10:41.000000 recurtx-0.0.1/recurtx/search.py
--rw-r--r--   0 root         (0) root         (0)     1343 2023-06-19 15:10:52.000000 recurtx-0.0.1/recurtx/under.py
--rw-r--r--   0 root         (0) root         (0)      590 2023-06-19 15:10:52.000000 recurtx-0.0.1/recurtx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 15:46:13.460000 recurtx-0.0.1/recurtx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-19 15:46:13.000000 recurtx-0.0.1/recurtx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      361 2023-06-19 15:46:13.000000 recurtx-0.0.1/recurtx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 15:46:13.000000 recurtx-0.0.1/recurtx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-19 15:46:13.000000 recurtx-0.0.1/recurtx.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 15:46:13.000000 recurtx-0.0.1/recurtx.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-19 15:46:13.000000 recurtx-0.0.1/recurtx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-19 15:46:13.000000 recurtx-0.0.1/recurtx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-19 15:46:13.460000 recurtx-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1303 2023-06-19 11:46:54.000000 recurtx-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:45:36.000000 recurtx-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-20 00:32:16.000000 recurtx-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-23 14:45:36.000000 recurtx-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6039 2023-06-23 14:25:23.000000 recurtx-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-20 00:32:16.000000 recurtx-0.0.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:45:36.000000 recurtx-0.0.2/recurtx/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-21 11:55:26.000000 recurtx-0.0.2/recurtx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-22 02:20:02.000000 recurtx-0.0.2/recurtx/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-23 14:13:28.000000 recurtx-0.0.2/recurtx/find.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-06-23 14:15:10.000000 recurtx-0.0.2/recurtx/pandas.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2023-06-23 14:15:26.000000 recurtx-0.0.2/recurtx/polars.py
+-rw-r--r--   0 root         (0) root         (0)     3343 2023-06-23 14:09:15.000000 recurtx-0.0.2/recurtx/recur.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2023-06-23 14:12:56.000000 recurtx-0.0.2/recurtx/search.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-06-23 05:44:59.000000 recurtx-0.0.2/recurtx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:45:36.000000 recurtx-0.0.2/recurtx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      733 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      413 2023-06-23 14:45:36.000000 recurtx-0.0.2/recurtx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-23 14:45:35.000000 recurtx-0.0.2/recurtx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-23 14:45:36.000000 recurtx-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1303 2023-06-20 00:32:16.000000 recurtx-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `recurtx-0.0.1/LICENSE` & `recurtx-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `recurtx-0.0.1/PKG-INFO` & `recurtx-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.1
+Version: 0.0.2
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.1/recurtx/search.py` & `recurtx-0.0.2/recurtx/search.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import sys
 from pathlib import Path
 
 
 def search(
     target: str,
     path: str,
     sub: str = None,
     wildcard: str = "*",
     verbose: int = 1,
 ):
+    """Search a keyword, which may include wildcards, in the text file content, and optionally substitute (replace)."""
+
     target_ls = eval("'''" + target + "'''").split(wildcard)
 
     p = Path(path)
     try:
         text = p.read_text()
     except Exception:
         if verbose >= 3:
@@ -34,15 +37,15 @@
                 break
         if start_index and (index >= 0):
             end_index = index
             if sub is not None:
                 replacing = text[start_index:end_index]
                 replacing_ls.append(replacing)
             if verbose >= 1:
-                print(
+                sys.stdout.write(
                     f"{p} [{start_index}:{end_index}]\n{text[start_index:end_index]}\n"
                 )
         else:
             break
     for replacing in replacing_ls:
         text = text.replace(replacing, sub, 1)
     if sub is not None:
```

### Comparing `recurtx-0.0.1/recurtx.egg-info/PKG-INFO` & `recurtx-0.0.2/recurtx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurtx
-Version: 0.0.1
+Version: 0.0.2
 Summary: CLI to transform text files recursively
 Home-page: https://github.com/Minyus/recurtx
 Author: Yusuke Minami
 Author-email: me@minyus.github.com
 License: Apache Software License (Apache 2.0)
 Keywords: CLI,recursive,text,find,xargs,sed
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `recurtx-0.0.1/setup.py` & `recurtx-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 long_description = """
 Please see:
 https://github.com/Minyus/recurtx
 """
 
 setup(
     name="recurtx",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(exclude=["tests"]),
     entry_points={"console_scripts": [entry_point]},
     install_requires=requires,
     description="CLI to transform text files recursively",
     license="Apache Software License (Apache 2.0)",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

