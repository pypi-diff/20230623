# Comparing `tmp/sabledocs-0.4.184.dev0.tar.gz` & `tmp/sabledocs-0.4.186.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.4.184.dev0.tar", last modified: Fri Jun 23 19:09:43 2023, max compression
+gzip compressed data, was "sabledocs-0.4.186.tar", last modified: Fri Jun 23 19:27:12 2023, max compression
```

## Comparing `sabledocs-0.4.184.dev0.tar` & `sabledocs-0.4.186.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4261 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.599387 sabledocs-0.4.184.dev0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/src/sabledocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/lunr_search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13934 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.599387 sabledocs-0.4.184.dev0/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5412 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/search.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   260942 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2023-06-23 19:09:31.000000 sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:09:43.603387 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-23 19:09:43.000000 sabledocs-0.4.184.dev0/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:27:12.581940 sabledocs-0.4.186/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-23 19:26:51.000000 sabledocs-0.4.186/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-06-23 19:26:51.000000 sabledocs-0.4.186/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2023-06-23 19:27:12.581940 sabledocs-0.4.186/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4261 2023-06-23 19:26:51.000000 sabledocs-0.4.186/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-23 19:26:51.000000 sabledocs-0.4.186/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-06-23 19:27:12.581940 sabledocs-0.4.186/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:27:12.577940 sabledocs-0.4.186/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:27:12.577940 sabledocs-0.4.186/src/sabledocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/lunr_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13934 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:27:12.577940 sabledocs-0.4.186/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:27:12.581940 sabledocs-0.4.186/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5412 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/templates/_default/search.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:27:12.581940 sabledocs-0.4.186/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   260942 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2023-06-23 19:26:51.000000 sabledocs-0.4.186/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 19:27:12.577940 sabledocs-0.4.186/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2023-06-23 19:27:12.000000 sabledocs-0.4.186/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-06-23 19:27:12.000000 sabledocs-0.4.186/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-23 19:27:12.000000 sabledocs-0.4.186/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-23 19:27:12.000000 sabledocs-0.4.186/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-06-23 19:27:12.000000 sabledocs-0.4.186/src/sabledocs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-23 19:27:12.000000 sabledocs-0.4.186/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.4.184.dev0/LICENSE` & `sabledocs-0.4.186/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/PKG-INFO` & `sabledocs-0.4.186/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.4.184.dev0
+Version: 0.4.186
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.4.184.dev0/README.md` & `sabledocs-0.4.186/README.md`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/pyproject.toml` & `sabledocs-0.4.186/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/__main__.py` & `sabledocs-0.4.186/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/lunr_search.py` & `sabledocs-0.4.186/src/sabledocs/lunr_search.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.4.186/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/proto_model.py` & `sabledocs-0.4.186/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/sable_config.py` & `sabledocs-0.4.186/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/base.html` & `sabledocs-0.4.186/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.4.186/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/index.html` & `sabledocs-0.4.186/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/message.html` & `sabledocs-0.4.186/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/package.html` & `sabledocs-0.4.186/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/search.html` & `sabledocs-0.4.186/src/sabledocs/templates/_default/search.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/service.html` & `sabledocs-0.4.186/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.4.186/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.4.186/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.4.186/src/sabledocs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.4.184.dev0
+Version: 0.4.186
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.4.184.dev0/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.4.186/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

