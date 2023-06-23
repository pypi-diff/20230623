# Comparing `tmp/apache-airflow-providers-apache-kafka-1.1.1.tar.gz` & `tmp/apache-airflow-providers-apache-kafka-1.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-apache-kafka-1.1.1.tar", last modified: Tue Jun 20 11:27:30 2023, max compression
+gzip compressed data, was "apache-airflow-providers-apache-kafka-1.1.1rc1.tar", last modified: Tue Jun 20 11:41:21 2023, max compression
```

## Comparing `apache-airflow-providers-apache-kafka-1.1.1.tar` & `apache-airflow-providers-apache-kafka-1.1.1rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:30.448065 apache-airflow-providers-apache-kafka-1.1.1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:27:29.000000 apache-airflow-providers-apache-kafka-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5931 2023-06-20 11:27:30.448621 apache-airflow-providers-apache-kafka-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4388 2023-06-20 11:27:29.000000 apache-airflow-providers-apache-kafka-1.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:30.348816 apache-airflow-providers-apache-kafka-1.1.1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:30.350501 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:30.352157 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:30.387147 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-06-20 11:27:29.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:30.401326 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/hooks/base.py
--rw-r--r--   0 root         (0) root         (0)     2353 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/hooks/client.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/hooks/consume.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/hooks/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:30.410237 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8020 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/operators/consume.py
--rw-r--r--   0 root         (0) root         (0)     4951 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/operators/produce.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:30.416067 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8272 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/sensors/kafka.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:30.421877 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/triggers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4914 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/triggers/await_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:27:30.445367 apache-airflow-providers-apache-kafka-1.1.1/apache_airflow_providers_apache_kafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5931 2023-06-20 11:27:30.000000 apache-airflow-providers-apache-kafka-1.1.1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1196 2023-06-20 11:27:30.000000 apache-airflow-providers-apache-kafka-1.1.1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:30.000000 apache-airflow-providers-apache-kafka-1.1.1/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:27:30.000000 apache-airflow-providers-apache-kafka-1.1.1/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:27:30.000000 apache-airflow-providers-apache-kafka-1.1.1/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-20 11:27:30.000000 apache-airflow-providers-apache-kafka-1.1.1/apache_airflow_providers_apache_kafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:27:30.000000 apache-airflow-providers-apache-kafka-1.1.1/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-kafka-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1890 2023-06-20 11:27:30.450481 apache-airflow-providers-apache-kafka-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:27:29.000000 apache-airflow-providers-apache-kafka-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.234331 apache-airflow-providers-apache-kafka-1.1.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5937 2023-06-20 11:41:21.234885 apache-airflow-providers-apache-kafka-1.1.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.137110 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.138409 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.139745 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.174605 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/
+-rw-r--r--   0 root         (0) root         (0)     1537 2023-06-20 11:01:09.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.188594 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/base.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/client.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/consume.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.197120 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8020 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/consume.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/produce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.202842 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8272 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/kafka.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.208920 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4914 2023-06-01 07:44:14.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/await_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:21.232008 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5937 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:21.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-06-20 11:41:21.236883 apache-airflow-providers-apache-kafka-1.1.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 11:41:20.000000 apache-airflow-providers-apache-kafka-1.1.1rc1/setup.py
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/LICENSE` & `apache-airflow-providers-apache-kafka-1.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/MANIFEST.in` & `apache-airflow-providers-apache-kafka-1.1.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/PKG-INFO` & `apache-airflow-providers-apache-kafka-1.1.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kafka
-Version: 1.1.1
+Version: 1.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kafka package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.1``
+Release: ``1.1.1rc1``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/README.rst` & `apache-airflow-providers-apache-kafka-1.1.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.1``
+Release: ``1.1.1rc1``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/get_provider_info.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/hooks/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/hooks/base.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/hooks/client.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/hooks/consume.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/consume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/hooks/produce.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/hooks/produce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/operators/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/operators/consume.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/consume.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/operators/produce.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/operators/produce.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/sensors/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/sensors/kafka.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/sensors/kafka.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/triggers/__init__.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/airflow/providers/apache/kafka/triggers/await_message.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/airflow/providers/apache/kafka/triggers/await_message.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO` & `apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-apache-kafka
-Version: 1.1.1
+Version: 1.1.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-apache-kafka package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-apache-kafka/1.1.1/
@@ -48,15 +48,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-apache-kafka``
 
-Release: ``1.1.1``
+Release: ``1.1.1rc1``
 
 
 `Apache Kafka  <https://kafka.apache.org/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt` & `apache-airflow-providers-apache-kafka-1.1.1rc1/apache_airflow_providers_apache_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/pyproject.toml` & `apache-airflow-providers-apache-kafka-1.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/setup.cfg` & `apache-airflow-providers-apache-kafka-1.1.1rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	asgiref
 	confluent-kafka>=1.8.2
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.apache.kafka.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.apache.kafka
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-apache-kafka-1.1.1/setup.py` & `apache-airflow-providers-apache-kafka-1.1.1rc1/setup.py`

 * *Files identical despite different names*

