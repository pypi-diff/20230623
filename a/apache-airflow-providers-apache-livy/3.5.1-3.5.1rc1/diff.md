# Comparing `tmp/apache-airflow-providers-apache-livy-3.5.1.tar.gz` & `tmp/apache-airflow-providers-apache-livy-3.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-livy-3.5.1.tar", last modified: Tue Jun 20 11:27:33 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-livy-3.5.1rc1.tar", last modified: Tue Jun 20 11:41:24 2023, max compression
```

## Comparing `apache-airflow-providers-apache-livy-3.5.1.tar` & `apache-airflow-providers-apache-livy-3.5.1rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:33.922685 apache-airflow-providers-apache-livy-3.5.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:32.000000 apache-airflow-providers-apache-livy-3.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13004 2023-06-20 11:27:33.923715 apache-airflow-providers-apache-livy-3.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11443 2023-06-20 11:27:32.000000 apache-airflow-providers-apache-livy-3.5.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:33.832403 apache-airflow-providers-apache-livy-3.5.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:33.833479 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:33.834525 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:33.869154 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3082 2023-06-20 11:27:32.000000 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:33.874800 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31553 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/hooks/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:33.880660 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9572 2023-06-05 12:50:36.000000 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/operators/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:33.886365 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2574 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/sensors/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:33.893572 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6251 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/triggers/livy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:33.920028 apache-airflow-providers-apache-livy-3.5.1/apache_airflow_providers_apache_livy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13004 2023-06-20 11:27:33.000000 apache-airflow-providers-apache-livy-3.5.1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      971 2023-06-20 11:27:33.000000 apache-airflow-providers-apache-livy-3.5.1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:33.000000 apache-airflow-providers-apache-livy-3.5.1/apache_airflow_providers_apache_livy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:27:33.000000 apache-airflow-providers-apache-livy-3.5.1/apache_airflow_providers_apache_livy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:33.000000 apache-airflow-providers-apache-livy-3.5.1/apache_airflow_providers_apache_livy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:27:33.000000 apache-airflow-providers-apache-livy-3.5.1/apache_airflow_providers_apache_livy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:33.000000 apache-airflow-providers-apache-livy-3.5.1/apache_airflow_providers_apache_livy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-livy-3.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1900 2023-06-20 11:27:33.925577 apache-airflow-providers-apache-livy-3.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-20 11:27:32.000000 apache-airflow-providers-apache-livy-3.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.829920 apache-airflow-providers-apache-livy-3.5.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-livy-3.5.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13010 2023-06-20 11:41:24.831002 apache-airflow-providers-apache-livy-3.5.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11446 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.735007 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.736232 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.737260 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.773034 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.778826 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31553 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.785185 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9572 2023-06-05 12:50:36.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.793079 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.798737 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/livy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:24.827293 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13010 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      971 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:24.000000 apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-livy-3.5.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1908 2023-06-20 11:41:24.833029 apache-airflow-providers-apache-livy-3.5.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-20 11:41:23.000000 apache-airflow-providers-apache-livy-3.5.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-livy-3.5.1/LICENSE` & `apache-airflow-providers-apache-livy-3.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/MANIFEST.in` & `apache-airflow-providers-apache-livy-3.5.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/PKG-INFO` & `apache-airflow-providers-apache-livy-3.5.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-livy
-Version: 3.5.1
+Version: 3.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-livy package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.5.1``
+Release: ``3.5.1rc1``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-livy-3.5.1/README.rst` & `apache-airflow-providers-apache-livy-3.5.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.5.1``
+Release: ``3.5.1rc1``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/__init__.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/get_provider_info.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/hooks/__init__.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/hooks/livy.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/hooks/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/operators/__init__.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/operators/livy.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/operators/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/sensors/__init__.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/sensors/livy.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/sensors/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/triggers/__init__.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/airflow/providers/apache/livy/triggers/livy.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/airflow/providers/apache/livy/triggers/livy.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO` & `apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-livy
-Version: 3.5.1
+Version: 3.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-livy package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-livy/3.5.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-livy``
 
-Release: ``3.5.1``
+Release: ``3.5.1rc1``
 
 
 `Apache Livy <https://livy.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-livy-3.5.1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-livy-3.5.1rc1/apache_airflow_providers_apache_livy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/pyproject.toml` & `apache-airflow-providers-apache-livy-3.5.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-livy-3.5.1/setup.cfg` & `apache-airflow-providers-apache-livy-3.5.1rc1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -44,21 +44,21 @@
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	aiohttp
 	apache-airflow-providers-http
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	asgiref
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.livy.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.livy
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-livy-3.5.1/setup.py` & `apache-airflow-providers-apache-livy-3.5.1rc1/setup.py`

 * *Files identical despite different names*

