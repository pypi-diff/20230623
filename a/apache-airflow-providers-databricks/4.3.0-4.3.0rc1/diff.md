# Comparing `tmp/apache-airflow-providers-databricks-4.3.0.tar.gz` & `tmp/apache-airflow-providers-databricks-4.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-databricks-4.3.0.tar", last modified: Tue Jun 20 11:27:56 2023, max compression
+gzip compressed data, was "apache-airflow-providers-databricks-4.3.0rc1.tar", last modified: Tue Jun 20 11:41:47 2023, max compression
```

## Comparing `apache-airflow-providers-databricks-4.3.0.tar` & `apache-airflow-providers-databricks-4.3.0rc1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:56.323992 apache-airflow-providers-databricks-4.3.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:55.000000 apache-airflow-providers-databricks-4.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    21137 2023-06-20 11:27:56.325099 apache-airflow-providers-databricks-4.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19573 2023-06-20 11:27:55.000000 apache-airflow-providers-databricks-4.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:56.206238 apache-airflow-providers-databricks-4.3.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:56.207454 apache-airflow-providers-databricks-4.3.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:56.244603 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-20 11:01:09.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5506 2023-06-20 11:27:55.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:56.258011 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16771 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/hooks/databricks.py
--rw-r--r--   0 root         (0) root         (0)    26695 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/hooks/databricks_base.py
--rw-r--r--   0 root         (0) root         (0)     9359 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/hooks/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:56.271430 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33383 2023-06-19 10:14:19.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/operators/databricks.py
--rw-r--r--   0 root         (0) root         (0)    13212 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/operators/databricks_repos.py
--rw-r--r--   0 root         (0) root         (0)    16994 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/operators/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:56.281000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10000 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/sensors/databricks_partition.py
--rw-r--r--   0 root         (0) root         (0)     5543 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/sensors/databricks_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:56.287980 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3997 2023-06-18 13:29:11.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/triggers/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:56.294310 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/utils/databricks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:56.321532 apache-airflow-providers-databricks-4.3.0/apache_airflow_providers_databricks.egg-info/
--rw-r--r--   0 root         (0) root         (0)    21137 2023-06-20 11:27:56.000000 apache-airflow-providers-databricks-4.3.0/apache_airflow_providers_databricks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1362 2023-06-20 11:27:56.000000 apache-airflow-providers-databricks-4.3.0/apache_airflow_providers_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:56.000000 apache-airflow-providers-databricks-4.3.0/apache_airflow_providers_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-20 11:27:56.000000 apache-airflow-providers-databricks-4.3.0/apache_airflow_providers_databricks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:56.000000 apache-airflow-providers-databricks-4.3.0/apache_airflow_providers_databricks.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      190 2023-06-20 11:27:56.000000 apache-airflow-providers-databricks-4.3.0/apache_airflow_providers_databricks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:56.000000 apache-airflow-providers-databricks-4.3.0/apache_airflow_providers_databricks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-databricks-4.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1969 2023-06-20 11:27:56.327175 apache-airflow-providers-databricks-4.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1715 2023-06-20 11:27:55.000000 apache-airflow-providers-databricks-4.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.334610 apache-airflow-providers-databricks-4.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-databricks-4.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    21143 2023-06-20 11:41:47.335992 apache-airflow-providers-databricks-4.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    19576 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.212152 apache-airflow-providers-databricks-4.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.213485 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.255680 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-20 11:01:09.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5506 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.269076 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16771 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    26695 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_base.py
+-rw-r--r--   0 root         (0) root         (0)     9359 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.281889 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33383 2023-06-19 10:14:19.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks.py
+-rw-r--r--   0 root         (0) root         (0)    13212 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_repos.py
+-rw-r--r--   0 root         (0) root         (0)    16994 2023-06-17 16:45:00.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.290943 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10000 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_partition.py
+-rw-r--r--   0 root         (0) root         (0)     5543 2023-06-01 07:44:14.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.297042 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3997 2023-06-18 13:29:11.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.303088 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-06-02 11:31:21.000000 apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/databricks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:47.330922 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    21143 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      200 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:47.000000 apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-databricks-4.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-06-20 11:41:47.340065 apache-airflow-providers-databricks-4.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-06-20 11:41:46.000000 apache-airflow-providers-databricks-4.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-databricks-4.3.0/LICENSE` & `apache-airflow-providers-databricks-4.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/MANIFEST.in` & `apache-airflow-providers-databricks-4.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/PKG-INFO` & `apache-airflow-providers-databricks-4.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.3.0
+Version: 4.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.3.0``
+Release: ``4.3.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-databricks-4.3.0/README.rst` & `apache-airflow-providers-databricks-4.3.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.3.0``
+Release: ``4.3.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/get_provider_info.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/hooks/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/hooks/databricks.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/hooks/databricks_base.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/hooks/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/hooks/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/operators/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/operators/databricks.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/operators/databricks_repos.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_repos.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/operators/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/operators/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/sensors/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/sensors/databricks_partition.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/sensors/databricks_sql.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/sensors/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/triggers/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/triggers/databricks.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/triggers/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/utils/__init__.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/airflow/providers/databricks/utils/databricks.py` & `apache-airflow-providers-databricks-4.3.0rc1/airflow/providers/databricks/utils/databricks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/apache_airflow_providers_databricks.egg-info/PKG-INFO` & `apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-databricks
-Version: 4.3.0
+Version: 4.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-databricks package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-databricks/4.3.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-databricks``
 
-Release: ``4.3.0``
+Release: ``4.3.0rc1``
 
 
 `Databricks <https://databricks.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-databricks-4.3.0/apache_airflow_providers_databricks.egg-info/SOURCES.txt` & `apache-airflow-providers-databricks-4.3.0rc1/apache_airflow_providers_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/pyproject.toml` & `apache-airflow-providers-databricks-4.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-databricks-4.3.0/setup.cfg` & `apache-airflow-providers-databricks-4.3.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,23 @@
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	aiohttp>=3.6.3, <4
-	apache-airflow-providers-common-sql>=1.5.0
-	apache-airflow>=2.4.0
+	apache-airflow-providers-common-sql>=1.5.0.dev0
+	apache-airflow>=2.4.0.dev0
 	databricks-sql-connector>=2.0.0, <3.0.0
 	requests>=2.27,<3
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.databricks.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.databricks
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-databricks-4.3.0/setup.py` & `apache-airflow-providers-databricks-4.3.0rc1/setup.py`

 * *Files identical despite different names*

