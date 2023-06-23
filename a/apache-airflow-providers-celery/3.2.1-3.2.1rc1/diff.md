# Comparing `tmp/apache-airflow-providers-celery-3.2.1.tar.gz` & `tmp/apache-airflow-providers-celery-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-celery-3.2.1.tar", last modified: Tue Jun 20 11:27:48 2023, max compression
+gzip compressed data, was "apache-airflow-providers-celery-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:39 2023, max compression
```

## Comparing `apache-airflow-providers-celery-3.2.1.tar` & `apache-airflow-providers-celery-3.2.1rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:48.796460 apache-airflow-providers-celery-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:47.000000 apache-airflow-providers-celery-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9647 2023-06-20 11:27:48.797520 apache-airflow-providers-celery-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8122 2023-06-20 11:27:47.000000 apache-airflow-providers-celery-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:48.717646 apache-airflow-providers-celery-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:48.719076 apache-airflow-providers-celery-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:48.759506 apache-airflow-providers-celery-3.2.1/airflow/providers/celery/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-celery-3.2.1/airflow/providers/celery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-06-20 11:27:47.000000 apache-airflow-providers-celery-3.2.1/airflow/providers/celery/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:48.765972 apache-airflow-providers-celery-3.2.1/airflow/providers/celery/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-celery-3.2.1/airflow/providers/celery/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-06-01 06:14:28.000000 apache-airflow-providers-celery-3.2.1/airflow/providers/celery/sensors/celery_queue.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:48.793814 apache-airflow-providers-celery-3.2.1/apache_airflow_providers_celery.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9647 2023-06-20 11:27:48.000000 apache-airflow-providers-celery-3.2.1/apache_airflow_providers_celery.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      634 2023-06-20 11:27:48.000000 apache-airflow-providers-celery-3.2.1/apache_airflow_providers_celery.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:48.000000 apache-airflow-providers-celery-3.2.1/apache_airflow_providers_celery.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:27:48.000000 apache-airflow-providers-celery-3.2.1/apache_airflow_providers_celery.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:48.000000 apache-airflow-providers-celery-3.2.1/apache_airflow_providers_celery.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-20 11:27:48.000000 apache-airflow-providers-celery-3.2.1/apache_airflow_providers_celery.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:48.000000 apache-airflow-providers-celery-3.2.1/apache_airflow_providers_celery.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-celery-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-20 11:27:48.799780 apache-airflow-providers-celery-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1638 2023-06-20 11:27:47.000000 apache-airflow-providers-celery-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.607708 apache-airflow-providers-celery-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:38.000000 apache-airflow-providers-celery-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-celery-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9653 2023-06-20 11:41:39.609077 apache-airflow-providers-celery-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8125 2023-06-20 11:41:38.000000 apache-airflow-providers-celery-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.531177 apache-airflow-providers-celery-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.532943 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.570323 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-20 11:41:38.000000 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.576244 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-06-01 06:14:28.000000 apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/sensors/celery_queue.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:39.604153 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9653 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      634 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:39.000000 apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-celery-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-06-20 11:41:39.611375 apache-airflow-providers-celery-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-06-20 11:41:38.000000 apache-airflow-providers-celery-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-celery-3.2.1/LICENSE` & `apache-airflow-providers-celery-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.1/MANIFEST.in` & `apache-airflow-providers-celery-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.1/PKG-INFO` & `apache-airflow-providers-celery-3.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-celery
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-celery package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-celery-3.2.1/README.rst` & `apache-airflow-providers-celery-3.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-celery-3.2.1/airflow/providers/celery/__init__.py` & `apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.1/airflow/providers/celery/get_provider_info.py` & `apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.1/airflow/providers/celery/sensors/__init__.py` & `apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.1/airflow/providers/celery/sensors/celery_queue.py` & `apache-airflow-providers-celery-3.2.1rc1/airflow/providers/celery/sensors/celery_queue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.1/apache_airflow_providers_celery.egg-info/PKG-INFO` & `apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-celery
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-celery package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-celery/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-celery``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Celery <http://www.celeryproject.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-celery-3.2.1/apache_airflow_providers_celery.egg-info/SOURCES.txt` & `apache-airflow-providers-celery-3.2.1rc1/apache_airflow_providers_celery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.1/pyproject.toml` & `apache-airflow-providers-celery-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-celery-3.2.1/setup.cfg` & `apache-airflow-providers-celery-3.2.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

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
 	celery>=5.2.3,<6
 	flower>=1.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.celery.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.celery
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-celery-3.2.1/setup.py` & `apache-airflow-providers-celery-3.2.1rc1/setup.py`

 * *Files identical despite different names*

