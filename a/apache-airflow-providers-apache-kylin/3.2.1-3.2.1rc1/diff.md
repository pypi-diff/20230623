# Comparing `tmp/apache-airflow-providers-apache-kylin-3.2.1.tar.gz` & `tmp/apache-airflow-providers-apache-kylin-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-kylin-3.2.1.tar", last modified: Tue Jun 20 11:27:32 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-kylin-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:23 2023, max compression
```

## Comparing `apache-airflow-providers-apache-kylin-3.2.1.tar` & `apache-airflow-providers-apache-kylin-3.2.1rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:32.180071 apache-airflow-providers-apache-kylin-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kylin-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:31.000000 apache-airflow-providers-apache-kylin-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kylin-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10714 2023-06-20 11:27:32.181042 apache-airflow-providers-apache-kylin-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9171 2023-06-20 11:27:31.000000 apache-airflow-providers-apache-kylin-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:32.106439 apache-airflow-providers-apache-kylin-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:32.107609 apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:32.108783 apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:32.142886 apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2274 2023-06-20 11:27:31.000000 apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:32.148503 apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2670 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/hooks/kylin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:32.154279 apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7309 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/operators/kylin_cube.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:32.177726 apache-airflow-providers-apache-kylin-3.2.1/apache_airflow_providers_apache_kylin.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10714 2023-06-20 11:27:32.000000 apache-airflow-providers-apache-kylin-3.2.1/apache_airflow_providers_apache_kylin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      797 2023-06-20 11:27:32.000000 apache-airflow-providers-apache-kylin-3.2.1/apache_airflow_providers_apache_kylin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:32.000000 apache-airflow-providers-apache-kylin-3.2.1/apache_airflow_providers_apache_kylin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:27:32.000000 apache-airflow-providers-apache-kylin-3.2.1/apache_airflow_providers_apache_kylin.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:32.000000 apache-airflow-providers-apache-kylin-3.2.1/apache_airflow_providers_apache_kylin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-20 11:27:32.000000 apache-airflow-providers-apache-kylin-3.2.1/apache_airflow_providers_apache_kylin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:32.000000 apache-airflow-providers-apache-kylin-3.2.1/apache_airflow_providers_apache_kylin.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-kylin-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1871 2023-06-20 11:27:32.182927 apache-airflow-providers-apache-kylin-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:27:31.000000 apache-airflow-providers-apache-kylin-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:23.012667 apache-airflow-providers-apache-kylin-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10720 2023-06-20 11:41:23.013723 apache-airflow-providers-apache-kylin-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:22.938147 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:22.939262 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:22.940430 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:22.973631 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:22.980347 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/hooks/kylin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:22.986125 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7309 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/operators/kylin_cube.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:23.010093 apache-airflow-providers-apache-kylin-3.2.1rc1/apache_airflow_providers_apache_kylin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10720 2023-06-20 11:41:22.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/apache_airflow_providers_apache_kylin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      797 2023-06-20 11:41:22.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/apache_airflow_providers_apache_kylin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:22.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/apache_airflow_providers_apache_kylin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:22.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/apache_airflow_providers_apache_kylin.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:22.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/apache_airflow_providers_apache_kylin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-20 11:41:22.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/apache_airflow_providers_apache_kylin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:22.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/apache_airflow_providers_apache_kylin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-06-20 11:41:23.015660 apache-airflow-providers-apache-kylin-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kylin-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/LICENSE` & `apache-airflow-providers-apache-kylin-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/MANIFEST.in` & `apache-airflow-providers-apache-kylin-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/PKG-INFO` & `apache-airflow-providers-apache-kylin-3.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kylin
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kylin package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kylin/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-kylin``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Apache Kylin <https://kylin.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/README.rst` & `apache-airflow-providers-apache-kylin-3.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-kylin``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Apache Kylin <https://kylin.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/__init__.py` & `apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/get_provider_info.py` & `apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/hooks/__init__.py` & `apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/hooks/kylin.py` & `apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/hooks/kylin.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/operators/__init__.py` & `apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/airflow/providers/apache/kylin/operators/kylin_cube.py` & `apache-airflow-providers-apache-kylin-3.2.1rc1/airflow/providers/apache/kylin/operators/kylin_cube.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/apache_airflow_providers_apache_kylin.egg-info/PKG-INFO` & `apache-airflow-providers-apache-kylin-3.2.1rc1/apache_airflow_providers_apache_kylin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kylin
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kylin package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kylin/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-kylin``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Apache Kylin <https://kylin.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/apache_airflow_providers_apache_kylin.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-kylin-3.2.1rc1/apache_airflow_providers_apache_kylin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/pyproject.toml` & `apache-airflow-providers-apache-kylin-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/setup.cfg` & `apache-airflow-providers-apache-kylin-3.2.1rc1/setup.cfg`

 * *Files 7% similar despite different names*

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
 	kylinpy>=2.6
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.kylin.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.kylin
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-kylin-3.2.1/setup.py` & `apache-airflow-providers-apache-kylin-3.2.1rc1/setup.py`

 * *Files identical despite different names*

