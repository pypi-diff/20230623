# Comparing `tmp/apache-airflow-providers-pagerduty-3.3.0.tar.gz` & `tmp/apache-airflow-providers-pagerduty-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-pagerduty-3.3.0.tar", last modified: Tue Jun 20 11:29:03 2023, max compression
+gzip compressed data, was "apache-airflow-providers-pagerduty-3.3.0rc1.tar", last modified: Tue Jun 20 11:42:48 2023, max compression
```

## Comparing `apache-airflow-providers-pagerduty-3.3.0.tar` & `apache-airflow-providers-pagerduty-3.3.0rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:03.869843 apache-airflow-providers-pagerduty-3.3.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-pagerduty-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:02.000000 apache-airflow-providers-pagerduty-3.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-pagerduty-3.3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10472 2023-06-20 11:29:03.871335 apache-airflow-providers-pagerduty-3.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8938 2023-06-20 11:29:02.000000 apache-airflow-providers-pagerduty-3.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:03.755594 apache-airflow-providers-pagerduty-3.3.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:03.756841 apache-airflow-providers-pagerduty-3.3.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:03.807127 apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-06-20 11:29:02.000000 apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:03.818255 apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-06-02 11:31:21.000000 apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/hooks/pagerduty.py
--rw-r--r--   0 root         (0) root         (0)    12253 2023-06-02 11:31:21.000000 apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/hooks/pagerduty_events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:03.827428 apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/notifications/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-17 16:45:00.000000 apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-06-17 16:45:00.000000 apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/notifications/pagerduty.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:03.866148 apache-airflow-providers-pagerduty-3.3.0/apache_airflow_providers_pagerduty.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10472 2023-06-20 11:29:03.000000 apache-airflow-providers-pagerduty-3.3.0/apache_airflow_providers_pagerduty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      823 2023-06-20 11:29:03.000000 apache-airflow-providers-pagerduty-3.3.0/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:03.000000 apache-airflow-providers-pagerduty-3.3.0/apache_airflow_providers_pagerduty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:29:03.000000 apache-airflow-providers-pagerduty-3.3.0/apache_airflow_providers_pagerduty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:03.000000 apache-airflow-providers-pagerduty-3.3.0/apache_airflow_providers_pagerduty.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-20 11:29:03.000000 apache-airflow-providers-pagerduty-3.3.0/apache_airflow_providers_pagerduty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:03.000000 apache-airflow-providers-pagerduty-3.3.0/apache_airflow_providers_pagerduty.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-pagerduty-3.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1855 2023-06-20 11:29:03.873958 apache-airflow-providers-pagerduty-3.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1656 2023-06-20 11:29:02.000000 apache-airflow-providers-pagerduty-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.942650 apache-airflow-providers-pagerduty-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-pagerduty-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:47.000000 apache-airflow-providers-pagerduty-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-pagerduty-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10478 2023-06-20 11:42:48.943701 apache-airflow-providers-pagerduty-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8941 2023-06-20 11:42:47.000000 apache-airflow-providers-pagerduty-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.864393 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.865464 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.897002 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-06-20 11:42:47.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.909189 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-06-02 11:31:21.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py
+-rw-r--r--   0 root         (0) root         (0)    12253 2023-06-02 11:31:21.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.915660 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/notifications/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-17 16:45:00.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-06-17 16:45:00.000000 apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/notifications/pagerduty.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:48.939944 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10478 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      823 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:48.000000 apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-pagerduty-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-06-20 11:42:48.945687 apache-airflow-providers-pagerduty-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-06-20 11:42:47.000000 apache-airflow-providers-pagerduty-3.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-pagerduty-3.3.0/LICENSE` & `apache-airflow-providers-pagerduty-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.3.0/MANIFEST.in` & `apache-airflow-providers-pagerduty-3.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.3.0/PKG-INFO` & `apache-airflow-providers-pagerduty-3.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pagerduty
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-pagerduty package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.3.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-pagerduty-3.3.0/README.rst` & `apache-airflow-providers-pagerduty-3.3.0rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/__init__.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/get_provider_info.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/hooks/__init__.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/hooks/pagerduty.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/pagerduty.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/hooks/pagerduty_events.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/hooks/pagerduty_events.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/notifications/__init__.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.3.0/airflow/providers/pagerduty/notifications/pagerduty.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/airflow/providers/pagerduty/notifications/pagerduty.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.3.0/apache_airflow_providers_pagerduty.egg-info/PKG-INFO` & `apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-pagerduty
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-pagerduty package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-pagerduty/3.3.0/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-pagerduty``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Pagerduty <https://www.pagerduty.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-pagerduty-3.3.0/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt` & `apache-airflow-providers-pagerduty-3.3.0rc1/apache_airflow_providers_pagerduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.3.0/pyproject.toml` & `apache-airflow-providers-pagerduty-3.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-pagerduty-3.3.0/setup.cfg` & `apache-airflow-providers-pagerduty-3.3.0rc1/setup.cfg`

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
 	pdpyras>=4.1.2
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.pagerduty.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.pagerduty
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-pagerduty-3.3.0/setup.py` & `apache-airflow-providers-pagerduty-3.3.0rc1/setup.py`

 * *Files identical despite different names*

