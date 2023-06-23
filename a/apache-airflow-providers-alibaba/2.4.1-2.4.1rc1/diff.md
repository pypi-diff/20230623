# Comparing `tmp/apache-airflow-providers-alibaba-2.4.1.tar.gz` & `tmp/apache-airflow-providers-alibaba-2.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-alibaba-2.4.1.tar", last modified: Tue Jun 20 11:27:10 2023, max compression
+gzip compressed data, was "apache-airflow-providers-alibaba-2.4.1rc1.tar", last modified: Tue Jun 20 11:41:00 2023, max compression
```

## Comparing `apache-airflow-providers-alibaba-2.4.1.tar` & `apache-airflow-providers-alibaba-2.4.1rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:10.351731 apache-airflow-providers-alibaba-2.4.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:09.000000 apache-airflow-providers-alibaba-2.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10225 2023-06-20 11:27:10.352733 apache-airflow-providers-alibaba-2.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8697 2023-06-20 11:27:09.000000 apache-airflow-providers-alibaba-2.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:10.256919 apache-airflow-providers-alibaba-2.4.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:10.258280 apache-airflow-providers-alibaba-2.4.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:10.298602 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:10.301460 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:10.307273 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12646 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/hooks/oss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:10.312782 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8634 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/log/oss_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:10.318703 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6320 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/operators/oss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:10.325175 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3659 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/sensors/oss_key.py
--rw-r--r--   0 root         (0) root         (0)     2904 2023-06-20 11:27:09.000000 apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:10.349090 apache-airflow-providers-alibaba-2.4.1/apache_airflow_providers_alibaba.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10225 2023-06-20 11:27:10.000000 apache-airflow-providers-alibaba-2.4.1/apache_airflow_providers_alibaba.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      998 2023-06-20 11:27:10.000000 apache-airflow-providers-alibaba-2.4.1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:10.000000 apache-airflow-providers-alibaba-2.4.1/apache_airflow_providers_alibaba.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:27:10.000000 apache-airflow-providers-alibaba-2.4.1/apache_airflow_providers_alibaba.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:10.000000 apache-airflow-providers-alibaba-2.4.1/apache_airflow_providers_alibaba.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-20 11:27:10.000000 apache-airflow-providers-alibaba-2.4.1/apache_airflow_providers_alibaba.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:10.000000 apache-airflow-providers-alibaba-2.4.1/apache_airflow_providers_alibaba.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-alibaba-2.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1841 2023-06-20 11:27:10.354642 apache-airflow-providers-alibaba-2.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:27:09.000000 apache-airflow-providers-alibaba-2.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.613326 apache-airflow-providers-alibaba-2.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-alibaba-2.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10231 2023-06-20 11:41:00.614390 apache-airflow-providers-alibaba-2.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8700 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.507688 apache-airflow-providers-alibaba-2.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.509220 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.557541 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.560595 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.566586 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12646 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/oss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.572527 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8634 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.578845 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6320 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/oss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.585396 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2023-06-02 11:31:21.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:00.610519 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10231 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      998 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:00.000000 apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-alibaba-2.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-06-20 11:41:00.616407 apache-airflow-providers-alibaba-2.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:40:59.000000 apache-airflow-providers-alibaba-2.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-alibaba-2.4.1/LICENSE` & `apache-airflow-providers-alibaba-2.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/MANIFEST.in` & `apache-airflow-providers-alibaba-2.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/PKG-INFO` & `apache-airflow-providers-alibaba-2.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-alibaba
-Version: 2.4.1
+Version: 2.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-alibaba package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.4.1``
+Release: ``2.4.1rc1``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-alibaba-2.4.1/README.rst` & `apache-airflow-providers-alibaba-2.4.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.4.1``
+Release: ``2.4.1rc1``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/hooks/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/hooks/oss.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/hooks/oss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/log/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/log/oss_task_handler.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/log/oss_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/operators/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/operators/oss.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/operators/oss.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/sensors/__init__.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/cloud/sensors/oss_key.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/cloud/sensors/oss_key.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/airflow/providers/alibaba/get_provider_info.py` & `apache-airflow-providers-alibaba-2.4.1rc1/airflow/providers/alibaba/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/apache_airflow_providers_alibaba.egg-info/PKG-INFO` & `apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-alibaba
-Version: 2.4.1
+Version: 2.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-alibaba package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-alibaba/2.4.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-alibaba``
 
-Release: ``2.4.1``
+Release: ``2.4.1rc1``
 
 
 Alibaba Cloud integration (including `Alibaba Cloud <https://www.alibabacloud.com//>`__).
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-alibaba-2.4.1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt` & `apache-airflow-providers-alibaba-2.4.1rc1/apache_airflow_providers_alibaba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/pyproject.toml` & `apache-airflow-providers-alibaba-2.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-alibaba-2.4.1/setup.cfg` & `apache-airflow-providers-alibaba-2.4.1rc1/setup.cfg`

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
 	oss2>=2.14.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.alibaba.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.alibaba
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-alibaba-2.4.1/setup.py` & `apache-airflow-providers-alibaba-2.4.1rc1/setup.py`

 * *Files identical despite different names*

