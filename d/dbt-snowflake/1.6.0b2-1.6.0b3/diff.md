# Comparing `tmp/dbt-snowflake-1.6.0b2.tar.gz` & `tmp/dbt-snowflake-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-snowflake-1.6.0b2.tar", last modified: Thu May 25 21:25:52 2023, max compression
+gzip compressed data, was "dbt-snowflake-1.6.0b3.tar", last modified: Thu Jun  8 23:32:37 2023, max compression
```

## Comparing `dbt-snowflake-1.6.0b2.tar` & `dbt-snowflake-1.6.0b3.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.335729 dbt-snowflake-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-25 21:25:52.335729 dbt-snowflake-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.327728 dbt-snowflake-1.6.0b2/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.327728 dbt-snowflake-1.6.0b2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.331728 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.327728 dbt-snowflake-1.6.0b2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.331728 dbt-snowflake-1.6.0b2/dbt/include/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.331728 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.331728 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.335729 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/dbt/include/snowflake/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 21:25:52.335729 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 21:25:52.000000 dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 21:25:52.335729 dbt-snowflake-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-25 21:25:38.000000 dbt-snowflake-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.756438 dbt-snowflake-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-08 23:32:37.756438 dbt-snowflake-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.744438 dbt-snowflake-1.6.0b3/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.740438 dbt-snowflake-1.6.0b3/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.748438 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20966 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9779 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.748438 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation_configs/dynamic_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/relation_configs/target_lag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.744438 dbt-snowflake-1.6.0b3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.748438 dbt-snowflake-1.6.0b3/dbt/include/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.748438 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.752438 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.752438 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/dynamic_table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/dynamic_table/ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/dynamic_table/materialization.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.752438 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/dbt/include/snowflake/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:32:37.756438 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 23:32:37.000000 dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:32:37.756438 dbt-snowflake-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-08 23:32:22.000000 dbt-snowflake-1.6.0b3/setup.py
```

### Comparing `dbt-snowflake-1.6.0b2/LICENSE.md` & `dbt-snowflake-1.6.0b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b2/PKG-INFO` & `dbt-snowflake-1.6.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b2 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b3 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
+Programming Language :: Python :: 3.11 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
```

### Comparing `dbt-snowflake-1.6.0b2/README.md` & `dbt-snowflake-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/__init__.py` & `dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/column.py` & `dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/column.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/connections.py` & `dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from dbt.events.functions import warn_or_error
 from dbt.events.types import AdapterEventWarning
 from dbt.ui import line_wrap_message, warning_tag
 
 
 logger = AdapterLogger("Snowflake")
 _TOKEN_REQUEST_URL = "https://{}.snowflakecomputing.com/oauth/token-request"
-ROW_VALUE_REGEX = re.compile(r"Row Values: \[.*\]")
+ROW_VALUE_REGEX = re.compile(r"Row Values: \[(.|\n)*\]")
 
 
 @dataclass
 class SnowflakeAdapterResponse(AdapterResponse):
     query_id: str = ""
 
 
@@ -104,19 +104,36 @@
         return self.account
 
     def _connection_keys(self):
         return (
             "account",
             "user",
             "database",
-            "schema",
             "warehouse",
             "role",
-            "client_session_keep_alive",
+            "schema",
+            "authenticator",
+            "private_key",
+            "private_key_path",
+            "private_key_passphrase",
+            "token",
+            "oauth_client_id",
             "query_tag",
+            "client_session_keep_alive",
+            "host",
+            "port",
+            "proxy_host",
+            "proxy_port",
+            "protocol",
+            "connect_retries",
+            "connect_timeout",
+            "retry_on_database_errors",
+            "retry_all",
+            "insecure_mode",
+            "reuse_connections",
         )
 
     def auth_args(self):
         # Pull all of the optional authentication args for the connector,
         # let connector handle the actual arg validation
         result = {}
         if self.password:
```

### Comparing `dbt-snowflake-1.6.0b2/dbt/adapters/snowflake/impl.py` & `dbt-snowflake-1.6.0b3/dbt/adapters/snowflake/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,7 +250,11 @@
                 auto_begin=False,
                 fetch=False,
             )
         return response
 
     def valid_incremental_strategies(self):
         return ["append", "merge", "delete+insert"]
+
+    def debug_query(self):
+        """Override for DebugTask method"""
+        self.execute("select 1 as id")
```

### Comparing `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/adapters.sql` & `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/adapters.sql`

 * *Files 0% similar despite different names*

```diff
@@ -368,7 +368,18 @@
   {% set truncate_dml %}
     truncate table {{ relation }}
   {% endset %}
   {% call statement('truncate_relation') -%}
     {{ snowflake_dml_explicit_transaction(truncate_dml) }}
   {%- endcall %}
 {% endmacro %}
+
+
+{% macro snowflake__drop_relation(relation) -%}
+    {%- if relation.is_dynamic_table -%}
+        {% call statement('drop_relation', auto_begin=False) -%}
+            drop dynamic table if exists {{ relation }}
+        {%- endcall %}
+    {%- else -%}
+        {{- default__drop_relation(relation) -}}
+    {%- endif -%}
+{% endmacro %}
```

### Comparing `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/catalog.sql` & `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/incremental.sql` & `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/merge.sql` & `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/seed.sql` & `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/materializations/table.sql` & `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b2/dbt/include/snowflake/macros/utils/timestamps.sql` & `dbt-snowflake-1.6.0b3/dbt/include/snowflake/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b2/dbt/include/snowflake/profile_template.yml` & `dbt-snowflake-1.6.0b3/dbt/include/snowflake/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/PKG-INFO` & `dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b2 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.6.0b3 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
+Programming Language :: Python :: 3.11 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE.md
                                   [dbt logo]
                  [Unit_Tests_Badge] [Integration_Tests_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
```

### Comparing `dbt-snowflake-1.6.0b2/dbt_snowflake.egg-info/SOURCES.txt` & `dbt-snowflake-1.6.0b3/dbt_snowflake.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,32 @@
 dbt/__init__.py
 dbt/adapters/snowflake/__init__.py
 dbt/adapters/snowflake/__version__.py
 dbt/adapters/snowflake/column.py
 dbt/adapters/snowflake/connections.py
 dbt/adapters/snowflake/impl.py
 dbt/adapters/snowflake/relation.py
+dbt/adapters/snowflake/relation_configs/__init__.py
+dbt/adapters/snowflake/relation_configs/dynamic_table.py
+dbt/adapters/snowflake/relation_configs/target_lag.py
 dbt/include/snowflake/__init__.py
 dbt/include/snowflake/dbt_project.yml
 dbt/include/snowflake/profile_template.yml
 dbt/include/snowflake/macros/adapters.sql
 dbt/include/snowflake/macros/apply_grants.sql
 dbt/include/snowflake/macros/catalog.sql
 dbt/include/snowflake/macros/materializations/incremental.sql
 dbt/include/snowflake/macros/materializations/merge.sql
 dbt/include/snowflake/macros/materializations/seed.sql
 dbt/include/snowflake/macros/materializations/snapshot.sql
 dbt/include/snowflake/macros/materializations/table.sql
 dbt/include/snowflake/macros/materializations/test.sql
 dbt/include/snowflake/macros/materializations/view.sql
+dbt/include/snowflake/macros/materializations/dynamic_table/ddl.sql
+dbt/include/snowflake/macros/materializations/dynamic_table/materialization.sql
 dbt/include/snowflake/macros/utils/array_construct.sql
 dbt/include/snowflake/macros/utils/bool_or.sql
 dbt/include/snowflake/macros/utils/escape_single_quotes.sql
 dbt/include/snowflake/macros/utils/right.sql
 dbt/include/snowflake/macros/utils/safe_cast.sql
 dbt/include/snowflake/macros/utils/timestamps.sql
 dbt_snowflake.egg-info/PKG-INFO
```

### Comparing `dbt-snowflake-1.6.0b2/setup.py` & `dbt-snowflake-1.6.0b3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 import os
 import sys
 import re
 
-# require python 3.7 or newer
-if sys.version_info < (3, 7):
+# require python 3.8 or newer
+if sys.version_info < (3, 8):
     print("Error: dbt does not support this version of Python.")
-    print("Please upgrade to Python 3.7 or higher.")
+    print("Please upgrade to Python 3.8 or higher.")
     sys.exit(1)
 
 
 # require version of setuptools that supports find_namespace_packages
 from setuptools import setup
 
 try:
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-snowflake"
-package_version = "1.6.0b2"
+package_version = "1.6.0b3"
 dbt_core_version = _get_dbt_core_version()
 description = """The Snowflake adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
@@ -73,15 +73,15 @@
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

