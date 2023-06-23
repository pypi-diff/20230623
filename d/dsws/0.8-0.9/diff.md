# Comparing `tmp/dsws-0.8.tar.gz` & `tmp/dsws-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dsws-0.8.tar", last modified: Thu Feb  7 15:52:35 2019, max compression
+gzip compressed data, was "dist/dsws-0.9.tar", last modified: Thu Feb  7 17:38:41 2019, max compression
```

## Comparing `dsws-0.8.tar` & `dsws-0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2019-02-07 15:52:35.000000 dsws-0.8/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2019-02-07 15:52:35.000000 dsws-0.8/setup.cfg
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2019-01-31 16:04:49.000000 dsws-0.8/MANIFEST.in
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      539 2019-02-07 15:43:42.000000 dsws-0.8/setup.py
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2019-02-07 15:52:35.000000 dsws-0.8/dsws/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1690 2019-01-31 16:04:49.000000 dsws-0.8/dsws/ws_webapp_tb.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1510 2019-02-07 14:44:24.000000 dsws-0.8/dsws/ws_impala_imp.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1160 2019-02-04 21:08:58.000000 dsws-0.8/dsws/ws_spark_spark.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     2096 2019-02-07 14:53:52.000000 dsws-0.8/dsws/ws_impala_impyla.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        0 2019-01-31 16:04:49.000000 dsws-0.8/dsws/__init__.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     3072 2019-02-04 21:08:58.000000 dsws-0.8/dsws/duct.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     2399 2019-02-07 15:37:41.000000 dsws-0.8/dsws/ws_hive_himpyla.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1850 2019-02-04 21:08:58.000000 dsws-0.8/dsws/ws_hive_hbl.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     4709 2019-02-07 15:16:49.000000 dsws-0.8/dsws/util.py
-drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2019-02-07 15:52:35.000000 dsws-0.8/dsws.egg-info/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       67 2019-02-07 15:52:35.000000 dsws-0.8/dsws.egg-info/requires.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        5 2019-02-07 15:52:35.000000 dsws-0.8/dsws.egg-info/top_level.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2019-02-04 23:11:32.000000 dsws-0.8/dsws.egg-info/not-zip-safe
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2019-02-07 15:52:35.000000 dsws-0.8/dsws.egg-info/dependency_links.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      238 2019-02-07 15:52:35.000000 dsws-0.8/dsws.egg-info/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      375 2019-02-07 15:52:35.000000 dsws-0.8/dsws.egg-info/SOURCES.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      238 2019-02-07 15:52:35.000000 dsws-0.8/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       64 2019-01-31 16:04:49.000000 dsws-0.8/README.rst
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2019-02-07 17:38:41.000000 dsws-0.9/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2019-02-07 17:38:41.000000 dsws-0.9/setup.cfg
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2019-01-31 16:04:49.000000 dsws-0.9/MANIFEST.in
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      539 2019-02-07 17:37:38.000000 dsws-0.9/setup.py
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2019-02-07 17:38:41.000000 dsws-0.9/dsws/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1690 2019-01-31 16:04:49.000000 dsws-0.9/dsws/ws_webapp_tb.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1510 2019-02-07 14:44:24.000000 dsws-0.9/dsws/ws_impala_imp.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1160 2019-02-04 21:08:58.000000 dsws-0.9/dsws/ws_spark_spark.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     2096 2019-02-07 14:53:52.000000 dsws-0.9/dsws/ws_impala_impyla.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        0 2019-01-31 16:04:49.000000 dsws-0.9/dsws/__init__.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     3072 2019-02-04 21:08:58.000000 dsws-0.9/dsws/duct.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     2399 2019-02-07 15:37:41.000000 dsws-0.9/dsws/ws_hive_himpyla.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1850 2019-02-04 21:08:58.000000 dsws-0.9/dsws/ws_hive_hbl.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     4703 2019-02-07 17:34:17.000000 dsws-0.9/dsws/util.py
+drwxr-xr-x   0 cdsw      (8536) cdsw      (8536)        0 2019-02-07 17:38:41.000000 dsws-0.9/dsws.egg-info/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       67 2019-02-07 17:38:41.000000 dsws-0.9/dsws.egg-info/requires.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        5 2019-02-07 17:38:41.000000 dsws-0.9/dsws.egg-info/top_level.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2019-02-04 23:11:32.000000 dsws-0.9/dsws.egg-info/not-zip-safe
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2019-02-07 17:38:41.000000 dsws-0.9/dsws.egg-info/dependency_links.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      238 2019-02-07 17:38:41.000000 dsws-0.9/dsws.egg-info/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      375 2019-02-07 17:38:41.000000 dsws-0.9/dsws.egg-info/SOURCES.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      238 2019-02-07 17:38:41.000000 dsws-0.9/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       64 2019-01-31 16:04:49.000000 dsws-0.9/README.rst
```

### Comparing `dsws-0.8/setup.py` & `dsws-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(name='dsws',
-      version='0.8',
+      version='0.9',
       description='Data Science Work Space for CDSW',
       url='https://github.com/babarka/dsws',
       author='Brad Barker',
       author_email='brad@ratiocinate.com',
       license='MIT',
       packages=['dsws'],
       install_requires=[
```

### Comparing `dsws-0.8/dsws/ws_webapp_tb.py` & `dsws-0.9/dsws/ws_webapp_tb.py`

 * *Files identical despite different names*

### Comparing `dsws-0.8/dsws/ws_impala_imp.py` & `dsws-0.9/dsws/ws_impala_imp.py`

 * *Files identical despite different names*

### Comparing `dsws-0.8/dsws/ws_spark_spark.py` & `dsws-0.9/dsws/ws_spark_spark.py`

 * *Files identical despite different names*

### Comparing `dsws-0.8/dsws/ws_impala_impyla.py` & `dsws-0.9/dsws/ws_impala_impyla.py`

 * *Files identical despite different names*

### Comparing `dsws-0.8/dsws/duct.py` & `dsws-0.9/dsws/duct.py`

 * *Files identical despite different names*

### Comparing `dsws-0.8/dsws/ws_hive_himpyla.py` & `dsws-0.9/dsws/ws_hive_himpyla.py`

 * *Files identical despite different names*

### Comparing `dsws-0.8/dsws/ws_hive_hbl.py` & `dsws-0.9/dsws/ws_hive_hbl.py`

 * *Files identical despite different names*

### Comparing `dsws-0.8/dsws/util.py` & `dsws-0.9/dsws/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,16 @@
     Standard form for connection queries
     
     Allows grouping of commands using ";" seperator
     Each command can have the following form:
        Standard executable statement
        single file, read as sql
     """
-    #TODO: Add limit handle
     if qry.__class__ == str:
-        qry=qry.split(";")
+        qry=[q for q in qry.split(";") if q!='']
     rslt=[]
     for q in qry:
         if q[0]=="-":
             q=" ".join(q.split()[1:]).strip('"').strip("'")
         if "." in q.split()[0]:
             f==q.split()[0]
             if "/" not in f:
```

