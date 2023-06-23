# Comparing `tmp/apache-airflow-providers-apache-pig-4.1.1.tar.gz` & `tmp/apache-airflow-providers-apache-pig-4.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-pig-4.1.1.tar", last modified: Tue Jun 20 11:27:35 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-pig-4.1.1rc1.tar", last modified: Tue Jun 20 11:41:26 2023, max compression
```

## Comparing `apache-airflow-providers-apache-pig-4.1.1.tar` & `apache-airflow-providers-apache-pig-4.1.1rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:35.673323 apache-airflow-providers-apache-pig-4.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-pig-4.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:34.000000 apache-airflow-providers-apache-pig-4.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-pig-4.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11031 2023-06-20 11:27:35.674384 apache-airflow-providers-apache-pig-4.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9494 2023-06-20 11:27:34.000000 apache-airflow-providers-apache-pig-4.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:35.601203 apache-airflow-providers-apache-pig-4.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:35.602294 apache-airflow-providers-apache-pig-4.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:35.603330 apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:35.634879 apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2476 2023-06-20 11:27:34.000000 apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:35.640537 apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4253 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/hooks/pig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:35.646138 apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2978 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/operators/pig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:35.670611 apache-airflow-providers-apache-pig-4.1.1/apache_airflow_providers_apache_pig.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11031 2023-06-20 11:27:35.000000 apache-airflow-providers-apache-pig-4.1.1/apache_airflow_providers_apache_pig.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      762 2023-06-20 11:27:35.000000 apache-airflow-providers-apache-pig-4.1.1/apache_airflow_providers_apache_pig.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:35.000000 apache-airflow-providers-apache-pig-4.1.1/apache_airflow_providers_apache_pig.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-20 11:27:35.000000 apache-airflow-providers-apache-pig-4.1.1/apache_airflow_providers_apache_pig.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:35.000000 apache-airflow-providers-apache-pig-4.1.1/apache_airflow_providers_apache_pig.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-20 11:27:35.000000 apache-airflow-providers-apache-pig-4.1.1/apache_airflow_providers_apache_pig.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:35.000000 apache-airflow-providers-apache-pig-4.1.1/apache_airflow_providers_apache_pig.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-pig-4.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1845 2023-06-20 11:27:35.676364 apache-airflow-providers-apache-pig-4.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1662 2023-06-20 11:27:34.000000 apache-airflow-providers-apache-pig-4.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:26.632829 apache-airflow-providers-apache-pig-4.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-pig-4.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:25.000000 apache-airflow-providers-apache-pig-4.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-pig-4.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11037 2023-06-20 11:41:26.633918 apache-airflow-providers-apache-pig-4.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9497 2023-06-20 11:41:25.000000 apache-airflow-providers-apache-pig-4.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:26.559163 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:26.560388 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:26.561634 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:26.594516 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-06-20 11:41:25.000000 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:26.600262 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4253 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/hooks/pig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:26.606001 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/operators/pig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:26.630128 apache-airflow-providers-apache-pig-4.1.1rc1/apache_airflow_providers_apache_pig.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11037 2023-06-20 11:41:26.000000 apache-airflow-providers-apache-pig-4.1.1rc1/apache_airflow_providers_apache_pig.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      762 2023-06-20 11:41:26.000000 apache-airflow-providers-apache-pig-4.1.1rc1/apache_airflow_providers_apache_pig.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:26.000000 apache-airflow-providers-apache-pig-4.1.1rc1/apache_airflow_providers_apache_pig.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-20 11:41:26.000000 apache-airflow-providers-apache-pig-4.1.1rc1/apache_airflow_providers_apache_pig.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:26.000000 apache-airflow-providers-apache-pig-4.1.1rc1/apache_airflow_providers_apache_pig.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:41:26.000000 apache-airflow-providers-apache-pig-4.1.1rc1/apache_airflow_providers_apache_pig.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:26.000000 apache-airflow-providers-apache-pig-4.1.1rc1/apache_airflow_providers_apache_pig.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-pig-4.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-06-20 11:41:26.635885 apache-airflow-providers-apache-pig-4.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-06-20 11:41:25.000000 apache-airflow-providers-apache-pig-4.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-pig-4.1.1/LICENSE` & `apache-airflow-providers-apache-pig-4.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.1.1/MANIFEST.in` & `apache-airflow-providers-apache-pig-4.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.1.1/PKG-INFO` & `apache-airflow-providers-apache-pig-4.1.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-pig
-Version: 4.1.1
+Version: 4.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-pig package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.1.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-pig``
 
-Release: ``4.1.1``
+Release: ``4.1.1rc1``
 
 
 `Apache Pig <https://pig.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-pig-4.1.1/README.rst` & `apache-airflow-providers-apache-pig-4.1.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-pig``
 
-Release: ``4.1.1``
+Release: ``4.1.1rc1``
 
 
 `Apache Pig <https://pig.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/__init__.py` & `apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/get_provider_info.py` & `apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/hooks/__init__.py` & `apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/hooks/pig.py` & `apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/hooks/pig.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/operators/__init__.py` & `apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.1.1/airflow/providers/apache/pig/operators/pig.py` & `apache-airflow-providers-apache-pig-4.1.1rc1/airflow/providers/apache/pig/operators/pig.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.1.1/apache_airflow_providers_apache_pig.egg-info/PKG-INFO` & `apache-airflow-providers-apache-pig-4.1.1rc1/apache_airflow_providers_apache_pig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-pig
-Version: 4.1.1
+Version: 4.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-pig package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-pig/4.1.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-pig``
 
-Release: ``4.1.1``
+Release: ``4.1.1rc1``
 
 
 `Apache Pig <https://pig.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-pig-4.1.1/apache_airflow_providers_apache_pig.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-pig-4.1.1rc1/apache_airflow_providers_apache_pig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.1.1/pyproject.toml` & `apache-airflow-providers-apache-pig-4.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-pig-4.1.1/setup.cfg` & `apache-airflow-providers-apache-pig-4.1.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

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
 	provider_info=airflow.providers.apache.pig.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.pig
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-pig-4.1.1/setup.py` & `apache-airflow-providers-apache-pig-4.1.1rc1/setup.py`

 * *Files identical despite different names*

