# Comparing `tmp/cjm-pandas-utils-0.0.2.tar.gz` & `tmp/cjm-pandas-utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-pandas-utils-0.0.2.tar", last modified: Tue Feb 28 23:50:01 2023, max compression
+gzip compressed data, was "cjm-pandas-utils-0.0.3.tar", last modified: Thu Jun 22 23:50:42 2023, max compression
```

## Comparing `cjm-pandas-utils-0.0.2.tar` & `cjm-pandas-utils-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-02-28 23:50:01.849026 cjm-pandas-utils-0.0.2/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-02-05 22:11:52.000000 cjm-pandas-utils-0.0.2/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-01-20 02:50:04.000000 cjm-pandas-utils-0.0.2/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1507 2023-02-28 23:50:01.848816 cjm-pandas-utils-0.0.2/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      704 2023-02-28 23:48:43.000000 cjm-pandas-utils-0.0.2/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-02-28 23:50:01.846179 cjm-pandas-utils-0.0.2/cjm_pandas_utils/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-02-28 23:49:27.000000 cjm-pandas-utils-0.0.2/cjm_pandas_utils/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      660 2023-02-28 23:49:27.000000 cjm-pandas-utils-0.0.2/cjm_pandas_utils/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1677 2023-02-28 23:49:27.000000 cjm-pandas-utils-0.0.2/cjm_pandas_utils/core.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-02-28 23:50:01.848455 cjm-pandas-utils-0.0.2/cjm_pandas_utils.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1507 2023-02-28 23:50:01.000000 cjm-pandas-utils-0.0.2/cjm_pandas_utils.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      414 2023-02-28 23:50:01.000000 cjm-pandas-utils-0.0.2/cjm_pandas_utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-02-28 23:50:01.000000 cjm-pandas-utils-0.0.2/cjm_pandas_utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       54 2023-02-28 23:50:01.000000 cjm-pandas-utils-0.0.2/cjm_pandas_utils.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-02-05 22:33:09.000000 cjm-pandas-utils-0.0.2/cjm_pandas_utils.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       14 2023-02-28 23:50:01.000000 cjm-pandas-utils-0.0.2/cjm_pandas_utils.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       17 2023-02-28 23:50:01.000000 cjm-pandas-utils-0.0.2/cjm_pandas_utils.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      948 2023-02-28 23:26:42.000000 cjm-pandas-utils-0.0.2/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-02-28 23:50:01.849087 cjm-pandas-utils-0.0.2/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2560 2023-01-20 02:50:04.000000 cjm-pandas-utils-0.0.2/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-06-22 23:50:42.198017 cjm-pandas-utils-0.0.3/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-02-05 22:11:52.000000 cjm-pandas-utils-0.0.3/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-01-20 02:50:04.000000 cjm-pandas-utils-0.0.3/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1492 2023-06-22 23:50:42.197845 cjm-pandas-utils-0.0.3/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      689 2023-06-22 23:48:02.000000 cjm-pandas-utils-0.0.3/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-06-22 23:50:42.194841 cjm-pandas-utils-0.0.3/cjm_pandas_utils/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-06-22 23:48:01.000000 cjm-pandas-utils-0.0.3/cjm_pandas_utils/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1119 2023-06-22 23:48:01.000000 cjm-pandas-utils-0.0.3/cjm_pandas_utils/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2496 2023-06-22 23:48:01.000000 cjm-pandas-utils-0.0.3/cjm_pandas_utils/core.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-06-22 23:50:42.197486 cjm-pandas-utils-0.0.3/cjm_pandas_utils.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1492 2023-06-22 23:50:42.000000 cjm-pandas-utils-0.0.3/cjm_pandas_utils.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      414 2023-06-22 23:50:42.000000 cjm-pandas-utils-0.0.3/cjm_pandas_utils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-22 23:50:42.000000 cjm-pandas-utils-0.0.3/cjm_pandas_utils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       54 2023-06-22 23:50:42.000000 cjm-pandas-utils-0.0.3/cjm_pandas_utils.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-02-05 22:33:09.000000 cjm-pandas-utils-0.0.3/cjm_pandas_utils.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       14 2023-06-22 23:50:42.000000 cjm-pandas-utils-0.0.3/cjm_pandas_utils.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       17 2023-06-22 23:50:42.000000 cjm-pandas-utils-0.0.3/cjm_pandas_utils.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      948 2023-06-22 23:47:53.000000 cjm-pandas-utils-0.0.3/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-06-22 23:50:42.198071 cjm-pandas-utils-0.0.3/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2560 2023-01-20 02:50:04.000000 cjm-pandas-utils-0.0.3/setup.py
```

### Comparing `cjm-pandas-utils-0.0.2/LICENSE` & `cjm-pandas-utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-pandas-utils-0.0.2/PKG-INFO` & `cjm-pandas-utils-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-pandas-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Some utility functions for working with Pandas.
 Home-page: https://github.com/cj-mills/cjm-pandas-utils
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -16,16 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-cjm-pandas-utils
-================
+# cjm-pandas-utils
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This file will become your README and also the index of your
 documentation.
 
 ## Install
```

### Comparing `cjm-pandas-utils-0.0.2/README.md` & `cjm-pandas-utils-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-cjm-pandas-utils
-================
+# cjm-pandas-utils
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This file will become your README and also the index of your
 documentation.
 
 ## Install
```

### Comparing `cjm-pandas-utils-0.0.2/cjm_pandas_utils/_modidx.py` & `cjm-pandas-utils-0.0.3/cjm_pandas_utils/_modidx.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/cjm-pandas-utils',
                 'doc_host': 'https://cj-mills.github.io',
                 'git_url': 'https://github.com/cj-mills/cjm-pandas-utils',
                 'lib_path': 'cjm_pandas_utils'},
-  'syms': { 'cjm_pandas_utils.core': { 'cjm_pandas_utils.core.display_df': ('core.html#display_df', 'cjm_pandas_utils/core.py'),
+  'syms': { 'cjm_pandas_utils.core': { 'cjm_pandas_utils.core.convert_to_numeric': ( 'core.html#convert_to_numeric',
+                                                                                     'cjm_pandas_utils/core.py'),
+                                       'cjm_pandas_utils.core.convert_to_string': ( 'core.html#convert_to_string',
+                                                                                    'cjm_pandas_utils/core.py'),
+                                       'cjm_pandas_utils.core.display_df': ('core.html#display_df', 'cjm_pandas_utils/core.py'),
                                        'cjm_pandas_utils.core.markdown_to_pandas': ( 'core.html#markdown_to_pandas',
                                                                                      'cjm_pandas_utils/core.py')}}}
```

### Comparing `cjm-pandas-utils-0.0.2/cjm_pandas_utils.egg-info/PKG-INFO` & `cjm-pandas-utils-0.0.3/cjm_pandas_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-pandas-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Some utility functions for working with Pandas.
 Home-page: https://github.com/cj-mills/cjm-pandas-utils
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -16,16 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-cjm-pandas-utils
-================
+# cjm-pandas-utils
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This file will become your README and also the index of your
 documentation.
 
 ## Install
```

### Comparing `cjm-pandas-utils-0.0.2/settings.ini` & `cjm-pandas-utils-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-pandas-utils
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_pandas_utils
 nbs_path = nbs
```

### Comparing `cjm-pandas-utils-0.0.2/setup.py` & `cjm-pandas-utils-0.0.3/setup.py`

 * *Files identical despite different names*

