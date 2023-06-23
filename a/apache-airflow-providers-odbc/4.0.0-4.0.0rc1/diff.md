# Comparing `tmp/apache-airflow-providers-odbc-4.0.0.tar.gz` & `tmp/apache-airflow-providers-odbc-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-odbc-4.0.0.tar", last modified: Tue Jun 20 11:28:54 2023, max compression
+gzip compressed data, was "apache-airflow-providers-odbc-4.0.0rc1.tar", last modified: Tue Jun 20 11:42:41 2023, max compression
```

## Comparing `apache-airflow-providers-odbc-4.0.0.tar` & `apache-airflow-providers-odbc-4.0.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:54.306769 apache-airflow-providers-odbc-4.0.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-odbc-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:52.000000 apache-airflow-providers-odbc-4.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-odbc-4.0.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12459 2023-06-20 11:28:54.309209 apache-airflow-providers-odbc-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10913 2023-06-20 11:28:52.000000 apache-airflow-providers-odbc-4.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:54.209488 apache-airflow-providers-odbc-4.0.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:54.211040 apache-airflow-providers-odbc-4.0.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:54.262201 apache-airflow-providers-odbc-4.0.0/airflow/providers/odbc/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-odbc-4.0.0/airflow/providers/odbc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2254 2023-06-20 11:28:52.000000 apache-airflow-providers-odbc-4.0.0/airflow/providers/odbc/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:54.270860 apache-airflow-providers-odbc-4.0.0/airflow/providers/odbc/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-odbc-4.0.0/airflow/providers/odbc/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8946 2023-06-19 10:14:19.000000 apache-airflow-providers-odbc-4.0.0/airflow/providers/odbc/hooks/odbc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:54.301510 apache-airflow-providers-odbc-4.0.0/apache_airflow_providers_odbc.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12459 2023-06-20 11:28:54.000000 apache-airflow-providers-odbc-4.0.0/apache_airflow_providers_odbc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-20 11:28:54.000000 apache-airflow-providers-odbc-4.0.0/apache_airflow_providers_odbc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:54.000000 apache-airflow-providers-odbc-4.0.0/apache_airflow_providers_odbc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:28:54.000000 apache-airflow-providers-odbc-4.0.0/apache_airflow_providers_odbc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:54.000000 apache-airflow-providers-odbc-4.0.0/apache_airflow_providers_odbc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      122 2023-06-20 11:28:54.000000 apache-airflow-providers-odbc-4.0.0/apache_airflow_providers_odbc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:54.000000 apache-airflow-providers-odbc-4.0.0/apache_airflow_providers_odbc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-odbc-4.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1861 2023-06-20 11:28:54.312743 apache-airflow-providers-odbc-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-20 11:28:52.000000 apache-airflow-providers-odbc-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:41.478039 apache-airflow-providers-odbc-4.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-odbc-4.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:40.000000 apache-airflow-providers-odbc-4.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-odbc-4.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12465 2023-06-20 11:42:41.479149 apache-airflow-providers-odbc-4.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10916 2023-06-20 11:42:40.000000 apache-airflow-providers-odbc-4.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:41.408542 apache-airflow-providers-odbc-4.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:41.409942 apache-airflow-providers-odbc-4.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:41.442521 apache-airflow-providers-odbc-4.0.0rc1/airflow/providers/odbc/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-odbc-4.0.0rc1/airflow/providers/odbc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-06-20 11:42:40.000000 apache-airflow-providers-odbc-4.0.0rc1/airflow/providers/odbc/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:41.448297 apache-airflow-providers-odbc-4.0.0rc1/airflow/providers/odbc/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-odbc-4.0.0rc1/airflow/providers/odbc/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8946 2023-06-19 10:14:19.000000 apache-airflow-providers-odbc-4.0.0rc1/airflow/providers/odbc/hooks/odbc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:41.475379 apache-airflow-providers-odbc-4.0.0rc1/apache_airflow_providers_odbc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12465 2023-06-20 11:42:41.000000 apache-airflow-providers-odbc-4.0.0rc1/apache_airflow_providers_odbc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-20 11:42:41.000000 apache-airflow-providers-odbc-4.0.0rc1/apache_airflow_providers_odbc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:41.000000 apache-airflow-providers-odbc-4.0.0rc1/apache_airflow_providers_odbc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:42:41.000000 apache-airflow-providers-odbc-4.0.0rc1/apache_airflow_providers_odbc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:41.000000 apache-airflow-providers-odbc-4.0.0rc1/apache_airflow_providers_odbc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-20 11:42:41.000000 apache-airflow-providers-odbc-4.0.0rc1/apache_airflow_providers_odbc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:41.000000 apache-airflow-providers-odbc-4.0.0rc1/apache_airflow_providers_odbc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-odbc-4.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-06-20 11:42:41.481106 apache-airflow-providers-odbc-4.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-20 11:42:40.000000 apache-airflow-providers-odbc-4.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-odbc-4.0.0/LICENSE` & `apache-airflow-providers-odbc-4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-odbc-4.0.0/MANIFEST.in` & `apache-airflow-providers-odbc-4.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-odbc-4.0.0/PKG-INFO` & `apache-airflow-providers-odbc-4.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-odbc
-Version: 4.0.0
+Version: 4.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-odbc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.0.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``4.0.0``
+Release: ``4.0.0rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-odbc-4.0.0/README.rst` & `apache-airflow-providers-odbc-4.0.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``4.0.0``
+Release: ``4.0.0rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-odbc-4.0.0/airflow/providers/odbc/__init__.py` & `apache-airflow-providers-odbc-4.0.0rc1/airflow/providers/odbc/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-odbc-4.0.0/airflow/providers/odbc/get_provider_info.py` & `apache-airflow-providers-odbc-4.0.0rc1/airflow/providers/odbc/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-odbc-4.0.0/airflow/providers/odbc/hooks/__init__.py` & `apache-airflow-providers-odbc-4.0.0rc1/airflow/providers/odbc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-odbc-4.0.0/airflow/providers/odbc/hooks/odbc.py` & `apache-airflow-providers-odbc-4.0.0rc1/airflow/providers/odbc/hooks/odbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-odbc-4.0.0/apache_airflow_providers_odbc.egg-info/PKG-INFO` & `apache-airflow-providers-odbc-4.0.0rc1/apache_airflow_providers_odbc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-odbc
-Version: 4.0.0
+Version: 4.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-odbc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-odbc/4.0.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-odbc``
 
-Release: ``4.0.0``
+Release: ``4.0.0rc1``
 
 
 `ODBC <https://github.com/mkleehammer/pyodbc/wiki>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-odbc-4.0.0/apache_airflow_providers_odbc.egg-info/SOURCES.txt` & `apache-airflow-providers-odbc-4.0.0rc1/apache_airflow_providers_odbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-odbc-4.0.0/pyproject.toml` & `apache-airflow-providers-odbc-4.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-odbc-4.0.0/setup.cfg` & `apache-airflow-providers-odbc-4.0.0rc1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow-providers-common-sql>=1.3.1
-	apache-airflow>=2.4.0
+	apache-airflow-providers-common-sql>=1.3.1.dev0
+	apache-airflow>=2.4.0.dev0
 	pyodbc
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.odbc.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.odbc
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-odbc-4.0.0/setup.py` & `apache-airflow-providers-odbc-4.0.0rc1/setup.py`

 * *Files identical despite different names*

