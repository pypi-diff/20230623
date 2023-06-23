# Comparing `tmp/apache-airflow-providers-facebook-3.2.0rc2.tar.gz` & `tmp/apache-airflow-providers-facebook-3.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-facebook-3.2.0rc2.tar", last modified: Fri May 19 17:52:24 2023, max compression
+gzip compressed data, was "apache-airflow-providers-facebook-3.2.1rc1.tar", last modified: Tue Jun 20 11:42:01 2023, max compression
```

## Comparing `apache-airflow-providers-facebook-3.2.0rc2.tar` & `apache-airflow-providers-facebook-3.2.1rc1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:24.000000 apache-airflow-providers-facebook-3.2.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-facebook-3.2.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-19 17:52:23.000000 apache-airflow-providers-facebook-3.2.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-facebook-3.2.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     9960 2023-05-19 17:52:24.000000 apache-airflow-providers-facebook-3.2.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8427 2023-05-19 17:52:23.000000 apache-airflow-providers-facebook-3.2.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:24.000000 apache-airflow-providers-facebook-3.2.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:24.000000 apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:24.000000 apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/
--rw-r--r--   0 root         (0) root         (0)     1533 2023-05-19 12:06:21.000000 apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:24.000000 apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/ads/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/ads/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:24.000000 apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/ads/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/ads/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7777 2023-02-24 18:43:53.000000 apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/ads/hooks/ads.py
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-19 17:52:23.000000 apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 17:52:24.000000 apache-airflow-providers-facebook-3.2.0rc2/apache_airflow_providers_facebook.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9960 2023-05-19 17:52:23.000000 apache-airflow-providers-facebook-3.2.0rc2/apache_airflow_providers_facebook.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      694 2023-05-19 17:52:23.000000 apache-airflow-providers-facebook-3.2.0rc2/apache_airflow_providers_facebook.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:23.000000 apache-airflow-providers-facebook-3.2.0rc2/apache_airflow_providers_facebook.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-19 17:52:23.000000 apache-airflow-providers-facebook-3.2.0rc2/apache_airflow_providers_facebook.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 17:52:23.000000 apache-airflow-providers-facebook-3.2.0rc2/apache_airflow_providers_facebook.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-19 17:52:23.000000 apache-airflow-providers-facebook-3.2.0rc2/apache_airflow_providers_facebook.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-19 17:52:23.000000 apache-airflow-providers-facebook-3.2.0rc2/apache_airflow_providers_facebook.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5338 2023-05-18 08:56:29.000000 apache-airflow-providers-facebook-3.2.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1866 2023-05-19 17:52:24.000000 apache-airflow-providers-facebook-3.2.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1650 2023-05-19 17:52:23.000000 apache-airflow-providers-facebook-3.2.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:01.835251 apache-airflow-providers-facebook-3.2.1rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-facebook-3.2.1rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-06-20 11:42:00.000000 apache-airflow-providers-facebook-3.2.1rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-facebook-3.2.1rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    10390 2023-06-20 11:42:01.836286 apache-airflow-providers-facebook-3.2.1rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8856 2023-06-20 11:42:00.000000 apache-airflow-providers-facebook-3.2.1rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:01.768404 apache-airflow-providers-facebook-3.2.1rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:01.769562 apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:01.801090 apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-20 11:01:09.000000 apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:01.804140 apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/ads/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/ads/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:01.809852 apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/ads/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/ads/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2023-06-05 12:50:36.000000 apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/ads/hooks/ads.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-06-20 11:42:00.000000 apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 11:42:01.833060 apache-airflow-providers-facebook-3.2.1rc1/apache_airflow_providers_facebook.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10390 2023-06-20 11:42:01.000000 apache-airflow-providers-facebook-3.2.1rc1/apache_airflow_providers_facebook.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      694 2023-06-20 11:42:01.000000 apache-airflow-providers-facebook-3.2.1rc1/apache_airflow_providers_facebook.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:01.000000 apache-airflow-providers-facebook-3.2.1rc1/apache_airflow_providers_facebook.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-20 11:42:01.000000 apache-airflow-providers-facebook-3.2.1rc1/apache_airflow_providers_facebook.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 11:42:01.000000 apache-airflow-providers-facebook-3.2.1rc1/apache_airflow_providers_facebook.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-20 11:42:01.000000 apache-airflow-providers-facebook-3.2.1rc1/apache_airflow_providers_facebook.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 11:42:01.000000 apache-airflow-providers-facebook-3.2.1rc1/apache_airflow_providers_facebook.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-08 05:42:54.000000 apache-airflow-providers-facebook-3.2.1rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-06-20 11:42:01.838309 apache-airflow-providers-facebook-3.2.1rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-06-20 11:42:00.000000 apache-airflow-providers-facebook-3.2.1rc1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/LICENSE` & `apache-airflow-providers-facebook-3.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/MANIFEST.in` & `apache-airflow-providers-facebook-3.2.1rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/PKG-INFO` & `apache-airflow-providers-facebook-3.2.1rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-facebook
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-facebook package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.1/
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
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -48,38 +48,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-facebook``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Facebook Ads <http://business.facebook.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``facebook`` provider. All classes for this provider package
 are in ``airflow.providers.facebook`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-facebook``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
@@ -109,14 +109,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/README.rst` & `apache-airflow-providers-facebook-3.2.1rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,38 +15,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-facebook``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Facebook Ads <http://business.facebook.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``facebook`` provider. All classes for this provider package
 are in ``airflow.providers.facebook`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-facebook``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
@@ -76,14 +76,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/__init__.py` & `apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 from __future__ import annotations
 
 import packaging.version
 
 __all__ = ["__version__"]
 
-__version__ = "3.2.0"
+__version__ = "3.2.1"
 
 try:
     from airflow import __version__ as airflow_version
 except ImportError:
     from airflow.version import version as airflow_version
 
 if packaging.version.parse(airflow_version) < packaging.version.parse("2.4.0"):
```

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/ads/__init__.py` & `apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/ads/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/ads/hooks/__init__.py` & `apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/ads/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/ads/hooks/ads.py` & `apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/ads/hooks/ads.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,44 +11,43 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
-"""This module contains Facebook Ads Reporting hooks"""
+"""This module contains Facebook Ads Reporting hooks."""
 from __future__ import annotations
 
 import time
 from enum import Enum
+from functools import cached_property
 from typing import Any
 
 from facebook_business.adobjects.adaccount import AdAccount
 from facebook_business.adobjects.adreportrun import AdReportRun
 from facebook_business.adobjects.adsinsights import AdsInsights
 from facebook_business.api import FacebookAdsApi
 
-from airflow.compat.functools import cached_property
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 
 
 class JobStatus(Enum):
-    """Available options for facebook async task status"""
+    """Available options for facebook async task status."""
 
     COMPLETED = "Job Completed"
     STARTED = "Job Started"
     RUNNING = "Job Running"
     FAILED = "Job Failed"
     SKIPPED = "Job Skipped"
 
 
 class FacebookAdsReportingHook(BaseHook):
-    """
-    Hook for the Facebook Ads API
+    """Facebook Ads API.
 
     .. seealso::
         For more information on the Facebook Ads API, take a look at the API docs:
         https://developers.facebook.com/docs/marketing-apis/
 
     :param facebook_conn_id: Airflow Facebook Ads connection ID
     :param api_version: The version of Facebook API. Default to None. If it is None,
@@ -68,33 +67,34 @@
     ) -> None:
         super().__init__()
         self.facebook_conn_id = facebook_conn_id
         self.api_version = api_version
         self.client_required_fields = ["app_id", "app_secret", "access_token", "account_id"]
 
     def _get_service(self) -> FacebookAdsApi:
-        """Returns Facebook Ads Client using a service account"""
+        """Returns Facebook Ads Client using a service account."""
         config = self.facebook_ads_config
         return FacebookAdsApi.init(
             app_id=config["app_id"],
             app_secret=config["app_secret"],
             access_token=config["access_token"],
             api_version=self.api_version,
         )
 
     @cached_property
     def multiple_accounts(self) -> bool:
-        """Checks whether provided account_id in the Facebook Ads Connection is provided as a list"""
+        """Checks whether provided account_id in the Facebook Ads Connection is provided as a list."""
         return isinstance(self.facebook_ads_config["account_id"], list)
 
     @cached_property
     def facebook_ads_config(self) -> dict:
-        """
-        Gets Facebook ads connection from meta db and sets
-        facebook_ads_config attribute with returned config file
+        """Get the ``facebook_ads_config`` attribute.
+
+        This fetches Facebook Ads connection from meta database, and sets the
+        ``facebook_ads_config`` attribute with returned config file.
         """
         self.log.info("Fetching fb connection: %s", self.facebook_conn_id)
         conn = self.get_connection(self.facebook_conn_id)
         config = conn.extra_dejson
         missing_keys = self.client_required_fields - config.keys()
         if missing_keys:
             message = f"{missing_keys} fields are missing"
@@ -103,15 +103,15 @@
 
     def bulk_facebook_report(
         self,
         params: dict[str, Any] | None,
         fields: list[str],
         sleep_time: int = 5,
     ) -> list[AdsInsights] | dict[str, list[AdsInsights]]:
-        """Pulls data from the Facebook Ads API regarding Account ID with matching return type.
+        """Pull data from Facebook Ads API regarding Account ID with matching return type.
 
         The return type and value depends on the ``account_id`` configuration. If the
         configuration is a str representing a single Account ID, the return value is the
         list of reports for that ID. If the configuration is a list of str representing
         multiple Account IDs, the return value is a dict of Account IDs and their
         respective list of reports.
 
@@ -148,19 +148,18 @@
         self,
         account_id: str,
         api: FacebookAdsApi,
         params: dict[str, Any] | None,
         fields: list[str],
         sleep_time: int = 5,
     ) -> list[AdsInsights]:
-        """
-        Pulls data from the Facebook Ads API with given account_id
+        """Pull data from the Facebook Ads API with given ``account_id``.
 
         :param account_id: Facebook Account ID that holds ads information
-                https://developers.facebook.com/docs/marketing-api/reference/ads-insights/
+            https://developers.facebook.com/docs/marketing-api/reference/ads-insights/
         :param api: FacebookAdsApi created in the hook
         :param fields: List of fields that is obtained from Facebook. Found in AdsInsights.Field class.
             https://developers.facebook.com/docs/marketing-api/insights/parameters/v6.0
         :param params: Parameters that determine the query for Facebook
             https://developers.facebook.com/docs/marketing-api/insights/parameters/v6.0
         :param sleep_time: Time to sleep when async call is happening
         """
```

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/airflow/providers/facebook/get_provider_info.py` & `apache-airflow-providers-facebook-3.2.1rc1/airflow/providers/facebook/get_provider_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 def get_provider_info():
     return {
         "package-name": "apache-airflow-providers-facebook",
         "name": "Facebook",
         "description": "`Facebook Ads <http://business.facebook.com/>`__\n",
         "suspended": False,
         "versions": [
+            "3.2.1",
             "3.2.0",
             "3.1.0",
             "3.0.1",
             "3.0.0",
             "2.2.3",
             "2.2.2",
             "2.2.1",
```

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/apache_airflow_providers_facebook.egg-info/PKG-INFO` & `apache-airflow-providers-facebook-3.2.1rc1/apache_airflow_providers_facebook.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-facebook
-Version: 3.2.0rc2
+Version: 3.2.1rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-facebook package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
-Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.0/
+Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.1/
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
 License-File: LICENSE
 License-File: NOTICE
 
 
 .. Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
@@ -48,38 +48,38 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-facebook``
 
-Release: ``3.2.0rc2``
+Release: ``3.2.1rc1``
 
 
 `Facebook Ads <http://business.facebook.com/>`__
 
 
 Provider package
 ----------------
 
 This is a provider package for ``facebook`` provider. All classes for this provider package
 are in ``airflow.providers.facebook`` python package.
 
 You can find package information and changelog for the provider
-in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.0/>`_.
+in the `documentation <https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.1/>`_.
 
 
 Installation
 ------------
 
 You can install this package on top of an existing Airflow 2 installation (see ``Requirements`` below
 for the minimum Airflow version supported) via
 ``pip install apache-airflow-providers-facebook``
 
-The package supports the following python versions: 3.7,3.8,3.9,3.10
+The package supports the following python versions: 3.8,3.9,3.10,3.11
 
 Requirements
 ------------
 
 =====================  ==================
 PIP package            Version required
 =====================  ==================
@@ -109,14 +109,31 @@
    Please, only add notes to the Changelog just below the "Changelog" header when there are some breaking changes
    and you want to add an explanation to the users on how they are supposed to deal with them.
    The changelog is updated and maintained semi-automatically by release manager.
 
 Changelog
 ---------
 
+3.2.1
+.....
+
+.. note::
+  This release dropped support for Python 3.7
+
+Misc
+~~~~
+
+* ``Remove Python 3.7 support (#30963)``
+
+.. Below changes are excluded from the changelog. Move them to
+   appropriate section above if needed. Do not delete the lines(!):
+   * ``Improve docstrings in providers (#31681)``
+   * ``Add D400 pydocstyle check - Providers (#31427)``
+   * ``Add note about dropping Python 3.7 for providers (#32015)``
+
 3.2.0
 .....
 
 .. note::
   This release of provider is only available for Airflow 2.4+ as explained in the
   `Apache Airflow providers support policy <https://github.com/apache/airflow/blob/main/PROVIDERS.rst#minimum-supported-version-of-airflow-for-community-managed-providers>`_.
```

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/apache_airflow_providers_facebook.egg-info/SOURCES.txt` & `apache-airflow-providers-facebook-3.2.1rc1/apache_airflow_providers_facebook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/pyproject.toml` & `apache-airflow-providers-facebook-3.2.1rc1/pyproject.toml`

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

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/setup.cfg` & `apache-airflow-providers-facebook-3.2.1rc1/setup.cfg`

 * *Files 9% similar despite different names*

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
-	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.0/
+	Documentation=https://airflow.apache.org/docs/apache-airflow-providers-facebook/3.2.1/
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
 	apache-airflow>=2.4.0.dev0
 	facebook-business>=6.0.2
@@ -53,10 +53,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.facebook.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.facebook
 
 [egg_info]
-tag_build = rc2
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-facebook-3.2.0rc2/setup.py` & `apache-airflow-providers-facebook-3.2.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # IF YOU WANT TO MODIFY IT, YOU SHOULD MODIFY THE TEMPLATE
 # `SETUP_TEMPLATE.py.jinja2` IN the `dev/provider_packages` DIRECTORY
 
 """Setup.py for the apache-airflow-providers-facebook package."""
 
 from setuptools import find_namespace_packages, setup
 
-version = "3.2.0"
+version = "3.2.1"
 
 
 def do_setup():
     """Perform the package apache-airflow-providers-facebook setup."""
     setup(
         version=version,
         extras_require={},
```

