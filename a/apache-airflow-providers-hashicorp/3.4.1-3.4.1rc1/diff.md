# Comparing `tmp/apache-airflow-providers-hashicorp-3.4.1.tar.gz` & `tmp/apache-airflow-providers-hashicorp-3.4.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-hashicorp-3.4.1.tar", last modified: Tue Jun 20 11:28:26 2023, max compression
+gzip compressed data, was "apache-airflow-providers-hashicorp-3.4.1rc1.tar", last modified: Tue Jun 20 11:42:16 2023, max compression
```

## Comparing `apache-airflow-providers-hashicorp-3.4.1.tar` & `apache-airflow-providers-hashicorp-3.4.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:26.080711 apache-airflow-providers-hashicorp-3.4.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:25.000000 apache-airflow-providers-hashicorp-3.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13205 2023-06-20 11:28:26.081921 apache-airflow-providers-hashicorp-3.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11648 2023-06-20 11:28:25.000000 apache-airflow-providers-hashicorp-3.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:25.992825 apache-airflow-providers-hashicorp-3.4.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:25.993976 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:26.030574 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/
--rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:26.036811 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/_internal_client/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/_internal_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20545 2023-06-01 07:44:14.000000 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/_internal_client/vault_client.py
--rw-r--r--   0 root         (0) root         (0)     2544 2023-06-20 11:28:25.000000 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:26.043815 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18752 2023-06-02 11:31:21.000000 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/hooks/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:26.051651 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11991 2023-06-02 11:31:21.000000 apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/secrets/vault.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:26.077819 apache-airflow-providers-hashicorp-3.4.1/apache_airflow_providers_hashicorp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13205 2023-06-20 11:28:25.000000 apache-airflow-providers-hashicorp-3.4.1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      867 2023-06-20 11:28:25.000000 apache-airflow-providers-hashicorp-3.4.1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:25.000000 apache-airflow-providers-hashicorp-3.4.1/apache_airflow_providers_hashicorp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:28:25.000000 apache-airflow-providers-hashicorp-3.4.1/apache_airflow_providers_hashicorp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:25.000000 apache-airflow-providers-hashicorp-3.4.1/apache_airflow_providers_hashicorp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-20 11:28:25.000000 apache-airflow-providers-hashicorp-3.4.1/apache_airflow_providers_hashicorp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:25.000000 apache-airflow-providers-hashicorp-3.4.1/apache_airflow_providers_hashicorp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-hashicorp-3.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1851 2023-06-20 11:28:26.084197 apache-airflow-providers-hashicorp-3.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1701 2023-06-20 11:28:25.000000 apache-airflow-providers-hashicorp-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.318517 apache-airflow-providers-hashicorp-3.4.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:15.000000 apache-airflow-providers-hashicorp-3.4.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-hashicorp-3.4.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    13211 2023-06-20 11:42:16.319613 apache-airflow-providers-hashicorp-3.4.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11651 2023-06-20 11:42:15.000000 apache-airflow-providers-hashicorp-3.4.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.231924 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.233137 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.272212 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-20 11:01:09.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.278286 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/_internal_client/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/_internal_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20545 2023-06-01 07:44:14.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/_internal_client/vault_client.py
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-06-20 11:42:15.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.284373 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18752 2023-06-02 11:31:21.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/hooks/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.291964 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11991 2023-06-02 11:31:21.000000 apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/secrets/vault.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:16.315683 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13211 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      867 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:16.000000 apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-hashicorp-3.4.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-06-20 11:42:16.321603 apache-airflow-providers-hashicorp-3.4.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-06-20 11:42:15.000000 apache-airflow-providers-hashicorp-3.4.1rc1/setup.py
```

### Comparing `apache-airflow-providers-hashicorp-3.4.1/LICENSE` & `apache-airflow-providers-hashicorp-3.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/MANIFEST.in` & `apache-airflow-providers-hashicorp-3.4.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/PKG-INFO` & `apache-airflow-providers-hashicorp-3.4.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-hashicorp
-Version: 3.4.1
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-hashicorp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-hashicorp-3.4.1/README.rst` & `apache-airflow-providers-hashicorp-3.4.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/__init__.py` & `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/_internal_client/__init__.py` & `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/_internal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/_internal_client/vault_client.py` & `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/_internal_client/vault_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/get_provider_info.py` & `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/hooks/__init__.py` & `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/hooks/vault.py` & `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/hooks/vault.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/secrets/__init__.py` & `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/airflow/providers/hashicorp/secrets/vault.py` & `apache-airflow-providers-hashicorp-3.4.1rc1/airflow/providers/hashicorp/secrets/vault.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO` & `apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-hashicorp
-Version: 3.4.1
+Version: 3.4.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-hashicorp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-hashicorp/3.4.1/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-hashicorp``
 
-Release: ``3.4.1``
+Release: ``3.4.1rc1``
 
 
 Hashicorp including `Hashicorp Vault <https://www.vaultproject.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-hashicorp-3.4.1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt` & `apache-airflow-providers-hashicorp-3.4.1rc1/apache_airflow_providers_hashicorp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/pyproject.toml` & `apache-airflow-providers-hashicorp-3.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-hashicorp-3.4.1/setup.cfg` & `apache-airflow-providers-hashicorp-3.4.1rc1/setup.cfg`

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
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	hvac>=0.10
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.hashicorp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.hashicorp
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-hashicorp-3.4.1/setup.py` & `apache-airflow-providers-hashicorp-3.4.1rc1/setup.py`

 * *Files identical despite different names*

