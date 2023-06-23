# Comparing `tmp/apache-airflow-providers-imap-3.2.2.tar.gz` & `tmp/apache-airflow-providers-imap-3.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-imap-3.2.2.tar", last modified: Tue Jun 20 11:28:29 2023, max compression
+gzip compressed data, was "apache-airflow-providers-imap-3.2.2rc1.tar", last modified: Tue Jun 20 11:42:20 2023, max compression
```

## Comparing `apache-airflow-providers-imap-3.2.2.tar` & `apache-airflow-providers-imap-3.2.2rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:29.658741 apache-airflow-providers-imap-3.2.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:28.000000 apache-airflow-providers-imap-3.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.2.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10396 2023-06-20 11:28:29.659788 apache-airflow-providers-imap-3.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8877 2023-06-20 11:28:28.000000 apache-airflow-providers-imap-3.2.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:29.575369 apache-airflow-providers-imap-3.2.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:29.576629 apache-airflow-providers-imap-3.2.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:29.615020 apache-airflow-providers-imap-3.2.2/airflow/providers/imap/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-imap-3.2.2/airflow/providers/imap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2618 2023-06-20 11:28:28.000000 apache-airflow-providers-imap-3.2.2/airflow/providers/imap/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:29.621628 apache-airflow-providers-imap-3.2.2/airflow/providers/imap/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2/airflow/providers/imap/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14090 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2/airflow/providers/imap/hooks/imap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:29.627575 apache-airflow-providers-imap-3.2.2/airflow/providers/imap/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2/airflow/providers/imap/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2/airflow/providers/imap/sensors/imap_attachment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:29.656393 apache-airflow-providers-imap-3.2.2/apache_airflow_providers_imap.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10396 2023-06-20 11:28:29.000000 apache-airflow-providers-imap-3.2.2/apache_airflow_providers_imap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      693 2023-06-20 11:28:29.000000 apache-airflow-providers-imap-3.2.2/apache_airflow_providers_imap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:29.000000 apache-airflow-providers-imap-3.2.2/apache_airflow_providers_imap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:28:29.000000 apache-airflow-providers-imap-3.2.2/apache_airflow_providers_imap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:29.000000 apache-airflow-providers-imap-3.2.2/apache_airflow_providers_imap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-20 11:28:29.000000 apache-airflow-providers-imap-3.2.2/apache_airflow_providers_imap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:29.000000 apache-airflow-providers-imap-3.2.2/apache_airflow_providers_imap.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-imap-3.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1809 2023-06-20 11:28:29.661654 apache-airflow-providers-imap-3.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-20 11:28:28.000000 apache-airflow-providers-imap-3.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.226959 apache-airflow-providers-imap-3.2.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.2.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-imap-3.2.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-06-20 11:42:20.228169 apache-airflow-providers-imap-3.2.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8880 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.147596 apache-airflow-providers-imap-3.2.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.148910 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.187214 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.193153 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14090 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/imap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.198967 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-06-01 06:14:28.000000 apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/imap_attachment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:20.223903 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      693 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:20.000000 apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-imap-3.2.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-06-20 11:42:20.230574 apache-airflow-providers-imap-3.2.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-20 11:42:19.000000 apache-airflow-providers-imap-3.2.2rc1/setup.py
```

### Comparing `apache-airflow-providers-imap-3.2.2/LICENSE` & `apache-airflow-providers-imap-3.2.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2/MANIFEST.in` & `apache-airflow-providers-imap-3.2.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2/PKG-INFO` & `apache-airflow-providers-imap-3.2.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-imap
-Version: 3.2.2
+Version: 3.2.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-imap package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.2/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.2.2``
+Release: ``3.2.2rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-imap-3.2.2/README.rst` & `apache-airflow-providers-imap-3.2.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.2.2``
+Release: ``3.2.2rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-imap-3.2.2/airflow/providers/imap/__init__.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2/airflow/providers/imap/get_provider_info.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2/airflow/providers/imap/hooks/__init__.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2/airflow/providers/imap/hooks/imap.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/hooks/imap.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2/airflow/providers/imap/sensors/__init__.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2/airflow/providers/imap/sensors/imap_attachment.py` & `apache-airflow-providers-imap-3.2.2rc1/airflow/providers/imap/sensors/imap_attachment.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2/apache_airflow_providers_imap.egg-info/PKG-INFO` & `apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-imap
-Version: 3.2.2
+Version: 3.2.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-imap package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-imap/3.2.2/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-imap``
 
-Release: ``3.2.2``
+Release: ``3.2.2rc1``
 
 
 `Internet Message Access Protocol (IMAP) <https://tools.ietf.org/html/rfc3501>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-imap-3.2.2/apache_airflow_providers_imap.egg-info/SOURCES.txt` & `apache-airflow-providers-imap-3.2.2rc1/apache_airflow_providers_imap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2/pyproject.toml` & `apache-airflow-providers-imap-3.2.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-imap-3.2.2/setup.cfg` & `apache-airflow-providers-imap-3.2.2rc1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.imap.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.imap
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-imap-3.2.2/setup.py` & `apache-airflow-providers-imap-3.2.2rc1/setup.py`

 * *Files identical despite different names*

