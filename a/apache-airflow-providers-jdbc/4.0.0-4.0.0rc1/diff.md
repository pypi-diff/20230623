# Comparing `tmp/apache-airflow-providers-jdbc-4.0.0.tar.gz` & `tmp/apache-airflow-providers-jdbc-4.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-jdbc-4.0.0.tar", last modified: Tue Jun 20 11:28:33 2023, max compression
+gzip compressed data, was "apache-airflow-providers-jdbc-4.0.0rc1.tar", last modified: Tue Jun 20 11:42:23 2023, max compression
```

## Comparing `apache-airflow-providers-jdbc-4.0.0.tar` & `apache-airflow-providers-jdbc-4.0.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:33.791352 apache-airflow-providers-jdbc-4.0.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-jdbc-4.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:32.000000 apache-airflow-providers-jdbc-4.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-jdbc-4.0.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14101 2023-06-20 11:28:33.792717 apache-airflow-providers-jdbc-4.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12555 2023-06-20 11:28:32.000000 apache-airflow-providers-jdbc-4.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:33.685500 apache-airflow-providers-jdbc-4.0.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:33.686854 apache-airflow-providers-jdbc-4.0.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:33.733444 apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-06-20 11:28:32.000000 apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:33.743976 apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7023 2023-06-17 16:45:00.000000 apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/hooks/jdbc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:33.752901 apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/operators/jdbc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:33.787694 apache-airflow-providers-jdbc-4.0.0/apache_airflow_providers_jdbc.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14101 2023-06-20 11:28:33.000000 apache-airflow-providers-jdbc-4.0.0/apache_airflow_providers_jdbc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-20 11:28:33.000000 apache-airflow-providers-jdbc-4.0.0/apache_airflow_providers_jdbc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:33.000000 apache-airflow-providers-jdbc-4.0.0/apache_airflow_providers_jdbc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:28:33.000000 apache-airflow-providers-jdbc-4.0.0/apache_airflow_providers_jdbc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:33.000000 apache-airflow-providers-jdbc-4.0.0/apache_airflow_providers_jdbc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      133 2023-06-20 11:28:33.000000 apache-airflow-providers-jdbc-4.0.0/apache_airflow_providers_jdbc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:33.000000 apache-airflow-providers-jdbc-4.0.0/apache_airflow_providers_jdbc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-jdbc-4.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1872 2023-06-20 11:28:33.795346 apache-airflow-providers-jdbc-4.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-20 11:28:32.000000 apache-airflow-providers-jdbc-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.924525 apache-airflow-providers-jdbc-4.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-jdbc-4.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:22.000000 apache-airflow-providers-jdbc-4.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-jdbc-4.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14107 2023-06-20 11:42:23.925592 apache-airflow-providers-jdbc-4.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12558 2023-06-20 11:42:22.000000 apache-airflow-providers-jdbc-4.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.852378 apache-airflow-providers-jdbc-4.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.853627 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.885976 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-06-20 11:42:22.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.891740 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7023 2023-06-17 16:45:00.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/hooks/jdbc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.897447 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-06-01 06:14:28.000000 apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/operators/jdbc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:23.921741 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14107 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:23.000000 apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-jdbc-4.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-06-20 11:42:23.927528 apache-airflow-providers-jdbc-4.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-20 11:42:22.000000 apache-airflow-providers-jdbc-4.0.0rc1/setup.py
```

### Comparing `apache-airflow-providers-jdbc-4.0.0/LICENSE` & `apache-airflow-providers-jdbc-4.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.0/MANIFEST.in` & `apache-airflow-providers-jdbc-4.0.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.0/PKG-INFO` & `apache-airflow-providers-jdbc-4.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jdbc
-Version: 4.0.0
+Version: 4.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jdbc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jdbc/4.0.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``4.0.0``
+Release: ``4.0.0rc1``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-jdbc-4.0.0/README.rst` & `apache-airflow-providers-jdbc-4.0.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``4.0.0``
+Release: ``4.0.0rc1``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/__init__.py` & `apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/get_provider_info.py` & `apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/hooks/__init__.py` & `apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/hooks/jdbc.py` & `apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/hooks/jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/operators/__init__.py` & `apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.0/airflow/providers/jdbc/operators/jdbc.py` & `apache-airflow-providers-jdbc-4.0.0rc1/airflow/providers/jdbc/operators/jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.0/apache_airflow_providers_jdbc.egg-info/PKG-INFO` & `apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jdbc
-Version: 4.0.0
+Version: 4.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jdbc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jdbc/4.0.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-jdbc``
 
-Release: ``4.0.0``
+Release: ``4.0.0rc1``
 
 
 `Java Database Connectivity (JDBC) <https://docs.oracle.com/javase/8/docs/technotes/guides/jdbc/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-jdbc-4.0.0/apache_airflow_providers_jdbc.egg-info/SOURCES.txt` & `apache-airflow-providers-jdbc-4.0.0rc1/apache_airflow_providers_jdbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.0/pyproject.toml` & `apache-airflow-providers-jdbc-4.0.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jdbc-4.0.0/setup.cfg` & `apache-airflow-providers-jdbc-4.0.0rc1/setup.cfg`

 * *Files 6% similar despite different names*

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
 	jaydebeapi>=1.1.1
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.jdbc.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.jdbc
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-jdbc-4.0.0/setup.py` & `apache-airflow-providers-jdbc-4.0.0rc1/setup.py`

 * *Files identical despite different names*

