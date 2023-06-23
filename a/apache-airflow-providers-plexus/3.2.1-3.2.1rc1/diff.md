# Comparing `tmp/apache-airflow-providers-plexus-3.2.1.tar.gz` & `tmp/apache-airflow-providers-plexus-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-plexus-3.2.1.tar", last modified: Tue Jun 20 11:29:08 2023, max compression
+gzip compressed data, was "apache-airflow-providers-plexus-3.2.1rc1.tar", last modified: Tue Jun 20 11:42:52 2023, max compression
```

## Comparing `apache-airflow-providers-plexus-3.2.1.tar` & `apache-airflow-providers-plexus-3.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:08.855331 apache-airflow-providers-plexus-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-plexus-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:07.000000 apache-airflow-providers-plexus-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-plexus-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10072 2023-06-20 11:29:08.857219 apache-airflow-providers-plexus-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8547 2023-06-20 11:29:07.000000 apache-airflow-providers-plexus-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:08.723872 apache-airflow-providers-plexus-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:08.725508 apache-airflow-providers-plexus-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:08.793574 apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-06-20 11:29:07.000000 apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:08.804977 apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-06-02 11:31:21.000000 apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/hooks/plexus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:08.814059 apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6055 2023-06-01 06:14:28.000000 apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/operators/job.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:08.851077 apache-airflow-providers-plexus-3.2.1/apache_airflow_providers_plexus.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10072 2023-06-20 11:29:08.000000 apache-airflow-providers-plexus-3.2.1/apache_airflow_providers_plexus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      713 2023-06-20 11:29:08.000000 apache-airflow-providers-plexus-3.2.1/apache_airflow_providers_plexus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:08.000000 apache-airflow-providers-plexus-3.2.1/apache_airflow_providers_plexus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:29:08.000000 apache-airflow-providers-plexus-3.2.1/apache_airflow_providers_plexus.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:08.000000 apache-airflow-providers-plexus-3.2.1/apache_airflow_providers_plexus.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-20 11:29:08.000000 apache-airflow-providers-plexus-3.2.1/apache_airflow_providers_plexus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:08.000000 apache-airflow-providers-plexus-3.2.1/apache_airflow_providers_plexus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-plexus-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-20 11:29:08.860288 apache-airflow-providers-plexus-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1638 2023-06-20 11:29:07.000000 apache-airflow-providers-plexus-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:52.557613 apache-airflow-providers-plexus-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-plexus-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:51.000000 apache-airflow-providers-plexus-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-plexus-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10078 2023-06-20 11:42:52.558850 apache-airflow-providers-plexus-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8550 2023-06-20 11:42:51.000000 apache-airflow-providers-plexus-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:52.470318 apache-airflow-providers-plexus-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:52.471434 apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:52.517088 apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-06-20 11:42:51.000000 apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:52.523203 apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-06-02 11:31:21.000000 apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/hooks/plexus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:52.529667 apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6055 2023-06-01 06:14:28.000000 apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/operators/job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:52.554600 apache-airflow-providers-plexus-3.2.1rc1/apache_airflow_providers_plexus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10078 2023-06-20 11:42:52.000000 apache-airflow-providers-plexus-3.2.1rc1/apache_airflow_providers_plexus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      713 2023-06-20 11:42:52.000000 apache-airflow-providers-plexus-3.2.1rc1/apache_airflow_providers_plexus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:52.000000 apache-airflow-providers-plexus-3.2.1rc1/apache_airflow_providers_plexus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:42:52.000000 apache-airflow-providers-plexus-3.2.1rc1/apache_airflow_providers_plexus.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:52.000000 apache-airflow-providers-plexus-3.2.1rc1/apache_airflow_providers_plexus.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-20 11:42:52.000000 apache-airflow-providers-plexus-3.2.1rc1/apache_airflow_providers_plexus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:52.000000 apache-airflow-providers-plexus-3.2.1rc1/apache_airflow_providers_plexus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-plexus-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-06-20 11:42:52.560891 apache-airflow-providers-plexus-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-06-20 11:42:51.000000 apache-airflow-providers-plexus-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-plexus-3.2.1/LICENSE` & `apache-airflow-providers-plexus-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.2.1/MANIFEST.in` & `apache-airflow-providers-plexus-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.2.1/PKG-INFO` & `apache-airflow-providers-plexus-3.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-plexus
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-plexus package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-plexus``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Plexus <https://plexus.corescientific.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-plexus-3.2.1/README.rst` & `apache-airflow-providers-plexus-3.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-plexus``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Plexus <https://plexus.corescientific.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/__init__.py` & `apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/get_provider_info.py` & `apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/hooks/__init__.py` & `apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/hooks/plexus.py` & `apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/hooks/plexus.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/operators/__init__.py` & `apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.2.1/airflow/providers/plexus/operators/job.py` & `apache-airflow-providers-plexus-3.2.1rc1/airflow/providers/plexus/operators/job.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.2.1/apache_airflow_providers_plexus.egg-info/PKG-INFO` & `apache-airflow-providers-plexus-3.2.1rc1/apache_airflow_providers_plexus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-plexus
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-plexus package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-plexus/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-plexus``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Plexus <https://plexus.corescientific.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-plexus-3.2.1/apache_airflow_providers_plexus.egg-info/SOURCES.txt` & `apache-airflow-providers-plexus-3.2.1rc1/apache_airflow_providers_plexus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.2.1/pyproject.toml` & `apache-airflow-providers-plexus-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-plexus-3.2.1/setup.cfg` & `apache-airflow-providers-plexus-3.2.1rc1/setup.cfg`

 * *Files 9% similar despite different names*

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
 	arrow>=0.16.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.plexus.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.plexus
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-plexus-3.2.1/setup.py` & `apache-airflow-providers-plexus-3.2.1rc1/setup.py`

 * *Files identical despite different names*

