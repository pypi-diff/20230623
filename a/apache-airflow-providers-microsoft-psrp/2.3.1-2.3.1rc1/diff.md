# Comparing `tmp/apache-airflow-providers-microsoft-psrp-2.3.1.tar.gz` & `tmp/apache-airflow-providers-microsoft-psrp-2.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-microsoft-psrp-2.3.1.tar", last modified: Tue Jun 20 11:28:43 2023, max compression
+gzip compressed data, was "apache-airflow-providers-microsoft-psrp-2.3.1rc1.tar", last modified: Tue Jun 20 11:42:32 2023, max compression
```

## Comparing `apache-airflow-providers-microsoft-psrp-2.3.1.tar` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:43.232886 apache-airflow-providers-microsoft-psrp-2.3.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-psrp-2.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:41.000000 apache-airflow-providers-microsoft-psrp-2.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-psrp-2.3.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9302 2023-06-20 11:28:43.234098 apache-airflow-providers-microsoft-psrp-2.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7753 2023-06-20 11:28:41.000000 apache-airflow-providers-microsoft-psrp-2.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:43.142865 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:43.143891 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:43.144906 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:43.182206 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/
--rw-r--r--   0 root         (0) root         (0)     1539 2023-06-20 11:01:09.000000 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2503 2023-06-20 11:28:41.000000 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:43.190513 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/hooks/psrp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:43.198600 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7175 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/operators/psrp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:43.229405 apache-airflow-providers-microsoft-psrp-2.3.1/apache_airflow_providers_microsoft_psrp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9302 2023-06-20 11:28:43.000000 apache-airflow-providers-microsoft-psrp-2.3.1/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 11:28:43.000000 apache-airflow-providers-microsoft-psrp-2.3.1/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:43.000000 apache-airflow-providers-microsoft-psrp-2.3.1/apache_airflow_providers_microsoft_psrp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-20 11:28:43.000000 apache-airflow-providers-microsoft-psrp-2.3.1/apache_airflow_providers_microsoft_psrp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:43.000000 apache-airflow-providers-microsoft-psrp-2.3.1/apache_airflow_providers_microsoft_psrp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-20 11:28:43.000000 apache-airflow-providers-microsoft-psrp-2.3.1/apache_airflow_providers_microsoft_psrp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:43.000000 apache-airflow-providers-microsoft-psrp-2.3.1/apache_airflow_providers_microsoft_psrp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-microsoft-psrp-2.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1884 2023-06-20 11:28:43.236702 apache-airflow-providers-microsoft-psrp-2.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1686 2023-06-20 11:28:41.000000 apache-airflow-providers-microsoft-psrp-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:32.117417 apache-airflow-providers-microsoft-psrp-2.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:31.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9308 2023-06-20 11:42:32.118635 apache-airflow-providers-microsoft-psrp-2.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7756 2023-06-20 11:42:31.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:32.028106 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:32.029415 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:32.030630 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:32.066183 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-06-20 11:01:09.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2023-06-20 11:42:31.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:32.072953 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/hooks/psrp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:32.080380 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2023-06-01 06:14:28.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/operators/psrp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:32.114240 apache-airflow-providers-microsoft-psrp-2.3.1rc1/apache_airflow_providers_microsoft_psrp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9308 2023-06-20 11:42:31.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-20 11:42:31.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:31.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/apache_airflow_providers_microsoft_psrp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-20 11:42:31.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/apache_airflow_providers_microsoft_psrp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:31.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/apache_airflow_providers_microsoft_psrp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-20 11:42:31.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/apache_airflow_providers_microsoft_psrp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:31.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/apache_airflow_providers_microsoft_psrp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-20 11:42:32.120818 apache-airflow-providers-microsoft-psrp-2.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-06-20 11:42:31.000000 apache-airflow-providers-microsoft-psrp-2.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/LICENSE` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/MANIFEST.in` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/PKG-INFO` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-psrp
-Version: 2.3.1
+Version: 2.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-psrp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.3.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.3.1``
+Release: ``2.3.1rc1``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/>`__.
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/README.rst` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.3.1``
+Release: ``2.3.1rc1``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/>`__.
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/__init__.py` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/get_provider_info.py` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/hooks/__init__.py` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/hooks/psrp.py` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/hooks/psrp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/operators/__init__.py` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/airflow/providers/microsoft/psrp/operators/psrp.py` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/airflow/providers/microsoft/psrp/operators/psrp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/apache_airflow_providers_microsoft_psrp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-microsoft-psrp
-Version: 2.3.1
+Version: 2.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-microsoft-psrp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-microsoft-psrp/2.3.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-microsoft-psrp``
 
-Release: ``2.3.1``
+Release: ``2.3.1rc1``
 
 
 This package provides remote execution capabilities via the
 `PowerShell Remoting Protocol (PSRP)
 <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/>`__.
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/apache_airflow_providers_microsoft_psrp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/pyproject.toml` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/setup.cfg` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/setup.cfg`

 * *Files 4% similar despite different names*

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
 	pypsrp>=0.8.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.microsoft.psrp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.microsoft.psrp
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-microsoft-psrp-2.3.1/setup.py` & `apache-airflow-providers-microsoft-psrp-2.3.1rc1/setup.py`

 * *Files identical despite different names*

