# Comparing `tmp/apache-airflow-providers-exasol-4.2.1.tar.gz` & `tmp/apache-airflow-providers-exasol-4.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-exasol-4.2.1.tar", last modified: Tue Jun 20 11:28:09 2023, max compression
+gzip compressed data, was "apache-airflow-providers-exasol-4.2.1rc1.tar", last modified: Tue Jun 20 11:42:00 2023, max compression
```

## Comparing `apache-airflow-providers-exasol-4.2.1.tar` & `apache-airflow-providers-exasol-4.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:09.418763 apache-airflow-providers-exasol-4.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:08.000000 apache-airflow-providers-exasol-4.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13065 2023-06-20 11:28:09.419774 apache-airflow-providers-exasol-4.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11513 2023-06-20 11:28:08.000000 apache-airflow-providers-exasol-4.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:09.346521 apache-airflow-providers-exasol-4.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:09.347725 apache-airflow-providers-exasol-4.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:09.379768 apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-06-20 11:28:08.000000 apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:09.385336 apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10925 2023-06-05 12:50:36.000000 apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/hooks/exasol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:09.391186 apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-06-02 11:31:21.000000 apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/operators/exasol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:09.416116 apache-airflow-providers-exasol-4.2.1/apache_airflow_providers_exasol.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13065 2023-06-20 11:28:09.000000 apache-airflow-providers-exasol-4.2.1/apache_airflow_providers_exasol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      716 2023-06-20 11:28:09.000000 apache-airflow-providers-exasol-4.2.1/apache_airflow_providers_exasol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:09.000000 apache-airflow-providers-exasol-4.2.1/apache_airflow_providers_exasol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:28:09.000000 apache-airflow-providers-exasol-4.2.1/apache_airflow_providers_exasol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:09.000000 apache-airflow-providers-exasol-4.2.1/apache_airflow_providers_exasol.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-20 11:28:09.000000 apache-airflow-providers-exasol-4.2.1/apache_airflow_providers_exasol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:09.000000 apache-airflow-providers-exasol-4.2.1/apache_airflow_providers_exasol.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-exasol-4.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1898 2023-06-20 11:28:09.421729 apache-airflow-providers-exasol-4.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:28:08.000000 apache-airflow-providers-exasol-4.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.090548 apache-airflow-providers-exasol-4.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-exasol-4.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13071 2023-06-20 11:42:00.091679 apache-airflow-providers-exasol-4.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11516 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.010967 apache-airflow-providers-exasol-4.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.012178 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.051802 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.057572 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10925 2023-06-05 12:50:36.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/exasol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.063339 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-06-02 11:31:21.000000 apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/exasol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:00.087791 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13071 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-exasol-4.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-06-20 11:42:00.093634 apache-airflow-providers-exasol-4.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:41:59.000000 apache-airflow-providers-exasol-4.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-exasol-4.2.1/LICENSE` & `apache-airflow-providers-exasol-4.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1/MANIFEST.in` & `apache-airflow-providers-exasol-4.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1/PKG-INFO` & `apache-airflow-providers-exasol-4.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-exasol
-Version: 4.2.1
+Version: 4.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-exasol package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-exasol``
 
-Release: ``4.2.1``
+Release: ``4.2.1rc1``
 
 
 `Exasol <https://docs.exasol.com/home.htm>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-exasol-4.2.1/README.rst` & `apache-airflow-providers-exasol-4.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-exasol``
 
-Release: ``4.2.1``
+Release: ``4.2.1rc1``
 
 
 `Exasol <https://docs.exasol.com/home.htm>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/__init__.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/get_provider_info.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/hooks/__init__.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/hooks/exasol.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/hooks/exasol.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/operators/__init__.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1/airflow/providers/exasol/operators/exasol.py` & `apache-airflow-providers-exasol-4.2.1rc1/airflow/providers/exasol/operators/exasol.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1/apache_airflow_providers_exasol.egg-info/PKG-INFO` & `apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-exasol
-Version: 4.2.1
+Version: 4.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-exasol package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-exasol/4.2.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-exasol``
 
-Release: ``4.2.1``
+Release: ``4.2.1rc1``
 
 
 `Exasol <https://docs.exasol.com/home.htm>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-exasol-4.2.1/apache_airflow_providers_exasol.egg-info/SOURCES.txt` & `apache-airflow-providers-exasol-4.2.1rc1/apache_airflow_providers_exasol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1/pyproject.toml` & `apache-airflow-providers-exasol-4.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-exasol-4.2.1/setup.cfg` & `apache-airflow-providers-exasol-4.2.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -42,23 +42,23 @@
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
 	pandas>=0.17.1
 	pyexasol>=0.5.1
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.exasol.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.exasol
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-exasol-4.2.1/setup.py` & `apache-airflow-providers-exasol-4.2.1rc1/setup.py`

 * *Files identical despite different names*

