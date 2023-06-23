# Comparing `tmp/apache-airflow-providers-ftp-3.4.2.tar.gz` & `tmp/apache-airflow-providers-ftp-3.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-ftp-3.4.2.tar", last modified: Tue Jun 20 11:28:13 2023, max compression
+gzip compressed data, was "apache-airflow-providers-ftp-3.4.2rc1.tar", last modified: Tue Jun 20 11:42:03 2023, max compression
```

## Comparing `apache-airflow-providers-ftp-3.4.2.tar` & `apache-airflow-providers-ftp-3.4.2rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:13.031751 apache-airflow-providers-ftp-3.4.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:11.000000 apache-airflow-providers-ftp-3.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.4.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10290 2023-06-20 11:28:13.032831 apache-airflow-providers-ftp-3.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8774 2023-06-20 11:28:11.000000 apache-airflow-providers-ftp-3.4.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:12.949458 apache-airflow-providers-ftp-3.4.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:12.950715 apache-airflow-providers-ftp-3.4.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:12.987506 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/
--rw-r--r--   0 root         (0) root         (0)     1528 2023-06-20 11:01:09.000000 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-06-20 11:28:11.000000 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:12.993383 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9846 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/hooks/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:12.999272 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6079 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/operators/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:13.005343 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3364 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/sensors/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:13.029096 apache-airflow-providers-ftp-3.4.2/apache_airflow_providers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10290 2023-06-20 11:28:12.000000 apache-airflow-providers-ftp-3.4.2/apache_airflow_providers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      750 2023-06-20 11:28:12.000000 apache-airflow-providers-ftp-3.4.2/apache_airflow_providers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:12.000000 apache-airflow-providers-ftp-3.4.2/apache_airflow_providers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-20 11:28:12.000000 apache-airflow-providers-ftp-3.4.2/apache_airflow_providers_ftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:12.000000 apache-airflow-providers-ftp-3.4.2/apache_airflow_providers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-20 11:28:12.000000 apache-airflow-providers-ftp-3.4.2/apache_airflow_providers_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:12.000000 apache-airflow-providers-ftp-3.4.2/apache_airflow_providers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-ftp-3.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1803 2023-06-20 11:28:13.034851 apache-airflow-providers-ftp-3.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1620 2023-06-20 11:28:11.000000 apache-airflow-providers-ftp-3.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.623457 apache-airflow-providers-ftp-3.4.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.4.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-ftp-3.4.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10296 2023-06-20 11:42:03.624667 apache-airflow-providers-ftp-3.4.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8777 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.540377 apache-airflow-providers-ftp-3.4.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.541702 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.577906 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-06-20 11:01:09.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.583570 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9846 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.589324 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6079 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.595048 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2023-06-02 11:31:21.000000 apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:03.620290 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10296 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      750 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:03.000000 apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-ftp-3.4.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-20 11:42:03.626640 apache-airflow-providers-ftp-3.4.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-06-20 11:42:02.000000 apache-airflow-providers-ftp-3.4.2rc1/setup.py
```

### Comparing `apache-airflow-providers-ftp-3.4.2/LICENSE` & `apache-airflow-providers-ftp-3.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/MANIFEST.in` & `apache-airflow-providers-ftp-3.4.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/PKG-INFO` & `apache-airflow-providers-ftp-3.4.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.4.2
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.2/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-ftp-3.4.2/README.rst` & `apache-airflow-providers-ftp-3.4.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/__init__.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/get_provider_info.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/hooks/__init__.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/hooks/ftp.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/hooks/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/operators/__init__.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/operators/ftp.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/operators/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/sensors/__init__.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/airflow/providers/ftp/sensors/ftp.py` & `apache-airflow-providers-ftp-3.4.2rc1/airflow/providers/ftp/sensors/ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/apache_airflow_providers_ftp.egg-info/PKG-INFO` & `apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-ftp
-Version: 3.4.2
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-ftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-ftp/3.4.2/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-ftp``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `File Transfer Protocol (FTP) <https://tools.ietf.org/html/rfc114>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-ftp-3.4.2/apache_airflow_providers_ftp.egg-info/SOURCES.txt` & `apache-airflow-providers-ftp-3.4.2rc1/apache_airflow_providers_ftp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/pyproject.toml` & `apache-airflow-providers-ftp-3.4.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-ftp-3.4.2/setup.cfg` & `apache-airflow-providers-ftp-3.4.2rc1/setup.cfg`

 * *Files 14% similar despite different names*

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
 	provider_info=airflow.providers.ftp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.ftp
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-ftp-3.4.2/setup.py` & `apache-airflow-providers-ftp-3.4.2rc1/setup.py`

 * *Files identical despite different names*

