# Comparing `tmp/apache-airflow-providers-apache-hive-6.1.1.tar.gz` & `tmp/apache-airflow-providers-apache-hive-6.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-hive-6.1.1.tar", last modified: Tue Jun 20 11:27:26 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-hive-6.1.1rc1.tar", last modified: Tue Jun 20 11:41:17 2023, max compression
```

## Comparing `apache-airflow-providers-apache-hive-6.1.1.tar` & `apache-airflow-providers-apache-hive-6.1.1rc1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.906283 apache-airflow-providers-apache-hive-6.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:25.000000 apache-airflow-providers-apache-hive-6.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    19532 2023-06-20 11:27:26.907332 apache-airflow-providers-apache-hive-6.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17870 2023-06-20 11:27:25.000000 apache-airflow-providers-apache-hive-6.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.775318 apache-airflow-providers-apache-hive-6.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.776407 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.777472 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.819508 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5668 2023-06-20 11:27:25.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.825310 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42441 2023-06-18 13:29:11.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/hooks/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.831496 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/macros/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/macros/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4581 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/macros/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.840905 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/operators/hive.py
--rw-r--r--   0 root         (0) root         (0)     7502 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/operators/hive_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.846584 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/plugins/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/plugins/hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.859558 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/sensors/hive_partition.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/sensors/metastore_partition.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/sensors/named_hive_partition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.880440 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5279 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/hive_to_mysql.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/hive_to_samba.py
--rw-r--r--   0 root         (0) root         (0)     5662 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/mssql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     6713 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/mysql_to_hive.py
--rw-r--r--   0 root         (0) root         (0)    11742 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/s3_to_hive.py
--rw-r--r--   0 root         (0) root         (0)     5564 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/vertica_to_hive.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:26.903780 apache-airflow-providers-apache-hive-6.1.1/apache_airflow_providers_apache_hive.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19532 2023-06-20 11:27:26.000000 apache-airflow-providers-apache-hive-6.1.1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1643 2023-06-20 11:27:26.000000 apache-airflow-providers-apache-hive-6.1.1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:26.000000 apache-airflow-providers-apache-hive-6.1.1/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-06-20 11:27:26.000000 apache-airflow-providers-apache-hive-6.1.1/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:26.000000 apache-airflow-providers-apache-hive-6.1.1/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-20 11:27:26.000000 apache-airflow-providers-apache-hive-6.1.1/apache_airflow_providers_apache_hive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:26.000000 apache-airflow-providers-apache-hive-6.1.1/apache_airflow_providers_apache_hive.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2040 2023-06-20 11:27:26.909375 apache-airflow-providers-apache-hive-6.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2114 2023-06-20 11:27:25.000000 apache-airflow-providers-apache-hive-6.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.585976 apache-airflow-providers-apache-hive-6.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hive-6.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    19538 2023-06-20 11:41:17.587160 apache-airflow-providers-apache-hive-6.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17873 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.460881 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.462033 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.463236 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.501401 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5668 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.507300 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42441 2023-06-18 13:29:11.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.513956 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4581 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.522586 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive.py
+-rw-r--r--   0 root         (0) root         (0)     7502 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive_stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.528160 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.539416 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/hive_partition.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/metastore_partition.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.559887 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5279 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py
+-rw-r--r--   0 root         (0) root         (0)     5662 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     6713 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)    11742 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py
+-rw-r--r--   0 root         (0) root         (0)     5564 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:17.583345 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19538 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:17.000000 apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hive-6.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-06-20 11:41:17.590526 apache-airflow-providers-apache-hive-6.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-20 11:41:16.000000 apache-airflow-providers-apache-hive-6.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1/LICENSE` & `apache-airflow-providers-apache-hive-6.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/MANIFEST.in` & `apache-airflow-providers-apache-hive-6.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.1.1
+Version: 6.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.1/
@@ -54,15 +54,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.1``
+Release: ``6.1.1rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1/README.rst` & `apache-airflow-providers-apache-hive-6.1.1rc1/README.rst`

 * *Files identical despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.1``
+Release: ``6.1.1rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/get_provider_info.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/hooks/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/hooks/hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/hooks/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/macros/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/macros/hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/macros/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/operators/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/operators/hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/operators/hive_stats.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/operators/hive_stats.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/plugins/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/plugins/hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/plugins/hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/sensors/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/sensors/hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/sensors/metastore_partition.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/metastore_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/sensors/named_hive_partition.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/sensors/named_hive_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/__init__.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/hive_to_mysql.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_mysql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/hive_to_samba.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/hive_to_samba.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/mssql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mssql_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/mysql_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/mysql_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/s3_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/s3_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/airflow/providers/apache/hive/transfers/vertica_to_hive.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/airflow/providers/apache/hive/transfers/vertica_to_hive.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO` & `apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hive
-Version: 6.1.1
+Version: 6.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hive package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hive/6.1.1/
@@ -54,15 +54,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hive``
 
-Release: ``6.1.1``
+Release: ``6.1.1rc1``
 
 
 `Apache Hive <https://hive.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-hive-6.1.1rc1/apache_airflow_providers_apache_hive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/pyproject.toml` & `apache-airflow-providers-apache-hive-6.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hive-6.1.1/setup.cfg` & `apache-airflow-providers-apache-hive-6.1.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,16 @@
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
 	hmsclient>=0.1.0
 	pandas>=0.17.1
 	pyhive[hive]>=0.6.0
 	sasl>=0.3.1; python_version>="3.9"
 	thrift>=0.9.2
 
 [options.entry_points]
@@ -59,10 +59,10 @@
 airflow.plugins = 
 	hive=airflow.providers.apache.hive.plugins.hive:HivePlugin
 
 [files]
 packages = airflow.providers.apache.hive
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-hive-6.1.1/setup.py` & `apache-airflow-providers-apache-hive-6.1.1rc1/setup.py`

 * *Files identical despite different names*

