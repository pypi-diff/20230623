# Comparing `tmp/apache-airflow-providers-sqlite-3.4.2.tar.gz` & `tmp/apache-airflow-providers-sqlite-3.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sqlite-3.4.2.tar", last modified: Tue Jun 20 11:29:38 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sqlite-3.4.2rc1.tar", last modified: Tue Jun 20 11:43:17 2023, max compression
```

## Comparing `apache-airflow-providers-sqlite-3.4.2.tar` & `apache-airflow-providers-sqlite-3.4.2rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:38.197169 apache-airflow-providers-sqlite-3.4.2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:37.000000 apache-airflow-providers-sqlite-3.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13409 2023-06-20 11:29:38.198799 apache-airflow-providers-sqlite-3.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11857 2023-06-20 11:29:37.000000 apache-airflow-providers-sqlite-3.4.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:38.119176 apache-airflow-providers-sqlite-3.4.2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:38.120294 apache-airflow-providers-sqlite-3.4.2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:38.154374 apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-06-20 11:29:37.000000 apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:38.160292 apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2402 2023-06-02 11:31:21.000000 apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/hooks/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:38.166894 apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2228 2023-06-02 11:31:21.000000 apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/operators/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:38.194235 apache-airflow-providers-sqlite-3.4.2/apache_airflow_providers_sqlite.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13409 2023-06-20 11:29:38.000000 apache-airflow-providers-sqlite-3.4.2/apache_airflow_providers_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      716 2023-06-20 11:29:38.000000 apache-airflow-providers-sqlite-3.4.2/apache_airflow_providers_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:38.000000 apache-airflow-providers-sqlite-3.4.2/apache_airflow_providers_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:29:38.000000 apache-airflow-providers-sqlite-3.4.2/apache_airflow_providers_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:38.000000 apache-airflow-providers-sqlite-3.4.2/apache_airflow_providers_sqlite.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      115 2023-06-20 11:29:38.000000 apache-airflow-providers-sqlite-3.4.2/apache_airflow_providers_sqlite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:38.000000 apache-airflow-providers-sqlite-3.4.2/apache_airflow_providers_sqlite.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-sqlite-3.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1865 2023-06-20 11:29:38.201271 apache-airflow-providers-sqlite-3.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:29:37.000000 apache-airflow-providers-sqlite-3.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.927449 apache-airflow-providers-sqlite-3.4.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:16.000000 apache-airflow-providers-sqlite-3.4.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13415 2023-06-20 11:43:17.928638 apache-airflow-providers-sqlite-3.4.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11860 2023-06-20 11:43:16.000000 apache-airflow-providers-sqlite-3.4.2rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.844732 apache-airflow-providers-sqlite-3.4.2rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.845749 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.881811 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-06-20 11:43:16.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.887856 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2023-06-02 11:31:21.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/hooks/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.893672 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-06-02 11:31:21.000000 apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/operators/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:17.924270 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13415 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:17.000000 apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-sqlite-3.4.2rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-06-20 11:43:17.930945 apache-airflow-providers-sqlite-3.4.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-20 11:43:16.000000 apache-airflow-providers-sqlite-3.4.2rc1/setup.py
```

### Comparing `apache-airflow-providers-sqlite-3.4.2/LICENSE` & `apache-airflow-providers-sqlite-3.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.2/MANIFEST.in` & `apache-airflow-providers-sqlite-3.4.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.2/PKG-INFO` & `apache-airflow-providers-sqlite-3.4.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sqlite
-Version: 3.4.2
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sqlite package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.2/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-sqlite-3.4.2/README.rst` & `apache-airflow-providers-sqlite-3.4.2rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/__init__.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/get_provider_info.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/hooks/__init__.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/hooks/sqlite.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/hooks/sqlite.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/operators/__init__.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.2/airflow/providers/sqlite/operators/sqlite.py` & `apache-airflow-providers-sqlite-3.4.2rc1/airflow/providers/sqlite/operators/sqlite.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.2/apache_airflow_providers_sqlite.egg-info/PKG-INFO` & `apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sqlite
-Version: 3.4.2
+Version: 3.4.2rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sqlite package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sqlite/3.4.2/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sqlite``
 
-Release: ``3.4.2``
+Release: ``3.4.2rc1``
 
 
 `SQLite <https://www.sqlite.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-sqlite-3.4.2/apache_airflow_providers_sqlite.egg-info/SOURCES.txt` & `apache-airflow-providers-sqlite-3.4.2rc1/apache_airflow_providers_sqlite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.2/pyproject.toml` & `apache-airflow-providers-sqlite-3.4.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sqlite-3.4.2/setup.cfg` & `apache-airflow-providers-sqlite-3.4.2rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,21 @@
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
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.sqlite.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.sqlite
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-sqlite-3.4.2/setup.py` & `apache-airflow-providers-sqlite-3.4.2rc1/setup.py`

 * *Files identical despite different names*

