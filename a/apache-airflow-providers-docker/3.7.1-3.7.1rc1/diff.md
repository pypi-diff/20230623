# Comparing `tmp/apache-airflow-providers-docker-3.7.1.tar.gz` & `tmp/apache-airflow-providers-docker-3.7.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-docker-3.7.1.tar", last modified: Tue Jun 20 11:28:05 2023, max compression
+gzip compressed data, was "apache-airflow-providers-docker-3.7.1rc1.tar", last modified: Tue Jun 20 11:41:56 2023, max compression
```

## Comparing `apache-airflow-providers-docker-3.7.1.tar` & `apache-airflow-providers-docker-3.7.1rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:05.594748 apache-airflow-providers-docker-3.7.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:04.000000 apache-airflow-providers-docker-3.7.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    17399 2023-06-20 11:28:05.596143 apache-airflow-providers-docker-3.7.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15874 2023-06-20 11:28:04.000000 apache-airflow-providers-docker-3.7.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:05.493392 apache-airflow-providers-docker-3.7.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:05.495151 apache-airflow-providers-docker-3.7.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:05.536358 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:05.542953 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/decorators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6805 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/decorators/docker.py
--rw-r--r--   0 root         (0) root         (0)     3280 2023-06-20 11:28:04.000000 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:05.550373 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7940 2023-06-02 11:31:21.000000 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/hooks/docker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:05.562598 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23414 2023-06-08 05:42:54.000000 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/operators/docker.py
--rw-r--r--   0 root         (0) root         (0)     9636 2023-06-02 11:31:21.000000 apache-airflow-providers-docker-3.7.1/airflow/providers/docker/operators/docker_swarm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:05.591348 apache-airflow-providers-docker-3.7.1/apache_airflow_providers_docker.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17399 2023-06-20 11:28:05.000000 apache-airflow-providers-docker-3.7.1/apache_airflow_providers_docker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      861 2023-06-20 11:28:05.000000 apache-airflow-providers-docker-3.7.1/apache_airflow_providers_docker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:05.000000 apache-airflow-providers-docker-3.7.1/apache_airflow_providers_docker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:28:05.000000 apache-airflow-providers-docker-3.7.1/apache_airflow_providers_docker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:05.000000 apache-airflow-providers-docker-3.7.1/apache_airflow_providers_docker.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-20 11:28:05.000000 apache-airflow-providers-docker-3.7.1/apache_airflow_providers_docker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:05.000000 apache-airflow-providers-docker-3.7.1/apache_airflow_providers_docker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-docker-3.7.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1859 2023-06-20 11:28:05.598370 apache-airflow-providers-docker-3.7.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1638 2023-06-20 11:28:04.000000 apache-airflow-providers-docker-3.7.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.415472 apache-airflow-providers-docker-3.7.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:55.000000 apache-airflow-providers-docker-3.7.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-docker-3.7.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    17405 2023-06-20 11:41:56.416806 apache-airflow-providers-docker-3.7.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15877 2023-06-20 11:41:55.000000 apache-airflow-providers-docker-3.7.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.308576 apache-airflow-providers-docker-3.7.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.310018 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.352270 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.360181 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/decorators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6805 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/decorators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     3280 2023-06-20 11:41:55.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.367660 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7940 2023-06-02 11:31:21.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/hooks/docker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.382129 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23414 2023-06-08 05:42:54.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/docker.py
+-rw-r--r--   0 root         (0) root         (0)     9636 2023-06-02 11:31:21.000000 apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/docker_swarm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:56.412192 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17405 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      861 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:56.000000 apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-docker-3.7.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-06-20 11:41:56.419389 apache-airflow-providers-docker-3.7.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-06-20 11:41:55.000000 apache-airflow-providers-docker-3.7.1rc1/setup.py
```

### Comparing `apache-airflow-providers-docker-3.7.1/LICENSE` & `apache-airflow-providers-docker-3.7.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/MANIFEST.in` & `apache-airflow-providers-docker-3.7.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/PKG-INFO` & `apache-airflow-providers-docker-3.7.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-docker
-Version: 3.7.1
+Version: 3.7.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-docker package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.7.1``
+Release: ``3.7.1rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-docker-3.7.1/README.rst` & `apache-airflow-providers-docker-3.7.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.7.1``
+Release: ``3.7.1rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-docker-3.7.1/airflow/providers/docker/__init__.py` & `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/airflow/providers/docker/decorators/__init__.py` & `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/airflow/providers/docker/decorators/docker.py` & `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/decorators/docker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/airflow/providers/docker/get_provider_info.py` & `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/airflow/providers/docker/hooks/__init__.py` & `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/airflow/providers/docker/hooks/docker.py` & `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/hooks/docker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/airflow/providers/docker/operators/__init__.py` & `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/airflow/providers/docker/operators/docker.py` & `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/docker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/airflow/providers/docker/operators/docker_swarm.py` & `apache-airflow-providers-docker-3.7.1rc1/airflow/providers/docker/operators/docker_swarm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/apache_airflow_providers_docker.egg-info/PKG-INFO` & `apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-docker
-Version: 3.7.1
+Version: 3.7.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-docker package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-docker/3.7.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-docker``
 
-Release: ``3.7.1``
+Release: ``3.7.1rc1``
 
 
 `Docker <https://docs.docker.com/install/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-docker-3.7.1/apache_airflow_providers_docker.egg-info/SOURCES.txt` & `apache-airflow-providers-docker-3.7.1rc1/apache_airflow_providers_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/pyproject.toml` & `apache-airflow-providers-docker-3.7.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-docker-3.7.1/setup.cfg` & `apache-airflow-providers-docker-3.7.1rc1/setup.cfg`

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
 	docker>=5.0.3
 	python-dotenv>=0.21.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.docker.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.docker
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-docker-3.7.1/setup.py` & `apache-airflow-providers-docker-3.7.1rc1/setup.py`

 * *Files identical despite different names*

