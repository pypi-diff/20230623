# Comparing `tmp/apache-airflow-providers-tableau-4.2.1.tar.gz` & `tmp/apache-airflow-providers-tableau-4.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-tableau-4.2.1.tar", last modified: Tue Jun 20 11:29:42 2023, max compression
+gzip compressed data, was "apache-airflow-providers-tableau-4.2.1rc1.tar", last modified: Tue Jun 20 11:43:21 2023, max compression
```

## Comparing `apache-airflow-providers-tableau-4.2.1.tar` & `apache-airflow-providers-tableau-4.2.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:42.121690 apache-airflow-providers-tableau-4.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:40.000000 apache-airflow-providers-tableau-4.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12036 2023-06-20 11:29:42.123308 apache-airflow-providers-tableau-4.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10508 2023-06-20 11:29:40.000000 apache-airflow-providers-tableau-4.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:42.001098 apache-airflow-providers-tableau-4.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:42.002514 apache-airflow-providers-tableau-4.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:42.057812 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-06-20 11:29:40.000000 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:42.065812 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7079 2023-06-02 11:31:21.000000 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/hooks/tableau.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:42.072186 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5415 2023-06-02 11:31:21.000000 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/operators/tableau.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:42.078180 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2701 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/sensors/tableau.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:42.117752 apache-airflow-providers-tableau-4.2.1/apache_airflow_providers_tableau.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12036 2023-06-20 11:29:41.000000 apache-airflow-providers-tableau-4.2.1/apache_airflow_providers_tableau.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      822 2023-06-20 11:29:41.000000 apache-airflow-providers-tableau-4.2.1/apache_airflow_providers_tableau.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:41.000000 apache-airflow-providers-tableau-4.2.1/apache_airflow_providers_tableau.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:29:41.000000 apache-airflow-providers-tableau-4.2.1/apache_airflow_providers_tableau.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:41.000000 apache-airflow-providers-tableau-4.2.1/apache_airflow_providers_tableau.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 11:29:41.000000 apache-airflow-providers-tableau-4.2.1/apache_airflow_providers_tableau.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:41.000000 apache-airflow-providers-tableau-4.2.1/apache_airflow_providers_tableau.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-tableau-4.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1848 2023-06-20 11:29:42.126010 apache-airflow-providers-tableau-4.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:29:40.000000 apache-airflow-providers-tableau-4.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:21.557670 apache-airflow-providers-tableau-4.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:20.000000 apache-airflow-providers-tableau-4.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12042 2023-06-20 11:43:21.558732 apache-airflow-providers-tableau-4.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10511 2023-06-20 11:43:20.000000 apache-airflow-providers-tableau-4.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:21.479135 apache-airflow-providers-tableau-4.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:21.480199 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:21.514203 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-06-20 11:43:20.000000 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:21.519986 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7079 2023-06-02 11:31:21.000000 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/hooks/tableau.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:21.525813 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5415 2023-06-02 11:31:21.000000 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/operators/tableau.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:21.531443 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-06-01 06:14:29.000000 apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/sensors/tableau.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:21.554987 apache-airflow-providers-tableau-4.2.1rc1/apache_airflow_providers_tableau.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12042 2023-06-20 11:43:21.000000 apache-airflow-providers-tableau-4.2.1rc1/apache_airflow_providers_tableau.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      822 2023-06-20 11:43:21.000000 apache-airflow-providers-tableau-4.2.1rc1/apache_airflow_providers_tableau.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:21.000000 apache-airflow-providers-tableau-4.2.1rc1/apache_airflow_providers_tableau.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:43:21.000000 apache-airflow-providers-tableau-4.2.1rc1/apache_airflow_providers_tableau.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:21.000000 apache-airflow-providers-tableau-4.2.1rc1/apache_airflow_providers_tableau.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-20 11:43:21.000000 apache-airflow-providers-tableau-4.2.1rc1/apache_airflow_providers_tableau.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:21.000000 apache-airflow-providers-tableau-4.2.1rc1/apache_airflow_providers_tableau.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-tableau-4.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-06-20 11:43:21.560728 apache-airflow-providers-tableau-4.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:43:20.000000 apache-airflow-providers-tableau-4.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-tableau-4.2.1/LICENSE` & `apache-airflow-providers-tableau-4.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/MANIFEST.in` & `apache-airflow-providers-tableau-4.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/PKG-INFO` & `apache-airflow-providers-tableau-4.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-tableau
-Version: 4.2.1
+Version: 4.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-tableau package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-tableau/4.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-tableau``
 
-Release: ``4.2.1``
+Release: ``4.2.1rc1``
 
 
 `Tableau <https://www.tableau.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-tableau-4.2.1/README.rst` & `apache-airflow-providers-tableau-4.2.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-tableau``
 
-Release: ``4.2.1``
+Release: ``4.2.1rc1``
 
 
 `Tableau <https://www.tableau.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/__init__.py` & `apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/get_provider_info.py` & `apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/hooks/__init__.py` & `apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/hooks/tableau.py` & `apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/hooks/tableau.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/operators/__init__.py` & `apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/operators/tableau.py` & `apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/operators/tableau.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/sensors/__init__.py` & `apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/airflow/providers/tableau/sensors/tableau.py` & `apache-airflow-providers-tableau-4.2.1rc1/airflow/providers/tableau/sensors/tableau.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/apache_airflow_providers_tableau.egg-info/PKG-INFO` & `apache-airflow-providers-tableau-4.2.1rc1/apache_airflow_providers_tableau.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-tableau
-Version: 4.2.1
+Version: 4.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-tableau package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-tableau/4.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-tableau``
 
-Release: ``4.2.1``
+Release: ``4.2.1rc1``
 
 
 `Tableau <https://www.tableau.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-tableau-4.2.1/apache_airflow_providers_tableau.egg-info/SOURCES.txt` & `apache-airflow-providers-tableau-4.2.1rc1/apache_airflow_providers_tableau.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/pyproject.toml` & `apache-airflow-providers-tableau-4.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tableau-4.2.1/setup.cfg` & `apache-airflow-providers-tableau-4.2.1rc1/setup.cfg`

 * *Files 5% similar despite different names*

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
 	tableauserverclient
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.tableau.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.tableau
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-tableau-4.2.1/setup.py` & `apache-airflow-providers-tableau-4.2.1rc1/setup.py`

 * *Files identical despite different names*

