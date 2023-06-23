# Comparing `tmp/apache-airflow-providers-qubole-3.4.1.tar.gz` & `tmp/apache-airflow-providers-qubole-3.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-qubole-3.4.1.tar", last modified: Tue Jun 20 11:29:14 2023, max compression
+gzip compressed data, was "apache-airflow-providers-qubole-3.4.1rc1.tar", last modified: Tue Jun 20 11:42:57 2023, max compression
```

## Comparing `apache-airflow-providers-qubole-3.4.1.tar` & `apache-airflow-providers-qubole-3.4.1rc1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:14.785123 apache-airflow-providers-qubole-3.4.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-qubole-3.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:13.000000 apache-airflow-providers-qubole-3.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-qubole-3.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14370 2023-06-20 11:29:14.786548 apache-airflow-providers-qubole-3.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12818 2023-06-20 11:29:13.000000 apache-airflow-providers-qubole-3.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:14.677359 apache-airflow-providers-qubole-3.4.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:14.678671 apache-airflow-providers-qubole-3.4.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:14.720570 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3310 2023-06-20 11:29:13.000000 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:14.731442 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11222 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/hooks/qubole.py
--rw-r--r--   0 root         (0) root         (0)     4091 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/hooks/qubole_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:14.742547 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12547 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/operators/qubole.py
--rw-r--r--   0 root         (0) root         (0)     8386 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/operators/qubole_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:14.749325 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4240 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/sensors/qubole.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:14.781700 apache-airflow-providers-qubole-3.4.1/apache_airflow_providers_qubole.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14370 2023-06-20 11:29:14.000000 apache-airflow-providers-qubole-3.4.1/apache_airflow_providers_qubole.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      902 2023-06-20 11:29:14.000000 apache-airflow-providers-qubole-3.4.1/apache_airflow_providers_qubole.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:14.000000 apache-airflow-providers-qubole-3.4.1/apache_airflow_providers_qubole.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:29:14.000000 apache-airflow-providers-qubole-3.4.1/apache_airflow_providers_qubole.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:14.000000 apache-airflow-providers-qubole-3.4.1/apache_airflow_providers_qubole.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-20 11:29:14.000000 apache-airflow-providers-qubole-3.4.1/apache_airflow_providers_qubole.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:14.000000 apache-airflow-providers-qubole-3.4.1/apache_airflow_providers_qubole.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-qubole-3.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1882 2023-06-20 11:29:14.788878 apache-airflow-providers-qubole-3.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:29:13.000000 apache-airflow-providers-qubole-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.949615 apache-airflow-providers-qubole-3.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-qubole-3.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:56.000000 apache-airflow-providers-qubole-3.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-qubole-3.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14376 2023-06-20 11:42:57.950640 apache-airflow-providers-qubole-3.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12821 2023-06-20 11:42:56.000000 apache-airflow-providers-qubole-3.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.865399 apache-airflow-providers-qubole-3.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.866678 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.900743 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2023-06-20 11:42:56.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.909317 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11222 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/qubole.py
+-rw-r--r--   0 root         (0) root         (0)     4091 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/qubole_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.917766 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12547 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/qubole.py
+-rw-r--r--   0 root         (0) root         (0)     8386 2023-06-02 11:31:21.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/qubole_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.923568 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-06-01 06:14:28.000000 apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/sensors/qubole.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:57.947039 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14376 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:57.000000 apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-qubole-3.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-06-20 11:42:57.952557 apache-airflow-providers-qubole-3.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:42:56.000000 apache-airflow-providers-qubole-3.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-qubole-3.4.1/LICENSE` & `apache-airflow-providers-qubole-3.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/MANIFEST.in` & `apache-airflow-providers-qubole-3.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/PKG-INFO` & `apache-airflow-providers-qubole-3.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-qubole
-Version: 3.4.1
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-qubole package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-qubole``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `Qubole <https://www.qubole.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-qubole-3.4.1/README.rst` & `apache-airflow-providers-qubole-3.4.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-qubole``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `Qubole <https://www.qubole.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/__init__.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/get_provider_info.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/hooks/__init__.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/hooks/qubole.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/qubole.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/hooks/qubole_check.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/hooks/qubole_check.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/operators/__init__.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/operators/qubole.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/qubole.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/operators/qubole_check.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/operators/qubole_check.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/sensors/__init__.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/airflow/providers/qubole/sensors/qubole.py` & `apache-airflow-providers-qubole-3.4.1rc1/airflow/providers/qubole/sensors/qubole.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/apache_airflow_providers_qubole.egg-info/PKG-INFO` & `apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-qubole
-Version: 3.4.1
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-qubole package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-qubole/3.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-qubole``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `Qubole <https://www.qubole.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-qubole-3.4.1/apache_airflow_providers_qubole.egg-info/SOURCES.txt` & `apache-airflow-providers-qubole-3.4.1rc1/apache_airflow_providers_qubole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/pyproject.toml` & `apache-airflow-providers-qubole-3.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-qubole-3.4.1/setup.cfg` & `apache-airflow-providers-qubole-3.4.1rc1/setup.cfg`

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
 	qds-sdk>=1.10.4
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.qubole.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.qubole
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-qubole-3.4.1/setup.py` & `apache-airflow-providers-qubole-3.4.1rc1/setup.py`

 * *Files identical despite different names*

