# Comparing `tmp/apache-airflow-providers-dingding-3.2.1.tar.gz` & `tmp/apache-airflow-providers-dingding-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-dingding-3.2.1.tar", last modified: Tue Jun 20 11:28:01 2023, max compression
+gzip compressed data, was "apache-airflow-providers-dingding-3.2.1rc1.tar", last modified: Tue Jun 20 11:41:52 2023, max compression
```

## Comparing `apache-airflow-providers-dingding-3.2.1.tar` & `apache-airflow-providers-dingding-3.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:01.792979 apache-airflow-providers-dingding-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-dingding-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:00.000000 apache-airflow-providers-dingding-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-dingding-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11892 2023-06-20 11:28:01.794173 apache-airflow-providers-dingding-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10340 2023-06-20 11:28:00.000000 apache-airflow-providers-dingding-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:01.715668 apache-airflow-providers-dingding-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:01.716815 apache-airflow-providers-dingding-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:01.749766 apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2592 2023-06-20 11:28:00.000000 apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:01.756429 apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4801 2023-06-05 12:50:36.000000 apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/hooks/dingding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:01.763691 apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-06-01 06:14:28.000000 apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/operators/dingding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:01.789824 apache-airflow-providers-dingding-3.2.1/apache_airflow_providers_dingding.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11892 2023-06-20 11:28:01.000000 apache-airflow-providers-dingding-3.2.1/apache_airflow_providers_dingding.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:28:01.000000 apache-airflow-providers-dingding-3.2.1/apache_airflow_providers_dingding.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:01.000000 apache-airflow-providers-dingding-3.2.1/apache_airflow_providers_dingding.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:28:01.000000 apache-airflow-providers-dingding-3.2.1/apache_airflow_providers_dingding.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:01.000000 apache-airflow-providers-dingding-3.2.1/apache_airflow_providers_dingding.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-20 11:28:01.000000 apache-airflow-providers-dingding-3.2.1/apache_airflow_providers_dingding.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:01.000000 apache-airflow-providers-dingding-3.2.1/apache_airflow_providers_dingding.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-dingding-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-20 11:28:01.796318 apache-airflow-providers-dingding-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:28:00.000000 apache-airflow-providers-dingding-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.785783 apache-airflow-providers-dingding-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-dingding-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:51.000000 apache-airflow-providers-dingding-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-dingding-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11898 2023-06-20 11:41:52.786777 apache-airflow-providers-dingding-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10343 2023-06-20 11:41:51.000000 apache-airflow-providers-dingding-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.715311 apache-airflow-providers-dingding-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.716505 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.748701 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-06-20 11:41:51.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.754309 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2023-06-05 12:50:36.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/hooks/dingding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.760152 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-06-01 06:14:28.000000 apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/operators/dingding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:52.783456 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11898 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:52.000000 apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-dingding-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-20 11:41:52.788740 apache-airflow-providers-dingding-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:41:51.000000 apache-airflow-providers-dingding-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-dingding-3.2.1/LICENSE` & `apache-airflow-providers-dingding-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.1/MANIFEST.in` & `apache-airflow-providers-dingding-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.1/PKG-INFO` & `apache-airflow-providers-dingding-3.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dingding
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dingding package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dingding``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Dingding <https://oapi.dingtalk.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dingding-3.2.1/README.rst` & `apache-airflow-providers-dingding-3.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dingding``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Dingding <https://oapi.dingtalk.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/__init__.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/get_provider_info.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/hooks/__init__.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/hooks/dingding.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/hooks/dingding.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/operators/__init__.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.1/airflow/providers/dingding/operators/dingding.py` & `apache-airflow-providers-dingding-3.2.1rc1/airflow/providers/dingding/operators/dingding.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.1/apache_airflow_providers_dingding.egg-info/PKG-INFO` & `apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-dingding
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-dingding package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-dingding/3.2.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-dingding``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Dingding <https://oapi.dingtalk.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-dingding-3.2.1/apache_airflow_providers_dingding.egg-info/SOURCES.txt` & `apache-airflow-providers-dingding-3.2.1rc1/apache_airflow_providers_dingding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.1/pyproject.toml` & `apache-airflow-providers-dingding-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-dingding-3.2.1/setup.cfg` & `apache-airflow-providers-dingding-3.2.1rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-http
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.dingding.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.dingding
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-dingding-3.2.1/setup.py` & `apache-airflow-providers-dingding-3.2.1rc1/setup.py`

 * *Files identical despite different names*

