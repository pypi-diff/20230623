# Comparing `tmp/apache-airflow-providers-cloudant-3.2.1.tar.gz` & `tmp/apache-airflow-providers-cloudant-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-cloudant-3.2.1.tar", last modified: Tue Jun 20 11:27:50 2023, max compression
+gzip compressed data, was "apache-airflow-providers-cloudant-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:41 2023, max compression
```

## Comparing `apache-airflow-providers-cloudant-3.2.1.tar` & `apache-airflow-providers-cloudant-3.2.1rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:50.540855 apache-airflow-providers-cloudant-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cloudant-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:49.000000 apache-airflow-providers-cloudant-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cloudant-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9822 2023-06-20 11:27:50.541853 apache-airflow-providers-cloudant-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8291 2023-06-20 11:27:49.000000 apache-airflow-providers-cloudant-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:50.471315 apache-airflow-providers-cloudant-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:50.472521 apache-airflow-providers-cloudant-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:50.508078 apache-airflow-providers-cloudant-3.2.1/airflow/providers/cloudant/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-cloudant-3.2.1/airflow/providers/cloudant/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-06-20 11:27:49.000000 apache-airflow-providers-cloudant-3.2.1/airflow/providers/cloudant/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:50.514092 apache-airflow-providers-cloudant-3.2.1/airflow/providers/cloudant/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cloudant-3.2.1/airflow/providers/cloudant/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2898 2023-06-02 11:31:21.000000 apache-airflow-providers-cloudant-3.2.1/airflow/providers/cloudant/hooks/cloudant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:50.538569 apache-airflow-providers-cloudant-3.2.1/apache_airflow_providers_cloudant.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9822 2023-06-20 11:27:50.000000 apache-airflow-providers-cloudant-3.2.1/apache_airflow_providers_cloudant.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      648 2023-06-20 11:27:50.000000 apache-airflow-providers-cloudant-3.2.1/apache_airflow_providers_cloudant.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:50.000000 apache-airflow-providers-cloudant-3.2.1/apache_airflow_providers_cloudant.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:27:50.000000 apache-airflow-providers-cloudant-3.2.1/apache_airflow_providers_cloudant.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:50.000000 apache-airflow-providers-cloudant-3.2.1/apache_airflow_providers_cloudant.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-20 11:27:50.000000 apache-airflow-providers-cloudant-3.2.1/apache_airflow_providers_cloudant.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:50.000000 apache-airflow-providers-cloudant-3.2.1/apache_airflow_providers_cloudant.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-cloudant-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1848 2023-06-20 11:27:50.543793 apache-airflow-providers-cloudant-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:27:49.000000 apache-airflow-providers-cloudant-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:41.395280 apache-airflow-providers-cloudant-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-cloudant-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:40.000000 apache-airflow-providers-cloudant-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-cloudant-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9828 2023-06-20 11:41:41.396302 apache-airflow-providers-cloudant-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8294 2023-06-20 11:41:40.000000 apache-airflow-providers-cloudant-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:41.330542 apache-airflow-providers-cloudant-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:41.331790 apache-airflow-providers-cloudant-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:41.362632 apache-airflow-providers-cloudant-3.2.1rc1/airflow/providers/cloudant/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-cloudant-3.2.1rc1/airflow/providers/cloudant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-06-20 11:41:40.000000 apache-airflow-providers-cloudant-3.2.1rc1/airflow/providers/cloudant/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:41.368906 apache-airflow-providers-cloudant-3.2.1rc1/airflow/providers/cloudant/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-cloudant-3.2.1rc1/airflow/providers/cloudant/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-06-02 11:31:21.000000 apache-airflow-providers-cloudant-3.2.1rc1/airflow/providers/cloudant/hooks/cloudant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:41.392980 apache-airflow-providers-cloudant-3.2.1rc1/apache_airflow_providers_cloudant.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9828 2023-06-20 11:41:41.000000 apache-airflow-providers-cloudant-3.2.1rc1/apache_airflow_providers_cloudant.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      648 2023-06-20 11:41:41.000000 apache-airflow-providers-cloudant-3.2.1rc1/apache_airflow_providers_cloudant.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:41.000000 apache-airflow-providers-cloudant-3.2.1rc1/apache_airflow_providers_cloudant.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:41:41.000000 apache-airflow-providers-cloudant-3.2.1rc1/apache_airflow_providers_cloudant.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:41.000000 apache-airflow-providers-cloudant-3.2.1rc1/apache_airflow_providers_cloudant.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-20 11:41:41.000000 apache-airflow-providers-cloudant-3.2.1rc1/apache_airflow_providers_cloudant.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:41.000000 apache-airflow-providers-cloudant-3.2.1rc1/apache_airflow_providers_cloudant.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-cloudant-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1856 2023-06-20 11:41:41.398194 apache-airflow-providers-cloudant-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:41:40.000000 apache-airflow-providers-cloudant-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-cloudant-3.2.1/LICENSE` & `apache-airflow-providers-cloudant-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cloudant-3.2.1/MANIFEST.in` & `apache-airflow-providers-cloudant-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cloudant-3.2.1/PKG-INFO` & `apache-airflow-providers-cloudant-3.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cloudant
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cloudant package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cloudant/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cloudant``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `IBM Cloudant <https://www.ibm.com/cloud/cloudant>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-cloudant-3.2.1/README.rst` & `apache-airflow-providers-cloudant-3.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cloudant``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `IBM Cloudant <https://www.ibm.com/cloud/cloudant>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-cloudant-3.2.1/airflow/providers/cloudant/__init__.py` & `apache-airflow-providers-cloudant-3.2.1rc1/airflow/providers/cloudant/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cloudant-3.2.1/airflow/providers/cloudant/get_provider_info.py` & `apache-airflow-providers-cloudant-3.2.1rc1/airflow/providers/cloudant/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cloudant-3.2.1/airflow/providers/cloudant/hooks/__init__.py` & `apache-airflow-providers-cloudant-3.2.1rc1/airflow/providers/cloudant/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cloudant-3.2.1/airflow/providers/cloudant/hooks/cloudant.py` & `apache-airflow-providers-cloudant-3.2.1rc1/airflow/providers/cloudant/hooks/cloudant.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cloudant-3.2.1/apache_airflow_providers_cloudant.egg-info/PKG-INFO` & `apache-airflow-providers-cloudant-3.2.1rc1/apache_airflow_providers_cloudant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cloudant
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-cloudant package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-cloudant/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-cloudant``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `IBM Cloudant <https://www.ibm.com/cloud/cloudant>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-cloudant-3.2.1/apache_airflow_providers_cloudant.egg-info/SOURCES.txt` & `apache-airflow-providers-cloudant-3.2.1rc1/apache_airflow_providers_cloudant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cloudant-3.2.1/pyproject.toml` & `apache-airflow-providers-cloudant-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-cloudant-3.2.1/setup.cfg` & `apache-airflow-providers-cloudant-3.2.1rc1/setup.cfg`

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
 	cloudant>=2.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.cloudant.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.cloudant
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-cloudant-3.2.1/setup.py` & `apache-airflow-providers-cloudant-3.2.1rc1/setup.py`

 * *Files identical despite different names*

