# Comparing `tmp/apache-airflow-providers-jenkins-3.3.1.tar.gz` & `tmp/apache-airflow-providers-jenkins-3.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-jenkins-3.3.1.tar", last modified: Tue Jun 20 11:28:35 2023, max compression
+gzip compressed data, was "apache-airflow-providers-jenkins-3.3.1rc1.tar", last modified: Tue Jun 20 11:42:25 2023, max compression
```

## Comparing `apache-airflow-providers-jenkins-3.3.1.tar` & `apache-airflow-providers-jenkins-3.3.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:35.916242 apache-airflow-providers-jenkins-3.3.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-jenkins-3.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:34.000000 apache-airflow-providers-jenkins-3.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-jenkins-3.3.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11706 2023-06-20 11:28:35.917332 apache-airflow-providers-jenkins-3.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10178 2023-06-20 11:28:34.000000 apache-airflow-providers-jenkins-3.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:35.810968 apache-airflow-providers-jenkins-3.3.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:35.812169 apache-airflow-providers-jenkins-3.3.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:35.859671 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-06-20 11:28:34.000000 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:35.867411 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-06-02 11:31:21.000000 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/hooks/jenkins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:35.874075 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10539 2023-06-05 12:50:36.000000 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/operators/jenkins_job_trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:35.881020 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2802 2023-06-05 12:50:36.000000 apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/sensors/jenkins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:35.913212 apache-airflow-providers-jenkins-3.3.1/apache_airflow_providers_jenkins.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11706 2023-06-20 11:28:35.000000 apache-airflow-providers-jenkins-3.3.1/apache_airflow_providers_jenkins.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      834 2023-06-20 11:28:35.000000 apache-airflow-providers-jenkins-3.3.1/apache_airflow_providers_jenkins.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:35.000000 apache-airflow-providers-jenkins-3.3.1/apache_airflow_providers_jenkins.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:28:35.000000 apache-airflow-providers-jenkins-3.3.1/apache_airflow_providers_jenkins.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:35.000000 apache-airflow-providers-jenkins-3.3.1/apache_airflow_providers_jenkins.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-20 11:28:35.000000 apache-airflow-providers-jenkins-3.3.1/apache_airflow_providers_jenkins.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:35.000000 apache-airflow-providers-jenkins-3.3.1/apache_airflow_providers_jenkins.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-jenkins-3.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1850 2023-06-20 11:28:35.919494 apache-airflow-providers-jenkins-3.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:28:34.000000 apache-airflow-providers-jenkins-3.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.776960 apache-airflow-providers-jenkins-3.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-jenkins-3.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:24.000000 apache-airflow-providers-jenkins-3.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-jenkins-3.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11712 2023-06-20 11:42:25.779160 apache-airflow-providers-jenkins-3.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10181 2023-06-20 11:42:24.000000 apache-airflow-providers-jenkins-3.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.687090 apache-airflow-providers-jenkins-3.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.688352 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.723106 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2023-06-20 11:42:24.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.729694 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-06-02 11:31:21.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/hooks/jenkins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.737257 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10539 2023-06-05 12:50:36.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/operators/jenkins_job_trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.745170 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2802 2023-06-05 12:50:36.000000 apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/sensors/jenkins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:25.774296 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11712 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      834 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:25.000000 apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-jenkins-3.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-06-20 11:42:25.781616 apache-airflow-providers-jenkins-3.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:42:24.000000 apache-airflow-providers-jenkins-3.3.1rc1/setup.py
```

### Comparing `apache-airflow-providers-jenkins-3.3.1/LICENSE` & `apache-airflow-providers-jenkins-3.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/MANIFEST.in` & `apache-airflow-providers-jenkins-3.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/PKG-INFO` & `apache-airflow-providers-jenkins-3.3.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jenkins
-Version: 3.3.1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jenkins package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-jenkins``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Jenkins <https://jenkins.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-jenkins-3.3.1/README.rst` & `apache-airflow-providers-jenkins-3.3.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-jenkins``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Jenkins <https://jenkins.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/__init__.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/get_provider_info.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/hooks/__init__.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/hooks/jenkins.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/hooks/jenkins.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/operators/__init__.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/operators/jenkins_job_trigger.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/operators/jenkins_job_trigger.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/sensors/__init__.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/airflow/providers/jenkins/sensors/jenkins.py` & `apache-airflow-providers-jenkins-3.3.1rc1/airflow/providers/jenkins/sensors/jenkins.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/apache_airflow_providers_jenkins.egg-info/PKG-INFO` & `apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-jenkins
-Version: 3.3.1
+Version: 3.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-jenkins package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-jenkins/3.3.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-jenkins``
 
-Release: ``3.3.1``
+Release: ``3.3.1rc1``
 
 
 `Jenkins <https://jenkins.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-jenkins-3.3.1/apache_airflow_providers_jenkins.egg-info/SOURCES.txt` & `apache-airflow-providers-jenkins-3.3.1rc1/apache_airflow_providers_jenkins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/pyproject.toml` & `apache-airflow-providers-jenkins-3.3.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-jenkins-3.3.1/setup.cfg` & `apache-airflow-providers-jenkins-3.3.1rc1/setup.cfg`

 * *Files 9% similar despite different names*

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
 	python-jenkins>=1.0.0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.jenkins.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.jenkins
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-jenkins-3.3.1/setup.py` & `apache-airflow-providers-jenkins-3.3.1rc1/setup.py`

 * *Files identical despite different names*

