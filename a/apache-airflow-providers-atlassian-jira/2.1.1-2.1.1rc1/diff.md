# Comparing `tmp/apache-airflow-providers-atlassian-jira-2.1.1.tar.gz` & `tmp/apache-airflow-providers-atlassian-jira-2.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-atlassian-jira-2.1.1.tar", last modified: Tue Jun 20 11:27:46 2023, max compression
+gzip compressed data, was "apache-airflow-providers-atlassian-jira-2.1.1rc1.tar", last modified: Tue Jun 20 11:41:37 2023, max compression
```

## Comparing `apache-airflow-providers-atlassian-jira-2.1.1.tar` & `apache-airflow-providers-atlassian-jira-2.1.1rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:46.958300 apache-airflow-providers-atlassian-jira-2.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-atlassian-jira-2.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:45.000000 apache-airflow-providers-atlassian-jira-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-atlassian-jira-2.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7347 2023-06-20 11:27:46.958870 apache-airflow-providers-atlassian-jira-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5798 2023-06-20 11:27:45.000000 apache-airflow-providers-atlassian-jira-2.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:46.874905 apache-airflow-providers-atlassian-jira-2.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:46.876198 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:46.877281 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:46.913000 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/
--rw-r--r--   0 root         (0) root         (0)     1539 2023-06-20 11:01:09.000000 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2530 2023-06-20 11:27:45.000000 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:46.918811 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2546 2023-06-02 11:31:21.000000 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/hooks/jira.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:46.924353 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3710 2023-06-17 16:45:00.000000 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/operators/jira.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:46.931965 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5194 2023-06-01 06:14:28.000000 apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/sensors/jira.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:46.955959 apache-airflow-providers-atlassian-jira-2.1.1/apache_airflow_providers_atlassian_jira.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7347 2023-06-20 11:27:46.000000 apache-airflow-providers-atlassian-jira-2.1.1/apache_airflow_providers_atlassian_jira.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      918 2023-06-20 11:27:46.000000 apache-airflow-providers-atlassian-jira-2.1.1/apache_airflow_providers_atlassian_jira.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:46.000000 apache-airflow-providers-atlassian-jira-2.1.1/apache_airflow_providers_atlassian_jira.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-20 11:27:46.000000 apache-airflow-providers-atlassian-jira-2.1.1/apache_airflow_providers_atlassian_jira.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:46.000000 apache-airflow-providers-atlassian-jira-2.1.1/apache_airflow_providers_atlassian_jira.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-20 11:27:46.000000 apache-airflow-providers-atlassian-jira-2.1.1/apache_airflow_providers_atlassian_jira.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:46.000000 apache-airflow-providers-atlassian-jira-2.1.1/apache_airflow_providers_atlassian_jira.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-atlassian-jira-2.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1899 2023-06-20 11:27:46.960697 apache-airflow-providers-atlassian-jira-2.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1686 2023-06-20 11:27:45.000000 apache-airflow-providers-atlassian-jira-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:37.399703 apache-airflow-providers-atlassian-jira-2.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:36.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     7353 2023-06-20 11:41:37.400505 apache-airflow-providers-atlassian-jira-2.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5801 2023-06-20 11:41:36.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:37.270682 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:37.272232 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:37.273705 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:37.328509 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-06-20 11:01:09.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-06-20 11:41:36.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:37.337739 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2023-06-02 11:31:21.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/hooks/jira.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:37.347497 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-06-17 16:45:00.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/operators/jira.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:37.356894 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5194 2023-06-01 06:14:28.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/sensors/jira.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:37.396088 apache-airflow-providers-atlassian-jira-2.1.1rc1/apache_airflow_providers_atlassian_jira.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7353 2023-06-20 11:41:37.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/apache_airflow_providers_atlassian_jira.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      918 2023-06-20 11:41:37.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/apache_airflow_providers_atlassian_jira.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:37.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/apache_airflow_providers_atlassian_jira.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-20 11:41:37.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/apache_airflow_providers_atlassian_jira.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:37.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/apache_airflow_providers_atlassian_jira.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-20 11:41:37.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/apache_airflow_providers_atlassian_jira.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:37.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/apache_airflow_providers_atlassian_jira.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1907 2023-06-20 11:41:37.403277 apache-airflow-providers-atlassian-jira-2.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-06-20 11:41:36.000000 apache-airflow-providers-atlassian-jira-2.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/LICENSE` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/MANIFEST.in` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/PKG-INFO` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-atlassian-jira
-Version: 2.1.1
+Version: 2.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-atlassian-jira package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-atlassian-jira/2.1.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-atlassian-jira``
 
-Release: ``2.1.1``
+Release: ``2.1.1rc1``
 
 
 `Atlassian Jira <https://www.atlassian.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/README.rst` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-atlassian-jira``
 
-Release: ``2.1.1``
+Release: ``2.1.1rc1``
 
 
 `Atlassian Jira <https://www.atlassian.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/__init__.py` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/get_provider_info.py` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/hooks/__init__.py` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/hooks/jira.py` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/hooks/jira.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/operators/__init__.py` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/operators/jira.py` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/operators/jira.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/sensors/__init__.py` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/airflow/providers/atlassian/jira/sensors/jira.py` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/airflow/providers/atlassian/jira/sensors/jira.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/apache_airflow_providers_atlassian_jira.egg-info/PKG-INFO` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/apache_airflow_providers_atlassian_jira.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-atlassian-jira
-Version: 2.1.1
+Version: 2.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-atlassian-jira package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-atlassian-jira/2.1.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-atlassian-jira``
 
-Release: ``2.1.1``
+Release: ``2.1.1rc1``
 
 
 `Atlassian Jira <https://www.atlassian.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/apache_airflow_providers_atlassian_jira.egg-info/SOURCES.txt` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/apache_airflow_providers_atlassian_jira.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/pyproject.toml` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/setup.cfg` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/setup.cfg`

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
 	atlassian-python-api>=1.14.2
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.atlassian.jira.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.atlassian.jira
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-atlassian-jira-2.1.1/setup.py` & `apache-airflow-providers-atlassian-jira-2.1.1rc1/setup.py`

 * *Files identical despite different names*

