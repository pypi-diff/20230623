# Comparing `tmp/databaseRestoreIntegrity-1.0.9.tar.gz` & `tmp/databaseRestoreIntegrity-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databaseRestoreIntegrity-1.0.9.tar", last modified: Thu Jun 15 14:21:19 2023, max compression
+gzip compressed data, was "databaseRestoreIntegrity-1.1.0.tar", last modified: Fri Jun 23 10:15:23 2023, max compression
```

## Comparing `databaseRestoreIntegrity-1.0.9.tar` & `databaseRestoreIntegrity-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 14:21:19.169314 databaseRestoreIntegrity-1.0.9/
--rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.9/LICENSE.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.9/MANIFEST.in
--rw-r--r--   0 mhasan     (502) staff       (20)     6223 2023-06-15 14:21:19.169491 databaseRestoreIntegrity-1.0.9/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)     4531 2023-06-15 14:19:55.000000 databaseRestoreIntegrity-1.0.9/README.md
--rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.9/pyproject.toml
--rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-15 14:21:19.171057 databaseRestoreIntegrity-1.0.9/setup.cfg
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 14:21:19.147468 databaseRestoreIntegrity-1.0.9/src/
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 14:21:19.165862 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/
--rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/__init__.py
--rw-r--r--   0 mhasan     (502) staff       (20)     2970 2023-06-07 12:36:19.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/mysql.py
--rw-r--r--   0 mhasan     (502) staff       (20)     2872 2023-06-15 13:02:54.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/postgres.py
-drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-15 14:21:19.168775 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity.egg-info/
--rw-r--r--   0 mhasan     (502) staff       (20)     6223 2023-06-15 14:21:19.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity.egg-info/PKG-INFO
--rw-r--r--   0 mhasan     (502) staff       (20)      386 2023-06-15 14:21:19.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
--rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-15 14:21:19.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
--rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-15 14:21:19.000000 databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity.egg-info/top_level.txt
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-23 10:15:23.322200 databaseRestoreIntegrity-1.1.0/
+-rw-r--r--   0 mhasan     (502) staff       (20)     1073 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.0/LICENSE.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.0/MANIFEST.in
+-rw-r--r--   0 mhasan     (502) staff       (20)     6231 2023-06-23 10:15:23.322308 databaseRestoreIntegrity-1.1.0/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)     4539 2023-06-23 10:14:38.000000 databaseRestoreIntegrity-1.1.0/README.md
+-rw-r--r--   0 mhasan     (502) staff       (20)       84 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.0/pyproject.toml
+-rw-r--r--   0 mhasan     (502) staff       (20)      740 2023-06-23 10:15:23.324343 databaseRestoreIntegrity-1.1.0/setup.cfg
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-23 10:15:23.310724 databaseRestoreIntegrity-1.1.0/src/
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-23 10:15:23.319167 databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity/
+-rw-r--r--   0 mhasan     (502) staff       (20)        0 2023-06-05 06:11:00.000000 databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity/__init__.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     3375 2023-06-23 09:59:19.000000 databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity/mysqldb.py
+-rw-r--r--   0 mhasan     (502) staff       (20)     2872 2023-06-15 13:02:54.000000 databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity/postgresdb.py
+drwxr-xr-x   0 mhasan     (502) staff       (20)        0 2023-06-23 10:15:23.321866 databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity.egg-info/
+-rw-r--r--   0 mhasan     (502) staff       (20)     6231 2023-06-23 10:15:23.000000 databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity.egg-info/PKG-INFO
+-rw-r--r--   0 mhasan     (502) staff       (20)      390 2023-06-23 10:15:23.000000 databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity.egg-info/SOURCES.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)        1 2023-06-23 10:15:23.000000 databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity.egg-info/dependency_links.txt
+-rw-r--r--   0 mhasan     (502) staff       (20)       25 2023-06-23 10:15:23.000000 databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity.egg-info/top_level.txt
```

### Comparing `databaseRestoreIntegrity-1.0.9/LICENSE.txt` & `databaseRestoreIntegrity-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.9/PKG-INFO` & `databaseRestoreIntegrity-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.0.9
+Version: 1.1.0
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
@@ -48,16 +48,16 @@
 src_db_user = os.environ['SRC_DB_USER']
 dst_db_host = os.environ['DST_DB_HOST']
 dst_db_pass = os.environ['DST_DB_PASS']
 dst_db_user = os.environ['DST_DB_USER']
 
 
 
-restored_db = mysql.mysqlReadData(dst_db_host, dst_db_user, dst_db_pass)
-active_db = mysql.mysqlReadData(src_db_host, src_db_user, src_db_pass)
+restored_db = mysqldb.mysqlReadData(dst_db_host, dst_db_user, dst_db_pass)
+active_db = mysqldb.mysqlReadData(src_db_host, src_db_user, src_db_pass)
 
 restored_db._create_tmp_file('restored_db')
 active_db._create_tmp_file('active_db')
 restored_db._insert_data('restored_db')
 restored_db._insert_data('active_db')
 
 
@@ -100,16 +100,16 @@
 dst_db_host = os.environ['DST_DB_HOST']
 dst_db_pass = os.environ['DST_DB_PASS']
 dst_db_user = os.environ['DST_DB_USER']
 db_name = os.environ['DB_NAME']
 
 
 
-restored_db = postgres.pgsqlReadData(dst_db_host, dst_db_user, dst_db_pass, db_name)
-active_db = postgres.pgsqlReadData(src_db_host, src_db_user, src_db_pass, db_name)
+restored_db = postgresdb.pgsqlReadData(dst_db_host, dst_db_user, dst_db_pass, db_name)
+active_db = postgresdb.pgsqlReadData(src_db_host, src_db_user, src_db_pass, db_name)
 
 restored_db._create_tmp_file('restored_db')
 active_db._create_tmp_file('active_db')
 restored_db._insert_data('restored_db')
 restored_db._insert_data('active_db')
```

### Comparing `databaseRestoreIntegrity-1.0.9/README.md` & `databaseRestoreIntegrity-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 src_db_user = os.environ['SRC_DB_USER']
 dst_db_host = os.environ['DST_DB_HOST']
 dst_db_pass = os.environ['DST_DB_PASS']
 dst_db_user = os.environ['DST_DB_USER']
 
 
 
-restored_db = mysql.mysqlReadData(dst_db_host, dst_db_user, dst_db_pass)
-active_db = mysql.mysqlReadData(src_db_host, src_db_user, src_db_pass)
+restored_db = mysqldb.mysqlReadData(dst_db_host, dst_db_user, dst_db_pass)
+active_db = mysqldb.mysqlReadData(src_db_host, src_db_user, src_db_pass)
 
 restored_db._create_tmp_file('restored_db')
 active_db._create_tmp_file('active_db')
 restored_db._insert_data('restored_db')
 restored_db._insert_data('active_db')
 
 
@@ -84,16 +84,16 @@
 dst_db_host = os.environ['DST_DB_HOST']
 dst_db_pass = os.environ['DST_DB_PASS']
 dst_db_user = os.environ['DST_DB_USER']
 db_name = os.environ['DB_NAME']
 
 
 
-restored_db = postgres.pgsqlReadData(dst_db_host, dst_db_user, dst_db_pass, db_name)
-active_db = postgres.pgsqlReadData(src_db_host, src_db_user, src_db_pass, db_name)
+restored_db = postgresdb.pgsqlReadData(dst_db_host, dst_db_user, dst_db_pass, db_name)
+active_db = postgresdb.pgsqlReadData(src_db_host, src_db_user, src_db_pass, db_name)
 
 restored_db._create_tmp_file('restored_db')
 active_db._create_tmp_file('active_db')
 restored_db._insert_data('restored_db')
 restored_db._insert_data('active_db')
```

### Comparing `databaseRestoreIntegrity-1.0.9/setup.cfg` & `databaseRestoreIntegrity-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = databaseRestoreIntegrity
-version = 1.0.9
+version = 1.1.0
 author = Maihraj Hasan
 author_email = maihrajhasan@gmail.com
 description = A package to check mysql restore integrity check
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/mysql.py` & `databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity/mysqldb.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,18 +51,23 @@
         return tables_names
 
     def _records_count(self):
         records_count = []
         conn = self.connection()
         t_name = self._table_list()
         for c in t_name:
-            sql_query = "select count(*) from " + c
+            ignore_dbs = ['performance_schema', 'information_schema', 'sys', 'mysql']
+            if any(db in c for db in ignore_dbs):
+                pass
+            else:
+                sql_query = "select count(*) from " + c
             r = conn.cursor()
             r.execute(sql_query)
             for count in r:
+                print("{},{}".format(c, *count))
                 records_count.append("{},{}".format(c, *count))  
         return records_count   
 
     def _create_tmp_file(self, name):
         self.name = name
         records = self._records_count()
         f = open(self.name, 'w+')
@@ -87,7 +92,10 @@
             count += 1
             sql_query = ("{}".format(line.strip()))
             ct.execute(sql_query)
             conn.commit()
         f.close()
         os.remove(self.name)
         conn.close()
+
+database = mysqlReadData('eqs-k8s-prod-1-integrity-line.cluster-ro-c3omjkoufrsh.eu-central-1.rds.amazonaws.com', 'root', 'xDYyTYnlr2')
+database._create_tmp_file('restored_db')
```

### Comparing `databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity/postgres.py` & `databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity/postgresdb.py`

 * *Files identical despite different names*

### Comparing `databaseRestoreIntegrity-1.0.9/src/databaseRestoreIntegrity.egg-info/PKG-INFO` & `databaseRestoreIntegrity-1.1.0/src/databaseRestoreIntegrity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databaseRestoreIntegrity
-Version: 1.0.9
+Version: 1.1.0
 Summary: A package to check mysql restore integrity check
 Home-page: 
 Author: Maihraj Hasan
 Author-email: maihrajhasan@gmail.com
 Project-URL: Bug Tracker, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck/-/issues
 Project-URL: repository, https://github.com/maihraj/Python3/mysqlRestoreIntegrityCheck
 Classifier: Programming Language :: Python :: 3
@@ -48,16 +48,16 @@
 src_db_user = os.environ['SRC_DB_USER']
 dst_db_host = os.environ['DST_DB_HOST']
 dst_db_pass = os.environ['DST_DB_PASS']
 dst_db_user = os.environ['DST_DB_USER']
 
 
 
-restored_db = mysql.mysqlReadData(dst_db_host, dst_db_user, dst_db_pass)
-active_db = mysql.mysqlReadData(src_db_host, src_db_user, src_db_pass)
+restored_db = mysqldb.mysqlReadData(dst_db_host, dst_db_user, dst_db_pass)
+active_db = mysqldb.mysqlReadData(src_db_host, src_db_user, src_db_pass)
 
 restored_db._create_tmp_file('restored_db')
 active_db._create_tmp_file('active_db')
 restored_db._insert_data('restored_db')
 restored_db._insert_data('active_db')
 
 
@@ -100,16 +100,16 @@
 dst_db_host = os.environ['DST_DB_HOST']
 dst_db_pass = os.environ['DST_DB_PASS']
 dst_db_user = os.environ['DST_DB_USER']
 db_name = os.environ['DB_NAME']
 
 
 
-restored_db = postgres.pgsqlReadData(dst_db_host, dst_db_user, dst_db_pass, db_name)
-active_db = postgres.pgsqlReadData(src_db_host, src_db_user, src_db_pass, db_name)
+restored_db = postgresdb.pgsqlReadData(dst_db_host, dst_db_user, dst_db_pass, db_name)
+active_db = postgresdb.pgsqlReadData(src_db_host, src_db_user, src_db_pass, db_name)
 
 restored_db._create_tmp_file('restored_db')
 active_db._create_tmp_file('active_db')
 restored_db._insert_data('restored_db')
 restored_db._insert_data('active_db')
```

