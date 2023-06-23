# Comparing `tmp/apache-airflow-providers-apache-cassandra-3.2.1.tar.gz` & `tmp/apache-airflow-providers-apache-cassandra-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-cassandra-3.2.1.tar", last modified: Tue Jun 20 11:27:18 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-cassandra-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:08 2023, max compression
```

## Comparing `apache-airflow-providers-apache-cassandra-3.2.1.tar` & `apache-airflow-providers-apache-cassandra-3.2.1rc1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:18.078773 apache-airflow-providers-apache-cassandra-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-cassandra-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:17.000000 apache-airflow-providers-apache-cassandra-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-cassandra-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11143 2023-06-20 11:27:18.079737 apache-airflow-providers-apache-cassandra-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9588 2023-06-20 11:27:17.000000 apache-airflow-providers-apache-cassandra-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:17.997830 apache-airflow-providers-apache-cassandra-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:17.998905 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:17.999996 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:18.035130 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/
--rw-r--r--   0 root         (0) root         (0)     1541 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-06-20 11:27:17.000000 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:18.040937 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7874 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/hooks/cassandra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:18.051852 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/sensors/record.py
--rw-r--r--   0 root         (0) root         (0)     2543 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/sensors/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:18.076454 apache-airflow-providers-apache-cassandra-3.2.1/apache_airflow_providers_apache_cassandra.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11143 2023-06-20 11:27:17.000000 apache-airflow-providers-apache-cassandra-3.2.1/apache_airflow_providers_apache_cassandra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      897 2023-06-20 11:27:17.000000 apache-airflow-providers-apache-cassandra-3.2.1/apache_airflow_providers_apache_cassandra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:17.000000 apache-airflow-providers-apache-cassandra-3.2.1/apache_airflow_providers_apache_cassandra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-20 11:27:17.000000 apache-airflow-providers-apache-cassandra-3.2.1/apache_airflow_providers_apache_cassandra.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:17.000000 apache-airflow-providers-apache-cassandra-3.2.1/apache_airflow_providers_apache_cassandra.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-20 11:27:17.000000 apache-airflow-providers-apache-cassandra-3.2.1/apache_airflow_providers_apache_cassandra.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:17.000000 apache-airflow-providers-apache-cassandra-3.2.1/apache_airflow_providers_apache_cassandra.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-cassandra-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1907 2023-06-20 11:27:18.081663 apache-airflow-providers-apache-cassandra-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1698 2023-06-20 11:27:17.000000 apache-airflow-providers-apache-cassandra-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.477367 apache-airflow-providers-apache-cassandra-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:07.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11149 2023-06-20 11:41:08.478418 apache-airflow-providers-apache-cassandra-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9591 2023-06-20 11:41:07.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.398358 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.399560 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.400829 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.432494 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/
+-rw-r--r--   0 root         (0) root         (0)     1541 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-06-20 11:41:07.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.438338 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7874 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/hooks/cassandra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.446914 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/record.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:08.475004 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11149 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      897 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:08.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-06-20 11:41:08.480313 apache-airflow-providers-apache-cassandra-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-20 11:41:07.000000 apache-airflow-providers-apache-cassandra-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/LICENSE` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/MANIFEST.in` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/PKG-INFO` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-cassandra
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-cassandra package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-cassandra``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Apache Cassandra <http://cassandra.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/README.rst` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-cassandra``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Apache Cassandra <http://cassandra.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/__init__.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/get_provider_info.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/hooks/__init__.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/hooks/cassandra.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/hooks/cassandra.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/sensors/__init__.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/sensors/record.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/record.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/airflow/providers/apache/cassandra/sensors/table.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/airflow/providers/apache/cassandra/sensors/table.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/apache_airflow_providers_apache_cassandra.egg-info/PKG-INFO` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-cassandra
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-cassandra package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-cassandra/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-cassandra``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Apache Cassandra <http://cassandra.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/apache_airflow_providers_apache_cassandra.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/apache_airflow_providers_apache_cassandra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/pyproject.toml` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/setup.cfg` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -42,21 +42,21 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	cassandra-driver>=3.13.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.cassandra.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.cassandra
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-cassandra-3.2.1/setup.py` & `apache-airflow-providers-apache-cassandra-3.2.1rc1/setup.py`

 * *Files identical despite different names*

