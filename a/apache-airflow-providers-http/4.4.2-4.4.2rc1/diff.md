# Comparing `tmp/apache-airflow-providers-http-4.4.2.tar.gz` & `tmp/apache-airflow-providers-http-4.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-http-4.4.2.tar", last modified: Tue Jun 20 11:28:27 2023, max compression
+gzip compressed data, was "apache-airflow-providers-http-4.4.2rc1.tar", last modified: Tue Jun 20 11:42:18 2023, max compression
```

## Comparing `apache-airflow-providers-http-4.4.2.tar` & `apache-airflow-providers-http-4.4.2rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:27.870560 apache-airflow-providers-http-4.4.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:26.000000 apache-airflow-providers-http-4.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.4.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12751 2023-06-20 11:28:27.871746 apache-airflow-providers-http-4.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11232 2023-06-20 11:28:26.000000 apache-airflow-providers-http-4.4.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:27.783780 apache-airflow-providers-http-4.4.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:27.784930 apache-airflow-providers-http-4.4.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:27.821959 apache-airflow-providers-http-4.4.2/airflow/providers/http/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-http-4.4.2/airflow/providers/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3088 2023-06-20 11:28:26.000000 apache-airflow-providers-http-4.4.2/airflow/providers/http/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:27.828068 apache-airflow-providers-http-4.4.2/airflow/providers/http/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2/airflow/providers/http/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16171 2023-06-05 12:50:36.000000 apache-airflow-providers-http-4.4.2/airflow/providers/http/hooks/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:27.834100 apache-airflow-providers-http-4.4.2/airflow/providers/http/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2/airflow/providers/http/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5829 2023-06-02 11:31:21.000000 apache-airflow-providers-http-4.4.2/airflow/providers/http/operators/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:27.840452 apache-airflow-providers-http-4.4.2/airflow/providers/http/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2/airflow/providers/http/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5885 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2/airflow/providers/http/sensors/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:27.867210 apache-airflow-providers-http-4.4.2/apache_airflow_providers_http.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12751 2023-06-20 11:28:27.000000 apache-airflow-providers-http-4.4.2/apache_airflow_providers_http.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      768 2023-06-20 11:28:27.000000 apache-airflow-providers-http-4.4.2/apache_airflow_providers_http.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:27.000000 apache-airflow-providers-http-4.4.2/apache_airflow_providers_http.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:28:27.000000 apache-airflow-providers-http-4.4.2/apache_airflow_providers_http.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:27.000000 apache-airflow-providers-http-4.4.2/apache_airflow_providers_http.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 11:28:27.000000 apache-airflow-providers-http-4.4.2/apache_airflow_providers_http.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:27.000000 apache-airflow-providers-http-4.4.2/apache_airflow_providers_http.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-http-4.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-20 11:28:27.874144 apache-airflow-providers-http-4.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-20 11:28:26.000000 apache-airflow-providers-http-4.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.277746 apache-airflow-providers-http-4.4.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.4.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:17.000000 apache-airflow-providers-http-4.4.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.4.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12757 2023-06-20 11:42:18.278886 apache-airflow-providers-http-4.4.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11235 2023-06-20 11:42:17.000000 apache-airflow-providers-http-4.4.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.184744 apache-airflow-providers-http-4.4.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.185980 apache-airflow-providers-http-4.4.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.228034 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-06-20 11:42:17.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.234411 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16171 2023-06-05 12:50:36.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/hooks/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.241051 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5829 2023-06-02 11:31:21.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/operators/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.247280 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5885 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/sensors/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:18.275094 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12757 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      768 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:18.000000 apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-http-4.4.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-20 11:42:18.280969 apache-airflow-providers-http-4.4.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-20 11:42:17.000000 apache-airflow-providers-http-4.4.2rc1/setup.py
```

### Comparing `apache-airflow-providers-http-4.4.2/LICENSE` & `apache-airflow-providers-http-4.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/MANIFEST.in` & `apache-airflow-providers-http-4.4.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/PKG-INFO` & `apache-airflow-providers-http-4.4.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-http
-Version: 4.4.2
+Version: 4.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-http package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.2/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.4.2``
+Release: ``4.4.2rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-http-4.4.2/README.rst` & `apache-airflow-providers-http-4.4.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.4.2``
+Release: ``4.4.2rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-http-4.4.2/airflow/providers/http/__init__.py` & `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/airflow/providers/http/get_provider_info.py` & `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/airflow/providers/http/hooks/__init__.py` & `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/airflow/providers/http/hooks/http.py` & `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/hooks/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/airflow/providers/http/operators/__init__.py` & `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/airflow/providers/http/operators/http.py` & `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/operators/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/airflow/providers/http/sensors/__init__.py` & `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/airflow/providers/http/sensors/http.py` & `apache-airflow-providers-http-4.4.2rc1/airflow/providers/http/sensors/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/apache_airflow_providers_http.egg-info/PKG-INFO` & `apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-http
-Version: 4.4.2
+Version: 4.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-http package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.4.2/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.4.2``
+Release: ``4.4.2rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-http-4.4.2/apache_airflow_providers_http.egg-info/SOURCES.txt` & `apache-airflow-providers-http-4.4.2rc1/apache_airflow_providers_http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/pyproject.toml` & `apache-airflow-providers-http-4.4.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.4.2/setup.cfg` & `apache-airflow-providers-http-4.4.2rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -43,23 +43,23 @@
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	aiohttp
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	asgiref
 	requests>=2.26.0
 	requests_toolbelt
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.http.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.http
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-http-4.4.2/setup.py` & `apache-airflow-providers-http-4.4.2rc1/setup.py`

 * *Files identical despite different names*

