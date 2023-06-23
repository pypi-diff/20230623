# Comparing `tmp/py_experimenter-1.2.1.tar.gz` & `tmp/py_experimenter-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_experimenter-1.2.1.tar", max compression
+gzip compressed data, was "py_experimenter-1.3.0.tar", max compression
```

## Comparing `py_experimenter-1.2.1.tar` & `py_experimenter-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1183 2023-02-16 12:30:15.046670 py_experimenter-1.2.1/LICENSE
--rw-r--r--   0        0        0     3461 2023-04-21 15:31:15.552785 py_experimenter-1.2.1/README.md
--rw-r--r--   0        0        0        1 2023-02-16 12:30:15.050204 py_experimenter-1.2.1/py_experimenter/__init__.py
--rw-r--r--   0        0        0    14295 2023-04-21 15:54:05.717303 py_experimenter-1.2.1/py_experimenter/database_connector.py
--rw-r--r--   0        0        0     3216 2023-04-21 15:54:05.717692 py_experimenter-1.2.1/py_experimenter/database_connector_lite.py
--rw-r--r--   0        0        0     5222 2023-04-21 15:54:05.718090 py_experimenter-1.2.1/py_experimenter/database_connector_mysql.py
--rw-r--r--   0        0        0      907 2023-04-04 09:33:58.357634 py_experimenter-1.2.1/py_experimenter/exceptions.py
--rw-r--r--   0        0        0      156 2023-02-16 12:30:15.050509 py_experimenter-1.2.1/py_experimenter/experiment_status.py
--rw-r--r--   0        0        0    22555 2023-04-04 09:33:58.358029 py_experimenter-1.2.1/py_experimenter/experimenter.py
--rw-r--r--   0        0        0     4476 2023-04-04 09:33:58.358327 py_experimenter-1.2.1/py_experimenter/result_processor.py
--rw-r--r--   0        0        0     8454 2023-04-04 09:33:58.358636 py_experimenter-1.2.1/py_experimenter/utils.py
--rw-r--r--   0        0        0     1671 2023-04-21 15:54:05.718291 py_experimenter-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     4430 1970-01-01 00:00:00.000000 py_experimenter-1.2.1/setup.py
--rw-r--r--   0        0        0     4849 1970-01-01 00:00:00.000000 py_experimenter-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1183 2023-02-16 12:30:15.046670 py_experimenter-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3461 2023-06-23 13:03:20.172030 py_experimenter-1.3.0/README.md
+-rw-r--r--   0        0        0        1 2023-02-16 12:30:15.050204 py_experimenter-1.3.0/py_experimenter/__init__.py
+-rw-r--r--   0        0        0    15392 2023-06-23 18:02:36.562762 py_experimenter-1.3.0/py_experimenter/database_connector.py
+-rw-r--r--   0        0        0     3226 2023-06-23 18:02:36.562916 py_experimenter-1.3.0/py_experimenter/database_connector_lite.py
+-rw-r--r--   0        0        0     5099 2023-06-23 18:02:36.563473 py_experimenter-1.3.0/py_experimenter/database_connector_mysql.py
+-rw-r--r--   0        0        0      907 2023-04-04 09:33:58.357634 py_experimenter-1.3.0/py_experimenter/exceptions.py
+-rw-r--r--   0        0        0      156 2023-02-16 12:30:15.050509 py_experimenter-1.3.0/py_experimenter/experiment_status.py
+-rw-r--r--   0        0        0    24341 2023-06-23 18:02:36.563701 py_experimenter-1.3.0/py_experimenter/experimenter.py
+-rw-r--r--   0        0        0     5274 2023-06-23 18:02:36.564378 py_experimenter-1.3.0/py_experimenter/result_processor.py
+-rw-r--r--   0        0        0    11246 2023-06-23 18:02:36.564714 py_experimenter-1.3.0/py_experimenter/utils.py
+-rw-r--r--   0        0        0     1680 2023-06-23 20:03:32.020159 py_experimenter-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4446 1970-01-01 00:00:00.000000 py_experimenter-1.3.0/setup.py
+-rw-r--r--   0        0        0     4879 1970-01-01 00:00:00.000000 py_experimenter-1.3.0/PKG-INFO
```

### Comparing `py_experimenter-1.2.1/LICENSE` & `py_experimenter-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_experimenter-1.2.1/README.md` & `py_experimenter-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `py_experimenter-1.2.1/py_experimenter/database_connector.py` & `py_experimenter-1.3.0/py_experimenter/database_connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import abc
+import itertools
 import logging
 from configparser import ConfigParser
 from typing import Dict, List, Optional, Tuple, Union
 
+import numpy as np
 import pandas as pd
 
 from py_experimenter import utils
 from py_experimenter.exceptions import (CreatingTableError, DatabaseConnectionError, EmptyFillDatabaseCallError, NoExperimentsLeftException,
                                         TableHasWrongStructureError)
 from py_experimenter.experiment_status import ExperimentStatus
 
 
 class DatabaseConnector(abc.ABC):
 
-    def __init__(self, config: ConfigParser):
+    def __init__(self, config: ConfigParser, use_codecarbon: bool, codecarbon_config: ConfigParser):
         self.config = config
+        self.codecarbon_config = codecarbon_config
         self.table_name = self.config.get('PY_EXPERIMENTER', 'table')
         self.database_name = self.config.get('PY_EXPERIMENTER', 'database')
 
         self.database_credentials = self._extract_credentials()
         self.timestamp_on_result_fields = utils.timestamps_for_result_fields(self.config)
 
+        self.use_codecarbon = use_codecarbon
         self._test_connection()
 
     @abc.abstractmethod
     def _extract_credentials(self):
         pass
 
     @abc.abstractmethod
@@ -43,17 +47,20 @@
 
     def commit(self, connection) -> None:
         try:
             connection.commit()
         except Exception as e:
             raise DatabaseConnectionError(f'error \n{e}\n raised when committing to database.')
 
-    def execute(self, cursor, sql_statement):
+    def execute(self, cursor, sql_statement, values=None) -> None:
         try:
-            cursor.execute(sql_statement)
+            if values is None:
+                cursor.execute(sql_statement)
+            else:
+                cursor.execute(sql_statement, values)
         except Exception as e:
             raise DatabaseConnectionError(f'error \n{e}\n raised when executing sql statement.')
 
     def cursor(self, connection):
         try:
             return connection.cursor()
         except Exception as e:
@@ -80,20 +87,24 @@
                 raise TableHasWrongStructureError("Keyfields or resultfields from the configuration do not match columns in the existing "
                                                   "table. Please change your configuration or delete the table in your database.")
         else:
             columns = self._compute_columns(keyfields, resultfields)
             self._create_table(cursor, columns, self.table_name)
 
             for logtable_name, logtable_columns in utils.extract_logtables(self.config, self.table_name).items():
-                self._create_table(cursor, logtable_columns, logtable_name, logtable=True)
+                self._create_table(cursor, logtable_columns, logtable_name, table_type='logtable')
+
+            if self.use_codecarbon:
+                codecarbon_columns = utils.extract_codecarbon_columns()
+                self._create_table(cursor, codecarbon_columns, f"{self.table_name}_codecarbon", table_type='codecarbon')
 
         self.close_connection(connection)
 
     @abc.abstractmethod
-    def _table_exists(self, cursor):
+    def _table_exists(self, cursor, table_name: str):
         pass
 
     @staticmethod
     def _compute_columns(keyfields, resultfields):
         return (keyfields +
                 [('creation_date', 'DATETIME'),
                     ('status', 'VARCHAR(255)'),
@@ -110,29 +121,33 @@
         amount_of_result_fields = len(utils.get_result_field_names(self.config))
 
         if self.timestamp_on_result_fields:
             amount_of_result_fields *= 2
 
         return columns[1:amount_of_keyfields + 1] + columns[-amount_of_result_fields - 2:-2]
 
-    def _create_table(self, cursor, columns: List[Tuple['str']], table_name: str, logtable: bool = False):
-        query = self._get_create_table_query(columns, table_name, logtable)
+    def _create_table(self, cursor, columns: List[Tuple['str']], table_name: str, table_type: str = 'standard'):
+        query = self._get_create_table_query(columns, table_name, table_type)
         try:
             self.execute(cursor, query)
         except Exception as err:
             raise CreatingTableError(f'Error when creating table: {err}')
 
-    def _get_create_table_query(self, columns: List[Tuple['str']], table_name: str, logtable: bool):
-        columns = ['%s %s DEFAULT NULL' % (self.escape_sql_chars(field)[0], datatype) for field, datatype in columns]
-        columns = ','.join(self.escape_sql_chars(*columns))
-        query = f"CREATE TABLE {self.escape_sql_chars(table_name)[0]} (ID INTEGER PRIMARY KEY {self.get_autoincrement()}"
-        if logtable:
+    def _get_create_table_query(self, columns: List[Tuple['str']], table_name: str, table_type: str = 'standard'):
+        columns = ['%s %s DEFAULT NULL' % (field, datatype) for field, datatype in columns]
+        columns = ','.join(columns)
+        query = f"CREATE TABLE {table_name} (ID INTEGER PRIMARY KEY {self.get_autoincrement()}"
+        if table_type == 'standard':
+            query += f", {columns}"
+        elif table_type == 'logtable':
             query += f", experiment_id INTEGER, timestamp DATETIME, {columns}, FOREIGN KEY (experiment_id) REFERENCES {self.table_name}(ID) ON DELETE CASCADE"
+        elif table_type == 'codecarbon':
+            query += f", experiment_id INTEGER, {columns}, FOREIGN KEY (experiment_id) REFERENCES {self.table_name}(ID) ON DELETE CASCADE"
         else:
-            query += f", {columns}"
+            raise ValueError(f"Unknown table type: {table_type}")
         return query + ');'
 
     @abc.abstractstaticmethod
     def get_autoincrement(self):
         pass
 
     @abc.abstractmethod
@@ -165,15 +180,15 @@
             values = list(combination.values())
             values.append(ExperimentStatus.CREATED.value)
             values.append(time)
             rows.append(values)
 
         if rows:
             logging.debug(f"Now adding {len(rows)} rows to database. {rows_skipped} rows were skipped.")
-            self._write_to_database(pd.DataFrame(rows, columns=column_names + ["status", "creation_date"]))
+            self._write_to_database(rows, column_names + ["status", "creation_date"])
             logging.info(f"{len(rows)} rows successfully added to database. {rows_skipped} rows were skipped.")
         else:
             logging.info(f"No rows to add. All the {len(combinations)} experiments already exist.")
 
     def _check_combination_in_existing_rows(self, combination, existing_rows, keyfield_names) -> bool:
         def _get_column_values():
             return [combination[keyfield_name] for keyfield_name in keyfield_names]
@@ -196,69 +211,52 @@
     def _execute_queries(self, connection, cursor) -> Tuple[int, List, List]:
         order_by = "id"
         time = utils.get_timestamp_representation()
 
         self.execute(cursor, f"SELECT id FROM {self.table_name} WHERE status = 'created' ORDER BY {order_by} LIMIT 1;")
         experiment_id = self.fetchall(cursor)[0][0]
         self.execute(
-            cursor, f"UPDATE {self.table_name} SET status = '{ExperimentStatus.RUNNING.value}', start_date = '{time}' WHERE id = {experiment_id};")
+            cursor, f"UPDATE {self.table_name} SET status = {self._prepared_statement_placeholder}, start_date = {self._prepared_statement_placeholder} WHERE id = {self._prepared_statement_placeholder};", (ExperimentStatus.RUNNING.value, time, experiment_id))
         keyfields = ','.join(utils.get_keyfield_names(self.config))
         self.execute(cursor, f"SELECT {keyfields} FROM {self.table_name} WHERE id = {experiment_id};")
         values = self.fetchall(cursor)
         self.commit(connection)
         description = cursor.description
         return experiment_id, description, values
 
     @abc.abstractmethod
     def _pull_open_experiment(self) -> Tuple[int, List, List]:
         pass
 
-    def _write_to_database(self, df) -> None:
-        keys = ", ".join(df.columns)
-        values = df.apply(lambda row: "('" + self.__class__._write_to_database_separator.join([str(value) for value in row]) + "')", axis=1)
-
-        stmt = f"INSERT INTO {self.table_name} ({keys}) VALUES {', '.join(values)}"
+    def _write_to_database(self, values: List, columns=List[str]) -> None:
+        values_prepared = ','.join([f"({', '.join([self._prepared_statement_placeholder] * len(columns))})"] * len(values))
+        values = list(map(lambda x: str(x) if x is not None else x, itertools.chain(*values)))
+        stmt = f"INSERT INTO {self.table_name} ({','.join(columns)}) VALUES {values_prepared}"
 
         connection = self.connect()
         cursor = self.cursor(connection)
-        self.execute(cursor, stmt)
+        self.execute(cursor, stmt, values)
         self.commit(connection)
         self.close_connection(connection)
 
+    def prepare_write_query(self, table_name: str, keys) -> str:
+        return f"INSERT INTO {table_name} ({', '.join(keys)}) VALUES ({','.join([self._prepared_statement_placeholder] * len(keys))})"
+
     def update_database(self, table_name: str, values: Dict[str, Union[str, int, object]], condition: str):
         connection = self.connect()
         cursor = self.cursor(connection)
-        cursor.execute(self._prepare_update_query(table_name, values.keys(), condition), list(values.values()))
+        self.execute(cursor, self._prepare_update_query(table_name, values.keys(), condition),
+                     list(values.values()))
         self.commit(connection)
         self.close_connection(connection)
 
     def _prepare_update_query(self, table_name: str, values: Dict[str, Union[str, int, object]],  condition: str) -> str:
         return (f"UPDATE {table_name} SET {', '.join(f'{key} = {self._prepared_statement_placeholder}' for key in values)}"
                 f" WHERE {condition}")
 
-    def not_executed_yet(self, where) -> bool:
-        not_executed = False
-
-        try:
-            connection = self.connect()
-            cursor = self.cursor(connection)
-
-            stmt = "SELECT status FROM %s WHERE %s" % (self.table_name, where)
-
-            self.execute(cursor, stmt)
-            for result in cursor:
-                if result[0] == 'created':
-                    not_executed = True
-
-        except Exception as err:
-            logging.error(err)
-        else:
-            connection.close()
-            return not_executed
-
     def reset_experiments(self, *states: str) -> None:
         def get_dict_for_keyfields_and_rows(keyfields: List[str], rows: List[List[str]]) -> List[dict]:
             return [{key: value for key, value in zip(keyfields, row)} for row in rows]
 
         for state in states:
             keyfields, rows = self._pop_experiments_with_status(state)
             rows = get_dict_for_keyfields_and_rows(keyfields, rows)
@@ -307,28 +305,38 @@
     def get_structure_from_table(self, cursor):
         pass
 
     def execute_queries(self, queries: List[str]):
         connection = self.connect()
         cursor = self.cursor(connection)
         for query in queries:
-            self.execute(cursor, query)
+            self.execute(cursor, query[0], tuple(query[1]))
         self.commit(connection)
         self.close_connection(connection)
 
     def delete_table(self) -> None:
         connection = self.connect()
         cursor = self.cursor(connection)
         for logtable_name in utils.extract_logtables(self.config, self.table_name).keys():
             self.execute(cursor, f'DROP TABLE IF EXISTS {logtable_name}')
+        if self.use_codecarbon:
+            self.execute(cursor, f'DROP TABLE IF EXISTS {self.table_name}_codecarbon')
+
         self.execute(cursor, f'DROP TABLE IF EXISTS {self.table_name}')
         self.commit(connection)
 
     def get_logtable(self, logtable_name: str) -> pd.DataFrame:
         return self.get_table(f'{self.table_name}__{logtable_name}')
 
+    def get_codecarbon_table(self) -> pd.DataFrame:
+        return self.get_table(f'{self.table_name}_codecarbon')
+
     def get_table(self, table_name: Optional[str] = None) -> pd.DataFrame:
         connection = self.connect()
         query = f"SELECT * FROM {self.table_name}" if table_name is None else f"SELECT * FROM {table_name}"
-        df = pd.read_sql(query, connection)
+        #suppress warning for pandas
+        import warnings
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=UserWarning)
+            df = pd.read_sql(query, connection)
         self.close_connection(connection)
         return df
```

### Comparing `py_experimenter-1.2.1/py_experimenter/database_connector_lite.py` & `py_experimenter-1.3.0/py_experimenter/database_connector_lite.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,20 +65,20 @@
     def _table_has_correct_structure(self, cursor, typed_fields) -> List[str]:
         self.execute(cursor, f"PRAGMA table_info({self.table_name})")
 
         columns = self._exclude_fixed_columns([k[1] for k in self.fetchall(cursor)])
         config_columns = [k[0] for k in typed_fields]
         return set(columns) == set(config_columns)
 
-    def _get_existing_rows(self, column_names):
+    def _get_existing_rows(self, column_names: List[str]):
         def _remove_string_markers(row):
             return row.replace("'", "")
         connection = self.connect()
         cursor = self.cursor(connection)
-        self.execute(cursor, f"SELECT {', '.join(column_names)} FROM {self.table_name}")
+        self.execute(cursor, f"SELECT {','.join(column_names)} FROM {self.table_name}")
         existing_rows = list(map(np.array2string, np.array(self.fetchall(cursor))))
         existing_rows = [' '.join(_remove_string_markers(row).split()) for row in existing_rows]
         self.close_connection(connection)
         return existing_rows
 
     def get_structure_from_table(self, cursor):
         def _get_column_names_from_entries(entries):
```

### Comparing `py_experimenter-1.2.1/py_experimenter/database_connector_mysql.py` & `py_experimenter-1.3.0/py_experimenter/database_connector_mysql.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import logging
 from configparser import ConfigParser
 from typing import List, Tuple
 
 import numpy as np
-from mysql.connector import Error, connect
+from pymysql import Error, connect
 
 from py_experimenter.database_connector import DatabaseConnector
-from py_experimenter.exceptions import CreatingTableError, DatabaseConnectionError, DatabaseCreationError
+from py_experimenter.exceptions import DatabaseConnectionError, DatabaseCreationError
 from py_experimenter.utils import load_config
 
 
 class DatabaseConnectorMYSQL(DatabaseConnector):
-    _write_to_database_separator = "', '"
     _prepared_statement_placeholder = '%s'
 
-    def __init__(self, experiment_configuration_file_path: ConfigParser, database_credential_file_path):
+    def __init__(self, experiment_configuration: ConfigParser, use_codecarbon:bool, codecarbon_config:ConfigParser, database_credential_file_path:str):
         database_credentials = load_config(database_credential_file_path)
         self.host = database_credentials.get('CREDENTIALS', 'host')
         self.user = database_credentials.get('CREDENTIALS', 'user')
         self.password = database_credentials.get('CREDENTIALS', 'password')
 
-        super().__init__(experiment_configuration_file_path)
+        super().__init__(experiment_configuration, use_codecarbon, codecarbon_config)
 
         self._create_database_if_not_existing()
 
     def _test_connection(self):
         modified_credentials = self.database_credentials.copy()
         del modified_credentials['database']
         try:
@@ -59,65 +58,58 @@
             if credentials is None:
                 credentials = self.database_credentials
             return connect(**credentials)
         except Error as err:
             raise DatabaseConnectionError(err)
 
     def _start_transaction(self, connection, readonly=False):
-        connection.start_transaction(readonly=readonly)
+        if not readonly:
+            connection.begin()
 
-    def _table_exists(self, cursor):
-        self.execute(cursor, f"SHOW TABLES LIKE '{self.table_name}'")
+    def _table_exists(self, cursor, table_name:str = None) -> bool:
+        table_name = table_name if table_name is not None else self.table_name
+        self.execute(cursor, f"SHOW TABLES LIKE '{table_name}'")
         return self.fetchall(cursor)
 
     @staticmethod
     def get_autoincrement():
         return "AUTO_INCREMENT"
 
     def _table_has_correct_structure(self, cursor, typed_fields):
         self.execute(cursor,
-                     f"SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME = '{self.table_name}' AND TABLE_SCHEMA = '{self.database_name}'")
+                     f"SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME = {self._prepared_statement_placeholder} AND TABLE_SCHEMA = {self._prepared_statement_placeholder}",
+                     (self.table_name, self.database_name))
 
         columns = self._exclude_fixed_columns([k[0] for k in self.fetchall(cursor)])
         config_columns = [k[0] for k in typed_fields]
-        return set(columns) == set(config_columns)
+        return set(columns) == set(config_columns) 
 
     def _pull_open_experiment(self) -> Tuple[int, List, List]:
         try:
             connection = self.connect()
             cursor = self.cursor(connection)
             self._start_transaction(connection, readonly=False)
             experiment_id, description, values = self._execute_queries(connection, cursor)
         except Exception as err:
             connection.rollback()
             raise err
         self.close_connection(connection)
 
         return experiment_id, description, values
-
-    @staticmethod
-    def escape_sql_chars(*args):
-        escaped_args = []
-        for arg in args:
-            if isinstance(arg, str):
-                escaped_args.append(arg.replace("'", "''").replace('"', '""').replace('`', '``'))
-            else:
-                escaped_args.append(arg)
-        return escaped_args
     
     def _get_existing_rows(self, column_names):
         def _remove_double_whitespaces(existing_rows):
             return [' '.join(row.split()) for row in existing_rows]
 
         def _remove_string_markers(existing_rows):
             return [row.replace("'", "") for row in existing_rows]
 
         connection = self.connect()
         cursor = self.cursor(connection)
-        self.execute(cursor, f"SELECT {', '.join(column_names)} FROM {self.table_name}")
+        self.execute(cursor, f"SELECT {','.join(column_names)} FROM {self.table_name}")
         existing_rows = list(map(np.array2string, np.array(self.fetchall(cursor))))
         existing_rows = _remove_string_markers(existing_rows)
         existing_rows = _remove_double_whitespaces(existing_rows)
         self.close_connection(connection)
         return existing_rows
 
     def get_structure_from_table(self, cursor):
```

### Comparing `py_experimenter-1.2.1/py_experimenter/exceptions.py` & `py_experimenter-1.3.0/py_experimenter/exceptions.py`

 * *Files identical despite different names*

### Comparing `py_experimenter-1.2.1/py_experimenter/experimenter.py` & `py_experimenter-1.3.0/py_experimenter/experimenter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import configparser
 import logging
 import os
 import socket
 import traceback
+from configparser import ConfigParser
 from typing import Callable, Dict, List, Tuple
 
 import pandas as pd
+from codecarbon import EmissionsTracker, OfflineEmissionsTracker
 from joblib import Parallel, delayed
 
 from py_experimenter import utils
 from py_experimenter.database_connector_lite import DatabaseConnectorLITE
 from py_experimenter.database_connector_mysql import DatabaseConnectorMYSQL
 from py_experimenter.exceptions import InvalidConfigError, InvalidValuesInConfiguration, NoExperimentsLeftException
 from py_experimenter.experiment_status import ExperimentStatus
@@ -22,14 +23,15 @@
     """
 
     def __init__(self,
                  experiment_configuration_file_path: str = os.path.join('config', 'experiment_configuration.cfg'),
                  database_credential_file_path: str = os.path.join('config', 'database_credentials.cfg'),
                  table_name: str = None,
                  database_name: str = None,
+                 use_codecarbon: bool = True,
                  name='PyExperimenter'):
         """
         Initializes the PyExperimenter with the given information.
 
         :param experiment_configuration_file_path: The path to the experiment configuration file. Defaults to
             'config/experiment_configuration.cfg'.
         :type experiment_configuration_file_path: str, optional
@@ -40,38 +42,50 @@
             `experiment_configuration_file_path`. If None, the table table name is taken from the experiment
             configuration file. Defaults to None.
         :type table_name: str, optional
         :param database_name: The name of the database, if given it will overwrite the database_name given in the
             `experiment_configuration_file_path`. If None, the database name is taken from the experiment configuration
             file. Defaults to None.
         :type database_name: str, optional
+        :param use_codecarbon: If True, the carbon emissions are tracked and stored in the database. Defaults to True.
+        :type use_codecarbon: bool, optional
         :param name: The name of the PyExperimenter, which will be logged in the according column in the database table.
             Defaults to 'PyExperimenter'.
         :type name: str, optional
         :raises InvalidConfigError: If either the experiment or database configuration are missing mandatory information.
         :raises ValueError: If an unsupported or unknown database connection provider is given.
         """
         self.config = utils.load_config(experiment_configuration_file_path)
+
+        self.use_codecarbon = use_codecarbon
+        self.config, self.codecarbon_config = utils.extract_codecarbon_config(self.config)
+        if self.codecarbon_config.has_option('codecarbon', 'offline_mode'):
+            self.codecarbon_offline_mode = self.codecarbon_config['codecarbon']['offline_mode'] == 'True'
+        else:
+            self.codecarbon_offline_mode = False
+            self.codecarbon_config.set('codecarbon', 'offline_mode', 'False')
+        utils.write_codecarbon_config(self.codecarbon_config)
+
         self.database_credential_file_path = database_credential_file_path
         if not PyExperimenter._is_valid_configuration(self.config, database_credential_file_path):
             raise InvalidConfigError('Invalid configuration')
 
         if table_name is not None:
             self.config.set('PY_EXPERIMENTER', 'table', table_name)
         if database_name is not None:
             self.config.set('PY_EXPERIMENTER', 'database', database_name)
         self.name = name
 
         self.experiment_configuration_file_path = experiment_configuration_file_path
         self.timestamp_on_result_fields = utils.timestamps_for_result_fields(self.config)
 
         if self.config['PY_EXPERIMENTER']['provider'] == 'sqlite':
-            self.dbconnector = DatabaseConnectorLITE(self.config)
+            self.dbconnector = DatabaseConnectorLITE(self.config, self.use_codecarbon, self.codecarbon_config)
         elif self.config['PY_EXPERIMENTER']['provider'] == 'mysql':
-            self.dbconnector = DatabaseConnectorMYSQL(self.config, database_credential_file_path)
+            self.dbconnector = DatabaseConnectorMYSQL(self.config, self.use_codecarbon, self.codecarbon_config, database_credential_file_path)
         else:
             raise ValueError('The provider indicated in the config file is not supported')
 
         logging.info('Initialized and connected to database')
 
     def set_config_value(self, section_name: str, key: str, value: str) -> None:
         """
@@ -134,49 +148,49 @@
         :return: True if the given `key` is contained in the experiment configuration within the section called
             `section_name`. False otherwise.
         :rtype: bool
         """
         return self.config.has_option(section_name, key)
 
     @ staticmethod
-    def _is_valid_configuration(_config: configparser, database_credential_file_path: str = None) -> bool:
+    def _is_valid_configuration(config: ConfigParser, database_credential_file_path: str = None) -> bool:
         """
         Checks whether the given experiment configuration is valid, i.e., it contains all necessary fields, the database provider
         is either mysql or sqlite, and in case of a mysql database provider, that the database credentials are available.
 
-        :param _config: The experiment configuration.
-        :type _config: configparser
+        :param config: The experiment configuration.
+        :type config: ConfigParser
         :param database_credential_file_path: The path to the database configuration file, i.e., the file defining
             the host, user and password. Defaults to None.
         :type database_credential_file_path: str, optional
         :return: True if the experiment configuration contains all necessary fields.
         :rtype: bool
         """
-        if not _config.has_section('PY_EXPERIMENTER'):
+        if not config.has_section('PY_EXPERIMENTER'):
             return False
 
-        if set(_config.keys()) > {'PY_EXPERIMENTER', 'CUSTOM', 'DEFAULT'}:
+        if set(config.keys()) > {'PY_EXPERIMENTER', 'CUSTOM', 'DEFAULT'}:
             return False
 
-        if not {'provider', 'database', 'table'}.issubset(set(_config.options('PY_EXPERIMENTER'))):
+        if not {'provider', 'database', 'table'}.issubset(set(config.options('PY_EXPERIMENTER'))):
             logging.error('Error in config file: DATABASE section must contain provider, database, and table')
             return False
 
-        if _config['PY_EXPERIMENTER']['provider'] not in ['sqlite', 'mysql']:
+        if config['PY_EXPERIMENTER']['provider'] not in ['sqlite', 'mysql']:
             logging.error('Error in config file: DATABASE provider must be either sqlite or mysql')
             return False
 
-        if _config['PY_EXPERIMENTER']['provider'] == 'mysql':
+        if config['PY_EXPERIMENTER']['provider'] == 'mysql':
             credentials = utils.load_config(database_credential_file_path)
             if not {'host', 'user', 'password'}.issubset(set(credentials.options('CREDENTIALS'))):
                 logging.error(
-                    f'Error in config file: DATABASE section must contain host, user, and password since provider is {_config["DATABASE"]["provider"]}')
+                    f'Error in config file: DATABASE section must contain host, user, and password since provider is {config["DATABASE"]["provider"]}')
                 return False
 
-        if not {'keyfields', 'resultfields'}.issubset(set(_config.options('PY_EXPERIMENTER'))):
+        if not {'keyfields', 'resultfields'}.issubset(set(config.options('PY_EXPERIMENTER'))):
             return False
         return True
 
     def fill_table_from_combination(self, fixed_parameter_combinations: List[dict] = None, parameters: dict = None) -> None:
         """
         Adds rows to the database table based on the given information.
 
@@ -298,15 +312,16 @@
         except ValueError:
             InvalidValuesInConfiguration('n_jobs must be an integer')
 
         with Parallel(n_jobs=n_jobs) as parallel:
             if max_experiments == -1:
                 parallel(delayed(self._worker)(experiment_function) for _ in range(n_jobs))
             else:
-                parallel(delayed(self._execution_wrapper)(experiment_function) for _ in range(max_experiments))
+                parallel(delayed(self._execution_wrapper)(experiment_function)
+                         for _ in range(max_experiments))
         logging.info("All configured executions finished.")
 
     def _worker(self, experiment_function: Callable[[Dict, Dict, ResultProcessor], None]) -> None:
         """
         Worker that repeatedly pulls open experiments from the database table and executes them.
 
         :param experiment_function: The function that should be executed with the different parametrizations.
@@ -314,70 +329,73 @@
         """
         while True:
             try:
                 self._execution_wrapper(experiment_function)
             except NoExperimentsLeftException:
                 break
 
-    def _execution_worker(self, experiment_function: Callable[[Dict, Dict, ResultProcessor], None]) -> None:
-        """
-        Worker that repeatedly pulls open experiments from the database table and executes them.
-
-        :param experiment_function: The function that should be executed with the different parametrizations.
-        :type experiment_function: Callable[[Dict, Dict, ResultProcessor], None]
-        """
-        while True:
-            try:
-                self._execution_wrapper(experiment_function)
-            except NoExperimentsLeftException:
-                break
-
     def _execution_wrapper(self,
                            experiment_function: Callable[[dict, dict, ResultProcessor], None]) -> None:
         """
         Executes the given `experiment_function` on one open experiment. To that end, one of the open experiments is pulled
         from the database table. Then `experiment_function` is executed on the keyfield values of the pulled experiment. 
 
         Thereby, the status of the experiment is continuously updated. The experiment can have the following states:
 
         * `running` when the experiment has been pulled from the database table, which will be executed directly afterwards.
         * `error` if an exception was raised during the execution of the experiment.
         * `done` if the execution of the experiment has finished successfully.
 
-        Errors raised during the execution of `experiment_function` are logged to the `error` column in the database table. 
-        Note that only errors raised within `experiment_function` are logged in to the database table. Therefore all errors 
-        raised before or after the execution of `experiment_function` are logged according to the local logging configuration 
+        Errors raised during the execution of `experiment_function` are logged to the `error` column in the database table.
+        Note that only errors raised within `experiment_function` are logged in to the database table. Therefore all errors
+        raised before or after the execution of `experiment_function` are logged according to the local logging configuration
         and do not appear in the table.
 
         :param experiment_function: The function that should be executed with the different parametrizations.
         :type experiment_function: Callable[[dict, dict, ResultProcessor], None]
         :raises NoExperimentsLeftError: If there are no experiments left to be executed.
         :raises DatabaseConnectionError: If an error occurred during the connection to the database.
         """
         experiment_id, keyfield_values = self.dbconnector.get_experiment_configuration()
 
         result_field_names = utils.get_result_field_names(self.config)
         custom_fields = dict(self.config.items('CUSTOM')) if self.has_section('CUSTOM') else None
         table_name = self.get_config_value('PY_EXPERIMENTER', 'table')
 
-        result_processor = ResultProcessor(self.config, self.database_credential_file_path, table_name=table_name,
+        result_processor = ResultProcessor(self.config, self.use_codecarbon, self.codecarbon_config, self.database_credential_file_path, table_name=table_name,
                                            result_fields=result_field_names, experiment_id=experiment_id)
         result_processor._set_name(self.name)
         result_processor._set_machine(socket.gethostname())
 
+        if self.use_codecarbon:
+            if self.codecarbon_offline_mode:
+                if not self.codecarbon_config.has_option('codecarbon', 'country_iso_code'):
+                    raise InvalidConfigError(('CodeCarbon offline mode requires a `country_iso_code` in the config file.'
+                                              'For more information see `https://mlco2.github.io/codecarbon/index.html`.'))
+                tracker = OfflineEmissionsTracker()
+            else:
+                tracker = EmissionsTracker()
+
         try:
             logging.debug(f"Start of experiment_function on process {socket.gethostname()}")
+            if self.use_codecarbon:
+                tracker.start()
             experiment_function(keyfield_values, result_processor, custom_fields)
         except Exception:
             error_msg = traceback.format_exc()
             logging.error(error_msg)
             result_processor._write_error(error_msg)
             result_processor._change_status(ExperimentStatus.ERROR.value)
         else:
             result_processor._change_status(ExperimentStatus.DONE.value)
+        finally:
+            if self.use_codecarbon:
+                tracker.stop()
+                emission_data = tracker._prepare_emissions_data().values
+                result_processor._write_emissions(emission_data, self.codecarbon_offline_mode)
 
     def reset_experiments(self, *states: Tuple['str']) -> None:
         """
         Deletes the experiments from the database table that have the given `states`. Afterward, all deleted rows are added to the 
         table again. 
 
         :param states: The status of experiments that should be reset. Either `created`, `running`, `error`, `done`, or `all`.
@@ -400,17 +418,30 @@
         Returns the database table as `Pandas.DataFrame`. 
 
         :return: The database table as `Pandas.DataFrame`. 
         :rtype: pd.DataFrame
         """
         return self.dbconnector.get_table()
 
-    def get_logtable(self, table_name: str) -> pd.DataFrame:
+    def get_logtable(self, logtable_name: str) -> pd.DataFrame:
         """
         Returns the log table as `Pandas.DataFrame`. 
 
         :param table_name: The name of the log table.
         :type table_name: str
         :return: The log table as `Pandas.DataFrame`. 
         :rtype: pd.DataFrame
         """
-        return self.dbconnector.get_logtable(table_name)
+        return self.dbconnector.get_logtable(logtable_name)
+
+    def get_codecarbon_table(self) -> pd.DataFrame:
+        """
+        Returns the CodeCarbon table as `Pandas.DataFrame`. If CodeCarbon is not used in this experiment, an error is raised.
+
+        :raises ValueError: If CodeCarbon is not used in this experiment.
+        :return: Returns the CodeCarbon table as `Pandas.DataFrame`.
+        :rtype: pd.DataFrame
+        """
+        if self.use_codecarbon:
+            return self.dbconnector.get_codecarbon_table()
+        else:
+            raise ValueError('CodeCarbon is not used in this experiment.')
```

### Comparing `py_experimenter-1.2.1/py_experimenter/result_processor.py` & `py_experimenter-1.3.0/py_experimenter/result_processor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import logging
+from configparser import ConfigParser
 from copy import deepcopy
 from typing import Dict, List, Tuple
 
+from codecarbon.output import EmissionsData
+
 import py_experimenter.utils as utils
 from py_experimenter.database_connector import DatabaseConnector
 from py_experimenter.database_connector_lite import DatabaseConnectorLITE
 from py_experimenter.database_connector_mysql import DatabaseConnectorMYSQL
 from py_experimenter.exceptions import InvalidConfigError, InvalidResultFieldError
 
 result_logger = logging.getLogger('result_logger')
@@ -20,46 +23,57 @@
 
 class ResultProcessor:
     """
     Class for processing the results from an experiment. Use this class whenever you want to write results to the
     database.
     """
 
-    def __init__(self, _config: dict, credential_path, table_name: str, result_fields: List[str], experiment_id: int):
+    def __init__(self, config: ConfigParser, use_codecarbon: bool, codecarbon_config: ConfigParser, credential_path, table_name: str, result_fields: List[str], experiment_id: int):
         self._table_name = table_name
         self._result_fields = result_fields
-        self._config = _config
+        self._config = config
         self._timestamp_on_result_fields = utils.timestamps_for_result_fields(self._config)
-
         self._experiment_id = experiment_id
         self._experiment_id_condition = f'ID = {self._experiment_id}'
 
-        if _config['PY_EXPERIMENTER']['provider'] == 'sqlite':
-            self._dbconnector: DatabaseConnector = DatabaseConnectorLITE(_config)
-        elif _config['PY_EXPERIMENTER']['provider'] == 'mysql':
-            self._dbconnector: DatabaseConnector = DatabaseConnectorMYSQL(_config, credential_path)
+        self.use_codecarbon = use_codecarbon
+        self._codecarbon_config = codecarbon_config
+
+        if config['PY_EXPERIMENTER']['provider'] == 'sqlite':
+            self._dbconnector: DatabaseConnector = DatabaseConnectorLITE(config, self.use_codecarbon, self._codecarbon_config)
+        elif config['PY_EXPERIMENTER']['provider'] == 'mysql':
+            self._dbconnector: DatabaseConnector = DatabaseConnectorMYSQL(config, self.use_codecarbon, self._codecarbon_config, credential_path)
         else:
             raise InvalidConfigError("Invalid database provider!")
 
     def process_results(self, results: dict) -> None:
         """
         Process results from the experiment and write them to the database. You can call this method, whenever you
         want to write results to the database.
         :param results: Dictionary with result field name and result value pairs.
         """
-        time = utils.get_timestamp_representation()
         if not self._valid_result_fields(list(results.keys())):
             invalid_result_keys = set(list(results.keys())) - set(self._result_fields)
             raise InvalidResultFieldError(f"Invalid result keys: {invalid_result_keys}")
 
         if self._timestamp_on_result_fields:
             results = self.__class__._add_timestamps_to_results(results)
 
         self._dbconnector.update_database(self._table_name, values=results, condition=self._experiment_id_condition)
 
+    def _write_emissions(self, emission_data: EmissionsData, offline_mode: bool) -> None:
+        emission_data['offline_mode'] = offline_mode
+        emission_data['experiment_id'] = self._experiment_id
+
+        keys = utils.extract_codecarbon_columns(with_type = False)
+        values = emission_data.values()
+        values = [value if not value == '' else None for value in values]
+        statement = self._dbconnector.prepare_write_query(f'{self._table_name}_codecarbon', keys)
+        self._dbconnector.execute_queries([(statement, values)])
+
     @staticmethod
     def _add_timestamps_to_results(results: dict) -> List[Tuple[str, object]]:
         time = utils.get_timestamp_representation()
         result_fields_with_timestep = deepcopy(results)
         for result_field, value in sorted(results.items()):
             result_fields_with_timestep[result_field] = value
             result_fields_with_timestep[f"{result_field}_timestamp"] = time
@@ -67,17 +81,17 @@
 
     def process_logs(self, logs: Dict[str, Dict[str, str]]) -> None:
         queries = []
         time = utils.get_timestamp_representation()
         for logtable_identifier, log_entries in logs.items():
             logtable_name = f'{self._table_name}__{logtable_identifier}'
             log_entries['experiment_id'] = str(self._experiment_id)
-            log_entries['timestamp'] = f"'{time}'"
-            queries.append(
-                f"INSERT INTO {logtable_name} ({', '.join(log_entries.keys())}) VALUES ({', '.join(map(lambda x: str(x), log_entries.values()))})")
+            log_entries['timestamp'] = f"{time}"
+            stmt = self._dbconnector.prepare_write_query(logtable_name, log_entries.keys())
+            queries.append((stmt, log_entries.values()))
         self._dbconnector.execute_queries(queries)
 
     def _change_status(self, status: str):
         values = {'status': status,
                   'end_date': utils.get_timestamp_representation()}
         self._dbconnector.update_database(self._table_name, values=values, condition=self._experiment_id_condition)
```

### Comparing `py_experimenter-1.2.1/pyproject.toml` & `py_experimenter-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-experimenter"
-version = "1.2.1"
+version = "1.3.0"
 description = "The PyExperimenter is a tool for the automatic execution of experiments, e.g. for machine learning (ML), capturing corresponding results in a unified manner in a database."
 authors = [
     "Tanja Tornede <t.tornede@ai.uni-hannover.de>",
     "Alexander Tornede <a.tornede@ai.uni-hannover.de>",
     "Lukas Fehring <lukas.fehring@stud.uni-hannover.de>",
     "Lukas Gehring",
     "Helena Graf <h.graf@ai.uni-hannover.de>",
@@ -27,17 +27,18 @@
     "Programming Language :: Python :: 3.9"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = ">=1.15"
 pandas = ">=1.0"
-mysql-connector-python = ">=8.0"
 jupyterlab = "^3.5.0"
 joblib = "^1.2.0"
+codecarbon = ">=2.2.1"
+pymysql = "^1.0.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.0"
 mock = ">=4.0"
 sphinx = ">=5.0"
 nbsphinx = "^0.8.9"
 sphinx-gallery = "^0.11.1"
```

### Comparing `py_experimenter-1.2.1/setup.py` & `py_experimenter-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 packages = \
 ['py_experimenter']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['joblib>=1.2.0,<2.0.0',
+['codecarbon>=2.2.1',
+ 'joblib>=1.2.0,<2.0.0',
  'jupyterlab>=3.5.0,<4.0.0',
- 'mysql-connector-python>=8.0',
  'numpy>=1.15',
- 'pandas>=1.0']
+ 'pandas>=1.0',
+ 'pymysql>=1.0.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'py-experimenter',
-    'version': '1.2.1',
+    'version': '1.3.0',
     'description': 'The PyExperimenter is a tool for the automatic execution of experiments, e.g. for machine learning (ML), capturing corresponding results in a unified manner in a database.',
     'long_description': '[![Project Homepage](https://img.shields.io/badge/Project%20Homepage-tornede.github.io/py_experimenter-0092CD)](https://tornede.github.io/py_experimenter)\n[![Pypi](https://img.shields.io/pypi/v/py_experimenter)](https://pypi.org/project/py-experimenter/)\n[![License](https://img.shields.io/github/license/tornede/py_experimenter)](https://tornede.github.io/py_experimenter/license.html)\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.05149/status.svg)](https://doi.org/10.21105/joss.05149)\n\n![Tests](https://github.com/tornede/py_experimenter/actions/workflows/tests.yml/badge.svg)\n![GitHub Pages](https://github.com/tornede/py_experimenter/actions/workflows/github-pages.yml/badge.svg)\n\n<img src="docs/source/_static/py-experimenter-logo.png" alt="PyExperimenter Logo: Python biting a database" width="200px"/>\n\n# PyExperimenter\n\n`PyExperimenter` is a tool to facilitate the setup, documentation, execution, and subsequent evaluation of results from an empirical study of algorithms and in particular is designed to reduce the involved manual effort significantly.\nIt is intended to be used by researchers in the field of artificial intelligence, but is not limited to those.\n\nThe empirical analysis of algorithms is often accompanied by the execution of algorithms for different inputs and variants of the algorithms (specified via parameters) and the measurement of non-functional properties.\nSince the individual evaluations are usually independent, the evaluation can be performed in a distributed manner on an HPC system.\nHowever, setting up, documenting, and evaluating the results of such a study is often file-based.\nUsually, this requires extensive manual work to create configuration files for the inputs or to read and aggregate measured results from a report file.\nIn addition, monitoring and restarting individual executions is tedious and time-consuming.\n\nThese challenges are addressed by `PyExperimenter` by means of a single well defined configuration file and a central database for managing massively parallel evaluations, as well as collecting and aggregating their results.\nThereby, `PyExperimenter` alleviates the aforementioned overhead and allows experiment executions to be defined and monitored with ease.\n\n![General schema of `PyExperimenter`.](docs/source/_static/workflow.png)\n\nFor more details check out the [`PyExperimenter` documentation](https://tornede.github.io/py_experimenter/):\n\n- [Installation](https://tornede.github.io/py_experimenter/installation.html)\n- [Examples](https://tornede.github.io/py_experimenter/examples/example_general_usage.html)\n\n## Cite PyExperimenter\n\nIf you use `PyExperimenter` in a scientific publication, we would appreciate a citation in one of the following ways.\n\n### Citation String\n\nTornede et al., (2023). PyExperimenter: Easily distribute experiments and track results. Journal of Open Source Software, 8(84), 5149, https://doi.org/10.21105/joss.05149\n\n### BibTex\n```\n@article{Tornede2023, \n    title = {{PyExperimenter}: Easily distribute experiments and track results}, \n    author = {Tanja Tornede and Alexander Tornede and Lukas Fehring and Lukas Gehring and Helena Graf and Jonas Hanselle and Felix Mohr and Marcel Wever}, \n    journal = {Journal of Open Source Software},\n    publisher = {The Open Journal},  \n    year = {2023}, \n    volume = {8}, \n    number = {84}, \n    pages = {5149}, \n    doi = {10.21105/joss.05149}, \n    url = {https://doi.org/10.21105/joss.05149}\n}\n```\n',
     'author': 'Tanja Tornede',
     'author_email': 't.tornede@ai.uni-hannover.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tornede/py_experimenter',
```

### Comparing `py_experimenter-1.2.1/PKG-INFO` & `py_experimenter-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-experimenter
-Version: 1.2.1
+Version: 1.3.0
 Summary: The PyExperimenter is a tool for the automatic execution of experiments, e.g. for machine learning (ML), capturing corresponding results in a unified manner in a database.
 Home-page: https://github.com/tornede/py_experimenter
 License: MIT
 Keywords: python,experiments,database,executor
 Author: Tanja Tornede
 Author-email: t.tornede@ai.uni-hannover.de
 Requires-Python: >=3.9,<4.0
@@ -15,19 +15,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Dist: codecarbon (>=2.2.1)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: jupyterlab (>=3.5.0,<4.0.0)
-Requires-Dist: mysql-connector-python (>=8.0)
 Requires-Dist: numpy (>=1.15)
 Requires-Dist: pandas (>=1.0)
+Requires-Dist: pymysql (>=1.0.3,<2.0.0)
 Project-URL: Documentation, https://tornede.github.io/py_experimenter/
 Project-URL: Repository, https://github.com/tornede/py_experimenter
 Description-Content-Type: text/markdown
 
 [![Project Homepage](https://img.shields.io/badge/Project%20Homepage-tornede.github.io/py_experimenter-0092CD)](https://tornede.github.io/py_experimenter)
 [![Pypi](https://img.shields.io/pypi/v/py_experimenter)](https://pypi.org/project/py-experimenter/)
 [![License](https://img.shields.io/github/license/tornede/py_experimenter)](https://tornede.github.io/py_experimenter/license.html)
```

