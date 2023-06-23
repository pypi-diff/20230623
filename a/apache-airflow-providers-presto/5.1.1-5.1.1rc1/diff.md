# Comparing `tmp/apache-airflow-providers-presto-5.1.1.tar.gz` & `tmp/apache-airflow-providers-presto-5.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-presto-5.1.1.tar", last modified: Tue Jun 20 11:29:12 2023, max compression
+gzip compressed data, was "apache-airflow-providers-presto-5.1.1rc1.tar", last modified: Tue Jun 20 11:42:56 2023, max compression
```

## Comparing `apache-airflow-providers-presto-5.1.1.tar` & `apache-airflow-providers-presto-5.1.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:12.670604 apache-airflow-providers-presto-5.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:11.000000 apache-airflow-providers-presto-5.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    14270 2023-06-20 11:29:12.671872 apache-airflow-providers-presto-5.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12695 2023-06-20 11:29:11.000000 apache-airflow-providers-presto-5.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:12.596928 apache-airflow-providers-presto-5.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:12.598219 apache-airflow-providers-presto-5.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:12.631968 apache-airflow-providers-presto-5.1.1/airflow/providers/presto/
--rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-presto-5.1.1/airflow/providers/presto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2927 2023-06-20 11:29:11.000000 apache-airflow-providers-presto-5.1.1/airflow/providers/presto/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:12.637865 apache-airflow-providers-presto-5.1.1/airflow/providers/presto/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.1/airflow/providers/presto/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8832 2023-06-02 11:31:21.000000 apache-airflow-providers-presto-5.1.1/airflow/providers/presto/hooks/presto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:12.643714 apache-airflow-providers-presto-5.1.1/airflow/providers/presto/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.1/airflow/providers/presto/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4836 2023-06-02 11:31:21.000000 apache-airflow-providers-presto-5.1.1/airflow/providers/presto/transfers/gcs_to_presto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:12.667480 apache-airflow-providers-presto-5.1.1/apache_airflow_providers_presto.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14270 2023-06-20 11:29:12.000000 apache-airflow-providers-presto-5.1.1/apache_airflow_providers_presto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      723 2023-06-20 11:29:12.000000 apache-airflow-providers-presto-5.1.1/apache_airflow_providers_presto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:12.000000 apache-airflow-providers-presto-5.1.1/apache_airflow_providers_presto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:29:12.000000 apache-airflow-providers-presto-5.1.1/apache_airflow_providers_presto.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:12.000000 apache-airflow-providers-presto-5.1.1/apache_airflow_providers_presto.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      200 2023-06-20 11:29:12.000000 apache-airflow-providers-presto-5.1.1/apache_airflow_providers_presto.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:12.000000 apache-airflow-providers-presto-5.1.1/apache_airflow_providers_presto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-presto-5.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1910 2023-06-20 11:29:12.674183 apache-airflow-providers-presto-5.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1773 2023-06-20 11:29:11.000000 apache-airflow-providers-presto-5.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.163627 apache-airflow-providers-presto-5.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-presto-5.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14276 2023-06-20 11:42:56.164703 apache-airflow-providers-presto-5.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12698 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.088803 apache-airflow-providers-presto-5.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.090015 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.122350 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-20 11:01:09.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2927 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.128435 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8832 2023-06-02 11:31:21.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/presto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.136308 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4836 2023-06-02 11:31:21.000000 apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/gcs_to_presto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:56.160935 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14276 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      723 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      210 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:56.000000 apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-presto-5.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-06-20 11:42:56.166648 apache-airflow-providers-presto-5.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-06-20 11:42:55.000000 apache-airflow-providers-presto-5.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-presto-5.1.1/LICENSE` & `apache-airflow-providers-presto-5.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1/MANIFEST.in` & `apache-airflow-providers-presto-5.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1/PKG-INFO` & `apache-airflow-providers-presto-5.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-presto
-Version: 5.1.1
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-presto package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.1/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-presto``
 
-Release: ``5.1.1``
+Release: ``5.1.1rc1``
 
 
 `Presto <https://prestodb.github.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-presto-5.1.1/README.rst` & `apache-airflow-providers-presto-5.1.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-presto``
 
-Release: ``5.1.1``
+Release: ``5.1.1rc1``
 
 
 `Presto <https://prestodb.github.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-presto-5.1.1/airflow/providers/presto/__init__.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1/airflow/providers/presto/get_provider_info.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1/airflow/providers/presto/hooks/__init__.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1/airflow/providers/presto/hooks/presto.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/hooks/presto.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1/airflow/providers/presto/transfers/__init__.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1/airflow/providers/presto/transfers/gcs_to_presto.py` & `apache-airflow-providers-presto-5.1.1rc1/airflow/providers/presto/transfers/gcs_to_presto.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1/apache_airflow_providers_presto.egg-info/PKG-INFO` & `apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-presto
-Version: 5.1.1
+Version: 5.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-presto package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-presto/5.1.1/
@@ -50,15 +50,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-presto``
 
-Release: ``5.1.1``
+Release: ``5.1.1rc1``
 
 
 `Presto <https://prestodb.github.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-presto-5.1.1/apache_airflow_providers_presto.egg-info/SOURCES.txt` & `apache-airflow-providers-presto-5.1.1rc1/apache_airflow_providers_presto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1/pyproject.toml` & `apache-airflow-providers-presto-5.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-presto-5.1.1/setup.cfg` & `apache-airflow-providers-presto-5.1.1rc1/setup.cfg`

 * *Files 8% similar despite different names*

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
 	presto-python-client>=0.8.2
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.presto.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.presto
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-presto-5.1.1/setup.py` & `apache-airflow-providers-presto-5.1.1rc1/setup.py`

 * *Files identical despite different names*

