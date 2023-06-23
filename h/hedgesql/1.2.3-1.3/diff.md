# Comparing `tmp/hedgesql-1.2.3.tar.gz` & `tmp/hedgesql-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hedgesql-1.2.3.tar", last modified: Mon Jun 19 16:30:02 2023, max compression
+gzip compressed data, was "hedgesql-1.3.tar", last modified: Fri Jun 23 19:28:46 2023, max compression
```

## Comparing `hedgesql-1.2.3.tar` & `hedgesql-1.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:30:02.884616 hedgesql-1.2.3/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.2.3/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-06-19 16:30:02.884616 hedgesql-1.2.3/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     1927 2023-06-18 18:28:20.000000 hedgesql-1.2.3/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:30:02.880616 hedgesql-1.2.3/hedgesql/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.2.3/hedgesql/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 hedgesql-1.2.3/hedgesql/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8921 2023-06-19 16:29:13.000000 hedgesql-1.2.3/hedgesql/hedge_sql.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-19 16:30:02.884616 hedgesql-1.2.3/hedgesql.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-06-19 16:30:02.000000 hedgesql-1.2.3/hedgesql.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      250 2023-06-19 16:30:02.000000 hedgesql-1.2.3/hedgesql.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-19 16:30:02.000000 hedgesql-1.2.3/hedgesql.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-19 16:30:02.000000 hedgesql-1.2.3/hedgesql.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-06-19 16:30:02.000000 hedgesql-1.2.3/hedgesql.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-19 16:30:02.884616 hedgesql-1.2.3/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      761 2023-06-19 16:29:13.000000 hedgesql-1.2.3/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-23 19:28:46.659167 hedgesql-1.3/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.3/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      614 2023-06-23 19:28:46.659167 hedgesql-1.3/PKG-INFO
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-23 19:28:46.659167 hedgesql-1.3/hedgesql/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.3/hedgesql/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     5214 2023-06-23 17:25:05.000000 hedgesql-1.3/hedgesql/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     9584 2023-06-23 19:28:05.000000 hedgesql-1.3/hedgesql/hedge_sql.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-23 19:28:46.659167 hedgesql-1.3/hedgesql.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      614 2023-06-23 19:28:46.000000 hedgesql-1.3/hedgesql.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      240 2023-06-23 19:28:46.000000 hedgesql-1.3/hedgesql.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-23 19:28:46.000000 hedgesql-1.3/hedgesql.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-23 19:28:46.000000 hedgesql-1.3/hedgesql.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-06-23 19:28:46.000000 hedgesql-1.3/hedgesql.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-23 19:28:46.659167 hedgesql-1.3/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      759 2023-06-23 19:28:19.000000 hedgesql-1.3/setup.py
```

### Comparing `hedgesql-1.2.3/LICENSE` & `hedgesql-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hedgesql-1.2.3/PKG-INFO` & `hedgesql-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.2.3
+Version: 1.3
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
 Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hedgesql-1.2.3/hedgesql/hedge_sql.py` & `hedgesql-1.3/hedgesql/hedge_sql.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def __enter__(self) -> 'Sqlite':
         self.open_conn()
         return self
 
     def create_table(self,
                      table_name: str,
-                     columns: Dict[str, Union[DataTypes, str]]) -> None:
+                     columns: Dict[str, Union[DataTypes.ColumnTypes, str]]) -> None:
         columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
         query = f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})"
         self.__cursor.execute(query)
         self.__conn.commit()
 
     def insert_data(self,
                     table_name: str,
@@ -38,17 +38,16 @@
         self.__cursor.execute(query, values)
         self.__conn.commit()
 
     def select_data(self,
                     table_name: str,
                     columns: Union[List[str], str] = '*',
                     where: Optional[List[Dict[str, Union[str, int, float]]]] = None,
-                    order_by: Optional[str] = None,
-                    limit: Optional[int] = None,
-                    offset: Optional[int] = None,
+                    order_by: Optional[Union[DataTypes.ORDER_BY, str]] = None,
+                    limit: Optional[Union[DataTypes.LIMIT.OFFSET, int]] = None,
                     fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
         if columns != '*':
             columns = ', '.join(columns)
         if where:
             where_clause = ' WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
             values = tuple(value for d in where for value in d.values())
         else:
@@ -58,43 +57,59 @@
             order_by_clause = f"ORDER BY {order_by}"
         else:
             order_by_clause = ''
         if limit:
             limit_clause = f"LIMIT {limit}"
         else:
             limit_clause = ""
-        if offset:
-            offset_clause = f'OFFSET {offset}'
-        else:
-            offset_clause = ""
-        query = f"SELECT {columns} FROM {table_name} {where_clause} {order_by_clause} {limit_clause} {offset_clause}"
+        query = f"SELECT {columns} FROM {table_name} {where_clause} {order_by_clause} {limit_clause}"
         self.__cursor.execute(query, values)
         if fetch == DataTypes.Fetch.FETCHONE:
             result = self.__cursor.fetchone()
         elif fetch == DataTypes.Fetch.FETCHALL:
             result = self.__cursor.fetchall()
         return result
 
     def update_data(self,
                     table_name: str,
                     set_data: Dict[str, Union[str, int, float]],
-                    where: Optional[List[Dict[str, Union[str, int, float]]]] = None,
-                    sign: Optional[str] = None) -> None:
-        values = tuple(set_data.values())
-        if sign:
-            set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
-        else:
-            set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
+                    where: Optional[List[Dict[str, Union[str, int, float]]]] = None) -> None:
+        values = []
+        set_clause_parts = []
+
+        for col, value in set_data.items():
+            if isinstance(value, str) and value.startswith('+'):
+                col_name = col
+                col_value = value[1:]
+                set_clause_parts.append(f"{col_name}={col_name}+?")
+                values.append(col_value)
+            else:
+                set_clause_parts.append(f"{col}=?")
+                values.append(value)
+
+        set_clause = ', '.join(set_clause_parts)
+
         if where:
-            where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
-            values = (values + tuple(value for d in where for value in d.values()))
+            where_clause_parts = []
+
+            for condition in where:
+                where_condition_parts = []
+
+                for col, value in condition.items():
+                    where_condition_parts.append(f"{col}=?")
+                    values.append(value)
+
+                where_clause_parts.append(" AND ".join(where_condition_parts))
+
+            where_clause = "WHERE " + " OR ".join(where_clause_parts)
         else:
             where_clause = ''
+
         query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
-        self.__cursor.execute(query, values)
+        self.__cursor.execute(query, tuple(values))
         self.__conn.commit()
 
     def delete_data(self,
                     table_name: str,
                     where: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
         if where:
             where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
@@ -127,15 +142,15 @@
 
     async def __aenter__(self) -> 'AioSqlite':
         await self.open_conn()
         return self
 
     async def create_table(self,
                            table_name: str,
-                           columns: Dict[str, Union[DataTypes, str]]) -> None:
+                           columns: Dict[str, Union[DataTypes.ColumnTypes, str]]) -> None:
         columns_def = ', '.join([f'{col_name} {col_type}' for col_name, col_type in columns.items()])
         query = f"CREATE TABLE IF NOT EXISTS {table_name} ({columns_def})"
         await self.__cursor.execute(query)
         await self.__conn.commit()
 
     async def insert_data(self,
                           table_name: str,
@@ -147,17 +162,16 @@
         await self.__cursor.execute(query, values)
         await self.__conn.commit()
 
     async def select_data(self,
                           table_name: str,
                           columns: Union[List[str], str] = '*',
                           where: Optional[List[Dict[str, Union[str, int, float]]]] = None,
-                          order_by: Optional[str] = None,
-                          limit: Optional[int] = None,
-                          offset: Optional[int] = None,
+                          order_by: Optional[Union[DataTypes.ORDER_BY, str]] = None,
+                          limit: Optional[Union[DataTypes.LIMIT.OFFSET, int]] = None,
                           fetch: DataTypes.Fetch = DataTypes.Fetch.FETCHONE) -> Union[Tuple, List[Tuple]]:
         if columns != '*':
             columns = ', '.join(columns)
         if where:
             where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
             values = tuple(value for d in where for value in d.values())
         else:
@@ -167,43 +181,59 @@
             order_by_clause = f"ORDER BY {order_by}"
         else:
             order_by_clause = ''
         if limit:
             limit_clause = f"LIMIT {limit}"
         else:
             limit_clause = ""
-        if offset:
-            offset_clause = f'OFFSET {offset}'
-        else:
-            offset_clause = ""
-        query = f"SELECT {columns} FROM {table_name} {where_clause} {order_by_clause} {limit_clause} {offset_clause}"
+        query = f"SELECT {columns} FROM {table_name} {where_clause} {order_by_clause} {limit_clause}"
         await self.__cursor.execute(query, values)
         if fetch == DataTypes.Fetch.FETCHONE:
             result = await self.__cursor.fetchone()
         elif fetch == DataTypes.Fetch.FETCHALL:
             result = await self.__cursor.fetchall()
         return result
 
     async def update_data(self,
                           table_name: str,
                           set_data: Dict[str, Union[str, int, float]],
-                          where: Optional[List[Dict[str, Union[str, int, float]]]] = None,
-                          sign: Optional[str] = None) -> None:
-        values = tuple(set_data.values())
-        if sign:
-            set_clause = ', '.join([f'{col}={col}{sign}?' for col in set_data.keys()])
-        else:
-            set_clause = ', '.join([f'{col}=?' for col in set_data.keys()])
+                          where: Optional[List[Dict[str, Union[str, int, float]]]] = None) -> None:
+        values = []
+        set_clause_parts = []
+
+        for col, value in set_data.items():
+            if isinstance(value, str) and value.startswith('+'):
+                col_name = col
+                col_value = value[1:]
+                set_clause_parts.append(f"{col_name}={col_name}+?")
+                values.append(col_value)
+            else:
+                set_clause_parts.append(f"{col}=?")
+                values.append(value)
+
+        set_clause = ', '.join(set_clause_parts)
+
         if where:
-            where_clause = 'WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
-            values = (values + tuple(value for d in where for value in d.values()))
+            where_clause_parts = []
+
+            for condition in where:
+                where_condition_parts = []
+
+                for col, value in condition.items():
+                    where_condition_parts.append(f"{col}=?")
+                    values.append(value)
+
+                where_clause_parts.append(" AND ".join(where_condition_parts))
+
+            where_clause = "WHERE " + " OR ".join(where_clause_parts)
         else:
             where_clause = ''
+
         query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
-        await self.__cursor.execute(query, values)
+        await self.__cursor.execute(query, tuple(values))
         await self.__conn.commit()
 
     async def delete_data(self,
                           table_name: str,
                           where: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
         if where:
             where_clause = 'WHERE' + ' AND '.join([f'{col}=?' for col in where.keys()])
@@ -212,11 +242,11 @@
             where_clause = ''
             values = ()
         query = f"DELETE FROM {table_name} {where_clause}"
         await self.__cursor.execute(query, values)
         await self.__conn.commit()
 
     async def close_conn(self) -> None:
-       await self.__conn.close()
+        await self.__conn.close()
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.close_conn()
```

### Comparing `hedgesql-1.2.3/hedgesql.egg-info/PKG-INFO` & `hedgesql-1.3/hedgesql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.2.3
+Version: 1.3
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
 Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hedgesql-1.2.3/setup.py` & `hedgesql-1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='hedgesql',
-    version='1.2.3',
+    version='1.3',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/I-HedgeDev/litesqlite',
     author='HedgeDev',
     author_email='hedge_dev@mail.ru',
     packages=['hedgesql'],
     install_requires=[
         'aiosqlite'
```

