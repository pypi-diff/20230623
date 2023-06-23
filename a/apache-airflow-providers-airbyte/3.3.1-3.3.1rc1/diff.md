# Comparing `tmp/apache-airflow-providers-airbyte-3.3.1.tar.gz` & `tmp/apache-airflow-providers-airbyte-3.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-airbyte-3.3.1.tar", last modified: Tue Jun 20 11:27:08 2023, max compression
+gzip compressed data, was "apache-airflow-providers-airbyte-3.3.1rc1.tar", last modified: Tue Jun 20 11:40:58 2023, max compression
```

## Comparing `apache-airflow-providers-airbyte-3.3.1.tar` & `apache-airflow-providers-airbyte-3.3.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:08.433676 apache-airflow-providers-airbyte-3.3.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-airbyte-3.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:07.000000 apache-airflow-providers-airbyte-3.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-airbyte-3.3.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11898 2023-06-20 11:27:08.434882 apache-airflow-providers-airbyte-3.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10349 2023-06-20 11:27:07.000000 apache-airflow-providers-airbyte-3.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:08.329919 apache-airflow-providers-airbyte-3.3.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:08.331086 apache-airflow-providers-airbyte-3.3.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:08.378070 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2638 2023-06-20 11:27:07.000000 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:08.384880 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5062 2023-06-02 11:31:21.000000 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/hooks/airbyte.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:08.395782 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-06-02 11:31:21.000000 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/operators/airbyte.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:08.403531 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2793 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/sensors/airbyte.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:08.430532 apache-airflow-providers-airbyte-3.3.1/apache_airflow_providers_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11898 2023-06-20 11:27:08.000000 apache-airflow-providers-airbyte-3.3.1/apache_airflow_providers_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      822 2023-06-20 11:27:08.000000 apache-airflow-providers-airbyte-3.3.1/apache_airflow_providers_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:08.000000 apache-airflow-providers-airbyte-3.3.1/apache_airflow_providers_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:27:08.000000 apache-airflow-providers-airbyte-3.3.1/apache_airflow_providers_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:08.000000 apache-airflow-providers-airbyte-3.3.1/apache_airflow_providers_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-20 11:27:08.000000 apache-airflow-providers-airbyte-3.3.1/apache_airflow_providers_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:08.000000 apache-airflow-providers-airbyte-3.3.1/apache_airflow_providers_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-airbyte-3.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1858 2023-06-20 11:27:08.437113 apache-airflow-providers-airbyte-3.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1685 2023-06-20 11:27:07.000000 apache-airflow-providers-airbyte-3.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.726176 apache-airflow-providers-airbyte-3.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-airbyte-3.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:40:57.000000 apache-airflow-providers-airbyte-3.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-airbyte-3.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11904 2023-06-20 11:40:58.727218 apache-airflow-providers-airbyte-3.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10352 2023-06-20 11:40:57.000000 apache-airflow-providers-airbyte-3.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.634029 apache-airflow-providers-airbyte-3.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.635088 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.669079 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-06-20 11:40:57.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.676813 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5062 2023-06-02 11:31:21.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/hooks/airbyte.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.682876 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-06-02 11:31:21.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/operators/airbyte.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.690628 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-06-01 06:14:28.000000 apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/sensors/airbyte.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:40:58.723493 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11904 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      822 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:40:58.000000 apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-airbyte-3.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-20 11:40:58.729147 apache-airflow-providers-airbyte-3.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-06-20 11:40:57.000000 apache-airflow-providers-airbyte-3.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-airbyte-3.3.1/LICENSE` & `apache-airflow-providers-airbyte-3.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/MANIFEST.in` & `apache-airflow-providers-airbyte-3.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/PKG-INFO` & `apache-airflow-providers-airbyte-3.3.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-airbyte
-Version: 3.3.1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-airbyte package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-airbyte``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Airbyte <https://airbyte.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-airbyte-3.3.1/README.rst` & `apache-airflow-providers-airbyte-3.3.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-airbyte``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Airbyte <https://airbyte.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/__init__.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/get_provider_info.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/hooks/__init__.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/hooks/airbyte.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/hooks/airbyte.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/operators/__init__.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/operators/airbyte.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/operators/airbyte.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/sensors/__init__.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/airflow/providers/airbyte/sensors/airbyte.py` & `apache-airflow-providers-airbyte-3.3.1rc1/airflow/providers/airbyte/sensors/airbyte.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/apache_airflow_providers_airbyte.egg-info/PKG-INFO` & `apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-airbyte
-Version: 3.3.1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-airbyte package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-airbyte/3.3.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-airbyte``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Airbyte <https://airbyte.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-airbyte-3.3.1/apache_airflow_providers_airbyte.egg-info/SOURCES.txt` & `apache-airflow-providers-airbyte-3.3.1rc1/apache_airflow_providers_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/pyproject.toml` & `apache-airflow-providers-airbyte-3.3.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-airbyte-3.3.1/setup.cfg` & `apache-airflow-providers-airbyte-3.3.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-http
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.airbyte.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.airbyte
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-airbyte-3.3.1/setup.py` & `apache-airflow-providers-airbyte-3.3.1rc1/setup.py`

 * *Files identical despite different names*

