# Comparing `tmp/apache-airflow-providers-arangodb-2.2.1.tar.gz` & `tmp/apache-airflow-providers-arangodb-2.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-arangodb-2.2.1.tar", last modified: Tue Jun 20 11:27:43 2023, max compression
+gzip compressed data, was "apache-airflow-providers-arangodb-2.2.1rc1.tar", last modified: Tue Jun 20 11:41:33 2023, max compression
```

## Comparing `apache-airflow-providers-arangodb-2.2.1.tar` & `apache-airflow-providers-arangodb-2.2.1rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:43.333080 apache-airflow-providers-arangodb-2.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-arangodb-2.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:42.000000 apache-airflow-providers-arangodb-2.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-arangodb-2.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7524 2023-06-20 11:27:43.333857 apache-airflow-providers-arangodb-2.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5993 2023-06-20 11:27:42.000000 apache-airflow-providers-arangodb-2.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:43.238244 apache-airflow-providers-arangodb-2.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:43.239319 apache-airflow-providers-arangodb-2.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:43.276655 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:43.283249 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/example_dags/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/example_dags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2210 2023-06-01 06:14:28.000000 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/example_dags/example_arangodb.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-06-20 11:27:42.000000 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:43.289522 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5502 2023-06-01 07:44:14.000000 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/hooks/arangodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:43.296131 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2403 2023-06-02 11:31:21.000000 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/operators/arangodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:43.302511 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-06-02 11:31:21.000000 apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/sensors/arangodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:43.329394 apache-airflow-providers-arangodb-2.2.1/apache_airflow_providers_arangodb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7524 2023-06-20 11:27:43.000000 apache-airflow-providers-arangodb-2.2.1/apache_airflow_providers_arangodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-20 11:27:43.000000 apache-airflow-providers-arangodb-2.2.1/apache_airflow_providers_arangodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:43.000000 apache-airflow-providers-arangodb-2.2.1/apache_airflow_providers_arangodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:27:43.000000 apache-airflow-providers-arangodb-2.2.1/apache_airflow_providers_arangodb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:43.000000 apache-airflow-providers-arangodb-2.2.1/apache_airflow_providers_arangodb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 11:27:43.000000 apache-airflow-providers-arangodb-2.2.1/apache_airflow_providers_arangodb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:43.000000 apache-airflow-providers-arangodb-2.2.1/apache_airflow_providers_arangodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-arangodb-2.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1855 2023-06-20 11:27:43.336191 apache-airflow-providers-arangodb-2.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:27:42.000000 apache-airflow-providers-arangodb-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:33.752347 apache-airflow-providers-arangodb-2.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-arangodb-2.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:32.000000 apache-airflow-providers-arangodb-2.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-arangodb-2.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     7530 2023-06-20 11:41:33.752928 apache-airflow-providers-arangodb-2.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-06-20 11:41:32.000000 apache-airflow-providers-arangodb-2.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:33.665444 apache-airflow-providers-arangodb-2.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:33.666679 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:33.703767 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:33.709466 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/example_dags/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/example_dags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-06-01 06:14:28.000000 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/example_dags/example_arangodb.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-06-20 11:41:32.000000 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:33.715259 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5502 2023-06-01 07:44:14.000000 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/hooks/arangodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:33.720994 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-06-02 11:31:21.000000 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/operators/arangodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:33.726783 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2023-06-02 11:31:21.000000 apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/sensors/arangodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:33.750063 apache-airflow-providers-arangodb-2.2.1rc1/apache_airflow_providers_arangodb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7530 2023-06-20 11:41:33.000000 apache-airflow-providers-arangodb-2.2.1rc1/apache_airflow_providers_arangodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-20 11:41:33.000000 apache-airflow-providers-arangodb-2.2.1rc1/apache_airflow_providers_arangodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:33.000000 apache-airflow-providers-arangodb-2.2.1rc1/apache_airflow_providers_arangodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:41:33.000000 apache-airflow-providers-arangodb-2.2.1rc1/apache_airflow_providers_arangodb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:33.000000 apache-airflow-providers-arangodb-2.2.1rc1/apache_airflow_providers_arangodb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-20 11:41:33.000000 apache-airflow-providers-arangodb-2.2.1rc1/apache_airflow_providers_arangodb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:33.000000 apache-airflow-providers-arangodb-2.2.1rc1/apache_airflow_providers_arangodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-arangodb-2.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-06-20 11:41:33.754932 apache-airflow-providers-arangodb-2.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:41:32.000000 apache-airflow-providers-arangodb-2.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-arangodb-2.2.1/LICENSE` & `apache-airflow-providers-arangodb-2.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/MANIFEST.in` & `apache-airflow-providers-arangodb-2.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/PKG-INFO` & `apache-airflow-providers-arangodb-2.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-arangodb
-Version: 2.2.1
+Version: 2.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-arangodb package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-arangodb/2.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-arangodb``
 
-Release: ``2.2.1``
+Release: ``2.2.1rc1``
 
 
 `ArangoDB <https://www.arangodb.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-arangodb-2.2.1/README.rst` & `apache-airflow-providers-arangodb-2.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-arangodb``
 
-Release: ``2.2.1``
+Release: ``2.2.1rc1``
 
 
 `ArangoDB <https://www.arangodb.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/__init__.py` & `apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/example_dags/__init__.py` & `apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/example_dags/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/example_dags/example_arangodb.py` & `apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/example_dags/example_arangodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/get_provider_info.py` & `apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/hooks/__init__.py` & `apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/hooks/arangodb.py` & `apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/hooks/arangodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/operators/__init__.py` & `apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/operators/arangodb.py` & `apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/operators/arangodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/sensors/__init__.py` & `apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/airflow/providers/arangodb/sensors/arangodb.py` & `apache-airflow-providers-arangodb-2.2.1rc1/airflow/providers/arangodb/sensors/arangodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/apache_airflow_providers_arangodb.egg-info/PKG-INFO` & `apache-airflow-providers-arangodb-2.2.1rc1/apache_airflow_providers_arangodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-arangodb
-Version: 2.2.1
+Version: 2.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-arangodb package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-arangodb/2.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-arangodb``
 
-Release: ``2.2.1``
+Release: ``2.2.1rc1``
 
 
 `ArangoDB <https://www.arangodb.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-arangodb-2.2.1/apache_airflow_providers_arangodb.egg-info/SOURCES.txt` & `apache-airflow-providers-arangodb-2.2.1rc1/apache_airflow_providers_arangodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/pyproject.toml` & `apache-airflow-providers-arangodb-2.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-arangodb-2.2.1/setup.cfg` & `apache-airflow-providers-arangodb-2.2.1rc1/setup.cfg`

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
 	python-arango>=7.3.2
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.arangodb.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.arangodb
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-arangodb-2.2.1/setup.py` & `apache-airflow-providers-arangodb-2.2.1rc1/setup.py`

 * *Files identical despite different names*

