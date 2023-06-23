# Comparing `tmp/apache-airflow-providers-apache-drill-2.4.1.tar.gz` & `tmp/apache-airflow-providers-apache-drill-2.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-drill-2.4.1.tar", last modified: Tue Jun 20 11:27:19 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-drill-2.4.1rc1.tar", last modified: Tue Jun 20 11:41:10 2023, max compression
```

## Comparing `apache-airflow-providers-apache-drill-2.4.1.tar` & `apache-airflow-providers-apache-drill-2.4.1rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:19.781491 apache-airflow-providers-apache-drill-2.4.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:18.000000 apache-airflow-providers-apache-drill-2.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11460 2023-06-20 11:27:19.782522 apache-airflow-providers-apache-drill-2.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9890 2023-06-20 11:27:18.000000 apache-airflow-providers-apache-drill-2.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:19.706678 apache-airflow-providers-apache-drill-2.4.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:19.707940 apache-airflow-providers-apache-drill-2.4.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:19.709107 apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:19.742693 apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-06-20 11:27:18.000000 apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:19.749129 apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3660 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/hooks/drill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:19.755272 apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2222 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/operators/drill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:19.778843 apache-airflow-providers-apache-drill-2.4.1/apache_airflow_providers_apache_drill.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11460 2023-06-20 11:27:19.000000 apache-airflow-providers-apache-drill-2.4.1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2023-06-20 11:27:19.000000 apache-airflow-providers-apache-drill-2.4.1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:19.000000 apache-airflow-providers-apache-drill-2.4.1/apache_airflow_providers_apache_drill.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:27:19.000000 apache-airflow-providers-apache-drill-2.4.1/apache_airflow_providers_apache_drill.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:19.000000 apache-airflow-providers-apache-drill-2.4.1/apache_airflow_providers_apache_drill.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      139 2023-06-20 11:27:19.000000 apache-airflow-providers-apache-drill-2.4.1/apache_airflow_providers_apache_drill.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:19.000000 apache-airflow-providers-apache-drill-2.4.1/apache_airflow_providers_apache_drill.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-drill-2.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1926 2023-06-20 11:27:19.784421 apache-airflow-providers-apache-drill-2.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1727 2023-06-20 11:27:18.000000 apache-airflow-providers-apache-drill-2.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:10.237331 apache-airflow-providers-apache-drill-2.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:09.000000 apache-airflow-providers-apache-drill-2.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-drill-2.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11466 2023-06-20 11:41:10.238393 apache-airflow-providers-apache-drill-2.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9893 2023-06-20 11:41:09.000000 apache-airflow-providers-apache-drill-2.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:10.162989 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:10.164130 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:10.165258 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:10.199470 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-06-20 11:41:09.000000 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:10.205214 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/hooks/drill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:10.210877 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/operators/drill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:10.234735 apache-airflow-providers-apache-drill-2.4.1rc1/apache_airflow_providers_apache_drill.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11466 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-drill-2.4.1rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-drill-2.4.1rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-drill-2.4.1rc1/apache_airflow_providers_apache_drill.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-drill-2.4.1rc1/apache_airflow_providers_apache_drill.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-drill-2.4.1rc1/apache_airflow_providers_apache_drill.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-drill-2.4.1rc1/apache_airflow_providers_apache_drill.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-drill-2.4.1rc1/apache_airflow_providers_apache_drill.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-drill-2.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1939 2023-06-20 11:41:10.240388 apache-airflow-providers-apache-drill-2.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-06-20 11:41:09.000000 apache-airflow-providers-apache-drill-2.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-drill-2.4.1/LICENSE` & `apache-airflow-providers-apache-drill-2.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.1/MANIFEST.in` & `apache-airflow-providers-apache-drill-2.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.1/PKG-INFO` & `apache-airflow-providers-apache-drill-2.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-drill
-Version: 2.4.1
+Version: 2.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-drill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.1``
+Release: ``2.4.1rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-drill-2.4.1/README.rst` & `apache-airflow-providers-apache-drill-2.4.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.1``
+Release: ``2.4.1rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/__init__.py` & `apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/get_provider_info.py` & `apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/hooks/__init__.py` & `apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/hooks/drill.py` & `apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/hooks/drill.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/operators/__init__.py` & `apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.1/airflow/providers/apache/drill/operators/drill.py` & `apache-airflow-providers-apache-drill-2.4.1rc1/airflow/providers/apache/drill/operators/drill.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO` & `apache-airflow-providers-apache-drill-2.4.1rc1/apache_airflow_providers_apache_drill.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-drill
-Version: 2.4.1
+Version: 2.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-drill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-drill/2.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-drill``
 
-Release: ``2.4.1``
+Release: ``2.4.1rc1``
 
 
 `Apache Drill <https://drill.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-drill-2.4.1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-drill-2.4.1rc1/apache_airflow_providers_apache_drill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.1/pyproject.toml` & `apache-airflow-providers-apache-drill-2.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-drill-2.4.1/setup.cfg` & `apache-airflow-providers-apache-drill-2.4.1rc1/setup.cfg`

 * *Files 7% similar despite different names*

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
 	sqlalchemy-drill>=1.1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.drill.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.drill
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-drill-2.4.1/setup.py` & `apache-airflow-providers-apache-drill-2.4.1rc1/setup.py`

 * *Files identical despite different names*

