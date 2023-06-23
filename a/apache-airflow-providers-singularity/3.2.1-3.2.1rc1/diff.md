# Comparing `tmp/apache-airflow-providers-singularity-3.2.1.tar.gz` & `tmp/apache-airflow-providers-singularity-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-singularity-3.2.1.tar", last modified: Tue Jun 20 11:29:29 2023, max compression
+gzip compressed data, was "apache-airflow-providers-singularity-3.2.1rc1.tar", last modified: Tue Jun 20 11:43:10 2023, max compression
```

## Comparing `apache-airflow-providers-singularity-3.2.1.tar` & `apache-airflow-providers-singularity-3.2.1rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:29.804478 apache-airflow-providers-singularity-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-singularity-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:28.000000 apache-airflow-providers-singularity-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-singularity-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10233 2023-06-20 11:29:29.805569 apache-airflow-providers-singularity-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8693 2023-06-20 11:29:28.000000 apache-airflow-providers-singularity-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:29.727454 apache-airflow-providers-singularity-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:29.728895 apache-airflow-providers-singularity-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:29.765562 apache-airflow-providers-singularity-3.2.1/airflow/providers/singularity/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-singularity-3.2.1/airflow/providers/singularity/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-06-20 11:29:28.000000 apache-airflow-providers-singularity-3.2.1/airflow/providers/singularity/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:29.771922 apache-airflow-providers-singularity-3.2.1/airflow/providers/singularity/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-singularity-3.2.1/airflow/providers/singularity/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6935 2023-06-02 11:31:21.000000 apache-airflow-providers-singularity-3.2.1/airflow/providers/singularity/operators/singularity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:29.801726 apache-airflow-providers-singularity-3.2.1/apache_airflow_providers_singularity.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10233 2023-06-20 11:29:29.000000 apache-airflow-providers-singularity-3.2.1/apache_airflow_providers_singularity.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-20 11:29:29.000000 apache-airflow-providers-singularity-3.2.1/apache_airflow_providers_singularity.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:29.000000 apache-airflow-providers-singularity-3.2.1/apache_airflow_providers_singularity.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:29:29.000000 apache-airflow-providers-singularity-3.2.1/apache_airflow_providers_singularity.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:29.000000 apache-airflow-providers-singularity-3.2.1/apache_airflow_providers_singularity.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 11:29:29.000000 apache-airflow-providers-singularity-3.2.1/apache_airflow_providers_singularity.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:29.000000 apache-airflow-providers-singularity-3.2.1/apache_airflow_providers_singularity.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-singularity-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1868 2023-06-20 11:29:29.807618 apache-airflow-providers-singularity-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-20 11:29:28.000000 apache-airflow-providers-singularity-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:10.340562 apache-airflow-providers-singularity-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-singularity-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:09.000000 apache-airflow-providers-singularity-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-singularity-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10239 2023-06-20 11:43:10.341642 apache-airflow-providers-singularity-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8696 2023-06-20 11:43:09.000000 apache-airflow-providers-singularity-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:10.274361 apache-airflow-providers-singularity-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:10.275532 apache-airflow-providers-singularity-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:10.308536 apache-airflow-providers-singularity-3.2.1rc1/airflow/providers/singularity/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-singularity-3.2.1rc1/airflow/providers/singularity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-06-20 11:43:09.000000 apache-airflow-providers-singularity-3.2.1rc1/airflow/providers/singularity/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:10.314406 apache-airflow-providers-singularity-3.2.1rc1/airflow/providers/singularity/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-singularity-3.2.1rc1/airflow/providers/singularity/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6935 2023-06-02 11:31:21.000000 apache-airflow-providers-singularity-3.2.1rc1/airflow/providers/singularity/operators/singularity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:10.338140 apache-airflow-providers-singularity-3.2.1rc1/apache_airflow_providers_singularity.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10239 2023-06-20 11:43:10.000000 apache-airflow-providers-singularity-3.2.1rc1/apache_airflow_providers_singularity.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-20 11:43:10.000000 apache-airflow-providers-singularity-3.2.1rc1/apache_airflow_providers_singularity.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:10.000000 apache-airflow-providers-singularity-3.2.1rc1/apache_airflow_providers_singularity.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:43:10.000000 apache-airflow-providers-singularity-3.2.1rc1/apache_airflow_providers_singularity.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:10.000000 apache-airflow-providers-singularity-3.2.1rc1/apache_airflow_providers_singularity.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 11:43:10.000000 apache-airflow-providers-singularity-3.2.1rc1/apache_airflow_providers_singularity.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:10.000000 apache-airflow-providers-singularity-3.2.1rc1/apache_airflow_providers_singularity.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-singularity-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-20 11:43:10.343555 apache-airflow-providers-singularity-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-20 11:43:09.000000 apache-airflow-providers-singularity-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-singularity-3.2.1/LICENSE` & `apache-airflow-providers-singularity-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-singularity-3.2.1/MANIFEST.in` & `apache-airflow-providers-singularity-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-singularity-3.2.1/PKG-INFO` & `apache-airflow-providers-singularity-3.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-singularity
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-singularity package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-singularity/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-singularity``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Singularity <https://sylabs.io/guides/latest/user-guide/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-singularity-3.2.1/README.rst` & `apache-airflow-providers-singularity-3.2.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-singularity``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Singularity <https://sylabs.io/guides/latest/user-guide/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-singularity-3.2.1/airflow/providers/singularity/__init__.py` & `apache-airflow-providers-singularity-3.2.1rc1/airflow/providers/singularity/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-singularity-3.2.1/airflow/providers/singularity/get_provider_info.py` & `apache-airflow-providers-singularity-3.2.1rc1/airflow/providers/singularity/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-singularity-3.2.1/airflow/providers/singularity/operators/__init__.py` & `apache-airflow-providers-singularity-3.2.1rc1/airflow/providers/singularity/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-singularity-3.2.1/airflow/providers/singularity/operators/singularity.py` & `apache-airflow-providers-singularity-3.2.1rc1/airflow/providers/singularity/operators/singularity.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-singularity-3.2.1/apache_airflow_providers_singularity.egg-info/PKG-INFO` & `apache-airflow-providers-singularity-3.2.1rc1/apache_airflow_providers_singularity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-singularity
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-singularity package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-singularity/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-singularity``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Singularity <https://sylabs.io/guides/latest/user-guide/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-singularity-3.2.1/apache_airflow_providers_singularity.egg-info/SOURCES.txt` & `apache-airflow-providers-singularity-3.2.1rc1/apache_airflow_providers_singularity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-singularity-3.2.1/pyproject.toml` & `apache-airflow-providers-singularity-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-singularity-3.2.1/setup.cfg` & `apache-airflow-providers-singularity-3.2.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

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
 	spython>=0.0.56
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.singularity.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.singularity
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-singularity-3.2.1/setup.py` & `apache-airflow-providers-singularity-3.2.1rc1/setup.py`

 * *Files identical despite different names*

