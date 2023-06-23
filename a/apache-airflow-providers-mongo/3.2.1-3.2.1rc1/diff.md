# Comparing `tmp/apache-airflow-providers-mongo-3.2.1.tar.gz` & `tmp/apache-airflow-providers-mongo-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-mongo-3.2.1.tar", last modified: Tue Jun 20 11:28:47 2023, max compression
+gzip compressed data, was "apache-airflow-providers-mongo-3.2.1rc1.tar", last modified: Tue Jun 20 11:42:36 2023, max compression
```

## Comparing `apache-airflow-providers-mongo-3.2.1.tar` & `apache-airflow-providers-mongo-3.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:47.619856 apache-airflow-providers-mongo-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-mongo-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:46.000000 apache-airflow-providers-mongo-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-mongo-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10759 2023-06-20 11:28:47.621618 apache-airflow-providers-mongo-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9237 2023-06-20 11:28:46.000000 apache-airflow-providers-mongo-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:47.514744 apache-airflow-providers-mongo-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:47.516006 apache-airflow-providers-mongo-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:47.559528 apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2370 2023-06-20 11:28:46.000000 apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:47.568321 apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13773 2023-06-02 11:31:21.000000 apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/hooks/mongo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:47.576199 apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2422 2023-06-02 11:31:21.000000 apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/sensors/mongo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:47.612824 apache-airflow-providers-mongo-3.2.1/apache_airflow_providers_mongo.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10759 2023-06-20 11:28:47.000000 apache-airflow-providers-mongo-3.2.1/apache_airflow_providers_mongo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      697 2023-06-20 11:28:47.000000 apache-airflow-providers-mongo-3.2.1/apache_airflow_providers_mongo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:47.000000 apache-airflow-providers-mongo-3.2.1/apache_airflow_providers_mongo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:28:47.000000 apache-airflow-providers-mongo-3.2.1/apache_airflow_providers_mongo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:47.000000 apache-airflow-providers-mongo-3.2.1/apache_airflow_providers_mongo.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-20 11:28:47.000000 apache-airflow-providers-mongo-3.2.1/apache_airflow_providers_mongo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:47.000000 apache-airflow-providers-mongo-3.2.1/apache_airflow_providers_mongo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-mongo-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1850 2023-06-20 11:28:47.624661 apache-airflow-providers-mongo-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1632 2023-06-20 11:28:46.000000 apache-airflow-providers-mongo-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:36.009263 apache-airflow-providers-mongo-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-mongo-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:34.000000 apache-airflow-providers-mongo-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-mongo-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10765 2023-06-20 11:42:36.010449 apache-airflow-providers-mongo-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9240 2023-06-20 11:42:34.000000 apache-airflow-providers-mongo-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:35.929404 apache-airflow-providers-mongo-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:35.930711 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:35.965918 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-06-20 11:42:34.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:35.971897 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13773 2023-06-02 11:31:21.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/hooks/mongo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:35.977864 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2422 2023-06-02 11:31:21.000000 apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/sensors/mongo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:36.006364 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10765 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      697 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:35.000000 apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-mongo-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-06-20 11:42:36.012547 apache-airflow-providers-mongo-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-06-20 11:42:34.000000 apache-airflow-providers-mongo-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-mongo-3.2.1/LICENSE` & `apache-airflow-providers-mongo-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.1/MANIFEST.in` & `apache-airflow-providers-mongo-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.1/PKG-INFO` & `apache-airflow-providers-mongo-3.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mongo
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mongo package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mongo``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `MongoDB <https://www.mongodb.com/what-is-mongodb>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-mongo-3.2.1/README.rst` & `apache-airflow-providers-mongo-3.2.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mongo``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `MongoDB <https://www.mongodb.com/what-is-mongodb>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/__init__.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/get_provider_info.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/hooks/__init__.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/hooks/mongo.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/hooks/mongo.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/sensors/__init__.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.1/airflow/providers/mongo/sensors/mongo.py` & `apache-airflow-providers-mongo-3.2.1rc1/airflow/providers/mongo/sensors/mongo.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.1/apache_airflow_providers_mongo.egg-info/PKG-INFO` & `apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-mongo
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-mongo package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-mongo/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-mongo``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `MongoDB <https://www.mongodb.com/what-is-mongodb>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-mongo-3.2.1/apache_airflow_providers_mongo.egg-info/SOURCES.txt` & `apache-airflow-providers-mongo-3.2.1rc1/apache_airflow_providers_mongo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.1/pyproject.toml` & `apache-airflow-providers-mongo-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-mongo-3.2.1/setup.cfg` & `apache-airflow-providers-mongo-3.2.1rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	dnspython>=1.13.0
 	pymongo>=3.6.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.mongo.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.mongo
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-mongo-3.2.1/setup.py` & `apache-airflow-providers-mongo-3.2.1rc1/setup.py`

 * *Files identical despite different names*

