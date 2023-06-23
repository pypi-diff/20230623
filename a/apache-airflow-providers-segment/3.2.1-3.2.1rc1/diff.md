# Comparing `tmp/apache-airflow-providers-segment-3.2.1.tar.gz` & `tmp/apache-airflow-providers-segment-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-segment-3.2.1.tar", last modified: Tue Jun 20 11:29:23 2023, max compression
+gzip compressed data, was "apache-airflow-providers-segment-3.2.1rc1.tar", last modified: Tue Jun 20 11:43:05 2023, max compression
```

## Comparing `apache-airflow-providers-segment-3.2.1.tar` & `apache-airflow-providers-segment-3.2.1rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:23.524805 apache-airflow-providers-segment-3.2.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-segment-3.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:29:22.000000 apache-airflow-providers-segment-3.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-segment-3.2.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9976 2023-06-20 11:29:23.526228 apache-airflow-providers-segment-3.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8448 2023-06-20 11:29:22.000000 apache-airflow-providers-segment-3.2.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:23.415786 apache-airflow-providers-segment-3.2.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:23.417089 apache-airflow-providers-segment-3.2.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:23.467079 apache-airflow-providers-segment-3.2.1/airflow/providers/segment/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-segment-3.2.1/airflow/providers/segment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2413 2023-06-20 11:29:22.000000 apache-airflow-providers-segment-3.2.1/airflow/providers/segment/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:23.476381 apache-airflow-providers-segment-3.2.1/airflow/providers/segment/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-segment-3.2.1/airflow/providers/segment/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-06-02 11:31:21.000000 apache-airflow-providers-segment-3.2.1/airflow/providers/segment/hooks/segment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:23.485231 apache-airflow-providers-segment-3.2.1/airflow/providers/segment/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-segment-3.2.1/airflow/providers/segment/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2646 2023-06-02 11:31:21.000000 apache-airflow-providers-segment-3.2.1/airflow/providers/segment/operators/segment_track_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:29:23.520724 apache-airflow-providers-segment-3.2.1/apache_airflow_providers_segment.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9976 2023-06-20 11:29:23.000000 apache-airflow-providers-segment-3.2.1/apache_airflow_providers_segment.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-20 11:29:23.000000 apache-airflow-providers-segment-3.2.1/apache_airflow_providers_segment.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:23.000000 apache-airflow-providers-segment-3.2.1/apache_airflow_providers_segment.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:29:23.000000 apache-airflow-providers-segment-3.2.1/apache_airflow_providers_segment.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:29:23.000000 apache-airflow-providers-segment-3.2.1/apache_airflow_providers_segment.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-20 11:29:23.000000 apache-airflow-providers-segment-3.2.1/apache_airflow_providers_segment.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:29:23.000000 apache-airflow-providers-segment-3.2.1/apache_airflow_providers_segment.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-segment-3.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1852 2023-06-20 11:29:23.528859 apache-airflow-providers-segment-3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:29:22.000000 apache-airflow-providers-segment-3.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:05.007316 apache-airflow-providers-segment-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-segment-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:03.000000 apache-airflow-providers-segment-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-segment-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9982 2023-06-20 11:43:05.008371 apache-airflow-providers-segment-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8451 2023-06-20 11:43:03.000000 apache-airflow-providers-segment-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:04.928049 apache-airflow-providers-segment-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:04.929448 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:04.964288 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-06-20 11:43:03.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:04.971002 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-06-02 11:31:21.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/hooks/segment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:04.977768 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2646 2023-06-02 11:31:21.000000 apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/operators/segment_track_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:05.004501 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9982 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:04.000000 apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-segment-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-06-20 11:43:05.010340 apache-airflow-providers-segment-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-20 11:43:03.000000 apache-airflow-providers-segment-3.2.1rc1/setup.py
```

### Comparing `apache-airflow-providers-segment-3.2.1/LICENSE` & `apache-airflow-providers-segment-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.1/MANIFEST.in` & `apache-airflow-providers-segment-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.1/PKG-INFO` & `apache-airflow-providers-segment-3.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-segment
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-segment package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-segment``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Segment <https://segment.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-segment-3.2.1/README.rst` & `apache-airflow-providers-segment-3.2.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-segment``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Segment <https://segment.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-segment-3.2.1/airflow/providers/segment/__init__.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.1/airflow/providers/segment/get_provider_info.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.1/airflow/providers/segment/hooks/__init__.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.1/airflow/providers/segment/hooks/segment.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/hooks/segment.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.1/airflow/providers/segment/operators/__init__.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.1/airflow/providers/segment/operators/segment_track_event.py` & `apache-airflow-providers-segment-3.2.1rc1/airflow/providers/segment/operators/segment_track_event.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.1/apache_airflow_providers_segment.egg-info/PKG-INFO` & `apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-segment
-Version: 3.2.1
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-segment package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-segment/3.2.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-segment``
 
-Release: ``3.2.1``
+Release: ``3.2.1rc1``
 
 
 `Segment <https://segment.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-segment-3.2.1/apache_airflow_providers_segment.egg-info/SOURCES.txt` & `apache-airflow-providers-segment-3.2.1rc1/apache_airflow_providers_segment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.1/pyproject.toml` & `apache-airflow-providers-segment-3.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-segment-3.2.1/setup.cfg` & `apache-airflow-providers-segment-3.2.1rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	analytics-python>=1.2.9
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.segment.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.segment
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-segment-3.2.1/setup.py` & `apache-airflow-providers-segment-3.2.1rc1/setup.py`

 * *Files identical despite different names*

