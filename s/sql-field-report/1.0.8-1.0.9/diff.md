# Comparing `tmp/sql_field_report-1.0.8.tar.gz` & `tmp/sql_field_report-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_field_report-1.0.8.tar", max compression
+gzip compressed data, was "sql_field_report-1.0.9.tar", max compression
```

## Comparing `sql_field_report-1.0.8.tar` & `sql_field_report-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      826 2023-06-22 09:44:53.765686 sql_field_report-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-1.0.8/README.md
--rw-r--r--   0        0        0      123 2023-06-22 08:39:56.322632 sql_field_report-1.0.8/sql_field_report/__init__.py
--rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-1.0.8/sql_field_report/__main__.py
--rw-r--r--   0        0        0     4909 2023-06-22 09:44:49.960983 sql_field_report-1.0.8/sql_field_report/sql_field_report.py
--rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-1.0.8/sql_field_report/utils/__init__.py
--rw-r--r--   0        0        0    11624 2023-06-22 08:37:32.888724 sql_field_report-1.0.8/sql_field_report/utils/analysis.py
--rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-1.0.8/sql_field_report/utils/databases.py
--rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-1.0.8/sql_field_report/utils/excel.py
--rw-r--r--   0        0        0      796 2023-06-22 08:38:51.367899 sql_field_report-1.0.8/sql_field_report/utils/file_utils.py
--rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 sql_field_report-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      826 2023-06-22 09:48:09.743291 sql_field_report-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      713 2023-04-27 15:17:01.445770 sql_field_report-1.0.9/README.md
+-rw-r--r--   0        0        0      123 2023-06-22 08:39:56.322632 sql_field_report-1.0.9/sql_field_report/__init__.py
+-rw-r--r--   0        0        0       72 2023-06-10 10:58:29.997444 sql_field_report-1.0.9/sql_field_report/__main__.py
+-rw-r--r--   0        0        0     4909 2023-06-22 09:48:03.671100 sql_field_report-1.0.9/sql_field_report/sql_field_report.py
+-rw-r--r--   0        0        0        0 2023-06-10 10:52:55.642003 sql_field_report-1.0.9/sql_field_report/utils/__init__.py
+-rw-r--r--   0        0        0    11624 2023-06-22 08:37:32.888724 sql_field_report-1.0.9/sql_field_report/utils/analysis.py
+-rw-r--r--   0        0        0     2678 2023-06-12 09:54:25.338912 sql_field_report-1.0.9/sql_field_report/utils/databases.py
+-rw-r--r--   0        0        0     3152 2023-06-12 09:33:04.069777 sql_field_report-1.0.9/sql_field_report/utils/excel.py
+-rw-r--r--   0        0        0      796 2023-06-22 08:38:51.367899 sql_field_report-1.0.9/sql_field_report/utils/file_utils.py
+-rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 sql_field_report-1.0.9/PKG-INFO
```

### Comparing `sql_field_report-1.0.8/pyproject.toml` & `sql_field_report-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sql-field-report"
-version = "1.0.8"
+version = "1.0.9"
 description = ""
 authors = ["Will James <willj@dealcloud.com>"]
 readme = "README.md"
 packages = [{include = "sql_field_report"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `sql_field_report-1.0.8/README.md` & `sql_field_report-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.8/sql_field_report/sql_field_report.py` & `sql_field_report-1.0.9/sql_field_report/sql_field_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
     if not output_file_name.endswith(".xlsx"):
         output_file_name = "{}.xlsx".format(output_file_name.split(".")[0])
 
     with MSSQLConnection(server, port, user, password, database_name) as conn:
         objects = pd.read_sql(
             text(
-                "SELECT DISTINCT('[' + TABLE_SCHEMA + '].[' + TABLE_NAME + ']') [TABLE_NAME] FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_SCHEMA=[{}]".format(schema)
+                "SELECT DISTINCT('[' + TABLE_SCHEMA + '].[' + TABLE_NAME + ']') [TABLE_NAME] FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_SCHEMA='{}'".format(schema)
             ),
             conn,
         )["TABLE_NAME"].to_list()
         build_sql_field_report(output_file_name, objects, conn)
 
 
 @app.command()
```

### Comparing `sql_field_report-1.0.8/sql_field_report/utils/analysis.py` & `sql_field_report-1.0.9/sql_field_report/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.8/sql_field_report/utils/databases.py` & `sql_field_report-1.0.9/sql_field_report/utils/databases.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.8/sql_field_report/utils/excel.py` & `sql_field_report-1.0.9/sql_field_report/utils/excel.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.8/sql_field_report/utils/file_utils.py` & `sql_field_report-1.0.9/sql_field_report/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `sql_field_report-1.0.8/PKG-INFO` & `sql_field_report-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-field-report
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Author: Will James
 Author-email: willj@dealcloud.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

