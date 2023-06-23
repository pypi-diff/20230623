# Comparing `tmp/apache-airflow-providers-oracle-3.7.1.tar.gz` & `tmp/apache-airflow-providers-oracle-3.7.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-oracle-3.7.1.tar", last modified: Tue Jun 20 11:29:01 2023, max compression
+gzip compressed data, was "apache-airflow-providers-oracle-3.7.1rc1.tar", last modified: Tue Jun 20 11:42:47 2023, max compression
```

## Comparing `apache-airflow-providers-oracle-3.7.1.tar` & `apache-airflow-providers-oracle-3.7.1rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:01.609375 apache-airflow-providers-oracle-3.7.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:00.000000 apache-airflow-providers-oracle-3.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13999 2023-06-20 11:29:01.610634 apache-airflow-providers-oracle-3.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12425 2023-06-20 11:29:00.000000 apache-airflow-providers-oracle-3.7.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:01.480547 apache-airflow-providers-oracle-3.7.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:01.482410 apache-airflow-providers-oracle-3.7.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:01.533418 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:01.543562 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/example_dags/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/example_dags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/example_dags/example_oracle.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-06-20 11:29:00.000000 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:01.553171 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17488 2023-06-05 12:50:36.000000 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/hooks/oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:01.564496 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4111 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/operators/oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:01.574122 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3647 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/transfers/oracle_to_oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:01.605671 apache-airflow-providers-oracle-3.7.1/apache_airflow_providers_oracle.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13999 2023-06-20 11:29:01.000000 apache-airflow-providers-oracle-3.7.1/apache_airflow_providers_oracle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      924 2023-06-20 11:29:01.000000 apache-airflow-providers-oracle-3.7.1/apache_airflow_providers_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:01.000000 apache-airflow-providers-oracle-3.7.1/apache_airflow_providers_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:29:01.000000 apache-airflow-providers-oracle-3.7.1/apache_airflow_providers_oracle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:01.000000 apache-airflow-providers-oracle-3.7.1/apache_airflow_providers_oracle.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-20 11:29:01.000000 apache-airflow-providers-oracle-3.7.1/apache_airflow_providers_oracle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:01.000000 apache-airflow-providers-oracle-3.7.1/apache_airflow_providers_oracle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-oracle-3.7.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1882 2023-06-20 11:29:01.612807 apache-airflow-providers-oracle-3.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1711 2023-06-20 11:29:00.000000 apache-airflow-providers-oracle-3.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.127364 apache-airflow-providers-oracle-3.7.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-oracle-3.7.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14005 2023-06-20 11:42:47.128474 apache-airflow-providers-oracle-3.7.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12428 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.026099 apache-airflow-providers-oracle-3.7.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.027356 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.070602 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.077652 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/example_dags/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/example_dags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/example_dags/example_oracle.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.084818 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17488 2023-06-05 12:50:36.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/hooks/oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.092233 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4111 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/operators/oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.099114 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3647 2023-06-01 06:14:28.000000 apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:47.125104 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14005 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      924 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:46.000000 apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-oracle-3.7.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-06-20 11:42:47.130389 apache-airflow-providers-oracle-3.7.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-06-20 11:42:45.000000 apache-airflow-providers-oracle-3.7.1rc1/setup.py
```

### Comparing `apache-airflow-providers-oracle-3.7.1/LICENSE` & `apache-airflow-providers-oracle-3.7.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/MANIFEST.in` & `apache-airflow-providers-oracle-3.7.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/PKG-INFO` & `apache-airflow-providers-oracle-3.7.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-oracle
-Version: 3.7.1
+Version: 3.7.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-oracle package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.1/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.7.1``
+Release: ``3.7.1rc1``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-oracle-3.7.1/README.rst` & `apache-airflow-providers-oracle-3.7.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.7.1``
+Release: ``3.7.1rc1``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/__init__.py` & `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/example_dags/__init__.py` & `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/example_dags/example_oracle.py` & `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/example_dags/example_oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/get_provider_info.py` & `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/hooks/__init__.py` & `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/hooks/oracle.py` & `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/hooks/oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/operators/__init__.py` & `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/operators/oracle.py` & `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/operators/oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/transfers/__init__.py` & `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/airflow/providers/oracle/transfers/oracle_to_oracle.py` & `apache-airflow-providers-oracle-3.7.1rc1/airflow/providers/oracle/transfers/oracle_to_oracle.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/apache_airflow_providers_oracle.egg-info/PKG-INFO` & `apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-oracle
-Version: 3.7.1
+Version: 3.7.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-oracle package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-oracle/3.7.1/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-oracle``
 
-Release: ``3.7.1``
+Release: ``3.7.1rc1``
 
 
 `Oracle <https://www.oracle.com/en/database/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-oracle-3.7.1/apache_airflow_providers_oracle.egg-info/SOURCES.txt` & `apache-airflow-providers-oracle-3.7.1rc1/apache_airflow_providers_oracle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/pyproject.toml` & `apache-airflow-providers-oracle-3.7.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-oracle-3.7.1/setup.cfg` & `apache-airflow-providers-oracle-3.7.1rc1/setup.cfg`

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
 	oracledb>=1.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.oracle.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.oracle
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-oracle-3.7.1/setup.py` & `apache-airflow-providers-oracle-3.7.1rc1/setup.py`

 * *Files identical despite different names*

