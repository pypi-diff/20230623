# Comparing `tmp/apache-airflow-providers-sftp-4.3.0rc2.tar.gz` & `tmp/apache-airflow-providers-sftp-4.3.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-sftp-4.3.0rc2.tar", last modified: Fri May 19 17:53:28 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sftp-4.3.1rc1.tar", last modified: Tue Jun 20 11:43:08 2023, max compression
```

## Comparing `apache-airflow-providers-sftp-4.3.0rc2.tar` & `apache-airflow-providers-sftp-4.3.1rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-sftp-4.3.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:53:27.000000 apache-airflow-providers-sftp-4.3.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-sftp-4.3.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    13997 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12456 2023-05-19 17:53:27.000000 apache-airflow-providers-sftp-4.3.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-05-19 12:21:23.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3034 2023-05-19 17:53:27.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14735 2023-05-03 19:47:07.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/hooks/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8460 2023-05-03 19:47:07.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/operators/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3543 2023-03-01 07:06:45.000000 apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/sensors/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/apache_airflow_providers_sftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13997 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/apache_airflow_providers_sftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      768 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/apache_airflow_providers_sftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/apache_airflow_providers_sftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/apache_airflow_providers_sftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/apache_airflow_providers_sftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/apache_airflow_providers_sftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/apache_airflow_providers_sftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-sftp-4.3.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1858 2023-05-19 17:53:28.000000 apache-airflow-providers-sftp-4.3.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1665 2023-05-19 17:53:27.000000 apache-airflow-providers-sftp-4.3.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.517921 apache-airflow-providers-sftp-4.3.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.3.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:43:07.000000 apache-airflow-providers-sftp-4.3.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.3.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    14383 2023-06-20 11:43:08.518966 apache-airflow-providers-sftp-4.3.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12841 2023-06-20 11:43:07.000000 apache-airflow-providers-sftp-4.3.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.433826 apache-airflow-providers-sftp-4.3.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.434921 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.468802 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-06-20 11:01:09.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-06-20 11:43:07.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.474511 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14745 2023-06-05 12:50:36.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/hooks/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.481711 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8461 2023-06-02 11:31:21.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/operators/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.490618 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3543 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/sensors/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:43:08.515320 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14383 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      768 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:43:08.000000 apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-sftp-4.3.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-06-20 11:43:08.521036 apache-airflow-providers-sftp-4.3.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-06-20 11:43:07.000000 apache-airflow-providers-sftp-4.3.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/LICENSE` & `apache-airflow-providers-sftp-4.3.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/MANIFEST.in` & `apache-airflow-providers-sftp-4.3.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/PKG-INFO` & `apache-airflow-providers-sftp-4.3.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sftp
-Version: 4.3.0rc2
+Version: 4.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: ssh
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -49,38 +49,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.3.0rc2``
+Release: ``4.3.1rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sftp`` provider. All classes for this provider package
 are in ``airflow.providers.sftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-sftp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ================================  ==================
 PIP package                       Version required
 ================================  ==================
@@ -129,14 +129,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.3.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 4.3.0
 .....
 
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/README.rst` & `apache-airflow-providers-sftp-4.3.1rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.3.0rc2``
+Release: ``4.3.1rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sftp`` provider. All classes for this provider package
 are in ``airflow.providers.sftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-sftp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ================================  ==================
 PIP package                       Version required
 ================================  ==================
@@ -95,14 +95,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.3.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 4.3.0
 .....
 
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/__init__.py` & `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "4.3.0"
+__version__ = "4.3.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/get_provider_info.py` & `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-sftp",
         "name": "SFTP",
         "description": "`SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__\n",
         "suspended": False,
         "versions": [
+            "4.3.1",
             "4.3.0",
             "4.2.4",
             "4.2.3",
             "4.2.2",
             "4.2.1",
             "4.2.0",
             "4.1.0",
```

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/hooks/__init__.py` & `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/hooks/sftp.py` & `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/hooks/sftp.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,19 +28,18 @@
 import paramiko
 
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.providers.ssh.hooks.ssh import SSHHook
 
 
 class SFTPHook(SSHHook):
-    """
-    This hook is inherited from SSH hook. Please refer to SSH hook for the input
-    arguments.
+    """Interact with SFTP.
 
-    Interact with SFTP.
+    This hook inherits the SSH hook. Please refer to SSH hook for the input
+    arguments.
 
     :Pitfalls::
 
         - In contrast with FTPHook describe_directory only returns size, type and
           modify. It doesn't return unix.owner, unix.mode, perm, unix.group and
           unique.
         - retrieve_file and store_file only take a local full path and not a
@@ -107,33 +106,34 @@
 
         kwargs["ssh_conn_id"] = ssh_conn_id
         self.ssh_conn_id = ssh_conn_id
 
         super().__init__(*args, **kwargs)
 
     def get_conn(self) -> paramiko.SFTPClient:  # type: ignore[override]
-        """Opens an SFTP connection to the remote host"""
+        """Opens an SFTP connection to the remote host."""
         if self.conn is None:
             # TODO: remove support for ssh_hook when it is removed from SFTPOperator
             if self.ssh_hook is not None:
                 self.conn = self.ssh_hook.get_conn().open_sftp()
             else:
                 self.conn = super().get_conn().open_sftp()
         return self.conn
 
     def close_conn(self) -> None:
-        """Closes the SFTP connection"""
+        """Closes the SFTP connection."""
         if self.conn is not None:
             self.conn.close()
             self.conn = None
 
     def describe_directory(self, path: str) -> dict[str, dict[str, str | int | None]]:
-        """
-        Returns a dictionary of {filename: {attributes}} for all files
-        on the remote system (where the MLSD command is supported).
+        """Get file information in a directory on the remote system.
+
+        The return format is ``{filename: {attributes}}``. The remote system
+        support the MLSD command.
 
         :param path: full path to the remote directory
         """
         conn = self.get_conn()
         flist = sorted(conn.listdir_attr(path), key=lambda x: x.filename)
         files = {}
         for f in flist:
@@ -142,64 +142,65 @@
                 "size": f.st_size,
                 "type": "dir" if stat.S_ISDIR(f.st_mode) else "file",  # type: ignore
                 "modify": modify,
             }
         return files
 
     def list_directory(self, path: str) -> list[str]:
-        """
-        Returns a list of files on the remote system.
+        """List files in a directory on the remote system.
 
         :param path: full path to the remote directory to list
         """
         conn = self.get_conn()
         files = sorted(conn.listdir(path))
         return files
 
     def mkdir(self, path: str, mode: int = 0o777) -> None:
-        """
-        Creates a directory on the remote system.
-        The default mode is 0777, but on some systems, the current umask value is first masked out.
+        """Create a directory on the remote system.
+
+        The default mode is ``0o777``, but on some systems, the current umask
+        value may be first masked out.
 
         :param path: full path to the remote directory to create
         :param mode: int permissions of octal mode for directory
         """
         conn = self.get_conn()
         conn.mkdir(path, mode=mode)
 
     def isdir(self, path: str) -> bool:
-        """
-        Checks if the path provided is a directory or not.
+        """Check if the path provided is a directory.
 
         :param path: full path to the remote directory to check
         """
         conn = self.get_conn()
         try:
             result = stat.S_ISDIR(conn.stat(path).st_mode)  # type: ignore
         except OSError:
             result = False
         return result
 
     def isfile(self, path: str) -> bool:
-        """
-        Checks if the path provided is a file or not.
+        """Check if the path provided is a file.
 
         :param path: full path to the remote file to check
         """
         conn = self.get_conn()
         try:
             result = stat.S_ISREG(conn.stat(path).st_mode)  # type: ignore
         except OSError:
             result = False
         return result
 
     def create_directory(self, path: str, mode: int = 0o777) -> None:
-        """
-        Creates a directory on the remote system.
-        The default mode is 0777, but on some systems, the current umask value is first masked out.
+        """Create a directory on the remote system.
+
+        The default mode is ``0o777``, but on some systems, the current umask
+        value may be first masked out. Different from :func:`.mkdir`, this
+        function attempts to create parent directories if needed, and returns
+        silently if the target directory already exists.
 
         :param path: full path to the remote directory to create
         :param mode: int permissions of octal mode for directory
         """
         conn = self.get_conn()
         if self.isdir(path):
             self.log.info("%s already exists", path)
@@ -211,82 +212,77 @@
             if dirname and not self.isdir(dirname):
                 self.create_directory(dirname, mode)
             if basename:
                 self.log.info("Creating %s", path)
                 conn.mkdir(path, mode=mode)
 
     def delete_directory(self, path: str) -> None:
-        """
-        Deletes a directory on the remote system.
+        """Delete a directory on the remote system.
 
         :param path: full path to the remote directory to delete
         """
         conn = self.get_conn()
         conn.rmdir(path)
 
     def retrieve_file(self, remote_full_path: str, local_full_path: str) -> None:
-        """
-        Transfers the remote file to a local location.
+        """Transfer the remote file to a local location.
+
         If local_full_path is a string path, the file will be put
-        at that location
+        at that location.
 
         :param remote_full_path: full path to the remote file
         :param local_full_path: full path to the local file
         """
         conn = self.get_conn()
         conn.get(remote_full_path, local_full_path)
 
     def store_file(self, remote_full_path: str, local_full_path: str, confirm: bool = True) -> None:
-        """
-        Transfers a local file to the remote location.
+        """Transfer a local file to the remote location.
+
         If local_full_path_or_buffer is a string path, the file will be read
-        from that location
+        from that location.
 
         :param remote_full_path: full path to the remote file
         :param local_full_path: full path to the local file
         """
         conn = self.get_conn()
         conn.put(local_full_path, remote_full_path, confirm=confirm)
 
     def delete_file(self, path: str) -> None:
-        """
-        Removes a file on the FTP Server
+        """Remove a file on the server.
 
         :param path: full path to the remote file
         """
         conn = self.get_conn()
         conn.remove(path)
 
     def get_mod_time(self, path: str) -> str:
-        """
-        Returns modification time.
+        """Get an entry's modification time.
 
         :param path: full path to the remote file
         """
         conn = self.get_conn()
         ftp_mdtm = conn.stat(path).st_mtime
         return datetime.datetime.fromtimestamp(ftp_mdtm).strftime("%Y%m%d%H%M%S")  # type: ignore
 
     def path_exists(self, path: str) -> bool:
-        """
-        Returns True if a remote entity exists
+        """Whether a remote entity exists.
 
         :param path: full path to the remote file or directory
         """
         conn = self.get_conn()
         try:
             conn.stat(path)
         except OSError:
             return False
         return True
 
     @staticmethod
     def _is_path_match(path: str, prefix: str | None = None, delimiter: str | None = None) -> bool:
-        """
-        Return True if given path starts with prefix (if set) and ends with delimiter (if set).
+        """Whether given path starts with ``prefix`` (if set) and ends with ``delimiter`` (if set).
 
         :param path: path to be checked
         :param prefix: if set path will be checked is starting with prefix
         :param delimiter: if set path will be checked is ending with suffix
         :return: bool
         """
         if prefix is not None and not path.startswith(prefix):
@@ -299,33 +295,31 @@
         self,
         path: str,
         fcallback: Callable[[str], Any | None],
         dcallback: Callable[[str], Any | None],
         ucallback: Callable[[str], Any | None],
         recurse: bool = True,
     ) -> None:
-        """
-        Recursively descend, depth first, the directory tree rooted at
-        path, calling discrete callback functions for each regular file,
-        directory and unknown file type.
+        """Recursively descend, depth first, the directory tree at ``path``.
+
+        This calls discrete callback functions for each regular file, directory,
+        and unknown file type.
 
         :param str path:
             root of remote directory to descend, use '.' to start at
             :attr:`.pwd`
         :param callable fcallback:
             callback function to invoke for a regular file.
             (form: ``func(str)``)
         :param callable dcallback:
             callback function to invoke for a directory. (form: ``func(str)``)
         :param callable ucallback:
             callback function to invoke for an unknown file type.
             (form: ``func(str)``)
         :param bool recurse: *Default: True* - should it recurse
-
-        :returns: None
         """
         conn = self.get_conn()
         for entry in self.list_directory(path):
             pathname = os.path.join(path, entry)
             mode = conn.stat(pathname).st_mode
             if stat.S_ISDIR(mode):  # type: ignore
                 # It's a directory, call the dcallback function
@@ -339,16 +333,16 @@
             else:
                 # Unknown file type
                 ucallback(pathname)
 
     def get_tree_map(
         self, path: str, prefix: str | None = None, delimiter: str | None = None
     ) -> tuple[list[str], list[str], list[str]]:
-        """
-        Return tuple with recursive lists of files, directories and unknown paths from given path.
+        """Get tuple with recursive lists of files, directories and unknown paths.
+
         It is possible to filter results by giving prefix and/or delimiter parameters.
 
         :param path: path from which tree will be built
         :param prefix: if set paths will be added if start with prefix
         :param delimiter: if set paths will be added if end with delimiter
         :return: tuple with list of files, dirs and unknown items
         """
@@ -366,39 +360,37 @@
             ucallback=append_matching_path_callback(unknowns),
             recurse=True,
         )
 
         return files, dirs, unknowns
 
     def test_connection(self) -> tuple[bool, str]:
-        """Test the SFTP connection by calling path with directory"""
+        """Test the SFTP connection by calling path with directory."""
         try:
             conn = self.get_conn()
             conn.normalize(".")
             return True, "Connection successfully tested"
         except Exception as e:
             return False, str(e)
 
     def get_file_by_pattern(self, path, fnmatch_pattern) -> str:
-        """
-        Returning the first matching file based on the given fnmatch type pattern
+        """Get the first matching file based on the given fnmatch type pattern.
 
         :param path: path to be checked
         :param fnmatch_pattern: The pattern that will be matched with `fnmatch`
         :return: string containing the first found file, or an empty string if none matched
         """
         for file in self.list_directory(path):
             if fnmatch(file, fnmatch_pattern):
                 return file
 
         return ""
 
     def get_files_by_pattern(self, path, fnmatch_pattern) -> list[str]:
-        """
-        Returning the list of matching files based on the given fnmatch type pattern
+        """Get all matching files based on the given fnmatch type pattern.
 
         :param path: path to be checked
         :param fnmatch_pattern: The pattern that will be matched with `fnmatch`
         :return: list of string containing the found files, or an empty list if none matched
         """
         matched_files = []
         for file in self.list_directory(path):
```

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/operators/__init__.py` & `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/operators/sftp.py` & `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/operators/sftp.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from airflow.exceptions import AirflowException, AirflowProviderDeprecationWarning
 from airflow.models import BaseOperator
 from airflow.providers.sftp.hooks.sftp import SFTPHook
 from airflow.providers.ssh.hooks.ssh import SSHHook
 
 
 class SFTPOperation:
-    """Operation that can be used with SFTP"""
+    """Operation that can be used with SFTP."""
 
     PUT = "put"
     GET = "get"
 
 
 class SFTPOperator(BaseOperator):
     """
```

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/sensors/__init__.py` & `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/airflow/providers/sftp/sensors/sftp.py` & `apache-airflow-providers-sftp-4.3.1rc1/airflow/providers/sftp/sensors/sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/apache_airflow_providers_sftp.egg-info/PKG-INFO` & `apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sftp
-Version: 4.3.0rc2
+Version: 4.3.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.1/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: ssh
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
@@ -49,38 +49,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.3.0rc2``
+Release: ``4.3.1rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``sftp`` provider. All classes for this provider package
 are in ``airflow.providers.sftp`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-sftp``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 ================================  ==================
 PIP package                       Version required
 ================================  ==================
@@ -129,14 +129,30 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+4.3.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Add note about dropping Python 3.7 for providers (#32015)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+
 4.3.0
 .....
 
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/apache_airflow_providers_sftp.egg-info/SOURCES.txt` & `apache-airflow-providers-sftp-4.3.1rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/pyproject.toml` & `apache-airflow-providers-sftp-4.3.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,42 +22,43 @@
 # and we have to pin it to 63.4.3 version
 # The problem is tracked (and this limitation might be removed if it is solved) in:
 # https://github.com/pypa/setuptools/issues/3548
 [build-system]
 requires = ['setuptools==67.2.0']
 build-backend = "setuptools.build_meta"
 
+[project]
+requires-python = ">=3.8"
+
 [tool.ruff]
 typing-modules = ["airflow.typing_compat"]
 line-length = 110
 extend-exclude = [
     ".eggs",
     "airflow/_vendor/*",
     "airflow/providers/google/ads/_vendor/*",
     # The files generated by stubgen aren't 100% valid syntax it turns out, and we don't ship them, so we can
     # ignore them in ruff
-    "airflow/providers/common/sql/*/*.pyi"
+    "airflow/providers/common/sql/*/*.pyi",
+    "airflow/migrations/versions/*.py"
 ]
 
-# TODO: Bump to Python 3.8 when support for Python 3.7 is dropped in Airflow.
-target-version = "py37"
-
 extend-select = [
     "I", # Missing required import (auto-fixable)
     "UP", # Pyupgrade
     "RUF100", # Unused noqa (auto-fixable)
 
     # implicit single-line string concatenation
     "ISC001",
     # We ignore more pydocstyle than we enable, so be more selective at what we enable
     "D101",
     "D106",
     "D2",
     "D3",
-    # "D400", WIP: see #31135
+    "D400",
     # "D401", # Not enabled by ruff, but we don't want it
     "D402",
     "D403",
     "D412",
     "D419"
 ]
 extend-ignore = [
```

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/setup.cfg` & `apache-airflow-providers-sftp-4.3.1rc1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 	Environment :: Console
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	Framework :: Apache Airflow
 	Framework :: Apache Airflow :: Provider
 	License :: OSI Approved :: Apache Software License
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.3.1/
 	Bug Tracker=https://github.com/apache/airflow/issues
 	Source Code=https://github.com/apache/airflow
 	Slack Chat=https://s.apache.org/airflow-slack
 	Twitter=https://twitter.com/ApacheAirflow
 	YouTube=https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
 
 [bdist_wheel]
 python_tag = py3
 
 [options]
 zip_safe = False
 include_package_data = True
-python_requires = ~=3.7
+python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	apache-airflow-providers-ssh>=2.1.0.dev0
 	apache-airflow>=2.4.0.dev0
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.sftp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.sftp
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-sftp-4.3.0rc2/setup.py` & `apache-airflow-providers-sftp-4.3.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-sftp package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "4.3.0"
+version = "4.3.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-sftp setup."""
     setup(
         version=version,
         extras_require={"ssh": ["apache-airflow-providers-ssh"]},
```

