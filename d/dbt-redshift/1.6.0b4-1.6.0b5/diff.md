# Comparing `tmp/dbt-redshift-1.6.0b4.tar.gz` & `tmp/dbt-redshift-1.6.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-redshift-1.6.0b4.tar", last modified: Fri Jun 16 17:49:50 2023, max compression
+gzip compressed data, was "dbt-redshift-1.6.0b5.tar", last modified: Fri Jun 23 21:42:01 2023, max compression
```

## Comparing `dbt-redshift-1.6.0b4.tar` & `dbt-redshift-1.6.0b5.tar`

### file list

```diff
@@ -1,51 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.564393 dbt-redshift-1.6.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-16 17:49:50.564393 dbt-redshift-1.6.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.556393 dbt-redshift-1.6.0b4/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/adapters/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.556393 dbt-redshift-1.6.0b4/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/include/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.564393 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.564393 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 17:49:50.564393 dbt-redshift-1.6.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.693997 dbt-redshift-1.6.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-23 21:42:01.693997 dbt-redshift-1.6.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.685997 dbt-redshift-1.6.0b5/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/adapters/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/materialized_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/adapters/redshift/relation_configs/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.685997 dbt-redshift-1.6.0b5/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/include/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/materializations/materialized_view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.689997 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.693997 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/dbt/include/redshift/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:42:01.693997 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 21:42:01.000000 dbt-redshift-1.6.0b5/dbt_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:42:01.693997 dbt-redshift-1.6.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-06-23 21:41:48.000000 dbt-redshift-1.6.0b5/setup.py
```

### Comparing `dbt-redshift-1.6.0b4/LICENSE.md` & `dbt-redshift-1.6.0b5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b4/PKG-INFO` & `dbt-redshift-1.6.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.6.0b4
+Version: 1.6.0b5
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b4 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b5 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dbt-redshift-1.6.0b4/README.md` & `dbt-redshift-1.6.0b5/README.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b4/dbt/adapters/redshift/__init__.py` & `dbt-redshift-1.6.0b5/dbt/adapters/redshift/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from dbt.adapters.redshift.connections import RedshiftConnectionManager  # noqa
-from dbt.adapters.redshift.connections import RedshiftCredentials
-from dbt.adapters.redshift.column import RedshiftColumn  # noqa
+from dbt.adapters.base import AdapterPlugin
+
+from dbt.adapters.redshift.connections import (  # noqa: F401
+    RedshiftConnectionManager,
+    RedshiftCredentials,
+)
 from dbt.adapters.redshift.relation import RedshiftRelation  # noqa: F401
 from dbt.adapters.redshift.impl import RedshiftAdapter
+from dbt.include import redshift
 
 
-from dbt.adapters.base import AdapterPlugin  # type: ignore
-from dbt.include import redshift  # type: ignore
-
 Plugin: AdapterPlugin = AdapterPlugin(
     adapter=RedshiftAdapter,  # type: ignore
     credentials=RedshiftCredentials,
     include_path=redshift.PACKAGE_PATH,
     dependencies=["postgres"],
 )
```

### Comparing `dbt-redshift-1.6.0b4/dbt/adapters/redshift/connections.py` & `dbt-redshift-1.6.0b5/dbt/adapters/redshift/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b4/dbt/adapters/redshift/impl.py` & `dbt-redshift-1.6.0b5/dbt/adapters/redshift/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from dataclasses import dataclass
 from typing import Optional, Set, Any, Dict, Type
 from collections import namedtuple
 
 from dbt.adapters.base import PythonJobHelper
 from dbt.adapters.base.impl import AdapterConfig, ConstraintSupport
-from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.base.meta import available
+from dbt.adapters.sql import SQLAdapter
 from dbt.contracts.connection import AdapterResponse
 from dbt.contracts.graph.nodes import ConstraintType
 from dbt.events import AdapterLogger
-
 import dbt.exceptions
 
-from dbt.adapters.redshift import RedshiftConnectionManager, RedshiftRelation, RedshiftColumn
+from dbt.adapters.redshift import RedshiftConnectionManager, RedshiftRelation
+
 
 logger = AdapterLogger("Redshift")
 
 
 GET_RELATIONS_MACRO_NAME = "redshift__get_relations"
 
 
 @dataclass
 class RedshiftConfig(AdapterConfig):
     sort_type: Optional[str] = None
     dist: Optional[str] = None
     sort: Optional[str] = None
     bind: Optional[bool] = None
     backup: Optional[bool] = True
+    autorefresh: Optional[bool] = False
 
 
 class RedshiftAdapter(SQLAdapter):
     Relation = RedshiftRelation
     ConnectionManager = RedshiftConnectionManager
     connections: RedshiftConnectionManager
-    Column = RedshiftColumn  # type: ignore
 
     AdapterSpecificConfigs = RedshiftConfig  # type: ignore
 
     CONSTRAINT_SUPPORT = {
         ConstraintType.check: ConstraintSupport.NOT_SUPPORTED,
         ConstraintType.not_null: ConstraintSupport.ENFORCED,
         ConstraintType.unique: ConstraintSupport.NOT_ENFORCED,
```

### Comparing `dbt-redshift-1.6.0b4/dbt/include/redshift/macros/adapters/apply_grants.sql` & `dbt-redshift-1.6.0b5/dbt/include/redshift/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b4/dbt/include/redshift/macros/adapters.sql` & `dbt-redshift-1.6.0b5/dbt/include/redshift/macros/adapters.sql`

 * *Files 6% similar despite different names*

```diff
@@ -234,15 +234,19 @@
     from pg_tables
     where schemaname ilike '{{ schema_relation.schema }}'
     union all
     select
       '{{ schema_relation.database }}' as database,
       viewname as name,
       schemaname as schema,
-      'view' as type
+      case
+        when definition ilike '%create materialized view%'
+          then 'materialized_view'
+        else 'view'
+      end as type
     from pg_views
     where schemaname ilike '{{ schema_relation.schema }}'
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
 
 
@@ -305,7 +309,16 @@
       {% endset %}
       {% do run_query(sql) %}
     {% endfor %}
 
   {% endif %}
 
 {% endmacro %}
+
+
+{% macro redshift__get_drop_relation_sql(relation) %}
+    {%- if relation.is_materialized_view -%}
+        {{ redshift__drop_materialized_view(relation) }}
+    {%- else -%}
+        drop {{ relation.type }} if exists {{ relation }} cascade
+    {%- endif -%}
+{% endmacro %}
```

### Comparing `dbt-redshift-1.6.0b4/dbt/include/redshift/macros/catalog.sql` & `dbt-redshift-1.6.0b5/dbt/include/redshift/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/listagg.sql` & `dbt-redshift-1.6.0b5/dbt/include/redshift/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b4/dbt/include/redshift/profile_template.yml` & `dbt-redshift-1.6.0b5/dbt/include/redshift/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b4/dbt_redshift.egg-info/PKG-INFO` & `dbt-redshift-1.6.0b5/dbt_redshift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.6.0b4
+Version: 1.6.0b5
 Summary: The Redshift adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b4 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b5 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dbt-redshift-1.6.0b4/dbt_redshift.egg-info/SOURCES.txt` & `dbt-redshift-1.6.0b5/dbt_redshift.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 LICENSE.md
 MANIFEST.in
 README.md
 setup.py
 dbt/__init__.py
 dbt/adapters/redshift/__init__.py
 dbt/adapters/redshift/__version__.py
-dbt/adapters/redshift/column.py
 dbt/adapters/redshift/connections.py
 dbt/adapters/redshift/impl.py
 dbt/adapters/redshift/relation.py
+dbt/adapters/redshift/relation_configs/__init__.py
+dbt/adapters/redshift/relation_configs/base.py
+dbt/adapters/redshift/relation_configs/dist.py
+dbt/adapters/redshift/relation_configs/materialized_view.py
+dbt/adapters/redshift/relation_configs/policies.py
+dbt/adapters/redshift/relation_configs/sort.py
 dbt/include/redshift/__init__.py
 dbt/include/redshift/dbt_project.yml
 dbt/include/redshift/profile_template.yml
 dbt/include/redshift/macros/adapters.sql
 dbt/include/redshift/macros/catalog.sql
 dbt/include/redshift/macros/relations.sql
 dbt/include/redshift/macros/timestamps.sql
 dbt/include/redshift/macros/adapters/apply_grants.sql
+dbt/include/redshift/macros/materializations/materialized_view.sql
 dbt/include/redshift/macros/materializations/snapshot_merge.sql
 dbt/include/redshift/macros/materializations/seeds/helpers.sql
 dbt/include/redshift/macros/utils/array_append.sql
 dbt/include/redshift/macros/utils/array_concat.sql
 dbt/include/redshift/macros/utils/array_construct.sql
 dbt/include/redshift/macros/utils/cast_bool_to_text.sql
 dbt/include/redshift/macros/utils/dateadd.sql
```

### Comparing `dbt-redshift-1.6.0b4/setup.py` & `dbt-redshift-1.6.0b5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,16 @@
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         f"dbt-core~={_core_version()}",
         f"dbt-postgres~={_core_version()}",
         "boto3~=1.26.26",
         "redshift-connector~=2.0.911",
+        # installed via dbt-core but referenced directly; don't pin to avoid version conflicts with dbt-core
+        "agate",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

