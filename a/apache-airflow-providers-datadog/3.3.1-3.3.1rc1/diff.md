# Comparing `tmp/apache-airflow-providers-datadog-3.3.1.tar.gz` & `tmp/apache-airflow-providers-datadog-3.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-datadog-3.3.1.tar", last modified: Tue Jun 20 11:27:58 2023, max compression
+gzip compressed data, was "apache-airflow-providers-datadog-3.3.1rc1.tar", last modified: Tue Jun 20 11:41:49 2023, max compression
```

## Comparing `apache-airflow-providers-datadog-3.3.1.tar` & `apache-airflow-providers-datadog-3.3.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:58.149744 apache-airflow-providers-datadog-3.3.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-datadog-3.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:57.000000 apache-airflow-providers-datadog-3.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-datadog-3.3.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10195 2023-06-20 11:27:58.150764 apache-airflow-providers-datadog-3.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8667 2023-06-20 11:27:57.000000 apache-airflow-providers-datadog-3.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:58.074105 apache-airflow-providers-datadog-3.3.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:58.075381 apache-airflow-providers-datadog-3.3.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:58.111335 apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2370 2023-06-20 11:27:57.000000 apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:58.117139 apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7321 2023-06-02 11:31:21.000000 apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/hooks/datadog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:58.122831 apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4060 2023-06-01 06:14:28.000000 apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/sensors/datadog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:58.147133 apache-airflow-providers-datadog-3.3.1/apache_airflow_providers_datadog.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10195 2023-06-20 11:27:58.000000 apache-airflow-providers-datadog-3.3.1/apache_airflow_providers_datadog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      727 2023-06-20 11:27:58.000000 apache-airflow-providers-datadog-3.3.1/apache_airflow_providers_datadog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:58.000000 apache-airflow-providers-datadog-3.3.1/apache_airflow_providers_datadog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:27:58.000000 apache-airflow-providers-datadog-3.3.1/apache_airflow_providers_datadog.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:58.000000 apache-airflow-providers-datadog-3.3.1/apache_airflow_providers_datadog.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 11:27:58.000000 apache-airflow-providers-datadog-3.3.1/apache_airflow_providers_datadog.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:58.000000 apache-airflow-providers-datadog-3.3.1/apache_airflow_providers_datadog.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-datadog-3.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1844 2023-06-20 11:27:58.152647 apache-airflow-providers-datadog-3.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:27:57.000000 apache-airflow-providers-datadog-3.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:49.219586 apache-airflow-providers-datadog-3.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-datadog-3.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:48.000000 apache-airflow-providers-datadog-3.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-datadog-3.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10201 2023-06-20 11:41:49.220613 apache-airflow-providers-datadog-3.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8670 2023-06-20 11:41:48.000000 apache-airflow-providers-datadog-3.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:49.144909 apache-airflow-providers-datadog-3.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:49.146218 apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:49.179510 apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-06-20 11:41:48.000000 apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:49.185768 apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7321 2023-06-02 11:31:21.000000 apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/hooks/datadog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:49.191623 apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4060 2023-06-01 06:14:28.000000 apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/sensors/datadog.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:49.216825 apache-airflow-providers-datadog-3.3.1rc1/apache_airflow_providers_datadog.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10201 2023-06-20 11:41:49.000000 apache-airflow-providers-datadog-3.3.1rc1/apache_airflow_providers_datadog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      727 2023-06-20 11:41:49.000000 apache-airflow-providers-datadog-3.3.1rc1/apache_airflow_providers_datadog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:49.000000 apache-airflow-providers-datadog-3.3.1rc1/apache_airflow_providers_datadog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:41:49.000000 apache-airflow-providers-datadog-3.3.1rc1/apache_airflow_providers_datadog.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:49.000000 apache-airflow-providers-datadog-3.3.1rc1/apache_airflow_providers_datadog.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 11:41:49.000000 apache-airflow-providers-datadog-3.3.1rc1/apache_airflow_providers_datadog.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:49.000000 apache-airflow-providers-datadog-3.3.1rc1/apache_airflow_providers_datadog.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-datadog-3.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-06-20 11:41:49.222586 apache-airflow-providers-datadog-3.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:41:48.000000 apache-airflow-providers-datadog-3.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-datadog-3.3.1/LICENSE` & `apache-airflow-providers-datadog-3.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.3.1/MANIFEST.in` & `apache-airflow-providers-datadog-3.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.3.1/PKG-INFO` & `apache-airflow-providers-datadog-3.3.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-datadog
-Version: 3.3.1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-datadog package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.3.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-datadog``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Datadog <https://www.datadoghq.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-datadog-3.3.1/README.rst` & `apache-airflow-providers-datadog-3.3.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-datadog``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Datadog <https://www.datadoghq.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/__init__.py` & `apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/get_provider_info.py` & `apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/hooks/__init__.py` & `apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/hooks/datadog.py` & `apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/hooks/datadog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/sensors/__init__.py` & `apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.3.1/airflow/providers/datadog/sensors/datadog.py` & `apache-airflow-providers-datadog-3.3.1rc1/airflow/providers/datadog/sensors/datadog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.3.1/apache_airflow_providers_datadog.egg-info/PKG-INFO` & `apache-airflow-providers-datadog-3.3.1rc1/apache_airflow_providers_datadog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-datadog
-Version: 3.3.1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-datadog package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-datadog/3.3.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-datadog``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Datadog <https://www.datadoghq.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-datadog-3.3.1/apache_airflow_providers_datadog.egg-info/SOURCES.txt` & `apache-airflow-providers-datadog-3.3.1rc1/apache_airflow_providers_datadog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.3.1/pyproject.toml` & `apache-airflow-providers-datadog-3.3.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-datadog-3.3.1/setup.cfg` & `apache-airflow-providers-datadog-3.3.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

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
 	datadog>=0.14.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.datadog.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.datadog
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-datadog-3.3.1/setup.py` & `apache-airflow-providers-datadog-3.3.1rc1/setup.py`

 * *Files identical despite different names*

