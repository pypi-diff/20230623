# Comparing `tmp/apache-airflow-providers-telegram-4.1.1.tar.gz` & `tmp/apache-airflow-providers-telegram-4.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-telegram-4.1.1.tar", last modified: Tue Jun 20 11:29:46 2023, max compression
+gzip compressed data, was "apache-airflow-providers-telegram-4.1.1rc1.tar", last modified: Tue Jun 20 11:43:25 2023, max compression
```

## Comparing `apache-airflow-providers-telegram-4.1.1.tar` & `apache-airflow-providers-telegram-4.1.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:46.068265 apache-airflow-providers-telegram-4.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:44.000000 apache-airflow-providers-telegram-4.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10995 2023-06-20 11:29:46.069413 apache-airflow-providers-telegram-4.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9464 2023-06-20 11:29:44.000000 apache-airflow-providers-telegram-4.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:45.970848 apache-airflow-providers-telegram-4.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:45.973395 apache-airflow-providers-telegram-4.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:46.014654 apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2363 2023-06-20 11:29:44.000000 apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:46.024494 apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5241 2023-06-02 11:31:21.000000 apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/hooks/telegram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:46.032302 apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3013 2023-06-02 11:31:21.000000 apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/operators/telegram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:46.065024 apache-airflow-providers-telegram-4.1.1/apache_airflow_providers_telegram.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10995 2023-06-20 11:29:45.000000 apache-airflow-providers-telegram-4.1.1/apache_airflow_providers_telegram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:29:45.000000 apache-airflow-providers-telegram-4.1.1/apache_airflow_providers_telegram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:45.000000 apache-airflow-providers-telegram-4.1.1/apache_airflow_providers_telegram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:29:45.000000 apache-airflow-providers-telegram-4.1.1/apache_airflow_providers_telegram.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:45.000000 apache-airflow-providers-telegram-4.1.1/apache_airflow_providers_telegram.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-20 11:29:45.000000 apache-airflow-providers-telegram-4.1.1/apache_airflow_providers_telegram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:45.000000 apache-airflow-providers-telegram-4.1.1/apache_airflow_providers_telegram.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-telegram-4.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1862 2023-06-20 11:29:46.072631 apache-airflow-providers-telegram-4.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:29:44.000000 apache-airflow-providers-telegram-4.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:25.100860 apache-airflow-providers-telegram-4.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11001 2023-06-20 11:43:25.102572 apache-airflow-providers-telegram-4.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9467 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:24.991067 apache-airflow-providers-telegram-4.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:24.992534 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:25.044391 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:25.051577 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5241 2023-06-02 11:31:21.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/hooks/telegram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:25.060847 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:29.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-06-02 11:31:21.000000 apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/operators/telegram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:25.096735 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11001 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-telegram-4.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-06-20 11:43:25.105507 apache-airflow-providers-telegram-4.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:43:24.000000 apache-airflow-providers-telegram-4.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-telegram-4.1.1/LICENSE` & `apache-airflow-providers-telegram-4.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.1/MANIFEST.in` & `apache-airflow-providers-telegram-4.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.1/PKG-INFO` & `apache-airflow-providers-telegram-4.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-telegram
-Version: 4.1.1
+Version: 4.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-telegram package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-telegram``
 
-Release: ``4.1.1``
+Release: ``4.1.1rc1``
 
 
 `Telegram <https://telegram.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-telegram-4.1.1/README.rst` & `apache-airflow-providers-telegram-4.1.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-telegram``
 
-Release: ``4.1.1``
+Release: ``4.1.1rc1``
 
 
 `Telegram <https://telegram.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/__init__.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/get_provider_info.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/hooks/__init__.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/hooks/telegram.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/hooks/telegram.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/operators/__init__.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.1/airflow/providers/telegram/operators/telegram.py` & `apache-airflow-providers-telegram-4.1.1rc1/airflow/providers/telegram/operators/telegram.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.1/apache_airflow_providers_telegram.egg-info/PKG-INFO` & `apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-telegram
-Version: 4.1.1
+Version: 4.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-telegram package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-telegram/4.1.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-telegram``
 
-Release: ``4.1.1``
+Release: ``4.1.1rc1``
 
 
 `Telegram <https://telegram.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-telegram-4.1.1/apache_airflow_providers_telegram.egg-info/SOURCES.txt` & `apache-airflow-providers-telegram-4.1.1rc1/apache_airflow_providers_telegram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.1/pyproject.toml` & `apache-airflow-providers-telegram-4.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-telegram-4.1.1/setup.cfg` & `apache-airflow-providers-telegram-4.1.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

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
 	python-telegram-bot>=20.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.telegram.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.telegram
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-telegram-4.1.1/setup.py` & `apache-airflow-providers-telegram-4.1.1rc1/setup.py`

 * *Files identical despite different names*

