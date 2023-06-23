# Comparing `tmp/nowcasting_datamodel-1.4.4.tar.gz` & `tmp/nowcasting_datamodel-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowcasting_datamodel-1.4.4.tar", last modified: Wed Jun 21 14:04:59 2023, max compression
+gzip compressed data, was "nowcasting_datamodel-1.4.5.tar", last modified: Fri Jun 23 10:03:09 2023, max compression
```

## Comparing `nowcasting_datamodel-1.4.4.tar` & `nowcasting_datamodel-1.4.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/diagram_pv.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.194617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/fake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.194617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/migrations/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.194617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/national.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_gsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.194617 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-21 14:04:59.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-21 14:04:59.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:04:59.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 14:04:59.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 14:04:59.000000 nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:04:59.198617 nowcasting_datamodel-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/tests/test_databaseconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/tests/test_fake.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/tests/test_fake_pv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/tests/test_national.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-21 14:04:44.000000 nowcasting_datamodel-1.4.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   151651 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/diagram_pv.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.835757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/fake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.839757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/migrations/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.839757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/national.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.839757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24247 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_gsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.835757 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-23 10:03:09.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-23 10:03:09.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:03:09.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 10:03:09.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 10:03:09.000000 nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:03:09.843757 nowcasting_datamodel-1.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/tests/test_databaseconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/tests/test_fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/tests/test_fake_pv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/tests/test_national.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-23 10:02:54.000000 nowcasting_datamodel-1.4.5/tests/test_utils.py
```

### Comparing `nowcasting_datamodel-1.4.4/PKG-INFO` & `nowcasting_datamodel-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting_datamodel
-Version: 1.4.4
+Version: 1.4.5
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.4/README.md` & `nowcasting_datamodel-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/diagram.png` & `nowcasting_datamodel-1.4.5/diagram.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/diagram_pv.png` & `nowcasting_datamodel-1.4.5/diagram_pv.png`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/connection.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/fake.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/migrations/app.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/migrations/app.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/__init__.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/api.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/api.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/convert.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/convert.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/forecast.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/forecast.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/gsp.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/metric.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/models.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/models.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/pv.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/models/utils.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/models/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/national.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/blend.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/blend.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/utils.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/blend/weights.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/blend/weights.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_gsp.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_gsp.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_metric.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_metric.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_pv.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/read/read_user.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/read/read_user.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/adjust.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/adjust.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/save.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/save.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Save forecasts to the database """
 import logging
+import os
 from typing import List, Optional
 
 from sqlalchemy.orm.session import Session
 
 from nowcasting_datamodel.models import PVSystem, PVSystemSQL
 from nowcasting_datamodel.models.forecast import ForecastSQL
 from nowcasting_datamodel.save.adjust import add_adjust_to_forecasts
@@ -25,20 +26,31 @@
 ):
     """
     Save forecast to database
 
     1. Add sqlalchemy onjects to database
     2. Saves to 'latest' table aswell
 
+    Note that apply_adjuster=True can be overwritten by "USE_ADJUSTER" env var
+
     :param forecasts: list of sql forecasts
     :param session: database session
     :param update_national: Optional (default true), to update the national forecast
     :param update_gsp: Optional (default true), to update all the GSP forecasts
     :param apply_adjuster: Optional (default true), to apply the adjuster
     """
+
+    use_adjuster_env_var = bool(os.getenv("USE_ADJUSTER", "True").lower() in ["true", "1"])
+    if apply_adjuster & (not use_adjuster_env_var):
+        logger.warning(
+            "USE_ADJUSTER is set to False, but apply_adjuster is set to True. "
+            "Therefore the adjuster will not be applied to the forecasts."
+        )
+        apply_adjuster = False
+
     if apply_adjuster:
         logger.debug("Add Adjust to forecasts")
         add_adjust_to_forecasts(session=session, forecasts_sql=forecasts)
 
     # save objects to database
     logger.debug("Saving models")
     session.add_all(forecasts)
```

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/save/update.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/save/update.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel/utils.py` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/PKG-INFO` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nowcasting-datamodel
-Version: 1.4.4
+Version: 1.4.5
 Summary: Data Model for the OCF nowcasting project
 Home-page: https://github.com/openclimatefix/nowcasting_datamodel
 Author: Peter Dudfield
 Author-email: peter@openclimatefix.org
 License: MIT
 Keywords: SQL,Datamodel
 Description-Content-Type: text/markdown
```

### Comparing `nowcasting_datamodel-1.4.4/nowcasting_datamodel.egg-info/SOURCES.txt` & `nowcasting_datamodel-1.4.5/nowcasting_datamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/setup.py` & `nowcasting_datamodel-1.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/tests/test_databaseconnection.py` & `nowcasting_datamodel-1.4.5/tests/test_databaseconnection.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/tests/test_fake.py` & `nowcasting_datamodel-1.4.5/tests/test_fake.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/tests/test_fake_pv.py` & `nowcasting_datamodel-1.4.5/tests/test_fake_pv.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/tests/test_national.py` & `nowcasting_datamodel-1.4.5/tests/test_national.py`

 * *Files identical despite different names*

### Comparing `nowcasting_datamodel-1.4.4/tests/test_utils.py` & `nowcasting_datamodel-1.4.5/tests/test_utils.py`

 * *Files identical despite different names*

