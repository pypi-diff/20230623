# Comparing `tmp/apache-airflow-providers-influxdb-2.2.1.tar.gz` & `tmp/apache-airflow-providers-influxdb-2.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-influxdb-2.2.1.tar", last modified: Tue Jun 20 11:28:31 2023, max compression
+gzip compressed data, was "apache-airflow-providers-influxdb-2.2.1rc1.tar", last modified: Tue Jun 20 11:42:22 2023, max compression
```

## Comparing `apache-airflow-providers-influxdb-2.2.1.tar` & `apache-airflow-providers-influxdb-2.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:31.522447 apache-airflow-providers-influxdb-2.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-influxdb-2.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:30.000000 apache-airflow-providers-influxdb-2.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-influxdb-2.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8948 2023-06-20 11:28:31.524014 apache-airflow-providers-influxdb-2.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7417 2023-06-20 11:28:30.000000 apache-airflow-providers-influxdb-2.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:31.421870 apache-airflow-providers-influxdb-2.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:31.422951 apache-airflow-providers-influxdb-2.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:31.460633 apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-06-20 11:28:30.000000 apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:31.470256 apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-06-08 05:42:54.000000 apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/hooks/influxdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:31.481323 apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-06-02 11:31:21.000000 apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/operators/influxdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:31.518520 apache-airflow-providers-influxdb-2.2.1/apache_airflow_providers_influxdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8948 2023-06-20 11:28:31.000000 apache-airflow-providers-influxdb-2.2.1/apache_airflow_providers_influxdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:28:31.000000 apache-airflow-providers-influxdb-2.2.1/apache_airflow_providers_influxdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:31.000000 apache-airflow-providers-influxdb-2.2.1/apache_airflow_providers_influxdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:28:31.000000 apache-airflow-providers-influxdb-2.2.1/apache_airflow_providers_influxdb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:31.000000 apache-airflow-providers-influxdb-2.2.1/apache_airflow_providers_influxdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-20 11:28:31.000000 apache-airflow-providers-influxdb-2.2.1/apache_airflow_providers_influxdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:31.000000 apache-airflow-providers-influxdb-2.2.1/apache_airflow_providers_influxdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-influxdb-2.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1876 2023-06-20 11:28:31.528349 apache-airflow-providers-influxdb-2.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:28:30.000000 apache-airflow-providers-influxdb-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.140363 apache-airflow-providers-influxdb-2.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-influxdb-2.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:21.000000 apache-airflow-providers-influxdb-2.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-influxdb-2.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8954 2023-06-20 11:42:22.141500 apache-airflow-providers-influxdb-2.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7420 2023-06-20 11:42:21.000000 apache-airflow-providers-influxdb-2.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.061728 apache-airflow-providers-influxdb-2.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.062916 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.098077 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-06-20 11:42:21.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.104101 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-06-08 05:42:54.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/hooks/influxdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.110916 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-06-02 11:31:21.000000 apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/operators/influxdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:22.136226 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8954 2023-06-20 11:42:21.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       68 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:22.000000 apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-influxdb-2.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-06-20 11:42:22.143583 apache-airflow-providers-influxdb-2.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:42:20.000000 apache-airflow-providers-influxdb-2.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-influxdb-2.2.1/LICENSE` & `apache-airflow-providers-influxdb-2.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.1/MANIFEST.in` & `apache-airflow-providers-influxdb-2.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.1/PKG-INFO` & `apache-airflow-providers-influxdb-2.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-influxdb
-Version: 2.2.1
+Version: 2.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-influxdb package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-influxdb``
 
-Release: ``2.2.1``
+Release: ``2.2.1rc1``
 
 
 `InfluxDB <https://www.influxdata.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-influxdb-2.2.1/README.rst` & `apache-airflow-providers-influxdb-2.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-influxdb``
 
-Release: ``2.2.1``
+Release: ``2.2.1rc1``
 
 
 `InfluxDB <https://www.influxdata.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/__init__.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/get_provider_info.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/hooks/__init__.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/hooks/influxdb.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/hooks/influxdb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/operators/__init__.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.1/airflow/providers/influxdb/operators/influxdb.py` & `apache-airflow-providers-influxdb-2.2.1rc1/airflow/providers/influxdb/operators/influxdb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.1/apache_airflow_providers_influxdb.egg-info/PKG-INFO` & `apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-influxdb
-Version: 2.2.1
+Version: 2.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-influxdb package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-influxdb/2.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-influxdb``
 
-Release: ``2.2.1``
+Release: ``2.2.1rc1``
 
 
 `InfluxDB <https://www.influxdata.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-influxdb-2.2.1/apache_airflow_providers_influxdb.egg-info/SOURCES.txt` & `apache-airflow-providers-influxdb-2.2.1rc1/apache_airflow_providers_influxdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.1/pyproject.toml` & `apache-airflow-providers-influxdb-2.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-influxdb-2.2.1/setup.cfg` & `apache-airflow-providers-influxdb-2.2.1rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	influxdb-client>=1.19.0
 	requests>=2.26.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.influxdb.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.influxdb
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-influxdb-2.2.1/setup.py` & `apache-airflow-providers-influxdb-2.2.1rc1/setup.py`

 * *Files identical despite different names*

