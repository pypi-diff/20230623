# Comparing `tmp/apache-airflow-providers-discord-3.3.0.tar.gz` & `tmp/apache-airflow-providers-discord-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-discord-3.3.0.tar", last modified: Tue Jun 20 11:28:03 2023, max compression
+gzip compressed data, was "apache-airflow-providers-discord-3.3.0rc1.tar", last modified: Tue Jun 20 11:41:54 2023, max compression
```

## Comparing `apache-airflow-providers-discord-3.3.0.tar` & `apache-airflow-providers-discord-3.3.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:03.629422 apache-airflow-providers-discord-3.3.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-discord-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:28:02.000000 apache-airflow-providers-discord-3.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-discord-3.3.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)    11208 2023-06-20 11:28:03.630454 apache-airflow-providers-discord-3.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9659 2023-06-20 11:28:02.000000 apache-airflow-providers-discord-3.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:03.547910 apache-airflow-providers-discord-3.3.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:03.549157 apache-airflow-providers-discord-3.3.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:03.584386 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2600 2023-06-20 11:28:02.000000 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:03.590350 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5393 2023-06-02 11:31:21.000000 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/hooks/discord_webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:03.596171 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/notifications/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-17 16:45:00.000000 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3105 2023-06-17 16:45:00.000000 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/notifications/discord.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:03.601983 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-06-02 11:31:21.000000 apache-airflow-providers-discord-3.3.0/airflow/providers/discord/operators/discord_webhook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:28:03.626399 apache-airflow-providers-discord-3.3.0/apache_airflow_providers_discord.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11208 2023-06-20 11:28:03.000000 apache-airflow-providers-discord-3.3.0/apache_airflow_providers_discord.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-06-20 11:28:03.000000 apache-airflow-providers-discord-3.3.0/apache_airflow_providers_discord.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:03.000000 apache-airflow-providers-discord-3.3.0/apache_airflow_providers_discord.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:28:03.000000 apache-airflow-providers-discord-3.3.0/apache_airflow_providers_discord.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:28:03.000000 apache-airflow-providers-discord-3.3.0/apache_airflow_providers_discord.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2023-06-20 11:28:03.000000 apache-airflow-providers-discord-3.3.0/apache_airflow_providers_discord.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:28:03.000000 apache-airflow-providers-discord-3.3.0/apache_airflow_providers_discord.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-discord-3.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1858 2023-06-20 11:28:03.632403 apache-airflow-providers-discord-3.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1685 2023-06-20 11:28:02.000000 apache-airflow-providers-discord-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:54.558033 apache-airflow-providers-discord-3.3.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-discord-3.3.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:53.000000 apache-airflow-providers-discord-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-discord-3.3.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    11214 2023-06-20 11:41:54.559062 apache-airflow-providers-discord-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9662 2023-06-20 11:41:53.000000 apache-airflow-providers-discord-3.3.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:54.474933 apache-airflow-providers-discord-3.3.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:54.476107 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:54.509839 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-06-20 11:01:09.000000 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-20 11:41:53.000000 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:54.516152 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5393 2023-06-02 11:31:21.000000 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/hooks/discord_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:54.521996 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/notifications/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-17 16:45:00.000000 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3105 2023-06-17 16:45:00.000000 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/notifications/discord.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:54.531109 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-06-02 11:31:21.000000 apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/operators/discord_webhook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:54.555394 apache-airflow-providers-discord-3.3.0rc1/apache_airflow_providers_discord.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11214 2023-06-20 11:41:54.000000 apache-airflow-providers-discord-3.3.0rc1/apache_airflow_providers_discord.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-06-20 11:41:54.000000 apache-airflow-providers-discord-3.3.0rc1/apache_airflow_providers_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:54.000000 apache-airflow-providers-discord-3.3.0rc1/apache_airflow_providers_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:41:54.000000 apache-airflow-providers-discord-3.3.0rc1/apache_airflow_providers_discord.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:54.000000 apache-airflow-providers-discord-3.3.0rc1/apache_airflow_providers_discord.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-20 11:41:54.000000 apache-airflow-providers-discord-3.3.0rc1/apache_airflow_providers_discord.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:54.000000 apache-airflow-providers-discord-3.3.0rc1/apache_airflow_providers_discord.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-discord-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-06-20 11:41:54.561032 apache-airflow-providers-discord-3.3.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-06-20 11:41:53.000000 apache-airflow-providers-discord-3.3.0rc1/setup.py
```

### Comparing `apache-airflow-providers-discord-3.3.0/LICENSE` & `apache-airflow-providers-discord-3.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/MANIFEST.in` & `apache-airflow-providers-discord-3.3.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/PKG-INFO` & `apache-airflow-providers-discord-3.3.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-discord
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-discord package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-discord/3.3.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-discord``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Discord <https://discordapp.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-discord-3.3.0/README.rst` & `apache-airflow-providers-discord-3.3.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-discord``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Discord <https://discordapp.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-discord-3.3.0/airflow/providers/discord/__init__.py` & `apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/airflow/providers/discord/get_provider_info.py` & `apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/airflow/providers/discord/hooks/__init__.py` & `apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/airflow/providers/discord/hooks/discord_webhook.py` & `apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/hooks/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/airflow/providers/discord/notifications/__init__.py` & `apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/airflow/providers/discord/notifications/discord.py` & `apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/notifications/discord.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/airflow/providers/discord/operators/__init__.py` & `apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/airflow/providers/discord/operators/discord_webhook.py` & `apache-airflow-providers-discord-3.3.0rc1/airflow/providers/discord/operators/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/apache_airflow_providers_discord.egg-info/PKG-INFO` & `apache-airflow-providers-discord-3.3.0rc1/apache_airflow_providers_discord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-discord
-Version: 3.3.0
+Version: 3.3.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-discord package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-discord/3.3.0/
@@ -49,15 +49,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-discord``
 
-Release: ``3.3.0``
+Release: ``3.3.0rc1``
 
 
 `Discord <https://discordapp.com/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-discord-3.3.0/apache_airflow_providers_discord.egg-info/SOURCES.txt` & `apache-airflow-providers-discord-3.3.0rc1/apache_airflow_providers_discord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/pyproject.toml` & `apache-airflow-providers-discord-3.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-discord-3.3.0/setup.cfg` & `apache-airflow-providers-discord-3.3.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -43,20 +43,20 @@
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-http
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.discord.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.discord
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-discord-3.3.0/setup.py` & `apache-airflow-providers-discord-3.3.0rc1/setup.py`

 * *Files identical despite different names*

