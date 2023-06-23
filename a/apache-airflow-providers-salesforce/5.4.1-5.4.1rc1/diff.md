# Comparing `tmp/apache-airflow-providers-salesforce-5.4.1.tar.gz` & `tmp/apache-airflow-providers-salesforce-5.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-salesforce-5.4.1.tar", last modified: Tue Jun 20 11:29:19 2023, max compression
+gzip compressed data, was "apache-airflow-providers-salesforce-5.4.1rc1.tar", last modified: Tue Jun 20 11:43:01 2023, max compression
```

## Comparing `apache-airflow-providers-salesforce-5.4.1.tar` & `apache-airflow-providers-salesforce-5.4.1rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:19.136680 apache-airflow-providers-salesforce-5.4.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-salesforce-5.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:17.000000 apache-airflow-providers-salesforce-5.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-salesforce-5.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12188 2023-06-20 11:29:19.138018 apache-airflow-providers-salesforce-5.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10651 2023-06-20 11:29:17.000000 apache-airflow-providers-salesforce-5.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:19.035711 apache-airflow-providers-salesforce-5.4.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:19.036783 apache-airflow-providers-salesforce-5.4.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:19.082380 apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-20 11:01:09.000000 apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3045 2023-06-20 11:29:17.000000 apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:19.089974 apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18065 2023-06-02 11:31:21.000000 apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/hooks/salesforce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:19.101554 apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4762 2023-06-01 06:14:28.000000 apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/operators/bulk.py
--rw-r--r--   0 root         (0) root         (0)     2555 2023-06-02 11:31:21.000000 apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/operators/salesforce_apex_rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:19.133300 apache-airflow-providers-salesforce-5.4.1/apache_airflow_providers_salesforce.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12188 2023-06-20 11:29:18.000000 apache-airflow-providers-salesforce-5.4.1/apache_airflow_providers_salesforce.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      833 2023-06-20 11:29:19.000000 apache-airflow-providers-salesforce-5.4.1/apache_airflow_providers_salesforce.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:18.000000 apache-airflow-providers-salesforce-5.4.1/apache_airflow_providers_salesforce.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-20 11:29:18.000000 apache-airflow-providers-salesforce-5.4.1/apache_airflow_providers_salesforce.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:18.000000 apache-airflow-providers-salesforce-5.4.1/apache_airflow_providers_salesforce.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-20 11:29:18.000000 apache-airflow-providers-salesforce-5.4.1/apache_airflow_providers_salesforce.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:18.000000 apache-airflow-providers-salesforce-5.4.1/apache_airflow_providers_salesforce.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-salesforce-5.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1887 2023-06-20 11:29:19.140704 apache-airflow-providers-salesforce-5.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1662 2023-06-20 11:29:17.000000 apache-airflow-providers-salesforce-5.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.535191 apache-airflow-providers-salesforce-5.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-salesforce-5.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:00.000000 apache-airflow-providers-salesforce-5.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-salesforce-5.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12194 2023-06-20 11:43:01.536272 apache-airflow-providers-salesforce-5.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10654 2023-06-20 11:43:00.000000 apache-airflow-providers-salesforce-5.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.462015 apache-airflow-providers-salesforce-5.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.463123 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.494400 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-20 11:01:09.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3045 2023-06-20 11:43:00.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.500139 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18065 2023-06-02 11:31:21.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/hooks/salesforce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.508943 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4762 2023-06-01 06:14:28.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/bulk.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2023-06-02 11:31:21.000000 apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/salesforce_apex_rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:01.532527 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12194 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      833 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:01.000000 apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-salesforce-5.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-06-20 11:43:01.538296 apache-airflow-providers-salesforce-5.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-06-20 11:43:00.000000 apache-airflow-providers-salesforce-5.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-salesforce-5.4.1/LICENSE` & `apache-airflow-providers-salesforce-5.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.1/MANIFEST.in` & `apache-airflow-providers-salesforce-5.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.1/PKG-INFO` & `apache-airflow-providers-salesforce-5.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-salesforce
-Version: 5.4.1
+Version: 5.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-salesforce package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.4.1``
+Release: ``5.4.1rc1``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-salesforce-5.4.1/README.rst` & `apache-airflow-providers-salesforce-5.4.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.4.1``
+Release: ``5.4.1rc1``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/__init__.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/get_provider_info.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/hooks/__init__.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/hooks/salesforce.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/hooks/salesforce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/operators/__init__.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/operators/bulk.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/bulk.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.1/airflow/providers/salesforce/operators/salesforce_apex_rest.py` & `apache-airflow-providers-salesforce-5.4.1rc1/airflow/providers/salesforce/operators/salesforce_apex_rest.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.1/apache_airflow_providers_salesforce.egg-info/PKG-INFO` & `apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-salesforce
-Version: 5.4.1
+Version: 5.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-salesforce package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-salesforce/5.4.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-salesforce``
 
-Release: ``5.4.1``
+Release: ``5.4.1rc1``
 
 
 `Salesforce <https://www.salesforce.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-salesforce-5.4.1/apache_airflow_providers_salesforce.egg-info/SOURCES.txt` & `apache-airflow-providers-salesforce-5.4.1rc1/apache_airflow_providers_salesforce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.1/pyproject.toml` & `apache-airflow-providers-salesforce-5.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-salesforce-5.4.1/setup.cfg` & `apache-airflow-providers-salesforce-5.4.1rc1/setup.cfg`

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
 	pandas>=0.17.1
 	simple-salesforce>=1.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.salesforce.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.salesforce
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-salesforce-5.4.1/setup.py` & `apache-airflow-providers-salesforce-5.4.1rc1/setup.py`

 * *Files identical despite different names*

