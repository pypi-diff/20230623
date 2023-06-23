# Comparing `tmp/apache-airflow-providers-snowflake-4.2.0.tar.gz` & `tmp/apache-airflow-providers-snowflake-4.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-snowflake-4.2.0.tar", last modified: Tue Jun 20 11:29:36 2023, max compression
+gzip compressed data, was "apache-airflow-providers-snowflake-4.2.0rc1.tar", last modified: Tue Jun 20 11:43:15 2023, max compression
```

## Comparing `apache-airflow-providers-snowflake-4.2.0.tar` & `apache-airflow-providers-snowflake-4.2.0rc1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:36.302119 apache-airflow-providers-snowflake-4.2.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:35.000000 apache-airflow-providers-snowflake-4.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    19901 2023-06-20 11:29:36.303263 apache-airflow-providers-snowflake-4.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    18318 2023-06-20 11:29:35.000000 apache-airflow-providers-snowflake-4.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:36.204754 apache-airflow-providers-snowflake-4.2.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:36.205868 apache-airflow-providers-snowflake-4.2.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:36.240209 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4724 2023-06-20 11:29:35.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:36.249208 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17859 2023-06-05 12:50:36.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/hooks/snowflake.py
--rw-r--r--   0 root         (0) root         (0)    11759 2023-06-08 05:42:54.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/hooks/snowflake_sql_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:36.254770 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22918 2023-06-17 16:45:00.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/operators/snowflake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:36.266383 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5786 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/transfers/copy_into_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/transfers/s3_to_snowflake.py
--rw-r--r--   0 root         (0) root         (0)     5078 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/transfers/snowflake_to_slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:36.274973 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/utils/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/utils/common.py
--rw-r--r--   0 root         (0) root         (0)     6878 2023-06-01 07:44:14.000000 apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:36.299530 apache-airflow-providers-snowflake-4.2.0/apache_airflow_providers_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19901 2023-06-20 11:29:36.000000 apache-airflow-providers-snowflake-4.2.0/apache_airflow_providers_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1192 2023-06-20 11:29:36.000000 apache-airflow-providers-snowflake-4.2.0/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:36.000000 apache-airflow-providers-snowflake-4.2.0/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:29:36.000000 apache-airflow-providers-snowflake-4.2.0/apache_airflow_providers_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:36.000000 apache-airflow-providers-snowflake-4.2.0/apache_airflow_providers_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      217 2023-06-20 11:29:36.000000 apache-airflow-providers-snowflake-4.2.0/apache_airflow_providers_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:36.000000 apache-airflow-providers-snowflake-4.2.0/apache_airflow_providers_snowflake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-snowflake-4.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1947 2023-06-20 11:29:36.305169 apache-airflow-providers-snowflake-4.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1789 2023-06-20 11:29:35.000000 apache-airflow-providers-snowflake-4.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.974181 apache-airflow-providers-snowflake-4.2.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    19907 2023-06-20 11:43:15.975546 apache-airflow-providers-snowflake-4.2.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18321 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.861078 apache-airflow-providers-snowflake-4.2.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.862300 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.902943 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4724 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.912718 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17859 2023-06-05 12:50:36.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/snowflake.py
+-rw-r--r--   0 root         (0) root         (0)    11759 2023-06-08 05:42:54.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.918823 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22918 2023-06-17 16:45:00.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/snowflake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.931338 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5786 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-06-02 11:31:21.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py
+-rw-r--r--   0 root         (0) root         (0)     5078 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.942711 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 06:14:29.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/common.py
+-rw-r--r--   0 root         (0) root         (0)     6878 2023-06-01 07:44:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:15.970806 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19907 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1192 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:15.000000 apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-snowflake-4.2.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-06-20 11:43:15.977871 apache-airflow-providers-snowflake-4.2.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-06-20 11:43:14.000000 apache-airflow-providers-snowflake-4.2.0rc1/setup.py
```

### Comparing `apache-airflow-providers-snowflake-4.2.0/LICENSE` & `apache-airflow-providers-snowflake-4.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/MANIFEST.in` & `apache-airflow-providers-snowflake-4.2.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/PKG-INFO` & `apache-airflow-providers-snowflake-4.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.2.0
+Version: 4.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.2.0/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.2.0``
+Release: ``4.2.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.2.0/README.rst` & `apache-airflow-providers-snowflake-4.2.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.2.0``
+Release: ``4.2.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/__init__.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/get_provider_info.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/hooks/__init__.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/hooks/snowflake.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/hooks/snowflake_sql_api.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/hooks/snowflake_sql_api.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/operators/__init__.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/operators/snowflake.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/operators/snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/transfers/__init__.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/transfers/copy_into_snowflake.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/copy_into_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/transfers/s3_to_snowflake.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/s3_to_snowflake.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/transfers/snowflake_to_slack.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/transfers/snowflake_to_slack.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/utils/__init__.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/utils/common.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/common.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/airflow/providers/snowflake/utils/sql_api_generate_jwt.py` & `apache-airflow-providers-snowflake-4.2.0rc1/airflow/providers/snowflake/utils/sql_api_generate_jwt.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/apache_airflow_providers_snowflake.egg-info/PKG-INFO` & `apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-snowflake
-Version: 4.2.0
+Version: 4.2.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-snowflake package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-snowflake/4.2.0/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-snowflake``
 
-Release: ``4.2.0``
+Release: ``4.2.0rc1``
 
 
 `Snowflake <https://www.snowflake.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-snowflake-4.2.0/apache_airflow_providers_snowflake.egg-info/SOURCES.txt` & `apache-airflow-providers-snowflake-4.2.0rc1/apache_airflow_providers_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/pyproject.toml` & `apache-airflow-providers-snowflake-4.2.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-snowflake-4.2.0/setup.cfg` & `apache-airflow-providers-snowflake-4.2.0rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -42,23 +42,23 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow-providers-common-sql>=1.3.1
-	apache-airflow>=2.4.0
+	apache-airflow-providers-common-sql>=1.3.1.dev0
+	apache-airflow>=2.4.0.dev0
 	snowflake-connector-python>=2.4.1
 	snowflake-sqlalchemy>=1.1.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.snowflake.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.snowflake
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-snowflake-4.2.0/setup.py` & `apache-airflow-providers-snowflake-4.2.0rc1/setup.py`

 * *Files identical despite different names*

