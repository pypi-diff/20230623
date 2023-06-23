# Comparing `tmp/apache-airflow-providers-apache-hdfs-4.1.0.tar.gz` & `tmp/apache-airflow-providers-apache-hdfs-4.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-hdfs-4.1.0.tar", last modified: Tue Jun 20 11:27:25 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-hdfs-4.1.0rc1.tar", last modified: Tue Jun 20 11:41:15 2023, max compression
```

## Comparing `apache-airflow-providers-apache-hdfs-4.1.0.tar` & `apache-airflow-providers-apache-hdfs-4.1.0rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:24.997375 apache-airflow-providers-apache-hdfs-4.1.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hdfs-4.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:23.000000 apache-airflow-providers-apache-hdfs-4.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hdfs-4.1.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13204 2023-06-20 11:27:24.998385 apache-airflow-providers-apache-hdfs-4.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11664 2023-06-20 11:27:23.000000 apache-airflow-providers-apache-hdfs-4.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:24.908542 apache-airflow-providers-apache-hdfs-4.1.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:24.909800 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:24.911029 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:24.944173 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 07:01:17.000000 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2953 2023-06-20 11:27:23.000000 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:24.953271 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2267 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/hooks/hdfs.py
--rw-r--r--   0 root         (0) root         (0)     6439 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/hooks/webhdfs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:24.959720 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5604 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/log/hdfs_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:24.968980 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/sensors/hdfs.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/sensors/web_hdfs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:24.995032 apache-airflow-providers-apache-hdfs-4.1.0/apache_airflow_providers_apache_hdfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13204 2023-06-20 11:27:24.000000 apache-airflow-providers-apache-hdfs-4.1.0/apache_airflow_providers_apache_hdfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      971 2023-06-20 11:27:24.000000 apache-airflow-providers-apache-hdfs-4.1.0/apache_airflow_providers_apache_hdfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:24.000000 apache-airflow-providers-apache-hdfs-4.1.0/apache_airflow_providers_apache_hdfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:27:24.000000 apache-airflow-providers-apache-hdfs-4.1.0/apache_airflow_providers_apache_hdfs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:24.000000 apache-airflow-providers-apache-hdfs-4.1.0/apache_airflow_providers_apache_hdfs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-20 11:27:24.000000 apache-airflow-providers-apache-hdfs-4.1.0/apache_airflow_providers_apache_hdfs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:24.000000 apache-airflow-providers-apache-hdfs-4.1.0/apache_airflow_providers_apache_hdfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hdfs-4.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1889 2023-06-20 11:27:25.000233 apache-airflow-providers-apache-hdfs-4.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-20 11:27:23.000000 apache-airflow-providers-apache-hdfs-4.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.593816 apache-airflow-providers-apache-hdfs-4.1.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:14.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13210 2023-06-20 11:41:15.594917 apache-airflow-providers-apache-hdfs-4.1.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11667 2023-06-20 11:41:14.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.498277 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.499678 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.501081 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.537689 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-20 07:01:17.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2953 2023-06-20 11:41:14.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.547725 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2267 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     6439 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/webhdfs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.554462 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5604 2023-06-17 16:45:00.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/log/hdfs_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.565499 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/hdfs.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/web_hdfs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:15.591094 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13210 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      971 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:15.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1897 2023-06-20 11:41:15.597161 apache-airflow-providers-apache-hdfs-4.1.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-20 11:41:14.000000 apache-airflow-providers-apache-hdfs-4.1.0rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/LICENSE` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/MANIFEST.in` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/PKG-INFO` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hdfs
-Version: 4.1.0
+Version: 4.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hdfs package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.1.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hdfs``
 
-Release: ``4.1.0``
+Release: ``4.1.0rc1``
 
 
 `Hadoop Distributed File System (HDFS) <https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html>`__
 and `WebHDFS <https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html>`__.
 
 
 Provider package
```

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/README.rst` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hdfs``
 
-Release: ``4.1.0``
+Release: ``4.1.0rc1``
 
 
 `Hadoop Distributed File System (HDFS) <https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html>`__
 and `WebHDFS <https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html>`__.
 
 
 Provider package
```

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/__init__.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/get_provider_info.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/hooks/__init__.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/hooks/hdfs.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/hdfs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/hooks/webhdfs.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/hooks/webhdfs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/log/__init__.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/log/hdfs_task_handler.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/log/hdfs_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/sensors/__init__.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/sensors/hdfs.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/hdfs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/airflow/providers/apache/hdfs/sensors/web_hdfs.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/airflow/providers/apache/hdfs/sensors/web_hdfs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/apache_airflow_providers_apache_hdfs.egg-info/PKG-INFO` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-hdfs
-Version: 4.1.0
+Version: 4.1.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-hdfs package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-hdfs/4.1.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-hdfs``
 
-Release: ``4.1.0``
+Release: ``4.1.0rc1``
 
 
 `Hadoop Distributed File System (HDFS) <https://hadoop.apache.org/docs/r1.2.1/hdfs_design.html>`__
 and `WebHDFS <https://hadoop.apache.org/docs/current/hadoop-project-dist/hadoop-hdfs/WebHDFS.html>`__.
 
 
 Provider package
```

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/apache_airflow_providers_apache_hdfs.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/apache_airflow_providers_apache_hdfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/pyproject.toml` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/setup.cfg` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/setup.cfg`

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
 	hdfs[avro,dataframe,kerberos]>=2.0.4
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.hdfs.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.hdfs
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-hdfs-4.1.0/setup.py` & `apache-airflow-providers-apache-hdfs-4.1.0rc1/setup.py`

 * *Files identical despite different names*

