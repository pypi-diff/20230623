# Comparing `tmp/apache-airflow-providers-mysql-5.1.1.tar.gz` & `tmp/apache-airflow-providers-mysql-5.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-mysql-5.1.1.tar", last modified: Tue Jun 20 11:28:49 2023, max compression
+gzip compressed data, was "apache-airflow-providers-mysql-5.1.1rc1.tar", last modified: Tue Jun 20 11:42:37 2023, max compression
```

## Comparing `apache-airflow-providers-mysql-5.1.1.tar` & `apache-airflow-providers-mysql-5.1.1rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:49.908472 apache-airflow-providers-mysql-5.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:48.000000 apache-airflow-providers-mysql-5.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15839 2023-06-20 11:28:49.909729 apache-airflow-providers-mysql-5.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14159 2023-06-20 11:28:48.000000 apache-airflow-providers-mysql-5.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:49.801144 apache-airflow-providers-mysql-5.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:49.802433 apache-airflow-providers-mysql-5.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:49.847417 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3769 2023-06-20 11:28:48.000000 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:49.853353 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12081 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/hooks/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:49.859463 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2863 2023-06-02 11:31:21.000000 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/operators/mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:49.875718 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3268 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/transfers/presto_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/transfers/s3_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/transfers/trino_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     6455 2023-06-08 05:42:54.000000 apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/transfers/vertica_to_mysql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:49.905766 apache-airflow-providers-mysql-5.1.1/apache_airflow_providers_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15839 2023-06-20 11:28:49.000000 apache-airflow-providers-mysql-5.1.1/apache_airflow_providers_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-20 11:28:49.000000 apache-airflow-providers-mysql-5.1.1/apache_airflow_providers_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:49.000000 apache-airflow-providers-mysql-5.1.1/apache_airflow_providers_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:28:49.000000 apache-airflow-providers-mysql-5.1.1/apache_airflow_providers_mysql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:49.000000 apache-airflow-providers-mysql-5.1.1/apache_airflow_providers_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      359 2023-06-20 11:28:49.000000 apache-airflow-providers-mysql-5.1.1/apache_airflow_providers_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:49.000000 apache-airflow-providers-mysql-5.1.1/apache_airflow_providers_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-mysql-5.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1879 2023-06-20 11:28:49.912053 apache-airflow-providers-mysql-5.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2018 2023-06-20 11:28:48.000000 apache-airflow-providers-mysql-5.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.914753 apache-airflow-providers-mysql-5.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:36.000000 apache-airflow-providers-mysql-5.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-mysql-5.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15845 2023-06-20 11:42:37.915873 apache-airflow-providers-mysql-5.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14162 2023-06-20 11:42:36.000000 apache-airflow-providers-mysql-5.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.819560 apache-airflow-providers-mysql-5.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.820891 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.859270 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2023-06-20 11:42:36.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.865202 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12081 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/hooks/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.870902 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2023-06-02 11:31:21.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/operators/mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.885529 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3268 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/presto_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/s3_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-06-01 06:14:28.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/trino_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     6455 2023-06-08 05:42:54.000000 apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:37.909948 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15845 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:37.000000 apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-mysql-5.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-20 11:42:37.917878 apache-airflow-providers-mysql-5.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2018 2023-06-20 11:42:36.000000 apache-airflow-providers-mysql-5.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-mysql-5.1.1/LICENSE` & `apache-airflow-providers-mysql-5.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/MANIFEST.in` & `apache-airflow-providers-mysql-5.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/PKG-INFO` & `apache-airflow-providers-mysql-5.1.1rc1/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 5.1.1
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.1/
@@ -54,15 +54,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.1.1``
+Release: ``5.1.1rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-mysql-5.1.1/README.rst` & `apache-airflow-providers-mysql-5.1.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.1.1``
+Release: ``5.1.1rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/__init__.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/get_provider_info.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/hooks/__init__.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/hooks/mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/operators/__init__.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/operators/mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/operators/mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/transfers/__init__.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/transfers/presto_to_mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/presto_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/transfers/s3_to_mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/s3_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/transfers/trino_to_mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/trino_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/airflow/providers/mysql/transfers/vertica_to_mysql.py` & `apache-airflow-providers-mysql-5.1.1rc1/airflow/providers/mysql/transfers/vertica_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/apache_airflow_providers_mysql.egg-info/PKG-INFO` & `apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mysql
-Version: 5.1.1
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mysql package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mysql/5.1.1/
@@ -54,15 +54,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mysql``
 
-Release: ``5.1.1``
+Release: ``5.1.1rc1``
 
 
 `MySQL <https://www.mysql.com/products/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-mysql-5.1.1/apache_airflow_providers_mysql.egg-info/SOURCES.txt` & `apache-airflow-providers-mysql-5.1.1rc1/apache_airflow_providers_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/pyproject.toml` & `apache-airflow-providers-mysql-5.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mysql-5.1.1/setup.cfg` & `apache-airflow-providers-mysql-5.1.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

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
 	mysqlclient>=1.3.6
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.mysql.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.mysql
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-mysql-5.1.1/setup.py` & `apache-airflow-providers-mysql-5.1.1rc1/setup.py`

 * *Files identical despite different names*

