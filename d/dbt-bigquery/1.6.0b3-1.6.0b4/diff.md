# Comparing `tmp/dbt-bigquery-1.6.0b3.tar.gz` & `tmp/dbt-bigquery-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-bigquery-1.6.0b3.tar", last modified: Thu Jun  8 23:43:29 2023, max compression
+gzip compressed data, was "dbt-bigquery-1.6.0b4.tar", last modified: Fri Jun 23 02:09:18 2023, max compression
```

## Comparing `dbt-bigquery-1.6.0b3.tar` & `dbt-bigquery-1.6.0b4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.586078 dbt-bigquery-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-08 23:43:29.586078 dbt-bigquery-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.578077 dbt-bigquery-1.6.0b3/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.574077 dbt-bigquery-1.6.0b3/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.578077 dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    37971 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.574077 dbt-bigquery-1.6.0b3/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.578077 dbt-bigquery-1.6.0b3/dbt/include/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.582078 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.582078 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/etc.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.582078 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/copy.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/incremental.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.582078 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/incremental_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.582078 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.586078 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/dbt/include/bigquery/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:43:29.586078 dbt-bigquery-1.6.0b3/dbt_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-08 23:43:29.000000 dbt-bigquery-1.6.0b3/dbt_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-08 23:43:29.000000 dbt-bigquery-1.6.0b3/dbt_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:43:29.000000 dbt-bigquery-1.6.0b3/dbt_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:43:29.000000 dbt-bigquery-1.6.0b3/dbt_bigquery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 23:43:29.000000 dbt-bigquery-1.6.0b3/dbt_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 23:43:29.000000 dbt-bigquery-1.6.0b3/dbt_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:43:29.586078 dbt-bigquery-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-08 23:43:14.000000 dbt-bigquery-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.614444 dbt-bigquery-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-23 02:09:18.614444 dbt-bigquery-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.602444 dbt-bigquery-1.6.0b4/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.598444 dbt-bigquery-1.6.0b4/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.606444 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39652 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.598444 dbt-bigquery-1.6.0b4/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.606444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.606444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.606444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/etc.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.606444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/copy.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.610444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.610444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.614444 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/dbt/include/bigquery/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:09:18.614444 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 02:09:18.000000 dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 02:09:18.614444 dbt-bigquery-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-23 02:09:02.000000 dbt-bigquery-1.6.0b4/setup.py
```

### Comparing `dbt-bigquery-1.6.0b3/LICENSE.md` & `dbt-bigquery-1.6.0b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/PKG-INFO` & `dbt-bigquery-1.6.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b3 Summary: The Bigquery
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b4 Summary: The Bigquery
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dbt-bigquery-1.6.0b3/README.md` & `dbt-bigquery-1.6.0b4/README.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/__init__.py` & `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/connections.py` & `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/dataset.py` & `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/dataset.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/gcloud.py` & `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/gcloud.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/impl.py` & `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     SchemaSearchMap,
     AdapterConfig,
     PythonJobHelper,
 )
 
 from dbt.adapters.cache import _make_ref_key_dict  # type: ignore
 
+from dbt.adapters.bigquery.column import get_nested_column_data_types
 from dbt.adapters.bigquery.relation import BigQueryRelation
 from dbt.adapters.bigquery.dataset import add_access_entry_to_dataset
 from dbt.adapters.bigquery import BigQueryColumn
 from dbt.adapters.bigquery import BigQueryConnectionManager
 from dbt.adapters.bigquery.python_submissions import (
     ClusterDataprocHelper,
     ServerlessDataProcHelper,
@@ -289,14 +290,23 @@
         except StopIteration:
             pass
         except google.api_core.exceptions.NotFound:
             # the schema does not exist
             return False
         return True
 
+    @available.parse(lambda *a, **k: {})
+    @classmethod
+    def nest_column_data_types(
+        cls,
+        columns: Dict[str, Dict[str, Any]],
+        constraints: Optional[Dict[str, str]] = None,
+    ) -> Dict[str, Dict[str, str]]:
+        return get_nested_column_data_types(columns, constraints)
+
     def get_columns_in_relation(self, relation: BigQueryRelation) -> List[BigQueryColumn]:
         try:
             table = self.connections.get_bq_table(
                 database=relation.database, schema=relation.schema, identifier=relation.identifier
             )
             return self._get_dbt_columns_from_bq_table(table)
 
@@ -522,15 +532,18 @@
         """Get a list of the column names and data types from the given sql.
 
         :param str sql: The sql to execute.
         :return: List[BigQueryColumn]
         """
         _, iterator = self.connections.raw_execute(sql)
         columns = [self.Column.create_from_field(field) for field in iterator.schema]
-        return columns
+        flattened_columns = []
+        for column in columns:
+            flattened_columns += column.flatten()
+        return flattened_columns
 
     @available.parse(lambda *a, **k: False)
     def get_columns_in_select_sql(self, select_sql: str) -> List[BigQueryColumn]:
         try:
             conn = self.connections.get_thread_connection()
             client = conn.handle
             query_job, iterator = self.connections.raw_execute(select_sql)
@@ -954,14 +967,39 @@
     @property
     def python_submission_helpers(self) -> Dict[str, Type[PythonJobHelper]]:
         return {
             "cluster": ClusterDataprocHelper,
             "serverless": ServerlessDataProcHelper,
         }
 
+    @available
+    @classmethod
+    def render_raw_columns_constraints(cls, raw_columns: Dict[str, Dict[str, Any]]) -> List:
+        rendered_constraints: Dict[str, str] = {}
+        for raw_column in raw_columns.values():
+            for con in raw_column.get("constraints", None):
+                constraint = cls._parse_column_constraint(con)
+                rendered_constraint = cls.process_parsed_constraint(
+                    constraint, cls.render_column_constraint
+                )
+
+                if rendered_constraint:
+                    column_name = raw_column["name"]
+                    if column_name not in rendered_constraints:
+                        rendered_constraints[column_name] = rendered_constraint
+                    else:
+                        rendered_constraints[column_name] += f" {rendered_constraint}"
+
+        nested_columns = cls.nest_column_data_types(raw_columns, rendered_constraints)
+        rendered_column_constraints = [
+            f"{cls.quote(column['name']) if column.get('quote') else column['name']} {column['data_type']}"
+            for column in nested_columns.values()
+        ]
+        return rendered_column_constraints
+
     @classmethod
     def render_column_constraint(cls, constraint: ColumnLevelConstraint) -> Optional[str]:
         c = super().render_column_constraint(constraint)  # type: ignore
         if (
             constraint.type == ConstraintType.primary_key
             or constraint.type == ConstraintType.foreign_key
         ):
```

### Comparing `dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/python_submissions.py` & `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/python_submissions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Dict, Union
 
 from dbt.adapters.base import PythonJobHelper
+from google.api_core.future.polling import POLLING_PREDICATE
+
 from dbt.adapters.bigquery import BigQueryConnectionManager, BigQueryCredentials
 from dbt.adapters.bigquery.connections import DataprocBatchConfig
 from google.api_core import retry
 from google.api_core.client_options import ClientOptions
 from google.cloud import storage, dataproc_v1  # type: ignore
 from google.protobuf.json_format import ParseDict
 
@@ -39,15 +41,17 @@
         )
         self.gcs_location = "gs://{}/{}".format(self.credential.gcs_bucket, self.model_file_name)
 
         # set retry policy, default to timeout after 24 hours
         self.timeout = self.parsed_model["config"].get(
             "timeout", self.credential.job_execution_timeout_seconds or 60 * 60 * 24
         )
-        self.retry = retry.Retry(maximum=10.0, deadline=self.timeout)
+        self.result_polling_policy = retry.Retry(
+            predicate=POLLING_PREDICATE, maximum=10.0, timeout=self.timeout
+        )
         self.client_options = ClientOptions(
             api_endpoint="{}-dataproc.googleapis.com:443".format(self.credential.dataproc_region)
         )
         self.job_client = self._get_job_client()
 
     def _upload_to_gcs(self, filename: str, compiled_code: str) -> None:
         bucket = self.storage_client.get_bucket(self.credential.gcs_bucket)
@@ -94,15 +98,15 @@
         operation = self.job_client.submit_job_as_operation(  # type: ignore
             request={
                 "project_id": self.credential.execution_project,
                 "region": self.credential.dataproc_region,
                 "job": job,
             }
         )
-        response = operation.result(retry=self.retry)
+        response = operation.result(polling=self.result_polling_policy)
         # check if job failed
         if response.status.state == 6:
             raise ValueError(response.status.details)
         return response
 
 
 class ServerlessDataProcHelper(BaseDataProcHelper):
@@ -119,15 +123,15 @@
             parent=parent,
             batch=batch,
         )
         # make the request
         operation = self.job_client.create_batch(request=request)  # type: ignore
         # this takes quite a while, waiting on GCP response to resolve
         # (not a google-api-core issue, more likely a dataproc serverless issue)
-        response = operation.result(retry=self.retry)
+        response = operation.result(polling=self.result_polling_policy)
         return response
         # there might be useful results here that we can parse and return
         # Dataproc job output is saved to the Cloud Storage bucket
         # allocated to the job. Use regex to obtain the bucket and blob info.
         # matches = re.match("gs://(.*?)/(.*)", response.driver_output_resource_uri)
         # output = (
         #     self.storage_client
```

### Comparing `dbt-bigquery-1.6.0b3/dbt/adapters/bigquery/relation.py` & `dbt-bigquery-1.6.0b4/dbt/adapters/bigquery/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/adapters/apply_grants.sql` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/adapters.sql` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/catalog.sql` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/copy.sql` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/copy.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/incremental.sql` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/seed.sql` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/table.sql` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/macros/materializations/view.sql` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt/include/bigquery/profile_template.yml` & `dbt-bigquery-1.6.0b4/dbt/include/bigquery/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/dbt_bigquery.egg-info/PKG-INFO` & `dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.6.0b3
+Version: 1.6.0b4
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b3 Summary: The Bigquery
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b4 Summary: The Bigquery
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dbt-bigquery-1.6.0b3/dbt_bigquery.egg-info/SOURCES.txt` & `dbt-bigquery-1.6.0b4/dbt_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b3/setup.py` & `dbt-bigquery-1.6.0b4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     else:
         core_patch = "0"
 
     return f"{major}.{minor}.{core_patch}"
 
 
 package_name = "dbt-bigquery"
-package_version = "1.6.0b3"
+package_version = "1.6.0b4"
 dbt_core_version = _dbt_core_version(_dbt_bigquery_version())
 description = """The BigQuery adapter plugin for dbt"""
 
 setup(
     name="dbt-bigquery",
     version=_dbt_bigquery_version(),
     description="The Bigquery adapter plugin for dbt",
@@ -74,15 +74,14 @@
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         f"dbt-core~={_dbt_core_version(_dbt_bigquery_version())}",
         "google-cloud-bigquery~=3.0",
         "google-cloud-storage~=2.4",
         "google-cloud-dataproc~=5.0",
-        "agate~=1.6.3",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

