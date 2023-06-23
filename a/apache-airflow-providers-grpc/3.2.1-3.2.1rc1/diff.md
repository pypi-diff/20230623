# Comparing `tmp/apache-airflow-providers-grpc-3.2.1.tar.gz` & `tmp/apache-airflow-providers-grpc-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-grpc-3.2.1.tar", last modified: Tue Jun 20 11:28:24 2023, max compression
+gzip compressed data, was "apache-airflow-providers-grpc-3.2.1rc1.tar", last modified: Tue Jun 20 11:42:14 2023, max compression
```

## Comparing `apache-airflow-providers-grpc-3.2.1.tar` & `apache-airflow-providers-grpc-3.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:24.304654 apache-airflow-providers-grpc-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-grpc-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:23.000000 apache-airflow-providers-grpc-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-grpc-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10660 2023-06-20 11:28:24.305639 apache-airflow-providers-grpc-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9141 2023-06-20 11:28:23.000000 apache-airflow-providers-grpc-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:24.226551 apache-airflow-providers-grpc-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:24.227678 apache-airflow-providers-grpc-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:24.264430 apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2234 2023-06-20 11:28:23.000000 apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:24.270589 apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6853 2023-06-02 11:31:21.000000 apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/hooks/grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:24.276412 apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3800 2023-06-02 11:31:21.000000 apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/operators/grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:24.301966 apache-airflow-providers-grpc-3.2.1/apache_airflow_providers_grpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10660 2023-06-20 11:28:24.000000 apache-airflow-providers-grpc-3.2.1/apache_airflow_providers_grpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      686 2023-06-20 11:28:24.000000 apache-airflow-providers-grpc-3.2.1/apache_airflow_providers_grpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:24.000000 apache-airflow-providers-grpc-3.2.1/apache_airflow_providers_grpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:28:24.000000 apache-airflow-providers-grpc-3.2.1/apache_airflow_providers_grpc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:24.000000 apache-airflow-providers-grpc-3.2.1/apache_airflow_providers_grpc.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       91 2023-06-20 11:28:24.000000 apache-airflow-providers-grpc-3.2.1/apache_airflow_providers_grpc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:24.000000 apache-airflow-providers-grpc-3.2.1/apache_airflow_providers_grpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-grpc-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1882 2023-06-20 11:28:24.308002 apache-airflow-providers-grpc-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-06-20 11:28:23.000000 apache-airflow-providers-grpc-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:14.491644 apache-airflow-providers-grpc-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-grpc-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:13.000000 apache-airflow-providers-grpc-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-grpc-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10666 2023-06-20 11:42:14.492702 apache-airflow-providers-grpc-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9144 2023-06-20 11:42:13.000000 apache-airflow-providers-grpc-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:14.415875 apache-airflow-providers-grpc-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:14.417016 apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:14.450264 apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-06-20 11:42:13.000000 apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:14.456652 apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6853 2023-06-02 11:31:21.000000 apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/hooks/grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:14.462976 apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-06-02 11:31:21.000000 apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/operators/grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:14.488976 apache-airflow-providers-grpc-3.2.1rc1/apache_airflow_providers_grpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10666 2023-06-20 11:42:14.000000 apache-airflow-providers-grpc-3.2.1rc1/apache_airflow_providers_grpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      686 2023-06-20 11:42:14.000000 apache-airflow-providers-grpc-3.2.1rc1/apache_airflow_providers_grpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:14.000000 apache-airflow-providers-grpc-3.2.1rc1/apache_airflow_providers_grpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:42:14.000000 apache-airflow-providers-grpc-3.2.1rc1/apache_airflow_providers_grpc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:14.000000 apache-airflow-providers-grpc-3.2.1rc1/apache_airflow_providers_grpc.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       96 2023-06-20 11:42:14.000000 apache-airflow-providers-grpc-3.2.1rc1/apache_airflow_providers_grpc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:14.000000 apache-airflow-providers-grpc-3.2.1rc1/apache_airflow_providers_grpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-grpc-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1890 2023-06-20 11:42:14.494583 apache-airflow-providers-grpc-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-20 11:42:13.000000 apache-airflow-providers-grpc-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-grpc-3.2.1/LICENSE` & `apache-airflow-providers-grpc-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.1/MANIFEST.in` & `apache-airflow-providers-grpc-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.1/PKG-INFO` & `apache-airflow-providers-grpc-3.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-grpc
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-grpc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-grpc``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `gRPC <https://grpc.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-grpc-3.2.1/README.rst` & `apache-airflow-providers-grpc-3.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-grpc``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `gRPC <https://grpc.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/__init__.py` & `apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/get_provider_info.py` & `apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/hooks/__init__.py` & `apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/hooks/grpc.py` & `apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/hooks/grpc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/operators/__init__.py` & `apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.1/airflow/providers/grpc/operators/grpc.py` & `apache-airflow-providers-grpc-3.2.1rc1/airflow/providers/grpc/operators/grpc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.1/apache_airflow_providers_grpc.egg-info/PKG-INFO` & `apache-airflow-providers-grpc-3.2.1rc1/apache_airflow_providers_grpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-grpc
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-grpc package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-grpc/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-grpc``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `gRPC <https://grpc.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-grpc-3.2.1/apache_airflow_providers_grpc.egg-info/SOURCES.txt` & `apache-airflow-providers-grpc-3.2.1rc1/apache_airflow_providers_grpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.1/pyproject.toml` & `apache-airflow-providers-grpc-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-grpc-3.2.1/setup.cfg` & `apache-airflow-providers-grpc-3.2.1rc1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -42,23 +42,23 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	google-auth-httplib2>=0.0.1
 	google-auth>=1.0.0, <3.0.0
 	grpcio>=1.15.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.grpc.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.grpc
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-grpc-3.2.1/setup.py` & `apache-airflow-providers-grpc-3.2.1rc1/setup.py`

 * *Files identical despite different names*

