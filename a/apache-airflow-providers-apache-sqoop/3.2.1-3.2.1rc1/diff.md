# Comparing `tmp/apache-airflow-providers-apache-sqoop-3.2.1.tar.gz` & `tmp/apache-airflow-providers-apache-sqoop-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-sqoop-3.2.1.tar", last modified: Tue Jun 20 11:27:41 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-sqoop-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:31 2023, max compression
```

## Comparing `apache-airflow-providers-apache-sqoop-3.2.1.tar` & `apache-airflow-providers-apache-sqoop-3.2.1rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:41.393678 apache-airflow-providers-apache-sqoop-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-sqoop-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:40.000000 apache-airflow-providers-apache-sqoop-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-sqoop-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10790 2023-06-20 11:27:41.394765 apache-airflow-providers-apache-sqoop-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9247 2023-06-20 11:27:40.000000 apache-airflow-providers-apache-sqoop-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:41.274608 apache-airflow-providers-apache-sqoop-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:41.276052 apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:41.277076 apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:41.336525 apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-06-20 11:27:40.000000 apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:41.346588 apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15763 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/hooks/sqoop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:41.357061 apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11403 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/operators/sqoop.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:41.390372 apache-airflow-providers-apache-sqoop-3.2.1/apache_airflow_providers_apache_sqoop.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10790 2023-06-20 11:27:41.000000 apache-airflow-providers-apache-sqoop-3.2.1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2023-06-20 11:27:41.000000 apache-airflow-providers-apache-sqoop-3.2.1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:41.000000 apache-airflow-providers-apache-sqoop-3.2.1/apache_airflow_providers_apache_sqoop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:27:41.000000 apache-airflow-providers-apache-sqoop-3.2.1/apache_airflow_providers_apache_sqoop.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:41.000000 apache-airflow-providers-apache-sqoop-3.2.1/apache_airflow_providers_apache_sqoop.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-20 11:27:41.000000 apache-airflow-providers-apache-sqoop-3.2.1/apache_airflow_providers_apache_sqoop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:41.000000 apache-airflow-providers-apache-sqoop-3.2.1/apache_airflow_providers_apache_sqoop.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-sqoop-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1857 2023-06-20 11:27:41.396876 apache-airflow-providers-apache-sqoop-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:27:40.000000 apache-airflow-providers-apache-sqoop-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.954770 apache-airflow-providers-apache-sqoop-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10796 2023-06-20 11:41:31.955793 apache-airflow-providers-apache-sqoop-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9250 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.877949 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.881474 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.882725 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.916856 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.922633 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15763 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/hooks/sqoop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.928480 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11403 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/operators/sqoop.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:31.952468 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10796 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:31.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1865 2023-06-20 11:41:31.957659 apache-airflow-providers-apache-sqoop-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-sqoop-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/LICENSE` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/MANIFEST.in` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/PKG-INFO` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-sqoop
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-sqoop package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/README.rst` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/__init__.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/get_provider_info.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/hooks/__init__.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/hooks/sqoop.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/hooks/sqoop.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/operators/__init__.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/airflow/providers/apache/sqoop/operators/sqoop.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/airflow/providers/apache/sqoop/operators/sqoop.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-sqoop
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-sqoop package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-sqoop/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-sqoop``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Apache Sqoop <https://sqoop.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/apache_airflow_providers_apache_sqoop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/pyproject.toml` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/setup.cfg` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

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
 	provider_info=airflow.providers.apache.sqoop.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.sqoop
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-sqoop-3.2.1/setup.py` & `apache-airflow-providers-apache-sqoop-3.2.1rc1/setup.py`

 * *Files identical despite different names*

