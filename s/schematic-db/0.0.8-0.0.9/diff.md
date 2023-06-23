# Comparing `tmp/schematic_db-0.0.8.tar.gz` & `tmp/schematic_db-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schematic_db-0.0.8.tar", max compression
+gzip compressed data, was "schematic_db-0.0.9.tar", max compression
```

## Comparing `schematic_db-0.0.8.tar` & `schematic_db-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      798 2023-02-03 17:59:51.809761 schematic_db-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1156 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/__init__.py
--rw-r--r--   0        0        0      198 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/db_config/__init__.py
--rw-r--r--   0        0        0     9809 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/db_config/db_config.py
--rw-r--r--   0        0        0      151 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/query_store/__init__.py
--rw-r--r--   0        0        0      914 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/query_store/query_store.py
--rw-r--r--   0        0        0      973 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/query_store/synapse_query_store.py
--rw-r--r--   0        0        0      203 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/rdb/__init__.py
--rw-r--r--   0        0        0    10066 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/rdb/mysql.py
--rw-r--r--   0        0        0     1900 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/rdb/postgres.py
--rw-r--r--   0        0        0     3054 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/rdb/rdb.py
--rw-r--r--   0        0        0    18534 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/rdb/synapse_database.py
--rw-r--r--   0        0        0      117 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/rdb_queryer/__init__.py
--rw-r--r--   0        0        0     1929 2023-02-03 17:59:51.809761 schematic_db-0.0.8/schematic_db/rdb_queryer/rdb_queryer.py
--rw-r--r--   0        0        0      148 2023-02-03 17:59:51.813762 schematic_db-0.0.8/schematic_db/rdb_updater/__init__.py
--rw-r--r--   0        0        0     5344 2023-02-03 17:59:51.813762 schematic_db-0.0.8/schematic_db/rdb_updater/rdb_updater.py
--rw-r--r--   0        0        0      180 2023-02-03 17:59:51.813762 schematic_db-0.0.8/schematic_db/schema/__init__.py
--rw-r--r--   0        0        0     9873 2023-02-03 17:59:51.813762 schematic_db-0.0.8/schematic_db/schema/api_utils.py
--rw-r--r--   0        0        0    15112 2023-02-03 17:59:51.813762 schematic_db-0.0.8/schematic_db/schema/schema.py
--rw-r--r--   0        0        0       97 2023-02-03 17:59:51.813762 schematic_db-0.0.8/schematic_db/synapse/__init__.py
--rw-r--r--   0        0        0    13770 2023-02-03 17:59:51.813762 schematic_db-0.0.8/schematic_db/synapse/synapse.py
--rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 schematic_db-0.0.8/setup.py
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 schematic_db-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-02-04 20:15:56.330790 schematic_db-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1156 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/__init__.py
+-rw-r--r--   0        0        0      198 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/db_config/__init__.py
+-rw-r--r--   0        0        0     9843 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/db_config/db_config.py
+-rw-r--r--   0        0        0      151 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/query_store/__init__.py
+-rw-r--r--   0        0        0      914 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/query_store/query_store.py
+-rw-r--r--   0        0        0      973 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/query_store/synapse_query_store.py
+-rw-r--r--   0        0        0      203 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/rdb/__init__.py
+-rw-r--r--   0        0        0    10066 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/rdb/mysql.py
+-rw-r--r--   0        0        0     1900 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/rdb/postgres.py
+-rw-r--r--   0        0        0     3054 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/rdb/rdb.py
+-rw-r--r--   0        0        0    18534 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/rdb/synapse_database.py
+-rw-r--r--   0        0        0      117 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/rdb_queryer/__init__.py
+-rw-r--r--   0        0        0     1929 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/rdb_queryer/rdb_queryer.py
+-rw-r--r--   0        0        0      148 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/rdb_updater/__init__.py
+-rw-r--r--   0        0        0     5344 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/rdb_updater/rdb_updater.py
+-rw-r--r--   0        0        0      180 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/schema/__init__.py
+-rw-r--r--   0        0        0     9873 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/schema/api_utils.py
+-rw-r--r--   0        0        0    15112 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/schema/schema.py
+-rw-r--r--   0        0        0       97 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/synapse/__init__.py
+-rw-r--r--   0        0        0    13770 2023-02-04 20:15:56.330790 schematic_db-0.0.9/schematic_db/synapse/synapse.py
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 schematic_db-0.0.9/setup.py
+-rw-r--r--   0        0        0     1355 1970-01-01 00:00:00.000000 schematic_db-0.0.9/PKG-INFO
```

### Comparing `schematic_db-0.0.8/schematic_db/__init__.py` & `schematic_db-0.0.9/schematic_db/__init__.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/schematic_db/db_config/db_config.py` & `schematic_db-0.0.9/schematic_db/db_config/db_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """DB config
 These are a set of classes for defining a database table in a dialect agnostic way.
 """
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any
+from typing import Any, Optional
 
 from sqlalchemy import ForeignKey
 
 
 class DBDatatype(Enum):
     """A generic datatype that should be supported by all database types."""
 
@@ -63,15 +63,17 @@
     def __str__(self) -> str:
         return f"{self.message}: {self.object_name}"
 
 
 class ConfigKeyError(Exception):
     """ConfigKeyError"""
 
-    def __init__(self, message: str, object_name: str, key: str = None) -> None:
+    def __init__(
+        self, message: str, object_name: str, key: Optional[str] = None
+    ) -> None:
         self.message = message
         self.object_name = object_name
         self.key = key
         super().__init__(self.message)
 
     def __str__(self) -> str:
         if self.key is None:
```

### Comparing `schematic_db-0.0.8/schematic_db/query_store/query_store.py` & `schematic_db-0.0.9/schematic_db/query_store/query_store.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/schematic_db/query_store/synapse_query_store.py` & `schematic_db-0.0.9/schematic_db/query_store/synapse_query_store.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/schematic_db/rdb/mysql.py` & `schematic_db-0.0.9/schematic_db/rdb/mysql.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/schematic_db/rdb/postgres.py` & `schematic_db-0.0.9/schematic_db/rdb/postgres.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/schematic_db/rdb/rdb.py` & `schematic_db-0.0.9/schematic_db/rdb/rdb.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/schematic_db/rdb/synapse_database.py` & `schematic_db-0.0.9/schematic_db/rdb/synapse_database.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/schematic_db/rdb_queryer/rdb_queryer.py` & `schematic_db-0.0.9/schematic_db/rdb_queryer/rdb_queryer.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/schematic_db/rdb_updater/rdb_updater.py` & `schematic_db-0.0.9/schematic_db/rdb_updater/rdb_updater.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/schematic_db/schema/api_utils.py` & `schematic_db-0.0.9/schematic_db/schema/api_utils.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/schematic_db/schema/schema.py` & `schematic_db-0.0.9/schematic_db/schema/schema.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/schematic_db/synapse/synapse.py` & `schematic_db-0.0.9/schematic_db/synapse/synapse.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.8/setup.py` & `schematic_db-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'SQLAlchemy-Utils>=0.38.3,<0.39.0',
  'SQLAlchemy>=1.4.39,<2.0.0',
- 'black==23.1.0',
- 'mypy>=0.982,<0.983',
  'networkx>=2.8.6,<3.0.0',
  'pandas>=1.4.3,<2.0.0',
- 'pdoc>=12.1.0,<13.0.0',
- 'pylint>=2.15.4,<3.0.0',
- 'pytest-mock>=3.10.0,<4.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'tenacity>=8.1.0,<9.0.0']
+ 'requests>=2.28.1,<3.0.0']
 
 extras_require = \
-{'mysql': ['mysqlclient>=2.1.1,<3.0.0'],
- 'postgres': ['psycopg2>=2.9.5,<3.0.0'],
- 'synapse': ['synapseclient>=2.6.0,<3.0.0']}
+{'black': ['black==23.1.0'],
+ 'mypy': ['mypy==0.991'],
+ 'mysql': ['mysqlclient>=2.1.1,<3.0.0'],
+ 'pdoc': ['pdoc>=12.1.0,<13.0.0'],
+ 'postgres': ['psycopg2-binary>=2.9.5,<3.0.0'],
+ 'pylint': ['pylint==2.16.1'],
+ 'pytest-mock': ['pytest-mock>=3.10.0,<4.0.0'],
+ 'synapse': ['synapseclient>=2.6.0,<3.0.0'],
+ 'tenacity': ['tenacity>=8.1.0,<9.0.0']}
 
 setup_kwargs = {
     'name': 'schematic-db',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '',
     'long_description': 'None',
     'author': 'andrewelamb',
     'author_email': 'andrewelamb@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `schematic_db-0.0.8/PKG-INFO` & `schematic_db-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: schematic-db
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: andrewelamb
 Author-email: andrewelamb@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: black
+Provides-Extra: mypy
 Provides-Extra: mysql
+Provides-Extra: pdoc
 Provides-Extra: postgres
+Provides-Extra: pylint
+Provides-Extra: pytest-mock
 Provides-Extra: synapse
+Provides-Extra: tenacity
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: SQLAlchemy (>=1.4.39,<2.0.0)
 Requires-Dist: SQLAlchemy-Utils (>=0.38.3,<0.39.0)
-Requires-Dist: black (==23.1.0)
-Requires-Dist: mypy (>=0.982,<0.983)
+Requires-Dist: black (==23.1.0) ; extra == "black"
+Requires-Dist: mypy (==0.991) ; extra == "mypy"
 Requires-Dist: mysqlclient (>=2.1.1,<3.0.0) ; extra == "mysql"
 Requires-Dist: networkx (>=2.8.6,<3.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
-Requires-Dist: pdoc (>=12.1.0,<13.0.0)
-Requires-Dist: psycopg2 (>=2.9.5,<3.0.0) ; extra == "postgres"
-Requires-Dist: pylint (>=2.15.4,<3.0.0)
-Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
+Requires-Dist: pdoc (>=12.1.0,<13.0.0) ; extra == "pdoc"
+Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0) ; extra == "postgres"
+Requires-Dist: pylint (==2.16.1) ; extra == "pylint"
+Requires-Dist: pytest-mock (>=3.10.0,<4.0.0) ; extra == "pytest-mock"
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: synapseclient (>=2.6.0,<3.0.0) ; extra == "synapse"
-Requires-Dist: tenacity (>=8.1.0,<9.0.0)
+Requires-Dist: tenacity (>=8.1.0,<9.0.0) ; extra == "tenacity"
```

