# Comparing `tmp/nowcasting_datamodel-1.4.5.tar.gz` & `tmp/nowcasting_datamodel-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.4.5.tar", last modified: Fri Jun 23 10:03:09 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.4.6.tar", last modified: Fri Jun 23 13:13:24 2023, max compression
```

## Comparing `nowcasting_datamodel-1.4.5.tar` & `nowcasting_datamodel-1.4.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.835757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.839757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.839757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.839757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.835757 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-23 10:03:09.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-23 10:03:09.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:03:09.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 10:03:09.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 10:03:09.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:13:24.217142 nowcasting_datamodel-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-23 13:13:24.217142 nowcasting_datamodel-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:13:24.213142 nowcasting_datamodel-1.4.6/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:13:24.213142 nowcasting_datamodel-1.4.6/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:13:24.213142 nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:13:24.213142 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:13:24.213142 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/read_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/read_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:13:24.217142 nowcasting_datamodel-1.4.6/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:13:24.213142 nowcasting_datamodel-1.4.6/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-23 13:13:24.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-23 13:13:24.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:13:24.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 13:13:24.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 13:13:24.000000 nowcasting_datamodel-1.4.6/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 13:13:24.217142 nowcasting_datamodel-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:13:24.217142 nowcasting_datamodel-1.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-23 13:13:14.000000 nowcasting_datamodel-1.4.6/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.4.5/PKG-INFO` & `nowcasting_datamodel-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.4.5
+Version: 1.4.6
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.5/README.md` & `nowcasting_datamodel-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/diagram.png` & `nowcasting_datamodel-1.4.6/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/diagram_pv.png` & `nowcasting_datamodel-1.4.6/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/api.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/api.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/gsp.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,14 +76,16 @@
 
     __tablename__ = "gsp_yield"
 
     id = Column(Integer, primary_key=True)
     datetime_utc = Column(DateTime, index=True)
     solar_generation_kw = Column(Float)
     regime = Column(String, nullable=True)
+    capacity_mwp = Column(Float, nullable=True)
+    pvlive_updated_utc = Column(DateTime, nullable=True)
 
     # many (gsp_yields) to one (location)
     location = relationship("LocationSQL", back_populates="gsp_yields")
     location_id = Column(Integer, ForeignKey("location.id"), index=True)
 
     Index("ix_gsp_yield_datetime_utc_desc", datetime_utc.desc())
 
@@ -92,18 +94,23 @@
     """GSP Yield data"""
 
     datetime_utc: datetime = Field(..., description="The timestamp of the gsp yield")
     solar_generation_kw: float = Field(..., description="The amount of solar generation")
     regime: str = Field(
         "in-day", description="When the GSP data is pulled, can be 'in-day' or 'day-after'"
     )
+    capacity_mwp: float = Field(None, description="The estimate current capacity")
+    pvlive_updated_utc: datetime = Field(None, description="When PVlive made this value")
 
     _normalize_target_time = validator("datetime_utc", allow_reuse=True)(
         datetime_must_have_timezone
     )
+    _normalize_pvlive_updated_utc = validator("pvlive_updated_utc", allow_reuse=True)(
+        datetime_must_have_timezone
+    )
 
     gsp: Optional[Location] = Field(
         None,
         description="The GSP associated with this model",
     )
 
     @validator("solar_generation_kw")
@@ -125,14 +132,16 @@
 
     def to_orm(self) -> GSPYieldSQL:
         """Change model to GSPYieldSQL"""
         return GSPYieldSQL(
             datetime_utc=self.datetime_utc,
             solar_generation_kw=self.solar_generation_kw,
             regime=self.regime,
+            capacity_mwp=self.capacity_mwp,
+            pvlive_updated_utc=self.pvlive_updated_utc,
         )
 
 
 class LocationWithGSPYields(Location):
     """Location object with GSPYields"""
 
     gsp_yields: Optional[List[GSPYield]] = Field([], description="List of gsp yields")
```

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/blend.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/blend/blend.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/utils.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/blend/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/weights.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/blend/weights.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_user.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/read/read_user.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/save/save.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/save/update.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from datetime import datetime, timezone
 
 logger = logging.getLogger(__name__)
 
 
 def datetime_must_have_timezone(cls, v: datetime):
     """Enforce that this variable must have a timezone"""
+    if v is None:
+        return v
     if v.tzinfo is None:
         logger.debug(f"{v} must have a timezone, for cls {cls}." f"So we are going to add UTC ")
         v = v.replace(tzinfo=timezone.utc)
     return v
 
 
 def convert_to_camelcase(snake_str: str) -> str:
```

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.4.5
+Version: 1.4.6
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.4.6/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/setup.py` & `nowcasting_datamodel-1.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.4.6/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/tests/test_fake.py` & `nowcasting_datamodel-1.4.6/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/tests/test_fake_pv.py` & `nowcasting_datamodel-1.4.6/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/tests/test_national.py` & `nowcasting_datamodel-1.4.6/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.5/tests/test_utils.py` & `nowcasting_datamodel-1.4.6/tests/test_utils.py`

 * *Files identical despite different names*

