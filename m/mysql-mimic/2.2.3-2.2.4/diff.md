# Comparing `tmp/mysql-mimic-2.2.3.tar.gz` & `tmp/mysql-mimic-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-mimic-2.2.3.tar", last modified: Mon Apr 10 17:20:18 2023, max compression
+gzip compressed data, was "mysql-mimic-2.2.4.tar", last modified: Fri Jun 23 21:35:51 2023, max compression
```

## Comparing `mysql-mimic-2.2.3.tar` & `mysql-mimic-2.2.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:20:18.081870 mysql-mimic-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-10 17:20:18.081870 mysql-mimic-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:20:18.077870 mysql-mimic-2.2.3/mysql_mimic/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/charset.py
--rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/intercept.py
--rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/prepared.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    16711 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/mysql_mimic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:20:18.077870 mysql-mimic-2.2.3/mysql_mimic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-04-10 17:20:18.000000 mysql-mimic-2.2.3/mysql_mimic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-10 17:20:18.000000 mysql-mimic-2.2.3/mysql_mimic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:20:18.000000 mysql-mimic-2.2.3/mysql_mimic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-10 17:20:18.000000 mysql-mimic-2.2.3/mysql_mimic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 17:20:18.000000 mysql-mimic-2.2.3/mysql_mimic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 17:20:18.081870 mysql-mimic-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:20:18.077870 mysql-mimic-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    28243 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-10 17:19:47.000000 mysql-mimic-2.2.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/mysql_mimic/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/charset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19310 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/prepared.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/mysql_mimic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/mysql_mimic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-23 21:35:51.000000 mysql-mimic-2.2.4/mysql_mimic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-23 21:35:51.000000 mysql-mimic-2.2.4/mysql_mimic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:35:51.000000 mysql-mimic-2.2.4/mysql_mimic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 21:35:51.000000 mysql-mimic-2.2.4/mysql_mimic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 21:35:51.000000 mysql-mimic-2.2.4/mysql_mimic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:35:51.527755 mysql-mimic-2.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28243 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-23 21:35:24.000000 mysql-mimic-2.2.4/tests/test_version.py
```

### Comparing `mysql-mimic-2.2.3/LICENSE` & `mysql-mimic-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/PKG-INFO` & `mysql-mimic-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.3
+Version: 2.2.4
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.3/README.md` & `mysql-mimic-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/auth.py` & `mysql-mimic-2.2.4/mysql_mimic/auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/charset.py` & `mysql-mimic-2.2.4/mysql_mimic/charset.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/connection.py` & `mysql-mimic-2.2.4/mysql_mimic/connection.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/constants.py` & `mysql-mimic-2.2.4/mysql_mimic/constants.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/errors.py` & `mysql-mimic-2.2.4/mysql_mimic/errors.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/intercept.py` & `mysql-mimic-2.2.4/mysql_mimic/intercept.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/packets.py` & `mysql-mimic-2.2.4/mysql_mimic/packets.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/results.py` & `mysql-mimic-2.2.4/mysql_mimic/results.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/schema.py` & `mysql-mimic-2.2.4/mysql_mimic/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,27 +158,27 @@
 
 def show_statement_to_info_schema_query(
     show: exp.Show, database: Optional[str] = None
 ) -> exp.Select:
     kind = show.name.upper()
     if kind == "COLUMNS":
         outputs = [
-            "column_name AS Field",
-            "data_type AS Type",
-            "is_nullable AS Null",
-            "column_key AS Key",
-            "column_default AS Default",
-            "extra AS Extra",
+            'column_name AS "Field"',
+            'data_type AS "Type"',
+            'is_nullable AS "Null"',
+            'column_key AS "Key"',
+            'column_default AS "Default"',
+            'extra AS "Extra"',
         ]
         if show.args.get("full"):
             outputs.extend(
                 [
-                    "collation_name AS Collation",
-                    "privileges AS Privileges",
-                    "column_comment AS Comment",
+                    'collation_name AS "Collation"',
+                    'privileges AS "Privileges"',
+                    'column_comment AS "Comment"',
                 ]
             )
         table = show.text("target")
         if not table:
             raise MysqlError(
                 "You have an error in your SQL syntax. Table name is missing.",
                 code=ErrorCode.PARSE_ERROR,
@@ -191,28 +191,28 @@
         db = show.text("db") or database
         if db:
             select = select.where(f"table_schema = '{db}'")
         like = show.text("like")
         if like:
             select = select.where(f"column_name LIKE '{like}'")
     elif kind == "TABLES":
-        outputs = ["table_name AS Table_name"]
+        outputs = ['table_name AS "Table_name"']
         if show.args.get("full"):
-            outputs.extend(["table_type AS Table_type"])
+            outputs.extend(['table_type AS "Table_type"'])
 
         select = exp.select(*outputs).from_("information_schema.tables")
         db = show.text("db") or database
         if not db:
             raise MysqlError("No database selected.", code=ErrorCode.NO_DB_ERROR)
         select = select.where(f"table_schema = '{db}'")
         like = show.text("like")
         if like:
             select = select.where(f"table_name LIKE '{like}'")
     elif kind == "DATABASES":
-        select = exp.select("schema_name AS Database").from_(
+        select = exp.select('schema_name AS "Database"').from_(
             "information_schema.schemata"
         )
         like = show.text("like")
         if like:
             select = select.where(f"schema_name LIKE '{like}'")
     elif kind == "INDEX":
         outputs = [
```

### Comparing `mysql-mimic-2.2.3/mysql_mimic/server.py` & `mysql-mimic-2.2.4/mysql_mimic/server.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/session.py` & `mysql-mimic-2.2.4/mysql_mimic/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
 from typing import (
     Dict,
+    List,
     TYPE_CHECKING,
     Optional,
     Callable,
     Awaitable,
     Type,
     Any,
     Iterator,
@@ -203,26 +204,29 @@
         """
         Called when the client closes the connection.
         """
         self._connection = None
 
     async def handle_query(self, sql: str, attrs: Dict[str, str]) -> AllowedResult:
         result = None
-        for expression in self.dialect().parse(sql):
+        for expression in self._parse(sql):
             if not expression:
                 continue
             with self._set_var_hint(expression):
                 result = await self._intercept(expression, sql, attrs)
                 if result is None:
                     result = await self.query(expression, sql, attrs)
         return result
 
     async def use(self, database: str) -> None:
         self.database = database
 
+    def _parse(self, sql: str) -> List[exp.Expression]:
+        return [e for e in self.dialect().parse(sql) if e]
+
     async def _query_info_schema(self, expression: exp.Expression) -> AllowedResult:
         return await ensure_info_schema(await self.schema()).query(expression)
 
     @contextmanager
     def _set_var_hint(self, expression: exp.Expression) -> Iterator[None]:
         """Handles any SET_VAR hints, which set system variables for a single statement"""
         hint = expression.args.get("hint")
```

### Comparing `mysql-mimic-2.2.3/mysql_mimic/stream.py` & `mysql-mimic-2.2.4/mysql_mimic/stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/types.py` & `mysql-mimic-2.2.4/mysql_mimic/types.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/utils.py` & `mysql-mimic-2.2.4/mysql_mimic/utils.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic/variables.py` & `mysql-mimic-2.2.4/mysql_mimic/variables.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/mysql_mimic.egg-info/PKG-INFO` & `mysql-mimic-2.2.4/mysql_mimic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-mimic
-Version: 2.2.3
+Version: 2.2.4
 Summary: A python implementation of the mysql server protocol
 Home-page: https://github.com/kelsin/mysql-mimic
 Author: Christopher Giroir
 Author-email: kelsin@valefor.com
 License: MIT
 Description: # MySQL-Mimic
```

### Comparing `mysql-mimic-2.2.3/mysql_mimic.egg-info/SOURCES.txt` & `mysql-mimic-2.2.4/mysql_mimic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/setup.py` & `mysql-mimic-2.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/tests/test_auth.py` & `mysql-mimic-2.2.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/tests/test_query.py` & `mysql-mimic-2.2.4/tests/test_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -477,15 +477,15 @@
         ("SET autocommit = 0; SELECT @@autocommit AS x", [{"x": False}]),
         (
             "SET lower_case_table_names = 1; SELECT @@lower_case_table_names AS x",
             [{"x": 1}],
         ),
         # Simple queries
         ("SELECT 1, 2", [{"1": 1, "2": 2}]),
-        ("SELECT '1' AS Hello", [{"Hello": "1"}]),
+        ("SELECT '1' AS Hello", [{"hello": "1"}]),
         # USE
         ("USE db2; SELECT DATABASE()", [{"DATABASE()": "db2"}]),
         # INFORMATION_SCHEMA
         (
             """
         SELECT
           *
@@ -612,15 +612,15 @@
         ),
         (
             queries.TABLEAU_INDEXES_1,
             [],
         ),
         (
             "SELECT CATALOG_NAME AS CatalogName FROM INFORMATION_SCHEMA.SCHEMATA LIMIT 1",
-            [{"CatalogName": "def"}],
+            [{"catalogname": "def"}],
         ),
         # SHOW
         (
             "show variables",
             [
                 {"Value": "1", "Variable_name": "auto_increment_increment"},
                 {"Value": "False", "Variable_name": "autocommit"},
@@ -750,36 +750,36 @@
             [{"DATABASE()": None, "SCHEMA()": None, "_col_2": "levon_helm"}],
         ),
         (queries.DATA_GRIP_PARAMETERS, []),
         (
             queries.DATA_GRIP_TABLES,
             [
                 {
-                    "REF_GENERATION": None,
-                    "REMARKS": None,
-                    "SELF_REFERENCING_COL_NAME": None,
-                    "TABLE_CAT": "db",
+                    "ref_generation": None,
+                    "remarks": None,
+                    "self_referencing_col_name": None,
+                    "table_cat": "db",
                     "table_name": "x",
-                    "TABLE_SCHEM": None,
-                    "TABLE_TYPE": "TABLE",
-                    "TYPE_CAT": None,
-                    "TYPE_NAME": None,
-                    "TYPE_SCHEM": None,
+                    "table_schem": None,
+                    "table_type": "TABLE",
+                    "type_cat": None,
+                    "type_name": None,
+                    "type_schem": None,
                 },
                 {
-                    "REF_GENERATION": None,
-                    "REMARKS": None,
-                    "SELF_REFERENCING_COL_NAME": None,
-                    "TABLE_CAT": "db",
+                    "ref_generation": None,
+                    "remarks": None,
+                    "self_referencing_col_name": None,
+                    "table_cat": "db",
                     "table_name": "y",
-                    "TABLE_SCHEM": None,
-                    "TABLE_TYPE": "TABLE",
-                    "TYPE_CAT": None,
-                    "TYPE_NAME": None,
-                    "TYPE_SCHEM": None,
+                    "table_schem": None,
+                    "table_type": "TABLE",
+                    "type_cat": None,
+                    "type_name": None,
+                    "type_schem": None,
                 },
             ],
         ),
     ],
 )
 async def test_commands(
     session: MockSession,
```

### Comparing `mysql-mimic-2.2.3/tests/test_ssl.py` & `mysql-mimic-2.2.4/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/tests/test_stream.py` & `mysql-mimic-2.2.4/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `mysql-mimic-2.2.3/tests/test_types.py` & `mysql-mimic-2.2.4/tests/test_types.py`

 * *Files identical despite different names*

