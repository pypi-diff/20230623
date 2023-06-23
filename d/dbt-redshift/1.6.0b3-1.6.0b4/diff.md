# Comparing `tmp/dbt-redshift-1.6.0b3.tar.gz` & `tmp/dbt-redshift-1.6.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-redshift-1.6.0b3.tar", last modified: Fri Jun  9 17:22:04 2023, max compression
+gzip compressed data, was "dbt-redshift-1.6.0b4.tar", last modified: Fri Jun 16 17:49:50 2023, max compression
```

## Comparing `dbt-redshift-1.6.0b3.tar` & `dbt-redshift-1.6.0b4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.827966 dbt-redshift-1.6.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-09 17:22:04.827966 dbt-redshift-1.6.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.811966 dbt-redshift-1.6.0b3/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.807966 dbt-redshift-1.6.0b3/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.815966 dbt-redshift-1.6.0b3/dbt/adapters/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    14575 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/adapters/redshift/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.807966 dbt-redshift-1.6.0b3/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.819966 dbt-redshift-1.6.0b3/dbt/include/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.819966 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.819966 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.819966 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.823966 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.827966 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/dbt/include/redshift/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:22:04.827966 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 17:22:04.000000 dbt-redshift-1.6.0b3/dbt_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:22:04.827966 dbt-redshift-1.6.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-09 17:21:47.000000 dbt-redshift-1.6.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.564393 dbt-redshift-1.6.0b4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-16 17:49:50.564393 dbt-redshift-1.6.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.556393 dbt-redshift-1.6.0b4/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/adapters/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/adapters/redshift/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.556393 dbt-redshift-1.6.0b4/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/include/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.560392 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.564393 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/dbt/include/redshift/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:49:50.564393 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-16 17:49:50.000000 dbt-redshift-1.6.0b4/dbt_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 17:49:50.564393 dbt-redshift-1.6.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-16 17:49:36.000000 dbt-redshift-1.6.0b4/setup.py
```

### Comparing `dbt-redshift-1.6.0b3/LICENSE.md` & `dbt-redshift-1.6.0b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b3/PKG-INFO` & `dbt-redshift-1.6.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.6.0b3
+Version: 1.6.0b4
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
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b3 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b4 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dbt-redshift-1.6.0b3/README.md` & `dbt-redshift-1.6.0b4/README.md`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b3/dbt/adapters/redshift/__init__.py` & `dbt-redshift-1.6.0b4/dbt/adapters/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b3/dbt/adapters/redshift/connections.py` & `dbt-redshift-1.6.0b4/dbt/adapters/redshift/connections.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from contextlib import contextmanager
 from typing import NewType, Tuple, Union, Optional, List
 from dataclasses import dataclass, field
 
 import agate
 import sqlparse
 import redshift_connector
-import urllib.request
-import json
 from redshift_connector.utils.oids import get_datatype_name
 
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import AdapterResponse, Connection, Credentials
 from dbt.contracts.util import Replaceable
 from dbt.dataclass_schema import FieldEncoder, dbtClassMixin, StrEnum, ValidationError
 from dbt.events import AdapterLogger
@@ -44,31 +42,14 @@
     def json_schema(self):
         return {"type": "integer", "minimum": 0, "maximum": 65535}
 
 
 dbtClassMixin.register_field_encoders({IAMDuration: IAMDurationEncoder()})
 
 
-def _get_aws_regions():
-    # Extract the prefixes from the AWS IP ranges JSON to determine the available regions
-    url = "https://ip-ranges.amazonaws.com/ip-ranges.json"
-    response = urllib.request.urlopen(url)
-    data = json.loads(response.read().decode())
-    regions = set()
-
-    for prefix in data["prefixes"]:
-        if prefix["service"] == "AMAZON":
-            regions.add(prefix["region"])
-
-    return regions
-
-
-_AVAILABLE_AWS_REGIONS = _get_aws_regions()
-
-
 class RedshiftConnectionMethod(StrEnum):
     DATABASE = "database"
     IAM = "iam"
 
 
 class UserSSLMode(StrEnum):
     disable = "disable"
@@ -145,15 +126,15 @@
     autocreate: bool = False
     db_groups: List[str] = field(default_factory=list)
     ra3_node: Optional[bool] = False
     connect_timeout: Optional[int] = None
     role: Optional[str] = None
     sslmode: Optional[UserSSLMode] = field(default_factory=UserSSLMode.default)
     retries: int = 1
-    region: Optional[str] = None  # if not provided, will be determined from host
+    region: Optional[str] = None
     # opt-in by default per team deliberation on https://peps.python.org/pep-0249/#autocommit
     autocommit: Optional[bool] = True
 
     _ALIASES = {"dbname": "database", "pass": "password"}
 
     @property
     def type(self):
@@ -184,21 +165,14 @@
         )
 
     @property
     def unique_field(self) -> str:
         return self.host
 
 
-def _is_valid_region(region):
-    if region is None or len(region) == 0:
-        logger.warning("Couldn't determine AWS regions. Skipping validation to avoid blocking.")
-        return True
-    return region in _AVAILABLE_AWS_REGIONS
-
-
 class RedshiftConnectMethodFactory:
     credentials: RedshiftCredentials
 
     def __init__(self, credentials):
         self.credentials = credentials
 
     def get_connect_method(self):
@@ -208,31 +182,14 @@
             "database": self.credentials.database,
             "port": self.credentials.port if self.credentials.port else 5439,
             "auto_create": self.credentials.autocreate,
             "db_groups": self.credentials.db_groups,
             "region": self.credentials.region,
             "timeout": self.credentials.connect_timeout,
         }
-        if kwargs["region"] is None:
-            logger.debug("No region provided, attempting to determine from host.")
-            try:
-                region_value = self.credentials.host.split(".")[2]
-            except IndexError:
-                raise dbt.exceptions.FailedToConnectError(
-                    "No region provided and unable to determine region from host: "
-                    "{}".format(self.credentials.host)
-                )
-
-            kwargs["region"] = region_value
-
-        # Validate the set region
-        if not _is_valid_region(kwargs["region"]):
-            raise dbt.exceptions.FailedToConnectError(
-                "Invalid region provided: {}".format(kwargs["region"])
-            )
 
         redshift_ssl_config = RedshiftSSLConfig.parse(self.credentials.sslmode)
         kwargs.update(redshift_ssl_config.to_dict())
 
         # Support missing 'method' for backwards compatibility
         if method == RedshiftConnectionMethod.DATABASE or method is None:
             # this requirement is really annoying to encode into json schema,
```

### Comparing `dbt-redshift-1.6.0b3/dbt/adapters/redshift/impl.py` & `dbt-redshift-1.6.0b4/dbt/adapters/redshift/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b3/dbt/adapters/redshift/relation.py` & `dbt-redshift-1.6.0b4/dbt/adapters/redshift/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b3/dbt/include/redshift/macros/adapters/apply_grants.sql` & `dbt-redshift-1.6.0b4/dbt/include/redshift/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b3/dbt/include/redshift/macros/adapters.sql` & `dbt-redshift-1.6.0b4/dbt/include/redshift/macros/adapters.sql`

 * *Files 18% similar despite different names*

```diff
@@ -305,25 +305,7 @@
       {% endset %}
       {% do run_query(sql) %}
     {% endfor %}
 
   {% endif %}
 
 {% endmacro %}
-
-{#
-  By using dollar-quoting like this, users can embed anything they want into their comments
-  (including nested dollar-quoting), as long as they do not use this exact dollar-quoting
-  label. It would be nice to just pick a new one but eventually you do have to give up.
-#}
-{% macro postgres_escape_comment(comment) -%}
-  {% if comment is not string %}
-    {% do exceptions.raise_compiler_error('cannot escape a non-string: ' ~ comment) %}
-  {% endif %}
-  {%- set magic = '$dbt_comment_literal_block$' -%}
-  {%- if magic in comment -%}
-    {%- do exceptions.raise_compiler_error('The string ' ~ magic ~ ' is not allowed in comments.') -%}
-  {%- endif -%}
-  {#- -- escape % until the underlying issue is fixed in redshift_connector -#}
-  {%- set comment = comment|replace("%", "%%") -%}
-  {{ magic }}{{ comment }}{{ magic }}
-{%- endmacro %}
```

### Comparing `dbt-redshift-1.6.0b3/dbt/include/redshift/macros/catalog.sql` & `dbt-redshift-1.6.0b4/dbt/include/redshift/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b3/dbt/include/redshift/macros/utils/listagg.sql` & `dbt-redshift-1.6.0b4/dbt/include/redshift/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b3/dbt/include/redshift/profile_template.yml` & `dbt-redshift-1.6.0b4/dbt/include/redshift/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b3/dbt_redshift.egg-info/PKG-INFO` & `dbt-redshift-1.6.0b4/dbt_redshift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-redshift
-Version: 1.6.0b3
+Version: 1.6.0b4
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
-Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b3 Summary: The Redshift
+Metadata-Version: 2.1 Name: dbt-redshift Version: 1.6.0b4 Summary: The Redshift
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-redshift
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dbt-redshift-1.6.0b3/dbt_redshift.egg-info/SOURCES.txt` & `dbt-redshift-1.6.0b4/dbt_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-redshift-1.6.0b3/setup.py` & `dbt-redshift-1.6.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     url="https://github.com/dbt-labs/dbt-redshift",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         f"dbt-core~={_core_version()}",
         f"dbt-postgres~={_core_version()}",
         "boto3~=1.26.26",
-        "redshift-connector~=2.0.910",
+        "redshift-connector~=2.0.911",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

