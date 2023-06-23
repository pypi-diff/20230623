# Comparing `tmp/nuvolos-0.4.8.tar.gz` & `tmp/nuvolos-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuvolos-0.4.8.tar", last modified: Tue Sep  6 11:23:50 2022, max compression
+gzip compressed data, was "nuvolos-0.5.0.tar", last modified: Fri Jun 23 16:45:04 2023, max compression
```

## Comparing `nuvolos-0.4.8.tar` & `nuvolos-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 salid      (501) staff       (20)        0 2022-09-06 11:23:50.984825 nuvolos-0.4.8/
--rw-r--r--   0 salid      (501) staff       (20)       18 2022-07-22 09:01:09.000000 nuvolos-0.4.8/MANIFEST.in
--rw-r--r--   0 salid      (501) staff       (20)      694 2022-09-06 11:23:50.984715 nuvolos-0.4.8/PKG-INFO
--rw-r--r--   0 salid      (501) staff       (20)      461 2022-07-22 09:01:09.000000 nuvolos-0.4.8/README.rst
-drwxr-xr-x   0 salid      (501) staff       (20)        0 2022-09-06 11:23:50.984008 nuvolos-0.4.8/nuvolos/
--rw-r--r--   0 salid      (501) staff       (20)    11647 2022-07-22 09:14:09.000000 nuvolos-0.4.8/nuvolos/__init__.py
--rw-r--r--   0 salid      (501) staff       (20)    17166 2022-07-22 09:21:50.000000 nuvolos-0.4.8/nuvolos/sql_utils.py
--rw-r--r--   0 salid      (501) staff       (20)       22 2022-09-06 10:26:53.000000 nuvolos-0.4.8/nuvolos/version.py
-drwxr-xr-x   0 salid      (501) staff       (20)        0 2022-09-06 11:23:50.984571 nuvolos-0.4.8/nuvolos.egg-info/
--rw-r--r--   0 salid      (501) staff       (20)      694 2022-09-06 11:23:50.000000 nuvolos-0.4.8/nuvolos.egg-info/PKG-INFO
--rw-r--r--   0 salid      (501) staff       (20)      275 2022-09-06 11:23:50.000000 nuvolos-0.4.8/nuvolos.egg-info/SOURCES.txt
--rw-r--r--   0 salid      (501) staff       (20)        1 2022-09-06 11:23:50.000000 nuvolos-0.4.8/nuvolos.egg-info/dependency_links.txt
--rw-r--r--   0 salid      (501) staff       (20)        1 2022-09-06 11:23:50.000000 nuvolos-0.4.8/nuvolos.egg-info/not-zip-safe
--rw-r--r--   0 salid      (501) staff       (20)      126 2022-09-06 11:23:50.000000 nuvolos-0.4.8/nuvolos.egg-info/requires.txt
--rw-r--r--   0 salid      (501) staff       (20)        8 2022-09-06 11:23:50.000000 nuvolos-0.4.8/nuvolos.egg-info/top_level.txt
--rw-r--r--   0 salid      (501) staff       (20)       38 2022-09-06 11:23:50.984862 nuvolos-0.4.8/setup.cfg
--rw-r--r--   0 salid      (501) staff       (20)      856 2022-09-06 11:15:37.000000 nuvolos-0.4.8/setup.py
+drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-23 16:45:04.449768 nuvolos-0.5.0/
+-rw-r--r--   0 salid      (501) staff       (20)       18 2022-07-22 09:01:09.000000 nuvolos-0.5.0/MANIFEST.in
+-rw-r--r--   0 salid      (501) staff       (20)      694 2023-06-23 16:45:04.449649 nuvolos-0.5.0/PKG-INFO
+-rw-r--r--   0 salid      (501) staff       (20)      461 2022-07-22 09:01:09.000000 nuvolos-0.5.0/README.rst
+drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-23 16:45:04.448506 nuvolos-0.5.0/nuvolos/
+-rw-r--r--   0 salid      (501) staff       (20)    11647 2022-07-22 09:14:09.000000 nuvolos-0.5.0/nuvolos/__init__.py
+-rw-r--r--   0 salid      (501) staff       (20)    17166 2022-07-22 09:21:50.000000 nuvolos-0.5.0/nuvolos/sql_utils.py
+-rw-r--r--   0 salid      (501) staff       (20)       22 2023-06-23 12:49:15.000000 nuvolos-0.5.0/nuvolos/version.py
+drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-23 16:45:04.449224 nuvolos-0.5.0/nuvolos.egg-info/
+-rw-r--r--   0 salid      (501) staff       (20)      694 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/PKG-INFO
+-rw-r--r--   0 salid      (501) staff       (20)      296 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/SOURCES.txt
+-rw-r--r--   0 salid      (501) staff       (20)        1 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/dependency_links.txt
+-rw-r--r--   0 salid      (501) staff       (20)        1 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/not-zip-safe
+-rw-r--r--   0 salid      (501) staff       (20)       90 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/requires.txt
+-rw-r--r--   0 salid      (501) staff       (20)        8 2023-06-23 16:45:04.000000 nuvolos-0.5.0/nuvolos.egg-info/top_level.txt
+-rw-r--r--   0 salid      (501) staff       (20)       38 2023-06-23 16:45:04.449800 nuvolos-0.5.0/setup.cfg
+-rw-r--r--   0 salid      (501) staff       (20)      815 2023-06-23 13:19:10.000000 nuvolos-0.5.0/setup.py
+drwxr-xr-x   0 salid      (501) staff       (20)        0 2023-06-23 16:45:04.449349 nuvolos-0.5.0/tests/
+-rw-r--r--   0 salid      (501) staff       (20)     8813 2023-06-23 14:50:50.000000 nuvolos-0.5.0/tests/test_to_sql.py
```

### Comparing `nuvolos-0.4.8/PKG-INFO` & `nuvolos-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvolos
-Version: 0.4.8
+Version: 0.5.0
 Summary: The Nuvolos python library for database connectivity
 Home-page: https://github.com/nuvolos-cloud/python-connector
 Author: Alphacruncher
 Author-email: support@nuvolos.cloud
 License: MIT
 
 nuvolos - The database connectivity library for Nuvolos
```

### Comparing `nuvolos-0.4.8/nuvolos/__init__.py` & `nuvolos-0.5.0/nuvolos/__init__.py`

 * *Files identical despite different names*

### Comparing `nuvolos-0.4.8/nuvolos/sql_utils.py` & `nuvolos-0.5.0/nuvolos/sql_utils.py`

 * *Files identical despite different names*

### Comparing `nuvolos-0.4.8/nuvolos.egg-info/PKG-INFO` & `nuvolos-0.5.0/nuvolos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuvolos
-Version: 0.4.8
+Version: 0.5.0
 Summary: The Nuvolos python library for database connectivity
 Home-page: https://github.com/nuvolos-cloud/python-connector
 Author: Alphacruncher
 Author-email: support@nuvolos.cloud
 License: MIT
 
 nuvolos - The database connectivity library for Nuvolos
```

### Comparing `nuvolos-0.4.8/setup.py` & `nuvolos-0.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,21 +12,20 @@
     version=__version__,
     description="The Nuvolos python library for database connectivity",
     long_description=readme(),
     url="https://github.com/nuvolos-cloud/python-connector",
     author="Alphacruncher",
     author_email="support@nuvolos.cloud",
     license="MIT",
-    packages=find_packages(exclude=("tests",)),
+    packages=find_packages(exclude=("tests","venv")),
     include_package_data=True,
     install_requires=[
+        "pyarrow"
         "keyring",
-        "pyarrow==8.0.0",
-        "sqlalchemy>='1.4.0'",
-        "pandas>=1.1.0",
-        "snowflake-connector-python>=2.7.12,<2.8.0",
-        "snowflake-sqlalchemy>1.4.0",
+        "pandas<2.1.0",
+        "snowflake-connector-python==3.0.4",
+        "snowflake-sqlalchemy==1.4.7",
     ],
     zip_safe=False,
     setup_requires=["pytest-runner"],
     tests_require=["pytest"],
 )
```

