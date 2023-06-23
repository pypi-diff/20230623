# Comparing `tmp/apache-airflow-providers-github-2.3.1.tar.gz` & `tmp/apache-airflow-providers-github-2.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-github-2.3.1.tar", last modified: Tue Jun 20 11:28:14 2023, max compression
+gzip compressed data, was "apache-airflow-providers-github-2.3.1rc1.tar", last modified: Tue Jun 20 11:42:05 2023, max compression
```

## Comparing `apache-airflow-providers-github-2.3.1.tar` & `apache-airflow-providers-github-2.3.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:14.861079 apache-airflow-providers-github-2.3.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-github-2.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:13.000000 apache-airflow-providers-github-2.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-github-2.3.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     8592 2023-06-20 11:28:14.862331 apache-airflow-providers-github-2.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7067 2023-06-20 11:28:13.000000 apache-airflow-providers-github-2.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:14.765522 apache-airflow-providers-github-2.3.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:14.766615 apache-airflow-providers-github-2.3.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:14.800996 apache-airflow-providers-github-2.3.1/airflow/providers/github/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-github-2.3.1/airflow/providers/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2384 2023-06-20 11:28:13.000000 apache-airflow-providers-github-2.3.1/airflow/providers/github/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:14.806643 apache-airflow-providers-github-2.3.1/airflow/providers/github/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-github-2.3.1/airflow/providers/github/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3350 2023-06-02 11:31:21.000000 apache-airflow-providers-github-2.3.1/airflow/providers/github/hooks/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:14.813103 apache-airflow-providers-github-2.3.1/airflow/providers/github/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-github-2.3.1/airflow/providers/github/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3006 2023-06-05 12:50:36.000000 apache-airflow-providers-github-2.3.1/airflow/providers/github/operators/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:14.819321 apache-airflow-providers-github-2.3.1/airflow/providers/github/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-github-2.3.1/airflow/providers/github/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5278 2023-06-02 11:31:21.000000 apache-airflow-providers-github-2.3.1/airflow/providers/github/sensors/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:14.857516 apache-airflow-providers-github-2.3.1/apache_airflow_providers_github.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8592 2023-06-20 11:28:14.000000 apache-airflow-providers-github-2.3.1/apache_airflow_providers_github.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-06-20 11:28:14.000000 apache-airflow-providers-github-2.3.1/apache_airflow_providers_github.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:14.000000 apache-airflow-providers-github-2.3.1/apache_airflow_providers_github.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:28:14.000000 apache-airflow-providers-github-2.3.1/apache_airflow_providers_github.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:14.000000 apache-airflow-providers-github-2.3.1/apache_airflow_providers_github.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-20 11:28:14.000000 apache-airflow-providers-github-2.3.1/apache_airflow_providers_github.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:14.000000 apache-airflow-providers-github-2.3.1/apache_airflow_providers_github.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-github-2.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1837 2023-06-20 11:28:14.864765 apache-airflow-providers-github-2.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1638 2023-06-20 11:28:13.000000 apache-airflow-providers-github-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.409521 apache-airflow-providers-github-2.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-github-2.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:04.000000 apache-airflow-providers-github-2.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-github-2.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     8598 2023-06-20 11:42:05.410709 apache-airflow-providers-github-2.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7070 2023-06-20 11:42:04.000000 apache-airflow-providers-github-2.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.321707 apache-airflow-providers-github-2.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.322761 apache-airflow-providers-github-2.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.356383 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2023-06-20 11:42:04.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.362590 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2023-06-02 11:31:21.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/hooks/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.369395 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3006 2023-06-05 12:50:36.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/operators/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.375929 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5278 2023-06-02 11:31:21.000000 apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/sensors/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:05.407186 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8598 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:05.000000 apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-github-2.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-20 11:42:05.412712 apache-airflow-providers-github-2.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-06-20 11:42:04.000000 apache-airflow-providers-github-2.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-github-2.3.1/LICENSE` & `apache-airflow-providers-github-2.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/MANIFEST.in` & `apache-airflow-providers-github-2.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/PKG-INFO` & `apache-airflow-providers-github-2.3.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-github
-Version: 2.3.1
+Version: 2.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-github package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-github``
 
-Release: ``2.3.1``
+Release: ``2.3.1rc1``
 
 
 `GitHub <https://www.github.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-github-2.3.1/README.rst` & `apache-airflow-providers-github-2.3.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-github``
 
-Release: ``2.3.1``
+Release: ``2.3.1rc1``
 
 
 `GitHub <https://www.github.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-github-2.3.1/airflow/providers/github/__init__.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/airflow/providers/github/get_provider_info.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/airflow/providers/github/hooks/__init__.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/airflow/providers/github/hooks/github.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/hooks/github.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/airflow/providers/github/operators/__init__.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/airflow/providers/github/operators/github.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/operators/github.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/airflow/providers/github/sensors/__init__.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/airflow/providers/github/sensors/github.py` & `apache-airflow-providers-github-2.3.1rc1/airflow/providers/github/sensors/github.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/apache_airflow_providers_github.egg-info/PKG-INFO` & `apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-github
-Version: 2.3.1
+Version: 2.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-github package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-github/2.3.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-github``
 
-Release: ``2.3.1``
+Release: ``2.3.1rc1``
 
 
 `GitHub <https://www.github.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-github-2.3.1/apache_airflow_providers_github.egg-info/SOURCES.txt` & `apache-airflow-providers-github-2.3.1rc1/apache_airflow_providers_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/pyproject.toml` & `apache-airflow-providers-github-2.3.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-github-2.3.1/setup.cfg` & `apache-airflow-providers-github-2.3.1rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	PyGithub!=1.58
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.github.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.github
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-github-2.3.1/setup.py` & `apache-airflow-providers-github-2.3.1rc1/setup.py`

 * *Files identical despite different names*

