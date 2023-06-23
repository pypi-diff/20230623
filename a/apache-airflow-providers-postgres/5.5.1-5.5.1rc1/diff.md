# Comparing `tmp/apache-airflow-providers-postgres-5.5.1.tar.gz` & `tmp/apache-airflow-providers-postgres-5.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-postgres-5.5.1.tar", last modified: Tue Jun 20 11:29:10 2023, max compression
+gzip compressed data, was "apache-airflow-providers-postgres-5.5.1rc1.tar", last modified: Tue Jun 20 11:42:54 2023, max compression
```

## Comparing `apache-airflow-providers-postgres-5.5.1.tar` & `apache-airflow-providers-postgres-5.5.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:10.849850 apache-airflow-providers-postgres-5.5.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:09.000000 apache-airflow-providers-postgres-5.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    15560 2023-06-20 11:29:10.851058 apache-airflow-providers-postgres-5.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13979 2023-06-20 11:29:09.000000 apache-airflow-providers-postgres-5.5.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:10.772148 apache-airflow-providers-postgres-5.5.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:10.773536 apache-airflow-providers-postgres-5.5.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:10.809836 apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3077 2023-06-20 11:29:09.000000 apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:10.815929 apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12967 2023-06-05 12:50:36.000000 apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/hooks/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:10.822133 apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3735 2023-06-02 11:31:21.000000 apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/operators/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:10.846432 apache-airflow-providers-postgres-5.5.1/apache_airflow_providers_postgres.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15560 2023-06-20 11:29:10.000000 apache-airflow-providers-postgres-5.5.1/apache_airflow_providers_postgres.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:29:10.000000 apache-airflow-providers-postgres-5.5.1/apache_airflow_providers_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:10.000000 apache-airflow-providers-postgres-5.5.1/apache_airflow_providers_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:29:10.000000 apache-airflow-providers-postgres-5.5.1/apache_airflow_providers_postgres.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:10.000000 apache-airflow-providers-postgres-5.5.1/apache_airflow_providers_postgres.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      187 2023-06-20 11:29:10.000000 apache-airflow-providers-postgres-5.5.1/apache_airflow_providers_postgres.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:10.000000 apache-airflow-providers-postgres-5.5.1/apache_airflow_providers_postgres.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-postgres-5.5.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1901 2023-06-20 11:29:10.853558 apache-airflow-providers-postgres-5.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1792 2023-06-20 11:29:09.000000 apache-airflow-providers-postgres-5.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.369568 apache-airflow-providers-postgres-5.5.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-postgres-5.5.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    15566 2023-06-20 11:42:54.371066 apache-airflow-providers-postgres-5.5.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13982 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.296192 apache-airflow-providers-postgres-5.5.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.297518 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.330567 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.336290 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12967 2023-06-05 12:50:36.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.342002 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3735 2023-06-02 11:31:21.000000 apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:54.366685 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15566 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-postgres-5.5.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-06-20 11:42:54.373575 apache-airflow-providers-postgres-5.5.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-06-20 11:42:53.000000 apache-airflow-providers-postgres-5.5.1rc1/setup.py
```

### Comparing `apache-airflow-providers-postgres-5.5.1/LICENSE` & `apache-airflow-providers-postgres-5.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1/MANIFEST.in` & `apache-airflow-providers-postgres-5.5.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1/PKG-INFO` & `apache-airflow-providers-postgres-5.5.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.5.1
+Version: 5.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.1/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.1``
+Release: ``5.5.1rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-postgres-5.5.1/README.rst` & `apache-airflow-providers-postgres-5.5.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.1``
+Release: ``5.5.1rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/__init__.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/get_provider_info.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/hooks/__init__.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/hooks/postgres.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/hooks/postgres.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/operators/__init__.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1/airflow/providers/postgres/operators/postgres.py` & `apache-airflow-providers-postgres-5.5.1rc1/airflow/providers/postgres/operators/postgres.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1/apache_airflow_providers_postgres.egg-info/PKG-INFO` & `apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-postgres
-Version: 5.5.1
+Version: 5.5.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-postgres package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-postgres/5.5.1/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-postgres``
 
-Release: ``5.5.1``
+Release: ``5.5.1rc1``
 
 
 `PostgreSQL <https://www.postgresql.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-postgres-5.5.1/apache_airflow_providers_postgres.egg-info/SOURCES.txt` & `apache-airflow-providers-postgres-5.5.1rc1/apache_airflow_providers_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1/pyproject.toml` & `apache-airflow-providers-postgres-5.5.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-postgres-5.5.1/setup.cfg` & `apache-airflow-providers-postgres-5.5.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -42,22 +42,22 @@
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
 	psycopg2-binary>=2.8.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.postgres.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.postgres
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-postgres-5.5.1/setup.py` & `apache-airflow-providers-postgres-5.5.1rc1/setup.py`

 * *Files identical despite different names*

