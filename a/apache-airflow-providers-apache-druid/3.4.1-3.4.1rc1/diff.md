# Comparing `tmp/apache-airflow-providers-apache-druid-3.4.1.tar.gz` & `tmp/apache-airflow-providers-apache-druid-3.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-druid-3.4.1.tar", last modified: Tue Jun 20 11:27:21 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-druid-3.4.1rc1.tar", last modified: Tue Jun 20 11:41:12 2023, max compression
```

## Comparing `apache-airflow-providers-apache-druid-3.4.1.tar` & `apache-airflow-providers-apache-druid-3.4.1rc1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:21.523498 apache-airflow-providers-apache-druid-3.4.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-druid-3.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:20.000000 apache-airflow-providers-apache-druid-3.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-druid-3.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13924 2023-06-20 11:27:21.524599 apache-airflow-providers-apache-druid-3.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12326 2023-06-20 11:27:20.000000 apache-airflow-providers-apache-druid-3.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:21.440253 apache-airflow-providers-apache-druid-3.4.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:21.441432 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:21.442560 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:21.476495 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3245 2023-06-20 11:27:20.000000 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:21.482219 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6903 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/hooks/druid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:21.490604 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/operators/druid.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/operators/druid_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:21.496878 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10081 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/transfers/hive_to_druid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:21.520819 apache-airflow-providers-apache-druid-3.4.1/apache_airflow_providers_apache_druid.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13924 2023-06-20 11:27:21.000000 apache-airflow-providers-apache-druid-3.4.1/apache_airflow_providers_apache_druid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      959 2023-06-20 11:27:21.000000 apache-airflow-providers-apache-druid-3.4.1/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:21.000000 apache-airflow-providers-apache-druid-3.4.1/apache_airflow_providers_apache_druid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:27:21.000000 apache-airflow-providers-apache-druid-3.4.1/apache_airflow_providers_apache_druid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:21.000000 apache-airflow-providers-apache-druid-3.4.1/apache_airflow_providers_apache_druid.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-20 11:27:21.000000 apache-airflow-providers-apache-druid-3.4.1/apache_airflow_providers_apache_druid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:21.000000 apache-airflow-providers-apache-druid-3.4.1/apache_airflow_providers_apache_druid.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-druid-3.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1917 2023-06-20 11:27:21.526539 apache-airflow-providers-apache-druid-3.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-20 11:27:20.000000 apache-airflow-providers-apache-druid-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:12.041424 apache-airflow-providers-apache-druid-3.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-druid-3.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-druid-3.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-druid-3.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13930 2023-06-20 11:41:12.042636 apache-airflow-providers-apache-druid-3.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12329 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-druid-3.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:11.950450 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:11.951673 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:11.954599 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:11.988713 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3245 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:11.994512 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6903 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/hooks/druid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:12.002986 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/druid.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/druid_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:12.008772 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10081 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/transfers/hive_to_druid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:12.038030 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13930 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      959 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      192 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:11.000000 apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-druid-3.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-06-20 11:41:12.045048 apache-airflow-providers-apache-druid-3.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-20 11:41:10.000000 apache-airflow-providers-apache-druid-3.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-druid-3.4.1/LICENSE` & `apache-airflow-providers-apache-druid-3.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/MANIFEST.in` & `apache-airflow-providers-apache-druid-3.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/PKG-INFO` & `apache-airflow-providers-apache-druid-3.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-druid
-Version: 3.4.1
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-druid package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.1/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-druid``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `Apache Druid <https://druid.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-druid-3.4.1/README.rst` & `apache-airflow-providers-apache-druid-3.4.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-druid``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `Apache Druid <https://druid.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/__init__.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/get_provider_info.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/hooks/__init__.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/hooks/druid.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/hooks/druid.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/operators/__init__.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/operators/druid.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/druid.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/operators/druid_check.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/operators/druid_check.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/transfers/__init__.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/airflow/providers/apache/druid/transfers/hive_to_druid.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/airflow/providers/apache/druid/transfers/hive_to_druid.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/apache_airflow_providers_apache_druid.egg-info/PKG-INFO` & `apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-druid
-Version: 3.4.1
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-druid package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-druid/3.4.1/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-druid``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 `Apache Druid <https://druid.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-druid-3.4.1/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-druid-3.4.1rc1/apache_airflow_providers_apache_druid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/pyproject.toml` & `apache-airflow-providers-apache-druid-3.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-druid-3.4.1/setup.cfg` & `apache-airflow-providers-apache-druid-3.4.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

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
 	pydruid>=0.4.1
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.druid.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.druid
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-druid-3.4.1/setup.py` & `apache-airflow-providers-apache-druid-3.4.1rc1/setup.py`

 * *Files identical despite different names*

