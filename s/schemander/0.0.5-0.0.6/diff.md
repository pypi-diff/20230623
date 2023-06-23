# Comparing `tmp/schemander-0.0.5.tar.gz` & `tmp/schemander-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemander-0.0.5.tar", last modified: Fri Jun 23 19:08:18 2023, max compression
+gzip compressed data, was "schemander-0.0.6.tar", last modified: Fri Jun 23 19:14:40 2023, max compression
```

## Comparing `schemander-0.0.5.tar` & `schemander-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:08:18.073492 schemander-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-23 19:07:40.000000 schemander-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-23 19:08:18.073492 schemander-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 19:07:40.000000 schemander-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-23 19:07:40.000000 schemander-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:08:18.073492 schemander-0.0.5/schemander.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-23 19:08:18.000000 schemander-0.0.5/schemander.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-23 19:08:18.000000 schemander-0.0.5/schemander.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:08:18.000000 schemander-0.0.5/schemander.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 19:08:18.000000 schemander-0.0.5/schemander.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 19:08:18.000000 schemander-0.0.5/schemander.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-23 19:07:40.000000 schemander-0.0.5/schemander.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:08:18.073492 schemander-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:14:40.458639 schemander-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-23 19:14:09.000000 schemander-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-23 19:14:40.458639 schemander-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-23 19:14:09.000000 schemander-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-23 19:14:09.000000 schemander-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:14:40.458639 schemander-0.0.6/schemander.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-23 19:14:40.000000 schemander-0.0.6/schemander.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-23 19:14:40.000000 schemander-0.0.6/schemander.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:14:40.000000 schemander-0.0.6/schemander.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 19:14:40.000000 schemander-0.0.6/schemander.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 19:14:40.000000 schemander-0.0.6/schemander.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-06-23 19:14:09.000000 schemander-0.0.6/schemander.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:14:40.458639 schemander-0.0.6/setup.cfg
```

### Comparing `schemander-0.0.5/LICENSE` & `schemander-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `schemander-0.0.5/PKG-INFO` & `schemander-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemander
-Version: 0.0.5
+Version: 0.0.6
 Summary: A single file schema validator for dictionaries.
 Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
 License: GPL-2.0
 Project-URL: Homepage, https://schemander.ekiim.xyz
 Project-URL: Source, https://github.com/ekiim/schemander
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `schemander-0.0.5/README.md` & `schemander-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `schemander-0.0.5/pyproject.toml` & `schemander-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [project]
-version = "0.0.5"
+version = "0.0.6"
 name = "schemander"
 authors = [
     { name="Miguel Alejandro Salgado Zapien", email="ekiim@ekiim.xyz"},
 ]
 description = "A single file schema validator for dictionaries."
 readme="README.md"
 requires-python = ">= 3.11"
```

### Comparing `schemander-0.0.5/schemander.egg-info/PKG-INFO` & `schemander-0.0.6/schemander.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemander
-Version: 0.0.5
+Version: 0.0.6
 Summary: A single file schema validator for dictionaries.
 Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
 License: GPL-2.0
 Project-URL: Homepage, https://schemander.ekiim.xyz
 Project-URL: Source, https://github.com/ekiim/schemander
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `schemander-0.0.5/schemander.py` & `schemander-0.0.6/schemander.py`

 * *Files identical despite different names*

