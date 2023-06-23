# Comparing `tmp/apache-airflow-providers-redis-3.2.1.tar.gz` & `tmp/apache-airflow-providers-redis-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-redis-3.2.1.tar", last modified: Tue Jun 20 11:29:17 2023, max compression
+gzip compressed data, was "apache-airflow-providers-redis-3.2.1rc1.tar", last modified: Tue Jun 20 11:42:59 2023, max compression
```

## Comparing `apache-airflow-providers-redis-3.2.1.tar` & `apache-airflow-providers-redis-3.2.1rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:16.962138 apache-airflow-providers-redis-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:15.000000 apache-airflow-providers-redis-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9784 2023-06-20 11:29:16.968810 apache-airflow-providers-redis-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8262 2023-06-20 11:29:15.000000 apache-airflow-providers-redis-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:16.745036 apache-airflow-providers-redis-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:16.746319 apache-airflow-providers-redis-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:16.792592 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2581 2023-06-20 11:29:15.000000 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:16.806967 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2945 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/hooks/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:16.818310 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/operators/redis_publish.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:16.842595 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/sensors/redis_key.py
--rw-r--r--   0 root         (0) root         (0)     2586 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.2.1/airflow/providers/redis/sensors/redis_pub_sub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:16.950925 apache-airflow-providers-redis-3.2.1/apache_airflow_providers_redis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9784 2023-06-20 11:29:16.000000 apache-airflow-providers-redis-3.2.1/apache_airflow_providers_redis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      847 2023-06-20 11:29:16.000000 apache-airflow-providers-redis-3.2.1/apache_airflow_providers_redis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:16.000000 apache-airflow-providers-redis-3.2.1/apache_airflow_providers_redis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:29:16.000000 apache-airflow-providers-redis-3.2.1/apache_airflow_providers_redis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:16.000000 apache-airflow-providers-redis-3.2.1/apache_airflow_providers_redis.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-20 11:29:16.000000 apache-airflow-providers-redis-3.2.1/apache_airflow_providers_redis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:16.000000 apache-airflow-providers-redis-3.2.1/apache_airflow_providers_redis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-redis-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1829 2023-06-20 11:29:16.981786 apache-airflow-providers-redis-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1632 2023-06-20 11:29:15.000000 apache-airflow-providers-redis-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:59.750392 apache-airflow-providers-redis-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:58.000000 apache-airflow-providers-redis-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-redis-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9790 2023-06-20 11:42:59.751425 apache-airflow-providers-redis-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8265 2023-06-20 11:42:58.000000 apache-airflow-providers-redis-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:59.669651 apache-airflow-providers-redis-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:59.670781 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:59.703882 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2581 2023-06-20 11:42:58.000000 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:59.709630 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2945 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/hooks/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:59.715542 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/operators/redis_publish.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:59.723981 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1585 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/sensors/redis_key.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-06-02 11:31:21.000000 apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/sensors/redis_pub_sub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:59.747713 apache-airflow-providers-redis-3.2.1rc1/apache_airflow_providers_redis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9790 2023-06-20 11:42:59.000000 apache-airflow-providers-redis-3.2.1rc1/apache_airflow_providers_redis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      847 2023-06-20 11:42:59.000000 apache-airflow-providers-redis-3.2.1rc1/apache_airflow_providers_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:59.000000 apache-airflow-providers-redis-3.2.1rc1/apache_airflow_providers_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:42:59.000000 apache-airflow-providers-redis-3.2.1rc1/apache_airflow_providers_redis.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:59.000000 apache-airflow-providers-redis-3.2.1rc1/apache_airflow_providers_redis.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-20 11:42:59.000000 apache-airflow-providers-redis-3.2.1rc1/apache_airflow_providers_redis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:59.000000 apache-airflow-providers-redis-3.2.1rc1/apache_airflow_providers_redis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-redis-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1837 2023-06-20 11:42:59.753440 apache-airflow-providers-redis-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-06-20 11:42:58.000000 apache-airflow-providers-redis-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-redis-3.2.1/LICENSE` & `apache-airflow-providers-redis-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/MANIFEST.in` & `apache-airflow-providers-redis-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/PKG-INFO` & `apache-airflow-providers-redis-3.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-redis
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-redis package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-redis-3.2.1/README.rst` & `apache-airflow-providers-redis-3.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-redis-3.2.1/airflow/providers/redis/__init__.py` & `apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/airflow/providers/redis/get_provider_info.py` & `apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/airflow/providers/redis/hooks/__init__.py` & `apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/airflow/providers/redis/hooks/redis.py` & `apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/hooks/redis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/airflow/providers/redis/operators/__init__.py` & `apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/airflow/providers/redis/operators/redis_publish.py` & `apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/operators/redis_publish.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/airflow/providers/redis/sensors/__init__.py` & `apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/airflow/providers/redis/sensors/redis_key.py` & `apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/sensors/redis_key.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/airflow/providers/redis/sensors/redis_pub_sub.py` & `apache-airflow-providers-redis-3.2.1rc1/airflow/providers/redis/sensors/redis_pub_sub.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/apache_airflow_providers_redis.egg-info/PKG-INFO` & `apache-airflow-providers-redis-3.2.1rc1/apache_airflow_providers_redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-redis
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-redis package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-redis/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-redis``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Redis <https://redis.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-redis-3.2.1/apache_airflow_providers_redis.egg-info/SOURCES.txt` & `apache-airflow-providers-redis-3.2.1rc1/apache_airflow_providers_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/pyproject.toml` & `apache-airflow-providers-redis-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-redis-3.2.1/setup.cfg` & `apache-airflow-providers-redis-3.2.1rc1/setup.cfg`

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
 	redis>=3.2.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.redis.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.redis
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-redis-3.2.1/setup.py` & `apache-airflow-providers-redis-3.2.1rc1/setup.py`

 * *Files identical despite different names*

