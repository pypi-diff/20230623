# Comparing `tmp/apache-airflow-providers-apache-flink-1.1.1.tar.gz` & `tmp/apache-airflow-providers-apache-flink-1.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-flink-1.1.1.tar", last modified: Tue Jun 20 11:27:23 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-flink-1.1.1rc1.tar", last modified: Tue Jun 20 11:41:13 2023, max compression
```

## Comparing `apache-airflow-providers-apache-flink-1.1.1.tar` & `apache-airflow-providers-apache-flink-1.1.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:23.242227 apache-airflow-providers-apache-flink-1.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-flink-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:22.000000 apache-airflow-providers-apache-flink-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-flink-1.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7466 2023-06-20 11:27:23.242764 apache-airflow-providers-apache-flink-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5891 2023-06-20 11:27:22.000000 apache-airflow-providers-apache-flink-1.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:23.160955 apache-airflow-providers-apache-flink-1.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:23.162202 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:23.163431 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:23.199482 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2324 2023-06-20 11:27:22.000000 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:23.202307 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/hooks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:23.208356 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/operators/flink_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:23.214520 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5714 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/sensors/flink_kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:23.240009 apache-airflow-providers-apache-flink-1.1.1/apache_airflow_providers_apache_flink.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7466 2023-06-20 11:27:23.000000 apache-airflow-providers-apache-flink-1.1.1/apache_airflow_providers_apache_flink.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      867 2023-06-20 11:27:23.000000 apache-airflow-providers-apache-flink-1.1.1/apache_airflow_providers_apache_flink.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:23.000000 apache-airflow-providers-apache-flink-1.1.1/apache_airflow_providers_apache_flink.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:27:23.000000 apache-airflow-providers-apache-flink-1.1.1/apache_airflow_providers_apache_flink.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:23.000000 apache-airflow-providers-apache-flink-1.1.1/apache_airflow_providers_apache_flink.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-20 11:27:23.000000 apache-airflow-providers-apache-flink-1.1.1/apache_airflow_providers_apache_flink.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:23.000000 apache-airflow-providers-apache-flink-1.1.1/apache_airflow_providers_apache_flink.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-flink-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1927 2023-06-20 11:27:23.244657 apache-airflow-providers-apache-flink-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1737 2023-06-20 11:27:22.000000 apache-airflow-providers-apache-flink-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:13.815397 apache-airflow-providers-apache-flink-1.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-flink-1.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:12.000000 apache-airflow-providers-apache-flink-1.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-flink-1.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     7472 2023-06-20 11:41:13.815965 apache-airflow-providers-apache-flink-1.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-06-20 11:41:12.000000 apache-airflow-providers-apache-flink-1.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:13.735606 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:13.736713 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:13.737820 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:13.774243 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-06-20 11:41:12.000000 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:13.777324 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/hooks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:13.782968 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/operators/flink_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:13.788740 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/sensors/flink_kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:13.812733 apache-airflow-providers-apache-flink-1.1.1rc1/apache_airflow_providers_apache_flink.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7472 2023-06-20 11:41:13.000000 apache-airflow-providers-apache-flink-1.1.1rc1/apache_airflow_providers_apache_flink.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      867 2023-06-20 11:41:13.000000 apache-airflow-providers-apache-flink-1.1.1rc1/apache_airflow_providers_apache_flink.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:13.000000 apache-airflow-providers-apache-flink-1.1.1rc1/apache_airflow_providers_apache_flink.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:13.000000 apache-airflow-providers-apache-flink-1.1.1rc1/apache_airflow_providers_apache_flink.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:13.000000 apache-airflow-providers-apache-flink-1.1.1rc1/apache_airflow_providers_apache_flink.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-20 11:41:13.000000 apache-airflow-providers-apache-flink-1.1.1rc1/apache_airflow_providers_apache_flink.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:13.000000 apache-airflow-providers-apache-flink-1.1.1rc1/apache_airflow_providers_apache_flink.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-flink-1.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-06-20 11:41:13.818039 apache-airflow-providers-apache-flink-1.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-06-20 11:41:12.000000 apache-airflow-providers-apache-flink-1.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-flink-1.1.1/LICENSE` & `apache-airflow-providers-apache-flink-1.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.1.1/MANIFEST.in` & `apache-airflow-providers-apache-flink-1.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.1.1/PKG-INFO` & `apache-airflow-providers-apache-flink-1.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-flink
-Version: 1.1.1
+Version: 1.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-flink package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.1.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-flink``
 
-Release: ``1.1.1``
+Release: ``1.1.1rc1``
 
 
 `Apache Flink <https://flink.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-flink-1.1.1/README.rst` & `apache-airflow-providers-apache-flink-1.1.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-flink``
 
-Release: ``1.1.1``
+Release: ``1.1.1rc1``
 
 
 `Apache Flink <https://flink.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/__init__.py` & `apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/get_provider_info.py` & `apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/hooks/__init__.py` & `apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/operators/__init__.py` & `apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/operators/flink_kubernetes.py` & `apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/operators/flink_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/sensors/__init__.py` & `apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.1.1/airflow/providers/apache/flink/sensors/flink_kubernetes.py` & `apache-airflow-providers-apache-flink-1.1.1rc1/airflow/providers/apache/flink/sensors/flink_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.1.1/apache_airflow_providers_apache_flink.egg-info/PKG-INFO` & `apache-airflow-providers-apache-flink-1.1.1rc1/apache_airflow_providers_apache_flink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-flink
-Version: 1.1.1
+Version: 1.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-flink package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-flink/1.1.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-flink``
 
-Release: ``1.1.1``
+Release: ``1.1.1rc1``
 
 
 `Apache Flink <https://flink.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-flink-1.1.1/apache_airflow_providers_apache_flink.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-flink-1.1.1rc1/apache_airflow_providers_apache_flink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.1.1/pyproject.toml` & `apache-airflow-providers-apache-flink-1.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-flink-1.1.1/setup.cfg` & `apache-airflow-providers-apache-flink-1.1.1rc1/setup.cfg`

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
-	apache-airflow-providers-cncf-kubernetes>=5.1.0
-	apache-airflow>=2.4.0
+	apache-airflow-providers-cncf-kubernetes>=5.1.0.dev0
+	apache-airflow>=2.4.0.dev0
 	cryptography>=2.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.flink.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.flink
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-flink-1.1.1/setup.py` & `apache-airflow-providers-apache-flink-1.1.1rc1/setup.py`

 * *Files identical despite different names*
