# Comparing `tmp/kedro_templar-0.0.5.tar.gz` & `tmp/kedro_templar-0.0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_templar-0.0.5.tar", last modified: Wed Jul  6 13:48:04 2022, max compression
+gzip compressed data, was "kedro_templar-0.0.6.dev0.tar", last modified: Fri Jun 23 11:47:30 2023, max compression
```

## Comparing `kedro_templar-0.0.5.tar` & `kedro_templar-0.0.6.dev0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:48:04.406316 kedro_templar-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3072 2022-07-06 13:48:04.406316 kedro_templar-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-07-06 13:48:04.406316 kedro_templar-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:48:04.402316 kedro_templar-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:48:04.406316 kedro_templar-0.0.5/src/kedro_templar/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/src/kedro_templar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:48:04.406316 kedro_templar-0.0.5/src/kedro_templar/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/src/kedro_templar/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/src/kedro_templar/core/templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/src/kedro_templar/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/src/kedro_templar/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2155 2022-07-06 13:47:54.000000 kedro_templar-0.0.5/src/kedro_templar/process_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 13:48:04.406316 kedro_templar-0.0.5/src/kedro_templar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3072 2022-07-06 13:48:04.000000 kedro_templar-0.0.5/src/kedro_templar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-07-06 13:48:04.000000 kedro_templar-0.0.5/src/kedro_templar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-06 13:48:04.000000 kedro_templar-0.0.5/src/kedro_templar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-07-06 13:48:04.000000 kedro_templar-0.0.5/src/kedro_templar.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-07-06 13:48:04.000000 kedro_templar-0.0.5/src/kedro_templar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-06 13:48:04.000000 kedro_templar-0.0.5/src/kedro_templar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.312755 kedro_templar-0.0.6.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-23 11:47:30.312755 kedro_templar-0.0.6.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-23 11:47:30.312755 kedro_templar-0.0.6.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.304755 kedro_templar-0.0.6.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.308755 kedro_templar-0.0.6.dev0/src/kedro_templar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/src/kedro_templar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.312755 kedro_templar-0.0.6.dev0/src/kedro_templar/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/src/kedro_templar/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/src/kedro_templar/core/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/src/kedro_templar/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/src/kedro_templar/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-23 11:47:19.000000 kedro_templar-0.0.6.dev0/src/kedro_templar/process_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:30.312755 kedro_templar-0.0.6.dev0/src/kedro_templar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-23 11:47:30.000000 kedro_templar-0.0.6.dev0/src/kedro_templar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-23 11:47:30.000000 kedro_templar-0.0.6.dev0/src/kedro_templar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:47:30.000000 kedro_templar-0.0.6.dev0/src/kedro_templar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 11:47:30.000000 kedro_templar-0.0.6.dev0/src/kedro_templar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 11:47:30.000000 kedro_templar-0.0.6.dev0/src/kedro_templar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 11:47:30.000000 kedro_templar-0.0.6.dev0/src/kedro_templar.egg-info/top_level.txt
```

### Comparing `kedro_templar-0.0.5/LICENSE` & `kedro_templar-0.0.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_templar-0.0.5/PKG-INFO` & `kedro_templar-0.0.6.dev0/src/kedro_templar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kedro_templar
-Version: 0.0.5
+Name: kedro-templar
+Version: 0.0.6.dev0
 Home-page: https://github.com/webinterpret-ds/kedro-templar
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/kedro-templar/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `kedro_templar-0.0.5/README.md` & `kedro_templar-0.0.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `kedro_templar-0.0.5/setup.cfg` & `kedro_templar-0.0.6.dev0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kedro-templar
-version = 0.0.5
+version = 0.0.6-dev
 author = webinterpret-datascience
 author_email = data-science@webinterpret.com
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/webinterpret-ds/kedro-templar
 project_urls =
```

### Comparing `kedro_templar-0.0.5/setup.py` & `kedro_templar-0.0.6.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `kedro_templar-0.0.5/src/kedro_templar/core/utils.py` & `kedro_templar-0.0.6.dev0/src/kedro_templar/core/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_templar-0.0.5/src/kedro_templar/process_templates.py` & `kedro_templar-0.0.6.dev0/src/kedro_templar/process_templates.py`

 * *Files identical despite different names*

### Comparing `kedro_templar-0.0.5/src/kedro_templar.egg-info/PKG-INFO` & `kedro_templar-0.0.6.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kedro-templar
-Version: 0.0.5
+Name: kedro_templar
+Version: 0.0.6.dev0
 Home-page: https://github.com/webinterpret-ds/kedro-templar
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/kedro-templar/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `kedro_templar-0.0.5/src/kedro_templar.egg-info/SOURCES.txt` & `kedro_templar-0.0.6.dev0/src/kedro_templar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

