# Comparing `tmp/apache-airflow-providers-dbt-cloud-3.2.1.tar.gz` & `tmp/apache-airflow-providers-dbt-cloud-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-dbt-cloud-3.2.1.tar", last modified: Tue Jun 20 11:27:59 2023, max compression
+gzip compressed data, was "apache-airflow-providers-dbt-cloud-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:51 2023, max compression
```

## Comparing `apache-airflow-providers-dbt-cloud-3.2.1.tar` & `apache-airflow-providers-dbt-cloud-3.2.1rc1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:59.983050 apache-airflow-providers-dbt-cloud-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:58.000000 apache-airflow-providers-dbt-cloud-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11722 2023-06-20 11:27:59.984076 apache-airflow-providers-dbt-cloud-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10167 2023-06-20 11:27:58.000000 apache-airflow-providers-dbt-cloud-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:59.893352 apache-airflow-providers-dbt-cloud-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:59.894495 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:59.895581 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:59.931384 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-06-20 11:27:58.000000 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:59.937399 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24235 2023-06-02 11:31:21.000000 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/hooks/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:59.943526 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13638 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/operators/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:59.949373 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5614 2023-06-05 12:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/sensors/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:59.955427 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4649 2023-06-05 12:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/triggers/dbt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:59.980796 apache-airflow-providers-dbt-cloud-3.2.1/apache_airflow_providers_dbt_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11722 2023-06-20 11:27:59.000000 apache-airflow-providers-dbt-cloud-3.2.1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      933 2023-06-20 11:27:59.000000 apache-airflow-providers-dbt-cloud-3.2.1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:59.000000 apache-airflow-providers-dbt-cloud-3.2.1/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:27:59.000000 apache-airflow-providers-dbt-cloud-3.2.1/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:59.000000 apache-airflow-providers-dbt-cloud-3.2.1/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:27:59.000000 apache-airflow-providers-dbt-cloud-3.2.1/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:59.000000 apache-airflow-providers-dbt-cloud-3.2.1/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-dbt-cloud-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1888 2023-06-20 11:27:59.985944 apache-airflow-providers-dbt-cloud-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1697 2023-06-20 11:27:58.000000 apache-airflow-providers-dbt-cloud-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:51.021236 apache-airflow-providers-dbt-cloud-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11728 2023-06-20 11:41:51.022307 apache-airflow-providers-dbt-cloud-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10170 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.931297 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.932461 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.933570 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.970994 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.976859 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24235 2023-06-02 11:31:21.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.983054 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13638 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.988790 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5614 2023-06-05 12:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:50.994693 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4649 2023-06-05 12:50:36.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:51.018368 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11728 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      933 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:50.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-06-20 11:41:51.024226 apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-06-20 11:41:49.000000 apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/LICENSE` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/MANIFEST.in` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/README.rst` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/get_provider_info.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/hooks/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/hooks/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/hooks/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/operators/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/operators/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/operators/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/sensors/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/sensors/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/sensors/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/triggers/__init__.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/airflow/providers/dbt/cloud/triggers/dbt.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/airflow/providers/dbt/cloud/triggers/dbt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dbt-cloud
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dbt-cloud package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dbt-cloud/3.2.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dbt-cloud``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `dbt Cloud <https://www.getdbt.com/product/what-is-dbt/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/apache_airflow_providers_dbt_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/pyproject.toml` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/setup.cfg` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -44,21 +44,21 @@
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	aiohttp
 	apache-airflow-providers-http
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	asgiref
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.dbt.cloud.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.dbt.cloud
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-dbt-cloud-3.2.1/setup.py` & `apache-airflow-providers-dbt-cloud-3.2.1rc1/setup.py`

 * *Files identical despite different names*

