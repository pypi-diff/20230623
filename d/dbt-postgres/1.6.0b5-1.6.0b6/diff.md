# Comparing `tmp/dbt-postgres-1.6.0b5.tar.gz` & `tmp/dbt-postgres-1.6.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-postgres-1.6.0b5.tar", last modified: Thu Jun 22 20:11:21 2023, max compression
+gzip compressed data, was "dbt-postgres-1.6.0b6.tar", last modified: Fri Jun 23 21:14:42 2023, max compression
```

## Comparing `dbt-postgres-1.6.0b5.tar` & `dbt-postgres-1.6.0b6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:21.699327 dbt-postgres-1.6.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-22 20:11:21.699327 dbt-postgres-1.6.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:21.691327 dbt-postgres-1.6.0b5/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:21.691327 dbt-postgres-1.6.0b5/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:21.691327 dbt-postgres-1.6.0b5/dbt/adapters/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/adapters/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/adapters/postgres/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/adapters/postgres/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/adapters/postgres/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/adapters/postgres/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/adapters/postgres/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:21.695327 dbt-postgres-1.6.0b5/dbt/adapters/postgres/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/adapters/postgres/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/adapters/postgres/relation_configs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/adapters/postgres/relation_configs/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/adapters/postgres/relation_configs/materialized_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:21.691327 dbt-postgres-1.6.0b5/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:21.695327 dbt-postgres-1.6.0b5/dbt/include/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:21.695327 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:21.695327 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/materializations/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/materializations/materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:21.695327 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/dbt/include/postgres/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:11:21.699327 dbt-postgres-1.6.0b5/dbt_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-22 20:11:21.000000 dbt-postgres-1.6.0b5/dbt_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-22 20:11:21.000000 dbt-postgres-1.6.0b5/dbt_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:11:21.000000 dbt-postgres-1.6.0b5/dbt_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:11:21.000000 dbt-postgres-1.6.0b5/dbt_postgres.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 20:11:21.000000 dbt-postgres-1.6.0b5/dbt_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 20:11:21.000000 dbt-postgres-1.6.0b5/dbt_postgres.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:11:21.699327 dbt-postgres-1.6.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-22 20:11:03.000000 dbt-postgres-1.6.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:42.075262 dbt-postgres-1.6.0b6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-23 21:14:42.075262 dbt-postgres-1.6.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:42.071262 dbt-postgres-1.6.0b6/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:42.071262 dbt-postgres-1.6.0b6/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:42.071262 dbt-postgres-1.6.0b6/dbt/adapters/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/adapters/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/adapters/postgres/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/adapters/postgres/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/adapters/postgres/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/adapters/postgres/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/adapters/postgres/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:42.071262 dbt-postgres-1.6.0b6/dbt/adapters/postgres/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/adapters/postgres/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/adapters/postgres/relation_configs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/adapters/postgres/relation_configs/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/adapters/postgres/relation_configs/materialized_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:42.067263 dbt-postgres-1.6.0b6/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:42.071262 dbt-postgres-1.6.0b6/dbt/include/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:42.071262 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:42.071262 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/materializations/materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:42.071262 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/dbt/include/postgres/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:14:42.075262 dbt-postgres-1.6.0b6/dbt_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-23 21:14:42.000000 dbt-postgres-1.6.0b6/dbt_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-23 21:14:42.000000 dbt-postgres-1.6.0b6/dbt_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:14:42.000000 dbt-postgres-1.6.0b6/dbt_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:14:42.000000 dbt-postgres-1.6.0b6/dbt_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 21:14:42.000000 dbt-postgres-1.6.0b6/dbt_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 21:14:42.000000 dbt-postgres-1.6.0b6/dbt_postgres.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:14:42.075262 dbt-postgres-1.6.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-23 21:14:29.000000 dbt-postgres-1.6.0b6/setup.py
```

### Comparing `dbt-postgres-1.6.0b5/PKG-INFO` & `dbt-postgres-1.6.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-postgres
-Version: 1.6.0b5
+Version: 1.6.0b6
 Summary: The postgres adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b5 Summary: The postgres
+Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b6 Summary: The postgres
 adapter plugin for dbt (data build tool) Home-page: https://github.com/dbt-
 labs/dbt-core Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `dbt-postgres-1.6.0b5/README.md` & `dbt-postgres-1.6.0b6/README.md`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/adapters/postgres/__init__.py` & `dbt-postgres-1.6.0b6/dbt/adapters/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/adapters/postgres/connections.py` & `dbt-postgres-1.6.0b6/dbt/adapters/postgres/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/adapters/postgres/impl.py` & `dbt-postgres-1.6.0b6/dbt/adapters/postgres/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/adapters/postgres/relation.py` & `dbt-postgres-1.6.0b6/dbt/adapters/postgres/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/adapters/postgres/relation_configs/index.py` & `dbt-postgres-1.6.0b6/dbt/adapters/postgres/relation_configs/index.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/adapters/postgres/relation_configs/materialized_view.py` & `dbt-postgres-1.6.0b6/dbt/adapters/postgres/relation_configs/materialized_view.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/include/postgres/macros/adapters.sql` & `dbt-postgres-1.6.0b6/dbt/include/postgres/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/include/postgres/macros/catalog.sql` & `dbt-postgres-1.6.0b6/dbt/include/postgres/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/include/postgres/macros/materializations/materialized_view.sql` & `dbt-postgres-1.6.0b6/dbt/include/postgres/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/include/postgres/macros/materializations/snapshot_merge.sql` & `dbt-postgres-1.6.0b6/dbt/include/postgres/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/include/postgres/macros/relations.sql` & `dbt-postgres-1.6.0b6/dbt/include/postgres/macros/relations.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/include/postgres/macros/timestamps.sql` & `dbt-postgres-1.6.0b6/dbt/include/postgres/macros/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/include/postgres/macros/utils/datediff.sql` & `dbt-postgres-1.6.0b6/dbt/include/postgres/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt/include/postgres/macros/utils/listagg.sql` & `dbt-postgres-1.6.0b6/dbt/include/postgres/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/dbt_postgres.egg-info/PKG-INFO` & `dbt-postgres-1.6.0b6/dbt_postgres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-postgres
-Version: 1.6.0b5
+Version: 1.6.0b6
 Summary: The postgres adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b5 Summary: The postgres
+Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b6 Summary: The postgres
 adapter plugin for dbt (data build tool) Home-page: https://github.com/dbt-
 labs/dbt-core Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `dbt-postgres-1.6.0b5/dbt_postgres.egg-info/SOURCES.txt` & `dbt-postgres-1.6.0b6/dbt_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b5/setup.py` & `dbt-postgres-1.6.0b6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     # default to psycopg2-binary for all OSes/versions
     print(PSYCOPG2_MESSAGE)
     return "psycopg2-binary"
 
 
 package_name = "dbt-postgres"
-package_version = "1.6.0b5"
+package_version = "1.6.0b6"
 description = """The postgres adapter plugin for dbt (data build tool)"""
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 DBT_PSYCOPG2_NAME = _dbt_psycopg2_name()
```

