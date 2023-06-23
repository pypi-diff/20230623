# Comparing `tmp/apache-airflow-providers-papermill-3.2.1.tar.gz` & `tmp/apache-airflow-providers-papermill-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-papermill-3.2.1.tar", last modified: Tue Jun 20 11:29:06 2023, max compression
+gzip compressed data, was "apache-airflow-providers-papermill-3.2.1rc1.tar", last modified: Tue Jun 20 11:42:50 2023, max compression
```

## Comparing `apache-airflow-providers-papermill-3.2.1.tar` & `apache-airflow-providers-papermill-3.2.1rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:06.192426 apache-airflow-providers-papermill-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-papermill-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:04.000000 apache-airflow-providers-papermill-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-papermill-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10851 2023-06-20 11:29:06.193449 apache-airflow-providers-papermill-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9317 2023-06-20 11:29:04.000000 apache-airflow-providers-papermill-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:06.101354 apache-airflow-providers-papermill-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:06.102922 apache-airflow-providers-papermill-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:06.147689 apache-airflow-providers-papermill-3.2.1/airflow/providers/papermill/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-papermill-3.2.1/airflow/providers/papermill/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-06-20 11:29:04.000000 apache-airflow-providers-papermill-3.2.1/airflow/providers/papermill/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:06.154125 apache-airflow-providers-papermill-3.2.1/airflow/providers/papermill/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-papermill-3.2.1/airflow/providers/papermill/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3714 2023-06-02 11:31:21.000000 apache-airflow-providers-papermill-3.2.1/airflow/providers/papermill/operators/papermill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:06.186791 apache-airflow-providers-papermill-3.2.1/apache_airflow_providers_papermill.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10851 2023-06-20 11:29:06.000000 apache-airflow-providers-papermill-3.2.1/apache_airflow_providers_papermill.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      668 2023-06-20 11:29:06.000000 apache-airflow-providers-papermill-3.2.1/apache_airflow_providers_papermill.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:06.000000 apache-airflow-providers-papermill-3.2.1/apache_airflow_providers_papermill.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:29:06.000000 apache-airflow-providers-papermill-3.2.1/apache_airflow_providers_papermill.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:06.000000 apache-airflow-providers-papermill-3.2.1/apache_airflow_providers_papermill.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-20 11:29:06.000000 apache-airflow-providers-papermill-3.2.1/apache_airflow_providers_papermill.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:06.000000 apache-airflow-providers-papermill-3.2.1/apache_airflow_providers_papermill.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-papermill-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1878 2023-06-20 11:29:06.196329 apache-airflow-providers-papermill-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1656 2023-06-20 11:29:04.000000 apache-airflow-providers-papermill-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:50.768182 apache-airflow-providers-papermill-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-papermill-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:49.000000 apache-airflow-providers-papermill-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-papermill-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10857 2023-06-20 11:42:50.769282 apache-airflow-providers-papermill-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9320 2023-06-20 11:42:49.000000 apache-airflow-providers-papermill-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:50.695578 apache-airflow-providers-papermill-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:50.696729 apache-airflow-providers-papermill-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:50.728147 apache-airflow-providers-papermill-3.2.1rc1/airflow/providers/papermill/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-papermill-3.2.1rc1/airflow/providers/papermill/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-06-20 11:42:49.000000 apache-airflow-providers-papermill-3.2.1rc1/airflow/providers/papermill/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:50.737528 apache-airflow-providers-papermill-3.2.1rc1/airflow/providers/papermill/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-papermill-3.2.1rc1/airflow/providers/papermill/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3714 2023-06-02 11:31:21.000000 apache-airflow-providers-papermill-3.2.1rc1/airflow/providers/papermill/operators/papermill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:50.765525 apache-airflow-providers-papermill-3.2.1rc1/apache_airflow_providers_papermill.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10857 2023-06-20 11:42:50.000000 apache-airflow-providers-papermill-3.2.1rc1/apache_airflow_providers_papermill.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      668 2023-06-20 11:42:50.000000 apache-airflow-providers-papermill-3.2.1rc1/apache_airflow_providers_papermill.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:50.000000 apache-airflow-providers-papermill-3.2.1rc1/apache_airflow_providers_papermill.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:42:50.000000 apache-airflow-providers-papermill-3.2.1rc1/apache_airflow_providers_papermill.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:50.000000 apache-airflow-providers-papermill-3.2.1rc1/apache_airflow_providers_papermill.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-20 11:42:50.000000 apache-airflow-providers-papermill-3.2.1rc1/apache_airflow_providers_papermill.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:50.000000 apache-airflow-providers-papermill-3.2.1rc1/apache_airflow_providers_papermill.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-papermill-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-20 11:42:50.771201 apache-airflow-providers-papermill-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-06-20 11:42:49.000000 apache-airflow-providers-papermill-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-papermill-3.2.1/LICENSE` & `apache-airflow-providers-papermill-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-papermill-3.2.1/MANIFEST.in` & `apache-airflow-providers-papermill-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-papermill-3.2.1/PKG-INFO` & `apache-airflow-providers-papermill-3.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-papermill
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-papermill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-papermill``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Papermill <https://github.com/nteract/papermill>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-papermill-3.2.1/README.rst` & `apache-airflow-providers-papermill-3.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-papermill``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Papermill <https://github.com/nteract/papermill>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-papermill-3.2.1/airflow/providers/papermill/__init__.py` & `apache-airflow-providers-papermill-3.2.1rc1/airflow/providers/papermill/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-papermill-3.2.1/airflow/providers/papermill/get_provider_info.py` & `apache-airflow-providers-papermill-3.2.1rc1/airflow/providers/papermill/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-papermill-3.2.1/airflow/providers/papermill/operators/__init__.py` & `apache-airflow-providers-papermill-3.2.1rc1/airflow/providers/papermill/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-papermill-3.2.1/airflow/providers/papermill/operators/papermill.py` & `apache-airflow-providers-papermill-3.2.1rc1/airflow/providers/papermill/operators/papermill.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-papermill-3.2.1/apache_airflow_providers_papermill.egg-info/PKG-INFO` & `apache-airflow-providers-papermill-3.2.1rc1/apache_airflow_providers_papermill.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-papermill
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-papermill package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-papermill/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-papermill``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Papermill <https://github.com/nteract/papermill>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-papermill-3.2.1/apache_airflow_providers_papermill.egg-info/SOURCES.txt` & `apache-airflow-providers-papermill-3.2.1rc1/apache_airflow_providers_papermill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-papermill-3.2.1/pyproject.toml` & `apache-airflow-providers-papermill-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-papermill-3.2.1/setup.cfg` & `apache-airflow-providers-papermill-3.2.1rc1/setup.cfg`

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
 	papermill[all]>=1.2.1
 	scrapbook[all]
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.papermill.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.papermill
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-papermill-3.2.1/setup.py` & `apache-airflow-providers-papermill-3.2.1rc1/setup.py`

 * *Files identical despite different names*

