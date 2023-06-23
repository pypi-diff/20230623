# Comparing `tmp/apache-airflow-providers-asana-2.2.1rc1.tar.gz` & `tmp/apache-airflow-providers-asana-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-asana-2.2.1rc1.tar", last modified: Tue Jun 20 11:41:35 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-asana-3.0.0rc1.tar", last modified: Tue Nov 15 00:14:08 2022, max compression
```

## Comparing `apache-airflow-providers-asana-2.2.1rc1.tar` & `apache-airflow-providers-asana-3.0.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:35.524643 apache-airflow-providers-asana-2.2.1rc1/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-asana-2.2.1rc1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:41:34.000000 apache-airflow-providers-asana-2.2.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-asana-2.2.1rc1/NOTICE
--rw-r--r--   0 root         (0) root         (0)    10486 2023-06-20 11:41:35.525776 apache-airflow-providers-asana-2.2.1rc1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8961 2023-06-20 11:41:34.000000 apache-airflow-providers-asana-2.2.1rc1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:35.453595 apache-airflow-providers-asana-2.2.1rc1/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:35.454690 apache-airflow-providers-asana-2.2.1rc1/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:35.485934 apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 11:01:09.000000 apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2269 2023-06-20 11:41:34.000000 apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:35.491688 apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13337 2023-06-02 11:31:21.000000 apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/hooks/asana.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:35.497835 apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5491 2023-06-05 12:50:36.000000 apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/operators/asana_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:41:35.521864 apache-airflow-providers-asana-2.2.1rc1/apache_airflow_providers_asana.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10486 2023-06-20 11:41:35.000000 apache-airflow-providers-asana-2.2.1rc1/apache_airflow_providers_asana.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      707 2023-06-20 11:41:35.000000 apache-airflow-providers-asana-2.2.1rc1/apache_airflow_providers_asana.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:35.000000 apache-airflow-providers-asana-2.2.1rc1/apache_airflow_providers_asana.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      102 2023-06-20 11:41:35.000000 apache-airflow-providers-asana-2.2.1rc1/apache_airflow_providers_asana.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:41:35.000000 apache-airflow-providers-asana-2.2.1rc1/apache_airflow_providers_asana.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-20 11:41:35.000000 apache-airflow-providers-asana-2.2.1rc1/apache_airflow_providers_asana.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:41:35.000000 apache-airflow-providers-asana-2.2.1rc1/apache_airflow_providers_asana.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-asana-2.2.1rc1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-20 11:41:35.527713 apache-airflow-providers-asana-2.2.1rc1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1632 2023-06-20 11:41:34.000000 apache-airflow-providers-asana-2.2.1rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2022-05-27 19:54:38.000000 apache-airflow-providers-asana-3.0.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1122 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2022-05-27 19:54:38.000000 apache-airflow-providers-asana-3.0.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     9024 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7480 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13369 2022-10-26 03:21:46.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/asana.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2022-09-13 10:31:21.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2022-09-14 19:22:24.000000 apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/asana_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9024 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      707 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       36 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1836 2022-10-26 03:21:46.000000 apache-airflow-providers-asana-3.0.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1832 2022-11-15 00:14:08.000000 apache-airflow-providers-asana-3.0.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1460 2022-11-15 00:14:07.000000 apache-airflow-providers-asana-3.0.0rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `apache-airflow-providers-asana-2.2.1rc1/LICENSE` & `apache-airflow-providers-asana-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.1rc1/MANIFEST.in` & `apache-airflow-providers-asana-3.0.0rc1/MANIFEST.in`

 * *Files 6% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 # `MANIFEST_TEMPLATE.py.jinja2` IN the `provider_packages` DIRECTORY
 
 
 
 
 include NOTICE
 include LICENSE
-include CHANGELOG.rst
+include CHANGELOG.txt
+include README.md
 global-exclude __pycache__  *.pyc
```

### Comparing `apache-airflow-providers-asana-2.2.1rc1/PKG-INFO` & `apache-airflow-providers-asana-3.0.0rc1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-asana
-Version: 2.2.1rc1
+Version: 3.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-asana package
 Home-page: https://airflow.apache.org/
-Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.1/
+Download-URL: https://archive.apache.org/dist/airflow/providers
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.8
+Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -48,46 +49,46 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-asana``
 
-Release: ``2.2.1rc1``
+Release: ``3.0.0rc1``
 
 
 `Asana <https://app.asana.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``asana`` provider. All classes for this provider package
 are in ``airflow.providers.asana`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-asana``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.7,3.8,3.9,3.10
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.4.0``
+``apache-airflow``  ``>=2.3.0``
 ``asana``           ``>=0.10``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -108,79 +109,42 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-2.2.1
-.....
-
-.. note::
-  This release dropped support for Python 3.7
-
-Misc
-~~~~
-
-* ``Remove Python 3.7 support (#30963)``
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-   * ``Improve docstrings in providers (#31681)``
-   * ``Add D400 pydocstyle check - Providers (#31427)``
-   * ``Add note about dropping Python 3.7 for providers (#32015)``
-
-2.2.0
+3.0.0
 .....
 
-.. note::
-  This release of provider is only available for Airflow 2.4+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+This release of provider is only available for Airflow 2.3+ as explained in the
+`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
 
-Misc
-~~~~
-
-* ``Bump minimum Airflow version in providers (#30917)``
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-   * ``Add full automation for min Airflow version for providers (#30994)``
-   * ``Add mechanism to suspend providers (#30422)``
-   * ``Use '__version__' in providers not 'version' (#31393)``
-   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
-   * ``Prepare docs for May 2023 wave of Providers (#31252)``
-
-2.1.0
-.....
+Breaking changes
+~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.3+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* In AsanaHook, non-prefixed extra fields are supported and are preferred.  So if you should update your
+  connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
 ~~~~~~~~
 
-In AsanaHook, non-prefixed extra fields are supported and are preferred. You should update your
-connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
-
-
 * ``Allow and prefer non-prefixed extra fields for AsanaHook (#27043)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Enable string normalization in python formatting - providers (#27205)``
    * ``Update docs for September Provider's release (#26731)``
    * ``Apply PEP-563 (Postponed Evaluation of Annotations) to non-core airflow (#26289)``
-   * ``pRepare docs for November 2022 wave of Providers (#27613)``
-   * ``Prepare for follow-up release for November providers (#27774)``
+
 
 2.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
@@ -193,17 +157,16 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.2+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
+  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Migrate Asana example DAGs to new design #22440 (#24131)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Use new Breese for building, pulling and verifying the images. (#23104)``
@@ -277,7 +240,9 @@
    * ``Prepare documentation for July release of providers. (#17015)``
    * ``Removes pylint from our toolchain (#16682)``
 
 1.0.0
 .....
 
 Initial version of the provider.
+
+
```

### Comparing `apache-airflow-providers-asana-2.2.1rc1/README.rst` & `apache-airflow-providers-asana-3.0.0rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -15,46 +15,46 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-asana``
 
-Release: ``2.2.1rc1``
+Release: ``3.0.0rc1``
 
 
 `Asana <https://app.asana.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``asana`` provider. All classes for this provider package
 are in ``airflow.providers.asana`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-asana``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.7,3.8,3.9,3.10
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.4.0``
+``apache-airflow``  ``>=2.3.0``
 ``asana``           ``>=0.10``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -75,79 +75,42 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-2.2.1
+3.0.0
 .....
 
-.. note::
-  This release dropped support for Python 3.7
+This release of provider is only available for Airflow 2.3+ as explained in the
+`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
 
-Misc
-~~~~
-
-* ``Remove Python 3.7 support (#30963)``
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-   * ``Improve docstrings in providers (#31681)``
-   * ``Add D400 pydocstyle check - Providers (#31427)``
-   * ``Add note about dropping Python 3.7 for providers (#32015)``
-
-2.2.0
-.....
-
-.. note::
-  This release of provider is only available for Airflow 2.4+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
-
-Misc
-~~~~
-
-* ``Bump minimum Airflow version in providers (#30917)``
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-   * ``Add full automation for min Airflow version for providers (#30994)``
-   * ``Add mechanism to suspend providers (#30422)``
-   * ``Use '__version__' in providers not 'version' (#31393)``
-   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
-   * ``Prepare docs for May 2023 wave of Providers (#31252)``
-
-2.1.0
-.....
+Breaking changes
+~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.3+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* In AsanaHook, non-prefixed extra fields are supported and are preferred.  So if you should update your
+  connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
 ~~~~~~~~
 
-In AsanaHook, non-prefixed extra fields are supported and are preferred. You should update your
-connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
-
-
 * ``Allow and prefer non-prefixed extra fields for AsanaHook (#27043)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Enable string normalization in python formatting - providers (#27205)``
    * ``Update docs for September Provider's release (#26731)``
    * ``Apply PEP-563 (Postponed Evaluation of Annotations) to non-core airflow (#26289)``
-   * ``pRepare docs for November 2022 wave of Providers (#27613)``
-   * ``Prepare for follow-up release for November providers (#27774)``
+
 
 2.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
@@ -160,17 +123,16 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.2+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
+  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Migrate Asana example DAGs to new design #22440 (#24131)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Use new Breese for building, pulling and verifying the images. (#23104)``
```

### Comparing `apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/get_provider_info.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/get_provider_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,28 +23,16 @@
 
 
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-asana",
         "name": "Asana",
         "description": "`Asana <https://app.asana.com/>`__\n",
-        "suspended": False,
-        "versions": [
-            "2.2.1",
-            "2.2.0",
-            "2.1.0",
-            "2.0.1",
-            "2.0.0",
-            "1.1.3",
-            "1.1.2",
-            "1.1.1",
-            "1.1.0",
-            "1.0.0",
-        ],
-        "dependencies": ["apache-airflow>=2.4.0", "asana>=0.10"],
+        "versions": ["3.0.0", "2.0.1", "2.0.0", "1.1.3", "1.1.2", "1.1.1", "1.1.0", "1.0.0"],
+        "dependencies": ["apache-airflow>=2.3.0", "asana>=0.10"],
         "integrations": [
             {
                 "integration-name": "Asana",
                 "external-doc-url": "https://developers.asana.com/docs",
                 "how-to-guide": ["/docs/apache-airflow-providers-asana/operators/asana.rst"],
                 "tags": ["software"],
             }
```

### Comparing `apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/hooks/__init__.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/hooks/asana.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/asana.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 """Connect to Asana."""
 from __future__ import annotations
 
-from functools import cached_property, wraps
+from functools import wraps
 from typing import Any
 
 from asana import Client  # type: ignore[attr-defined]
 from asana.error import NotFoundError  # type: ignore[attr-defined]
 
+from airflow.compat.functools import cached_property
 from airflow.hooks.base import BaseHook
 
 
 def _ensure_prefixes(conn_type):
     """
     Remove when provider min airflow version >= 2.5.0 since this is handled by
     provider manager from that version.
@@ -84,41 +85,41 @@
         return extras.get(prefixed_name) or None
 
     def get_conn(self) -> Client:
         return self.client
 
     @staticmethod
     def get_connection_form_widgets() -> dict[str, Any]:
-        """Returns connection widgets to add to connection form."""
+        """Returns connection widgets to add to connection form"""
         from flask_appbuilder.fieldwidgets import BS3TextFieldWidget
         from flask_babel import lazy_gettext
         from wtforms import StringField
 
         return {
             "workspace": StringField(lazy_gettext("Workspace"), widget=BS3TextFieldWidget()),
             "project": StringField(lazy_gettext("Project"), widget=BS3TextFieldWidget()),
         }
 
     @staticmethod
     @_ensure_prefixes(conn_type="asana")
     def get_ui_field_behaviour() -> dict[str, Any]:
-        """Returns custom field behaviour."""
+        """Returns custom field behaviour"""
         return {
             "hidden_fields": ["port", "host", "login", "schema"],
             "relabeling": {},
             "placeholders": {
                 "password": "Asana personal access token",
                 "workspace": "Asana workspace gid",
                 "project": "Asana project gid",
             },
         }
 
     @cached_property
     def client(self) -> Client:
-        """Instantiates python-asana Client."""
+        """Instantiates python-asana Client"""
         if not self.connection.password:
             raise ValueError(
                 "Asana connection password must contain a personal access token: "
                 "https://developers.asana.com/docs/personal-access-token"
             )
 
         return Client.access_token(self.connection.password)
@@ -257,15 +258,15 @@
         self._validate_create_project_parameters(merged_params)
         response = self.client.projects.create(merged_params)
         return response
 
     @staticmethod
     def _validate_create_project_parameters(params: dict) -> None:
         """
-        Check that user provided the minimum required parameters for project creation.
+        Check that user provided the minimum required parameters for project creation
 
         :param params: Attributes that the new project should have
         :return: None; raises a ValueError if `params` does not contain the minimum required attributes.
         """
         required_parameters = {"workspace", "team"}
         if required_parameters.isdisjoint(params):
             raise ValueError(
```

### Comparing `apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/operators/__init__.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.1rc1/airflow/providers/asana/operators/asana_tasks.py` & `apache-airflow-providers-asana-3.0.0rc1/airflow/providers/asana/operators/asana_tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,19 +24,16 @@
 
 if TYPE_CHECKING:
     from airflow.utils.context import Context
 
 
 class AsanaCreateTaskOperator(BaseOperator):
     """
-    This operator can be used to create Asana tasks.
-
-    .. seealso::
-        For more information on Asana optional task parameters:
-        https://developers.asana.com/docs/create-a-task
+    This operator can be used to create Asana tasks. For more information on
+    Asana optional task parameters, see https://developers.asana.com/docs/create-a-task
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:AsanaCreateTaskOperator`
 
     :param conn_id: The Asana connection to use.
     :param name: Name of the Asana task.
@@ -66,18 +63,16 @@
         self.log.info(response)
         return response["gid"]
 
 
 class AsanaUpdateTaskOperator(BaseOperator):
     """
     This operator can be used to update Asana tasks.
-
-    .. seealso::
-        For more information on Asana optional task parameters:
-        https://developers.asana.com/docs/update-a-task
+    For more information on Asana optional task parameters, see
+    https://developers.asana.com/docs/update-a-task
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:AsanaUpdateTaskOperator`
 
     :param conn_id: The Asana connection to use.
     :param asana_task_gid: Asana task ID to update
@@ -134,18 +129,15 @@
         response = hook.delete_task(self.asana_task_gid)
         self.log.info(response)
 
 
 class AsanaFindTaskOperator(BaseOperator):
     """
     This operator can be used to retrieve Asana tasks that match various filters.
-
-    .. seealso::
-        For a list of possible filters:
-        https://developers.asana.com/docs/update-a-task
+    See https://developers.asana.com/docs/update-a-task for a list of possible filters.
 
     .. seealso::
         For more information on how to use this operator, take a look at the guide:
         :ref:`howto/operator:AsanaFindTaskOperator`
 
     :param conn_id: The Asana connection to use.
     :param search_parameters: The parameters used to find relevant tasks. You must
```

### Comparing `apache-airflow-providers-asana-2.2.1rc1/apache_airflow_providers_asana.egg-info/PKG-INFO` & `apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-asana
-Version: 2.2.1rc1
+Version: 3.0.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-asana package
 Home-page: https://airflow.apache.org/
-Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.1/
+Download-URL: https://archive.apache.org/dist/airflow/providers
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Source Code, https://github.com/apache/airflow
 Project-URL: Slack Chat, https://s.apache.org/airflow-slack
 Project-URL: Twitter, https://twitter.com/ApacheAirflow
 Project-URL: YouTube, https://www.youtube.com/channel/UCSXwxpWZQ7XZ1WL3wqevChA/
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Monitoring
-Requires-Python: ~=3.8
+Requires-Python: ~=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -48,46 +49,46 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-asana``
 
-Release: ``2.2.1rc1``
+Release: ``3.0.0rc1``
 
 
 `Asana <https://app.asana.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``asana`` provider. All classes for this provider package
 are in ``airflow.providers.asana`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.1/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-asana``
 
-The package supports the following python versions: 3.8,3.9,3.10,3.11
+The package supports the following python versions: 3.7,3.8,3.9,3.10
 
 Requirements
 ------------
 
 ==================  ==================
 PIP package         Version required
 ==================  ==================
-``apache-airflow``  ``>=2.4.0``
+``apache-airflow``  ``>=2.3.0``
 ``asana``           ``>=0.10``
 ==================  ==================
 
  .. Licensed to the Apache Software Foundation (ASF) under one
     or more contributor license agreements.  See the NOTICE file
     distributed with this work for additional information
     regarding copyright ownership.  The ASF licenses this file
@@ -108,79 +109,42 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
-2.2.1
-.....
-
-.. note::
-  This release dropped support for Python 3.7
-
-Misc
-~~~~
-
-* ``Remove Python 3.7 support (#30963)``
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-   * ``Improve docstrings in providers (#31681)``
-   * ``Add D400 pydocstyle check - Providers (#31427)``
-   * ``Add note about dropping Python 3.7 for providers (#32015)``
-
-2.2.0
+3.0.0
 .....
 
-.. note::
-  This release of provider is only available for Airflow 2.4+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+This release of provider is only available for Airflow 2.3+ as explained in the
+`Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/README.md#support-for-providers>`_.
 
-Misc
-~~~~
-
-* ``Bump minimum Airflow version in providers (#30917)``
-
-.. Below changes are excluded from the changelog. Move them to
-   appropriate section above if needed. Do not delete the lines(!):
-   * ``Add full automation for min Airflow version for providers (#30994)``
-   * ``Add mechanism to suspend providers (#30422)``
-   * ``Use '__version__' in providers not 'version' (#31393)``
-   * ``Fixing circular import error in providers caused by airflow version check (#31379)``
-   * ``Prepare docs for May 2023 wave of Providers (#31252)``
-
-2.1.0
-.....
+Breaking changes
+~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.3+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* In AsanaHook, non-prefixed extra fields are supported and are preferred.  So if you should update your
+  connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
 
 Misc
 ~~~~
 
 * ``Move min airflow version to 2.3.0 for all providers (#27196)``
 
 Features
 ~~~~~~~~
 
-In AsanaHook, non-prefixed extra fields are supported and are preferred. You should update your
-connection to replace ``extra__asana__workspace`` with ``workspace`` etc.
-
-
 * ``Allow and prefer non-prefixed extra fields for AsanaHook (#27043)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Enable string normalization in python formatting - providers (#27205)``
    * ``Update docs for September Provider's release (#26731)``
    * ``Apply PEP-563 (Postponed Evaluation of Annotations) to non-core airflow (#26289)``
-   * ``pRepare docs for November 2022 wave of Providers (#27613)``
-   * ``Prepare for follow-up release for November providers (#27774)``
+
 
 2.0.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
 
@@ -193,17 +157,16 @@
 
 2.0.0
 .....
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-.. note::
-  This release of provider is only available for Airflow 2.2+ as explained in the
-  `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
+* This release of provider is only available for Airflow 2.2+ as explained in the Apache Airflow
+  providers support policy https://github.com/apache/airflow/blob/main/README.md#support-for-providers
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Add explanatory note for contributors about updating Changelog (#24229)``
    * ``Migrate Asana example DAGs to new design #22440 (#24131)``
    * ``Prepare provider documentation 2022.05.11 (#23631)``
    * ``Use new Breese for building, pulling and verifying the images. (#23104)``
@@ -277,7 +240,9 @@
    * ``Prepare documentation for July release of providers. (#17015)``
    * ``Removes pylint from our toolchain (#16682)``
 
 1.0.0
 .....
 
 Initial version of the provider.
+
+
```

### Comparing `apache-airflow-providers-asana-2.2.1rc1/apache_airflow_providers_asana.egg-info/SOURCES.txt` & `apache-airflow-providers-asana-3.0.0rc1/apache_airflow_providers_asana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-asana-2.2.1rc1/setup.cfg` & `apache-airflow-providers-asana-3.0.0rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -17,40 +17,40 @@
 	Environment :: Console
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	Framework :: Apache Airflow
 	Framework :: Apache Airflow :: Provider
 	License :: OSI Approved :: Apache Software License
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
 	Topic :: System :: Monitoring
 project_urls = 
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-asana/2.2.1/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-asana/3.0.0/
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
-python_requires = ~=3.8
+python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow>=2.4.0.dev0
+	apache-airflow>=2.3.0.*
 	asana>=0.10
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.asana.get_provider_info:get_provider_info
 
 [files]
```

### Comparing `apache-airflow-providers-asana-2.2.1rc1/setup.py` & `apache-airflow-providers-asana-3.0.0rc1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,28 +22,21 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-asana package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "2.2.1"
+version = "3.0.0"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-asana setup."""
     setup(
         version=version,
         extras_require={},
-        packages=find_namespace_packages(
-            include=[
-                "airflow.providers.asana",
-                "airflow.providers.asana.*",
-                "airflow.providers.asana_vendor",
-                "airflow.providers.asana_vendor.*",
-            ],
-        ),
+        packages=find_namespace_packages(include=["airflow.providers.asana", "airflow.providers.asana.*"]),
     )
 
 
 if __name__ == "__main__":
     do_setup()
```

