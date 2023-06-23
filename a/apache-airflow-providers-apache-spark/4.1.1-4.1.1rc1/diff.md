# Comparing `tmp/apache-airflow-providers-apache-spark-4.1.1.tar.gz` & `tmp/apache-airflow-providers-apache-spark-4.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-spark-4.1.1.tar", last modified: Tue Jun 20 11:27:39 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-spark-4.1.1rc1.tar", last modified: Tue Jun 20 11:41:30 2023, max compression
```

## Comparing `apache-airflow-providers-apache-spark-4.1.1.tar` & `apache-airflow-providers-apache-spark-4.1.1rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:39.323621 apache-airflow-providers-apache-spark-4.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:38.000000 apache-airflow-providers-apache-spark-4.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    12338 2023-06-20 11:27:39.325101 apache-airflow-providers-apache-spark-4.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10795 2023-06-20 11:27:38.000000 apache-airflow-providers-apache-spark-4.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:39.231442 apache-airflow-providers-apache-spark-4.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:39.232984 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:39.234154 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:39.267714 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3516 2023-06-20 11:27:38.000000 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:39.282404 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11383 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/hooks/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     6753 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
--rw-r--r--   0 root         (0) root         (0)     7054 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/hooks/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)    28715 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/hooks/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:39.294601 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9973 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/operators/spark_jdbc.py
--rw-r--r--   0 root         (0) root         (0)     4508 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/operators/spark_sql.py
--rw-r--r--   0 root         (0) root         (0)     8414 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/operators/spark_submit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:39.319935 apache-airflow-providers-apache-spark-4.1.1/apache_airflow_providers_apache_spark.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12338 2023-06-20 11:27:39.000000 apache-airflow-providers-apache-spark-4.1.1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1074 2023-06-20 11:27:39.000000 apache-airflow-providers-apache-spark-4.1.1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:39.000000 apache-airflow-providers-apache-spark-4.1.1/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:27:39.000000 apache-airflow-providers-apache-spark-4.1.1/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:39.000000 apache-airflow-providers-apache-spark-4.1.1/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-20 11:27:39.000000 apache-airflow-providers-apache-spark-4.1.1/apache_airflow_providers_apache_spark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:39.000000 apache-airflow-providers-apache-spark-4.1.1/apache_airflow_providers_apache_spark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-spark-4.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1866 2023-06-20 11:27:39.327618 apache-airflow-providers-apache-spark-4.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:27:38.000000 apache-airflow-providers-apache-spark-4.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.186280 apache-airflow-providers-apache-spark-4.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    12344 2023-06-20 11:41:30.187336 apache-airflow-providers-apache-spark-4.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.094919 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.096025 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.097257 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.132264 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3516 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.147465 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11383 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     6753 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py
+-rw-r--r--   0 root         (0) root         (0)     7054 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)    28715 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.159330 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_jdbc.py
+-rw-r--r--   0 root         (0) root         (0)     4508 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_sql.py
+-rw-r--r--   0 root         (0) root         (0)     8414 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_submit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:30.183585 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12344 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:30.000000 apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-spark-4.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-06-20 11:41:30.189305 apache-airflow-providers-apache-spark-4.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:41:29.000000 apache-airflow-providers-apache-spark-4.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1/LICENSE` & `apache-airflow-providers-apache-spark-4.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/MANIFEST.in` & `apache-airflow-providers-apache-spark-4.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/PKG-INFO` & `apache-airflow-providers-apache-spark-4.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.1.1
+Version: 4.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-spark package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.1``
+Release: ``4.1.1rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1/README.rst` & `apache-airflow-providers-apache-spark-4.1.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.1``
+Release: ``4.1.1rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/__init__.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/get_provider_info.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/hooks/__init__.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/hooks/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_jdbc_script.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/hooks/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/hooks/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/hooks/spark_submit.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/operators/__init__.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/operators/spark_jdbc.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_jdbc.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/operators/spark_sql.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/airflow/providers/apache/spark/operators/spark_submit.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/airflow/providers/apache/spark/operators/spark_submit.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO` & `apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-spark
-Version: 4.1.1
+Version: 4.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-spark package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-spark/4.1.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-spark``
 
-Release: ``4.1.1``
+Release: ``4.1.1rc1``
 
 
 `Apache Spark <https://spark.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-spark-4.1.1rc1/apache_airflow_providers_apache_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/pyproject.toml` & `apache-airflow-providers-apache-spark-4.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-spark-4.1.1/setup.cfg` & `apache-airflow-providers-apache-spark-4.1.1rc1/setup.cfg`

 * *Files 4% similar despite different names*

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
 	pyspark
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.spark.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.spark
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-spark-4.1.1/setup.py` & `apache-airflow-providers-apache-spark-4.1.1rc1/setup.py`

 * *Files identical despite different names*

