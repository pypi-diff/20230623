# Comparing `tmp/apache-airflow-providers-apache-beam-5.1.1.tar.gz` & `tmp/apache-airflow-providers-apache-beam-5.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-beam-5.1.1.tar", last modified: Tue Jun 20 11:27:16 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-beam-5.1.1rc1.tar", last modified: Tue Jun 20 11:41:06 2023, max compression
```

## Comparing `apache-airflow-providers-apache-beam-5.1.1.tar` & `apache-airflow-providers-apache-beam-5.1.1rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:16.341664 apache-airflow-providers-apache-beam-5.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-beam-5.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:15.000000 apache-airflow-providers-apache-beam-5.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-beam-5.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15855 2023-06-20 11:27:16.342750 apache-airflow-providers-apache-beam-5.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14292 2023-06-20 11:27:15.000000 apache-airflow-providers-apache-beam-5.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:16.261083 apache-airflow-providers-apache-beam-5.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:16.262254 apache-airflow-providers-apache-beam-5.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:16.263360 apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:16.298300 apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2532 2023-06-20 11:27:15.000000 apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:16.304908 apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14197 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/hooks/beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:16.311922 apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32492 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/operators/beam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:16.338939 apache-airflow-providers-apache-beam-5.1.1/apache_airflow_providers_apache_beam.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15855 2023-06-20 11:27:16.000000 apache-airflow-providers-apache-beam-5.1.1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2023-06-20 11:27:16.000000 apache-airflow-providers-apache-beam-5.1.1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:16.000000 apache-airflow-providers-apache-beam-5.1.1/apache_airflow_providers_apache_beam.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:27:16.000000 apache-airflow-providers-apache-beam-5.1.1/apache_airflow_providers_apache_beam.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:16.000000 apache-airflow-providers-apache-beam-5.1.1/apache_airflow_providers_apache_beam.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:27:16.000000 apache-airflow-providers-apache-beam-5.1.1/apache_airflow_providers_apache_beam.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:16.000000 apache-airflow-providers-apache-beam-5.1.1/apache_airflow_providers_apache_beam.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-beam-5.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1872 2023-06-20 11:27:16.344975 apache-airflow-providers-apache-beam-5.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1733 2023-06-20 11:27:15.000000 apache-airflow-providers-apache-beam-5.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.706713 apache-airflow-providers-apache-beam-5.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-beam-5.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:05.000000 apache-airflow-providers-apache-beam-5.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-beam-5.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15861 2023-06-20 11:41:06.707716 apache-airflow-providers-apache-beam-5.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14295 2023-06-20 11:41:05.000000 apache-airflow-providers-apache-beam-5.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.634552 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.635650 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.636649 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.668032 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-06-20 11:41:05.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.673565 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14197 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/hooks/beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.679189 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32492 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/operators/beam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:06.704020 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15861 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      777 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:06.000000 apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-beam-5.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-06-20 11:41:06.709699 apache-airflow-providers-apache-beam-5.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-06-20 11:41:05.000000 apache-airflow-providers-apache-beam-5.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-beam-5.1.1/LICENSE` & `apache-airflow-providers-apache-beam-5.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1/MANIFEST.in` & `apache-airflow-providers-apache-beam-5.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1/PKG-INFO` & `apache-airflow-providers-apache-beam-5.1.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-beam
-Version: 5.1.1
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-beam package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.1.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``5.1.1``
+Release: ``5.1.1rc1``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-beam-5.1.1/README.rst` & `apache-airflow-providers-apache-beam-5.1.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``5.1.1``
+Release: ``5.1.1rc1``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/__init__.py` & `apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/get_provider_info.py` & `apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/hooks/__init__.py` & `apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/hooks/beam.py` & `apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/hooks/beam.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/operators/__init__.py` & `apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1/airflow/providers/apache/beam/operators/beam.py` & `apache-airflow-providers-apache-beam-5.1.1rc1/airflow/providers/apache/beam/operators/beam.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO` & `apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-beam
-Version: 5.1.1
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-beam package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-beam/5.1.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-beam``
 
-Release: ``5.1.1``
+Release: ``5.1.1rc1``
 
 
 `Apache Beam <https://beam.apache.org/>`__.
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-beam-5.1.1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-beam-5.1.1rc1/apache_airflow_providers_apache_beam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1/pyproject.toml` & `apache-airflow-providers-apache-beam-5.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-beam-5.1.1/setup.cfg` & `apache-airflow-providers-apache-beam-5.1.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

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
 	apache-beam>=2.47.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.beam.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.beam
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-beam-5.1.1/setup.py` & `apache-airflow-providers-apache-beam-5.1.1rc1/setup.py`

 * *Files identical despite different names*

