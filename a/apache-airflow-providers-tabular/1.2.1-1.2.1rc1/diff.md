# Comparing `tmp/apache-airflow-providers-tabular-1.2.1.tar.gz` & `tmp/apache-airflow-providers-tabular-1.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-tabular-1.2.1.tar", last modified: Tue Jun 20 11:29:44 2023, max compression
+gzip compressed data, was "apache-airflow-providers-tabular-1.2.1rc1.tar", last modified: Tue Jun 20 11:43:23 2023, max compression
```

## Comparing `apache-airflow-providers-tabular-1.2.1.tar` & `apache-airflow-providers-tabular-1.2.1rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:44.147775 apache-airflow-providers-tabular-1.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-tabular-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:43.000000 apache-airflow-providers-tabular-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-tabular-1.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6454 2023-06-20 11:29:44.148391 apache-airflow-providers-tabular-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4926 2023-06-20 11:29:43.000000 apache-airflow-providers-tabular-1.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:44.067079 apache-airflow-providers-tabular-1.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:44.068297 apache-airflow-providers-tabular-1.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:44.107565 apache-airflow-providers-tabular-1.2.1/airflow/providers/tabular/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-tabular-1.2.1/airflow/providers/tabular/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-20 11:29:43.000000 apache-airflow-providers-tabular-1.2.1/airflow/providers/tabular/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:44.116353 apache-airflow-providers-tabular-1.2.1/airflow/providers/tabular/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-tabular-1.2.1/airflow/providers/tabular/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3331 2023-06-02 11:31:21.000000 apache-airflow-providers-tabular-1.2.1/airflow/providers/tabular/hooks/tabular.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:44.145181 apache-airflow-providers-tabular-1.2.1/apache_airflow_providers_tabular.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6454 2023-06-20 11:29:44.000000 apache-airflow-providers-tabular-1.2.1/apache_airflow_providers_tabular.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      636 2023-06-20 11:29:44.000000 apache-airflow-providers-tabular-1.2.1/apache_airflow_providers_tabular.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:44.000000 apache-airflow-providers-tabular-1.2.1/apache_airflow_providers_tabular.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:29:44.000000 apache-airflow-providers-tabular-1.2.1/apache_airflow_providers_tabular.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:44.000000 apache-airflow-providers-tabular-1.2.1/apache_airflow_providers_tabular.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-20 11:29:44.000000 apache-airflow-providers-tabular-1.2.1/apache_airflow_providers_tabular.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:44.000000 apache-airflow-providers-tabular-1.2.1/apache_airflow_providers_tabular.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-tabular-1.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1827 2023-06-20 11:29:44.150449 apache-airflow-providers-tabular-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:29:42.000000 apache-airflow-providers-tabular-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:23.309047 apache-airflow-providers-tabular-1.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-tabular-1.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:22.000000 apache-airflow-providers-tabular-1.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-tabular-1.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6460 2023-06-20 11:43:23.309631 apache-airflow-providers-tabular-1.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4929 2023-06-20 11:43:22.000000 apache-airflow-providers-tabular-1.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:23.243776 apache-airflow-providers-tabular-1.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:23.245019 apache-airflow-providers-tabular-1.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:23.276977 apache-airflow-providers-tabular-1.2.1rc1/airflow/providers/tabular/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-tabular-1.2.1rc1/airflow/providers/tabular/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-20 11:43:22.000000 apache-airflow-providers-tabular-1.2.1rc1/airflow/providers/tabular/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:23.282927 apache-airflow-providers-tabular-1.2.1rc1/airflow/providers/tabular/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-tabular-1.2.1rc1/airflow/providers/tabular/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3331 2023-06-02 11:31:21.000000 apache-airflow-providers-tabular-1.2.1rc1/airflow/providers/tabular/hooks/tabular.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:23.306754 apache-airflow-providers-tabular-1.2.1rc1/apache_airflow_providers_tabular.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6460 2023-06-20 11:43:23.000000 apache-airflow-providers-tabular-1.2.1rc1/apache_airflow_providers_tabular.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      636 2023-06-20 11:43:23.000000 apache-airflow-providers-tabular-1.2.1rc1/apache_airflow_providers_tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:23.000000 apache-airflow-providers-tabular-1.2.1rc1/apache_airflow_providers_tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:43:23.000000 apache-airflow-providers-tabular-1.2.1rc1/apache_airflow_providers_tabular.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:23.000000 apache-airflow-providers-tabular-1.2.1rc1/apache_airflow_providers_tabular.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:43:23.000000 apache-airflow-providers-tabular-1.2.1rc1/apache_airflow_providers_tabular.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:23.000000 apache-airflow-providers-tabular-1.2.1rc1/apache_airflow_providers_tabular.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-tabular-1.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-06-20 11:43:23.311593 apache-airflow-providers-tabular-1.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:43:22.000000 apache-airflow-providers-tabular-1.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-tabular-1.2.1/LICENSE` & `apache-airflow-providers-tabular-1.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tabular-1.2.1/MANIFEST.in` & `apache-airflow-providers-tabular-1.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tabular-1.2.1/PKG-INFO` & `apache-airflow-providers-tabular-1.2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-tabular
-Version: 1.2.1
+Version: 1.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-tabular package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-tabular``
 
-Release: ``1.2.1``
+Release: ``1.2.1rc1``
 
 
 `Tabular <https://tabular.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-tabular-1.2.1/README.rst` & `apache-airflow-providers-tabular-1.2.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-tabular``
 
-Release: ``1.2.1``
+Release: ``1.2.1rc1``
 
 
 `Tabular <https://tabular.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-tabular-1.2.1/airflow/providers/tabular/__init__.py` & `apache-airflow-providers-tabular-1.2.1rc1/airflow/providers/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tabular-1.2.1/airflow/providers/tabular/get_provider_info.py` & `apache-airflow-providers-tabular-1.2.1rc1/airflow/providers/tabular/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tabular-1.2.1/airflow/providers/tabular/hooks/__init__.py` & `apache-airflow-providers-tabular-1.2.1rc1/airflow/providers/tabular/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tabular-1.2.1/airflow/providers/tabular/hooks/tabular.py` & `apache-airflow-providers-tabular-1.2.1rc1/airflow/providers/tabular/hooks/tabular.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tabular-1.2.1/apache_airflow_providers_tabular.egg-info/PKG-INFO` & `apache-airflow-providers-tabular-1.2.1rc1/apache_airflow_providers_tabular.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-tabular
-Version: 1.2.1
+Version: 1.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-tabular package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-tabular/1.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-tabular``
 
-Release: ``1.2.1``
+Release: ``1.2.1rc1``
 
 
 `Tabular <https://tabular.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-tabular-1.2.1/apache_airflow_providers_tabular.egg-info/SOURCES.txt` & `apache-airflow-providers-tabular-1.2.1rc1/apache_airflow_providers_tabular.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tabular-1.2.1/pyproject.toml` & `apache-airflow-providers-tabular-1.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-tabular-1.2.1/setup.cfg` & `apache-airflow-providers-tabular-1.2.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.tabular.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.tabular
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-tabular-1.2.1/setup.py` & `apache-airflow-providers-tabular-1.2.1rc1/setup.py`

 * *Files identical despite different names*

