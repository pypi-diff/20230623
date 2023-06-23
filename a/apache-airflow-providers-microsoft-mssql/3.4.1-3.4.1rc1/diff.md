# Comparing `tmp/apache-airflow-providers-microsoft-mssql-3.4.1.tar.gz` & `tmp/apache-airflow-providers-microsoft-mssql-3.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-microsoft-mssql-3.4.1.tar", last modified: Tue Jun 20 11:28:41 2023, max compression
+gzip compressed data, was "apache-airflow-providers-microsoft-mssql-3.4.1rc1.tar", last modified: Tue Jun 20 11:42:30 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-mssql-3.4.1.tar` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:41.017217 apache-airflow-providers-microsoft-mssql-3.4.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:39.000000 apache-airflow-providers-microsoft-mssql-3.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12906 2023-06-20 11:28:41.018895 apache-airflow-providers-microsoft-mssql-3.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11327 2023-06-20 11:28:39.000000 apache-airflow-providers-microsoft-mssql-3.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:40.922201 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:40.923361 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:40.924561 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:40.964312 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-20 11:01:09.000000 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-06-20 11:28:39.000000 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:40.972290 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4227 2023-06-19 10:14:19.000000 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/hooks/mssql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:40.980368 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2786 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/operators/mssql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:41.013521 apache-airflow-providers-microsoft-mssql-3.4.1/apache_airflow_providers_microsoft_mssql.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12906 2023-06-20 11:28:40.000000 apache-airflow-providers-microsoft-mssql-3.4.1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-06-20 11:28:40.000000 apache-airflow-providers-microsoft-mssql-3.4.1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:40.000000 apache-airflow-providers-microsoft-mssql-3.4.1/apache_airflow_providers_microsoft_mssql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-06-20 11:28:40.000000 apache-airflow-providers-microsoft-mssql-3.4.1/apache_airflow_providers_microsoft_mssql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:40.000000 apache-airflow-providers-microsoft-mssql-3.4.1/apache_airflow_providers_microsoft_mssql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-20 11:28:40.000000 apache-airflow-providers-microsoft-mssql-3.4.1/apache_airflow_providers_microsoft_mssql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:40.000000 apache-airflow-providers-microsoft-mssql-3.4.1/apache_airflow_providers_microsoft_mssql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-microsoft-mssql-3.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1935 2023-06-20 11:28:41.021575 apache-airflow-providers-microsoft-mssql-3.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1745 2023-06-20 11:28:39.000000 apache-airflow-providers-microsoft-mssql-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.262299 apache-airflow-providers-microsoft-mssql-3.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12912 2023-06-20 11:42:30.263458 apache-airflow-providers-microsoft-mssql-3.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11330 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.188032 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.189095 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.190231 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.224205 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-20 11:01:09.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.230075 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2023-06-19 10:14:19.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/mssql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.235908 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-06-05 12:50:36.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/mssql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:30.259868 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12912 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      140 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:30.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-06-20 11:42:30.265458 apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-06-20 11:42:29.000000 apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/LICENSE` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/MANIFEST.in` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/PKG-INFO` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-mssql
-Version: 3.4.1
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-mssql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/README.rst` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/get_provider_info.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/hooks/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/hooks/mssql.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/hooks/mssql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/operators/__init__.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/airflow/providers/microsoft/mssql/operators/mssql.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/airflow/providers/microsoft/mssql/operators/mssql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-mssql
-Version: 3.4.1
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-mssql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-mssql/3.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-mssql``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `Microsoft SQL Server (MSSQL) <https://www.microsoft.com/en-us/sql-server/sql-server-downloads>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/apache_airflow_providers_microsoft_mssql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/pyproject.toml` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/setup.cfg` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.cfg`

 * *Files 5% similar despite different names*

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
 	pymssql>=2.1.5
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.microsoft.mssql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.microsoft.mssql
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-microsoft-mssql-3.4.1/setup.py` & `apache-airflow-providers-microsoft-mssql-3.4.1rc1/setup.py`

 * *Files identical despite different names*
