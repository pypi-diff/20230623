# Comparing `tmp/apache-airflow-providers-apache-impala-1.1.1.tar.gz` & `tmp/apache-airflow-providers-apache-impala-1.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-impala-1.1.1.tar", last modified: Tue Jun 20 11:27:28 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-impala-1.1.1rc1.tar", last modified: Tue Jun 20 11:41:19 2023, max compression
```

## Comparing `apache-airflow-providers-apache-impala-1.1.1.tar` & `apache-airflow-providers-apache-impala-1.1.1rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:28.675381 apache-airflow-providers-apache-impala-1.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:27.000000 apache-airflow-providers-apache-impala-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6762 2023-06-20 11:27:28.675992 apache-airflow-providers-apache-impala-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5189 2023-06-20 11:27:27.000000 apache-airflow-providers-apache-impala-1.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:28.611243 apache-airflow-providers-apache-impala-1.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:28.612458 apache-airflow-providers-apache-impala-1.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:28.613489 apache-airflow-providers-apache-impala-1.1.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:28.642998 apache-airflow-providers-apache-impala-1.1.1/airflow/providers/apache/impala/
--rw-r--r--   0 root         (0) root         (0)     1538 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-impala-1.1.1/airflow/providers/apache/impala/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-06-20 11:27:27.000000 apache-airflow-providers-apache-impala-1.1.1/airflow/providers/apache/impala/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:28.649022 apache-airflow-providers-apache-impala-1.1.1/airflow/providers/apache/impala/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.1/airflow/providers/apache/impala/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.1/airflow/providers/apache/impala/hooks/impala.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:28.672541 apache-airflow-providers-apache-impala-1.1.1/apache_airflow_providers_apache_impala.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6762 2023-06-20 11:27:28.000000 apache-airflow-providers-apache-impala-1.1.1/apache_airflow_providers_apache_impala.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-20 11:27:28.000000 apache-airflow-providers-apache-impala-1.1.1/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:28.000000 apache-airflow-providers-apache-impala-1.1.1/apache_airflow_providers_apache_impala.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-20 11:27:28.000000 apache-airflow-providers-apache-impala-1.1.1/apache_airflow_providers_apache_impala.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:28.000000 apache-airflow-providers-apache-impala-1.1.1/apache_airflow_providers_apache_impala.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       92 2023-06-20 11:27:28.000000 apache-airflow-providers-apache-impala-1.1.1/apache_airflow_providers_apache_impala.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:28.000000 apache-airflow-providers-apache-impala-1.1.1/apache_airflow_providers_apache_impala.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-impala-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1884 2023-06-20 11:27:28.677959 apache-airflow-providers-apache-impala-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1733 2023-06-20 11:27:27.000000 apache-airflow-providers-apache-impala-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.429555 apache-airflow-providers-apache-impala-1.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:18.000000 apache-airflow-providers-apache-impala-1.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-impala-1.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6768 2023-06-20 11:41:19.430172 apache-airflow-providers-apache-impala-1.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5192 2023-06-20 11:41:18.000000 apache-airflow-providers-apache-impala-1.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.363952 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.365284 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.366795 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.397920 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-06-20 11:41:18.000000 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.403483 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/hooks/impala.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:19.426877 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6768 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      701 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       97 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:19.000000 apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-impala-1.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-20 11:41:19.432158 apache-airflow-providers-apache-impala-1.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-06-20 11:41:18.000000 apache-airflow-providers-apache-impala-1.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-impala-1.1.1/LICENSE` & `apache-airflow-providers-apache-impala-1.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1/MANIFEST.in` & `apache-airflow-providers-apache-impala-1.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1/PKG-INFO` & `apache-airflow-providers-apache-impala-1.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-impala
-Version: 1.1.1
+Version: 1.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-impala package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-impala``
 
-Release: ``1.1.1``
+Release: ``1.1.1rc1``
 
 
 `Apache Impala <https://impala.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-impala-1.1.1/README.rst` & `apache-airflow-providers-apache-impala-1.1.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-impala``
 
-Release: ``1.1.1``
+Release: ``1.1.1rc1``
 
 
 `Apache Impala <https://impala.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-impala-1.1.1/airflow/providers/apache/impala/__init__.py` & `apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1/airflow/providers/apache/impala/get_provider_info.py` & `apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1/airflow/providers/apache/impala/hooks/__init__.py` & `apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1/airflow/providers/apache/impala/hooks/impala.py` & `apache-airflow-providers-apache-impala-1.1.1rc1/airflow/providers/apache/impala/hooks/impala.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1/apache_airflow_providers_apache_impala.egg-info/PKG-INFO` & `apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-impala
-Version: 1.1.1
+Version: 1.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-impala package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-impala/1.1.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-impala``
 
-Release: ``1.1.1``
+Release: ``1.1.1rc1``
 
 
 `Apache Impala <https://impala.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-impala-1.1.1/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-impala-1.1.1rc1/apache_airflow_providers_apache_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1/pyproject.toml` & `apache-airflow-providers-apache-impala-1.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-impala-1.1.1/setup.cfg` & `apache-airflow-providers-apache-impala-1.1.1rc1/setup.cfg`

 * *Files 5% similar despite different names*

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
 	impyla>=0.18.0,<1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.impala.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.impala
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-impala-1.1.1/setup.py` & `apache-airflow-providers-apache-impala-1.1.1rc1/setup.py`

 * *Files identical despite different names*

