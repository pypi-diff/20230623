# Comparing `tmp/apache-airflow-providers-openfaas-3.2.1.tar.gz` & `tmp/apache-airflow-providers-openfaas-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-openfaas-3.2.1.tar", last modified: Tue Jun 20 11:28:56 2023, max compression
+gzip compressed data, was "apache-airflow-providers-openfaas-3.2.1rc1.tar", last modified: Tue Jun 20 11:42:43 2023, max compression
```

## Comparing `apache-airflow-providers-openfaas-3.2.1.tar` & `apache-airflow-providers-openfaas-3.2.1rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:56.714271 apache-airflow-providers-openfaas-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-openfaas-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:55.000000 apache-airflow-providers-openfaas-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-openfaas-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9477 2023-06-20 11:28:56.718621 apache-airflow-providers-openfaas-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7946 2023-06-20 11:28:55.000000 apache-airflow-providers-openfaas-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:56.613629 apache-airflow-providers-openfaas-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:56.614725 apache-airflow-providers-openfaas-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:56.651514 apache-airflow-providers-openfaas-3.2.1/airflow/providers/openfaas/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-openfaas-3.2.1/airflow/providers/openfaas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-06-20 11:28:55.000000 apache-airflow-providers-openfaas-3.2.1/airflow/providers/openfaas/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:56.658313 apache-airflow-providers-openfaas-3.2.1/airflow/providers/openfaas/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-openfaas-3.2.1/airflow/providers/openfaas/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4890 2023-06-02 11:31:21.000000 apache-airflow-providers-openfaas-3.2.1/airflow/providers/openfaas/hooks/openfaas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:56.710384 apache-airflow-providers-openfaas-3.2.1/apache_airflow_providers_openfaas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9477 2023-06-20 11:28:56.000000 apache-airflow-providers-openfaas-3.2.1/apache_airflow_providers_openfaas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      648 2023-06-20 11:28:56.000000 apache-airflow-providers-openfaas-3.2.1/apache_airflow_providers_openfaas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:56.000000 apache-airflow-providers-openfaas-3.2.1/apache_airflow_providers_openfaas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:28:56.000000 apache-airflow-providers-openfaas-3.2.1/apache_airflow_providers_openfaas.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:56.000000 apache-airflow-providers-openfaas-3.2.1/apache_airflow_providers_openfaas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-20 11:28:56.000000 apache-airflow-providers-openfaas-3.2.1/apache_airflow_providers_openfaas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:56.000000 apache-airflow-providers-openfaas-3.2.1/apache_airflow_providers_openfaas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-openfaas-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1833 2023-06-20 11:28:56.721619 apache-airflow-providers-openfaas-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:28:55.000000 apache-airflow-providers-openfaas-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.305360 apache-airflow-providers-openfaas-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-openfaas-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:42.000000 apache-airflow-providers-openfaas-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-openfaas-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9483 2023-06-20 11:42:43.306616 apache-airflow-providers-openfaas-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7949 2023-06-20 11:42:42.000000 apache-airflow-providers-openfaas-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.229118 apache-airflow-providers-openfaas-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.230451 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.267907 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-06-20 11:42:42.000000 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.275174 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2023-06-02 11:31:21.000000 apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/hooks/openfaas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:43.302457 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9483 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      648 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:43.000000 apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-openfaas-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-06-20 11:42:43.308871 apache-airflow-providers-openfaas-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:42:42.000000 apache-airflow-providers-openfaas-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-openfaas-3.2.1/LICENSE` & `apache-airflow-providers-openfaas-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.1/MANIFEST.in` & `apache-airflow-providers-openfaas-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.1/PKG-INFO` & `apache-airflow-providers-openfaas-3.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openfaas
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-openfaas package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-openfaas``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `OpenFaaS <https://www.openfaas.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-openfaas-3.2.1/README.rst` & `apache-airflow-providers-openfaas-3.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-openfaas``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `OpenFaaS <https://www.openfaas.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-openfaas-3.2.1/airflow/providers/openfaas/__init__.py` & `apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.1/airflow/providers/openfaas/get_provider_info.py` & `apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.1/airflow/providers/openfaas/hooks/__init__.py` & `apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.1/airflow/providers/openfaas/hooks/openfaas.py` & `apache-airflow-providers-openfaas-3.2.1rc1/airflow/providers/openfaas/hooks/openfaas.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.1/apache_airflow_providers_openfaas.egg-info/PKG-INFO` & `apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-openfaas
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-openfaas package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-openfaas/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-openfaas``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `OpenFaaS <https://www.openfaas.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-openfaas-3.2.1/apache_airflow_providers_openfaas.egg-info/SOURCES.txt` & `apache-airflow-providers-openfaas-3.2.1rc1/apache_airflow_providers_openfaas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.1/pyproject.toml` & `apache-airflow-providers-openfaas-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-openfaas-3.2.1/setup.cfg` & `apache-airflow-providers-openfaas-3.2.1rc1/setup.cfg`

 * *Files 4% similar despite different names*

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
 	provider_info=airflow.providers.openfaas.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.openfaas
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-openfaas-3.2.1/setup.py` & `apache-airflow-providers-openfaas-3.2.1rc1/setup.py`

 * *Files identical despite different names*

