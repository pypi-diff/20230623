# Comparing `tmp/apache-airflow-providers-neo4j-3.3.1.tar.gz` & `tmp/apache-airflow-providers-neo4j-3.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-neo4j-3.3.1.tar", last modified: Tue Jun 20 11:28:52 2023, max compression
+gzip compressed data, was "apache-airflow-providers-neo4j-3.3.1rc1.tar", last modified: Tue Jun 20 11:42:39 2023, max compression
```

## Comparing `apache-airflow-providers-neo4j-3.3.1.tar` & `apache-airflow-providers-neo4j-3.3.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:52.048254 apache-airflow-providers-neo4j-3.3.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-neo4j-3.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:50.000000 apache-airflow-providers-neo4j-3.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-neo4j-3.3.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11316 2023-06-20 11:28:52.049445 apache-airflow-providers-neo4j-3.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9794 2023-06-20 11:28:50.000000 apache-airflow-providers-neo4j-3.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:51.956056 apache-airflow-providers-neo4j-3.3.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:51.957367 apache-airflow-providers-neo4j-3.3.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:51.995323 apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-06-20 11:28:50.000000 apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:52.005244 apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4347 2023-06-02 11:31:21.000000 apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/hooks/neo4j.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:52.012959 apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2052 2023-06-02 11:31:21.000000 apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/operators/neo4j.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:52.045431 apache-airflow-providers-neo4j-3.3.1/apache_airflow_providers_neo4j.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11316 2023-06-20 11:28:51.000000 apache-airflow-providers-neo4j-3.3.1/apache_airflow_providers_neo4j.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-20 11:28:51.000000 apache-airflow-providers-neo4j-3.3.1/apache_airflow_providers_neo4j.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:51.000000 apache-airflow-providers-neo4j-3.3.1/apache_airflow_providers_neo4j.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:28:51.000000 apache-airflow-providers-neo4j-3.3.1/apache_airflow_providers_neo4j.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:51.000000 apache-airflow-providers-neo4j-3.3.1/apache_airflow_providers_neo4j.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-20 11:28:51.000000 apache-airflow-providers-neo4j-3.3.1/apache_airflow_providers_neo4j.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:51.000000 apache-airflow-providers-neo4j-3.3.1/apache_airflow_providers_neo4j.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-neo4j-3.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1829 2023-06-20 11:28:52.051807 apache-airflow-providers-neo4j-3.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1632 2023-06-20 11:28:50.000000 apache-airflow-providers-neo4j-3.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:39.726548 apache-airflow-providers-neo4j-3.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-neo4j-3.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:38.000000 apache-airflow-providers-neo4j-3.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-neo4j-3.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11322 2023-06-20 11:42:39.727611 apache-airflow-providers-neo4j-3.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9797 2023-06-20 11:42:38.000000 apache-airflow-providers-neo4j-3.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:39.650579 apache-airflow-providers-neo4j-3.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:39.651677 apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:39.684407 apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-20 11:42:38.000000 apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:39.690070 apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4347 2023-06-02 11:31:21.000000 apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/hooks/neo4j.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:39.695889 apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-06-02 11:31:21.000000 apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/operators/neo4j.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:39.724226 apache-airflow-providers-neo4j-3.3.1rc1/apache_airflow_providers_neo4j.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11322 2023-06-20 11:42:39.000000 apache-airflow-providers-neo4j-3.3.1rc1/apache_airflow_providers_neo4j.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      701 2023-06-20 11:42:39.000000 apache-airflow-providers-neo4j-3.3.1rc1/apache_airflow_providers_neo4j.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:39.000000 apache-airflow-providers-neo4j-3.3.1rc1/apache_airflow_providers_neo4j.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:42:39.000000 apache-airflow-providers-neo4j-3.3.1rc1/apache_airflow_providers_neo4j.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:39.000000 apache-airflow-providers-neo4j-3.3.1rc1/apache_airflow_providers_neo4j.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-20 11:42:39.000000 apache-airflow-providers-neo4j-3.3.1rc1/apache_airflow_providers_neo4j.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:39.000000 apache-airflow-providers-neo4j-3.3.1rc1/apache_airflow_providers_neo4j.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-neo4j-3.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1837 2023-06-20 11:42:39.729515 apache-airflow-providers-neo4j-3.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-06-20 11:42:38.000000 apache-airflow-providers-neo4j-3.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-neo4j-3.3.1/LICENSE` & `apache-airflow-providers-neo4j-3.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.3.1/MANIFEST.in` & `apache-airflow-providers-neo4j-3.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.3.1/PKG-INFO` & `apache-airflow-providers-neo4j-3.3.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-neo4j
-Version: 3.3.1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-neo4j package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.3.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-neo4j``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Neo4j <https://neo4j.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-neo4j-3.3.1/README.rst` & `apache-airflow-providers-neo4j-3.3.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-neo4j``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Neo4j <https://neo4j.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/__init__.py` & `apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/get_provider_info.py` & `apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/hooks/__init__.py` & `apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/hooks/neo4j.py` & `apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/hooks/neo4j.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/operators/__init__.py` & `apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.3.1/airflow/providers/neo4j/operators/neo4j.py` & `apache-airflow-providers-neo4j-3.3.1rc1/airflow/providers/neo4j/operators/neo4j.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.3.1/apache_airflow_providers_neo4j.egg-info/PKG-INFO` & `apache-airflow-providers-neo4j-3.3.1rc1/apache_airflow_providers_neo4j.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-neo4j
-Version: 3.3.1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-neo4j package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-neo4j/3.3.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-neo4j``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Neo4j <https://neo4j.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-neo4j-3.3.1/apache_airflow_providers_neo4j.egg-info/SOURCES.txt` & `apache-airflow-providers-neo4j-3.3.1rc1/apache_airflow_providers_neo4j.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.3.1/pyproject.toml` & `apache-airflow-providers-neo4j-3.3.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-neo4j-3.3.1/setup.cfg` & `apache-airflow-providers-neo4j-3.3.1rc1/setup.cfg`

 * *Files 9% similar despite different names*

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
 	neo4j>=4.2.1
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.neo4j.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.neo4j
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-neo4j-3.3.1/setup.py` & `apache-airflow-providers-neo4j-3.3.1rc1/setup.py`

 * *Files identical despite different names*

