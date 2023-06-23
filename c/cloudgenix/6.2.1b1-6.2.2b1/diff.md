# Comparing `tmp/cloudgenix-6.2.1b1.tar.gz` & `tmp/cloudgenix-6.2.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudgenix-6.2.1b1.tar", last modified: Wed Apr 19 19:25:34 2023, max compression
+gzip compressed data, was "dist/cloudgenix-6.2.2b1.tar", last modified: Fri Jun 23 19:42:59 2023, max compression
```

## Comparing `cloudgenix-6.2.1b1.tar` & `cloudgenix-6.2.2b1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 dishah   (1305937620) 192360288        0 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/
--rw-r--r--   0 dishah   (1305937620) 192360288     1077 2023-04-10 06:05:48.000000 cloudgenix-6.2.1b1/LICENSE
--rw-r--r--   0 dishah   (1305937620) 192360288     4859 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/PKG-INFO
--rw-r--r--   0 dishah   (1305937620) 192360288     4215 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/README.md
-drwxr-xr-x   0 dishah   (1305937620) 192360288        0 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix/
--rw-r--r--   0 dishah   (1305937620) 192360288    66495 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/__init__.py
--rw-r--r--   0 dishah   (1305937620) 192360288    14160 2023-04-10 06:05:48.000000 cloudgenix-6.2.1b1/cloudgenix/ca_bundle.py
--rw-r--r--   0 dishah   (1305937620) 192360288   146123 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/delete_api.py
--rw-r--r--   0 dishah   (1305937620) 192360288   370766 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/get_api.py
--rw-r--r--   0 dishah   (1305937620) 192360288    48216 2023-04-10 06:05:48.000000 cloudgenix-6.2.1b1/cloudgenix/interactive.py
--rw-r--r--   0 dishah   (1305937620) 192360288    17707 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/patch_api.py
--rw-r--r--   0 dishah   (1305937620) 192360288   530779 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/post_api.py
--rw-r--r--   0 dishah   (1305937620) 192360288   290322 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/cloudgenix/put_api.py
--rw-r--r--   0 dishah   (1305937620) 192360288     4468 2023-04-10 06:05:48.000000 cloudgenix-6.2.1b1/cloudgenix/ws_api.py
-drwxr-xr-x   0 dishah   (1305937620) 192360288        0 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/
--rw-r--r--   0 dishah   (1305937620) 192360288     4859 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/PKG-INFO
--rw-r--r--   0 dishah   (1305937620) 192360288      415 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/SOURCES.txt
--rw-r--r--   0 dishah   (1305937620) 192360288        1 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/dependency_links.txt
--rw-r--r--   0 dishah   (1305937620) 192360288       71 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/requires.txt
--rw-r--r--   0 dishah   (1305937620) 192360288       11 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/cloudgenix.egg-info/top_level.txt
--rw-r--r--   0 dishah   (1305937620) 192360288      262 2023-04-19 19:25:34.000000 cloudgenix-6.2.1b1/setup.cfg
--rw-r--r--   0 dishah   (1305937620) 192360288      999 2023-04-19 18:44:19.000000 cloudgenix-6.2.1b1/setup.py
+drwxr-xr-x   0 dishah   (1305937620) 192360288        0 2023-06-23 19:42:59.000000 cloudgenix-6.2.2b1/
+-rw-r--r--   0 dishah   (1305937620) 192360288     1077 2023-05-30 06:23:00.000000 cloudgenix-6.2.2b1/LICENSE
+-rw-r--r--   0 dishah   (1305937620) 192360288     4997 2023-06-23 19:42:59.000000 cloudgenix-6.2.2b1/PKG-INFO
+-rw-r--r--   0 dishah   (1305937620) 192360288     4353 2023-06-23 19:34:27.000000 cloudgenix-6.2.2b1/README.md
+drwxr-xr-x   0 dishah   (1305937620) 192360288        0 2023-06-23 19:42:59.000000 cloudgenix-6.2.2b1/cloudgenix/
+-rw-r--r--   0 dishah   (1305937620) 192360288    66771 2023-06-23 19:34:13.000000 cloudgenix-6.2.2b1/cloudgenix/__init__.py
+-rw-r--r--   0 dishah   (1305937620) 192360288    14160 2023-05-30 06:23:00.000000 cloudgenix-6.2.2b1/cloudgenix/ca_bundle.py
+-rw-r--r--   0 dishah   (1305937620) 192360288   146123 2023-05-30 06:23:00.000000 cloudgenix-6.2.2b1/cloudgenix/delete_api.py
+-rw-r--r--   0 dishah   (1305937620) 192360288   370772 2023-06-23 14:53:45.000000 cloudgenix-6.2.2b1/cloudgenix/get_api.py
+-rw-r--r--   0 dishah   (1305937620) 192360288    48216 2023-05-30 06:23:00.000000 cloudgenix-6.2.2b1/cloudgenix/interactive.py
+-rw-r--r--   0 dishah   (1305937620) 192360288    17707 2023-05-30 06:23:00.000000 cloudgenix-6.2.2b1/cloudgenix/patch_api.py
+-rw-r--r--   0 dishah   (1305937620) 192360288   535551 2023-06-23 14:53:45.000000 cloudgenix-6.2.2b1/cloudgenix/post_api.py
+-rw-r--r--   0 dishah   (1305937620) 192360288   291585 2023-06-23 14:53:45.000000 cloudgenix-6.2.2b1/cloudgenix/put_api.py
+-rw-r--r--   0 dishah   (1305937620) 192360288     4468 2023-05-30 06:23:00.000000 cloudgenix-6.2.2b1/cloudgenix/ws_api.py
+drwxr-xr-x   0 dishah   (1305937620) 192360288        0 2023-06-23 19:42:59.000000 cloudgenix-6.2.2b1/cloudgenix.egg-info/
+-rw-r--r--   0 dishah   (1305937620) 192360288     4997 2023-06-23 19:42:59.000000 cloudgenix-6.2.2b1/cloudgenix.egg-info/PKG-INFO
+-rw-r--r--   0 dishah   (1305937620) 192360288      415 2023-06-23 19:42:59.000000 cloudgenix-6.2.2b1/cloudgenix.egg-info/SOURCES.txt
+-rw-r--r--   0 dishah   (1305937620) 192360288        1 2023-06-23 19:42:59.000000 cloudgenix-6.2.2b1/cloudgenix.egg-info/dependency_links.txt
+-rw-r--r--   0 dishah   (1305937620) 192360288       88 2023-06-23 19:42:59.000000 cloudgenix-6.2.2b1/cloudgenix.egg-info/requires.txt
+-rw-r--r--   0 dishah   (1305937620) 192360288       11 2023-06-23 19:42:59.000000 cloudgenix-6.2.2b1/cloudgenix.egg-info/top_level.txt
+-rw-r--r--   0 dishah   (1305937620) 192360288      262 2023-06-23 19:42:59.000000 cloudgenix-6.2.2b1/setup.cfg
+-rw-r--r--   0 dishah   (1305937620) 192360288     1033 2023-06-23 19:34:13.000000 cloudgenix-6.2.2b1/setup.py
```

### Comparing `cloudgenix-6.2.1b1/LICENSE` & `cloudgenix-6.2.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudgenix-6.2.1b1/PKG-INFO` & `cloudgenix-6.2.2b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudgenix
-Version: 6.2.1b1
+Version: 6.2.2b1
 Summary: Python2 and Python3 SDK for the CloudGenix AppFabric
 Home-page: https://github.com/CloudGenix/sdk-python
 Author: CloudGenix Developer Support
 Author-email: developers@cloudgenix.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,27 +19,28 @@
 [![CloudGenix Logo](https://raw.githubusercontent.com/CloudGenix/sdk-python/master/docs/CloudGenix_Logo.png)](https://www.cloudgenix.com)
 
 [![image](https://img.shields.io/pypi/v/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![image](https://img.shields.io/pypi/pyversions/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![Downloads](https://pepy.tech/badge/cloudgenix)](https://pepy.tech/project/cloudgenix)
 [![License: MIT](https://img.shields.io/pypi/l/cloudgenix.svg?color=brightgreen)](https://pypi.org/project/cloudgenix/)
 [![GitHub issues open](https://img.shields.io/github/issues/CloudGenix/sdk-python.svg)](https://github.com/CloudGenix/sdk-python/issues)
-# CloudGenix Python SDK v6.2.1b1
+# CloudGenix Python SDK v6.2.2b1
 Python2 and Python3 SDK for the CloudGenix AppFabric
 
 #### Synopsis
 Intended to be a small, lightweight SDK wrapper around the CloudGenix API for easy use. 
 Initial version requires knowledge of JSON/Dict objects for POST/PUT/PATCH operations.
 
 #### Requirements
 * Active CloudGenix Account
 * Python >= 2.7 or >=3.6
 * Python modules:
     * Requests + Security Extras >= 2.22.0 - <http://docs.python-requests.org/en/master/>
     * Websockets (if Python >= 3.6) >= 8.1 - <https://websockets.readthedocs.io/en/stable/index.html>
+    * urllib3 == 1.26.16 - <https://urllib3.readthedocs.io/en/stable/>
 
 #### Code Example
 Comes with `example.py` that shows usage to get a JSON list of sites.
 
 Super-simplified example code (rewrite of example.py in ~4 lines of code):
 ```python
 # Import the CloudGenix SDK API constructor and JSON response pretty printer
@@ -57,14 +58,15 @@
 
 #### License
 MIT
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
+| **6.2.2** | **b1** | Support for June 2023 Controller release. |
 | **6.2.1** | **b1** | Support for April 2023 Controller release. |
 | **6.1.2** | **b1** | Support for January 2023 Controller release. |
 | **6.1.1** | **b1** | Support for November 2022 Controller release. |
 | **6.0.2** | **b1** | Support for August 2022 Controller release. |
 | **6.0.1** | **b1** | Support for June 2022 Controller release. |
 | **5.6.1** | **b2** | Minor bugfix. |
 |           | **b1** | Support for Sept 2021 Controller release. |
```

### Comparing `cloudgenix-6.2.1b1/README.md` & `cloudgenix-6.2.2b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [![CloudGenix Logo](https://raw.githubusercontent.com/CloudGenix/sdk-python/master/docs/CloudGenix_Logo.png)](https://www.cloudgenix.com)
 
 [![image](https://img.shields.io/pypi/v/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![image](https://img.shields.io/pypi/pyversions/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![Downloads](https://pepy.tech/badge/cloudgenix)](https://pepy.tech/project/cloudgenix)
 [![License: MIT](https://img.shields.io/pypi/l/cloudgenix.svg?color=brightgreen)](https://pypi.org/project/cloudgenix/)
 [![GitHub issues open](https://img.shields.io/github/issues/CloudGenix/sdk-python.svg)](https://github.com/CloudGenix/sdk-python/issues)
-# CloudGenix Python SDK v6.2.1b1
+# CloudGenix Python SDK v6.2.2b1
 Python2 and Python3 SDK for the CloudGenix AppFabric
 
 #### Synopsis
 Intended to be a small, lightweight SDK wrapper around the CloudGenix API for easy use. 
 Initial version requires knowledge of JSON/Dict objects for POST/PUT/PATCH operations.
 
 #### Requirements
 * Active CloudGenix Account
 * Python >= 2.7 or >=3.6
 * Python modules:
     * Requests + Security Extras >= 2.22.0 - <http://docs.python-requests.org/en/master/>
     * Websockets (if Python >= 3.6) >= 8.1 - <https://websockets.readthedocs.io/en/stable/index.html>
+    * urllib3 == 1.26.16 - <https://urllib3.readthedocs.io/en/stable/>
 
 #### Code Example
 Comes with `example.py` that shows usage to get a JSON list of sites.
 
 Super-simplified example code (rewrite of example.py in ~4 lines of code):
 ```python
 # Import the CloudGenix SDK API constructor and JSON response pretty printer
@@ -39,14 +40,15 @@
 
 #### License
 MIT
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
+| **6.2.2** | **b1** | Support for June 2023 Controller release. |
 | **6.2.1** | **b1** | Support for April 2023 Controller release. |
 | **6.1.2** | **b1** | Support for January 2023 Controller release. |
 | **6.1.1** | **b1** | Support for November 2022 Controller release. |
 | **6.0.2** | **b1** | Support for August 2022 Controller release. |
 | **6.0.1** | **b1** | Support for June 2022 Controller release. |
 | **5.6.1** | **b2** | Minor bugfix. |
 |           | **b1** | Support for Sept 2021 Controller release. |
```

### Comparing `cloudgenix-6.2.1b1/cloudgenix/__init__.py` & `cloudgenix-6.2.2b1/cloudgenix/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Python2 and Python3 SDK for the CloudGenix AppFabric
 
-**Version:** v6.2.1b1
+**Version:** v6.2.2b1
 
 **Author:** CloudGenix
 
 **Copyright:** (c) 2017-2023 CloudGenix, Inc
 
 **License:** MIT
 
@@ -17,15 +17,15 @@
 
 #### Requirements
 * Active CloudGenix Account
 * Python >= 2.7 or >=3.6
 * Python modules:
     * Requests + Security Extras >= 2.22.0- <http://docs.python-requests.org/en/master/>
     * Websockets (if Python >= 3.6) >= 8.1- <https://websockets.readthedocs.io/en/stable/index.html>
-
+    * urllib3 == 1.26.16 - <https://urllib3.readthedocs.io/en/stable/>
 #### Code Example
 Super-simplified example code (rewrite of example.py in ~4 lines of code):
 
     #!python
     # Import the CloudGenix SDK API constructor and JSON response pretty printer
     from cloudgenix import API, jd
 
@@ -137,15 +137,15 @@
 """logging.getlogger object to enable debug printing via `cloudgenix.API.set_debug`"""
 
 if PYTHON36_FEATURES:
     ws_logger = logging.getLogger('websockets')
 
 
 # Version of SDK
-version = "6.2.1b1"
+version = "6.2.2b1"
 """SDK Version string"""
 __version__ = version
 
 # PyPI URL for checking for updates.
 update_info_url = "https://pypi.org/pypi/cloudgenix/json"
 """URL for checking for updates."""
 
@@ -458,14 +458,16 @@
         # except Exception as e:
         #     raise ValueError("Unable to create Requests session object: {0}.".format(e))
         api_logger.debug("DEBUG: URL: %s, SSL Verify: %s, Session: %s",
                          self.controller,
                          self.verify,
                          self._session)
 
+        print("WARNING: cloudgenix SDK will soon end support for python versions 2.x, 3.6 and below. "
+                "Please update your python environment to 3.7 or above by the end of September 2023.")
         # Websocket/Python 3.6_ features
         if PYTHON36_FEATURES:
             # Update Headers for WebSocket requests
             websocketlib_name = websockets.__name__
             websocketlib_version = websockets.version.version
             if not websocketlib_name:
                 websocketlib_name = 'websockets'
```

### Comparing `cloudgenix-6.2.1b1/cloudgenix/ca_bundle.py` & `cloudgenix-6.2.2b1/cloudgenix/ca_bundle.py`

 * *Files identical despite different names*

### Comparing `cloudgenix-6.2.1b1/cloudgenix/delete_api.py` & `cloudgenix-6.2.2b1/cloudgenix/delete_api.py`

 * *Files identical despite different names*

### Comparing `cloudgenix-6.2.1b1/cloudgenix/get_api.py` & `cloudgenix-6.2.2b1/cloudgenix/get_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -939,14 +939,44 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices".format(api_version,
                                                                             tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
+    def directoryservices_domainstatus(self, directoryservice_id, domainstatus_id, tenant_id=None, api_version="v2.0"):
+        """
+        GET Directoryservices_Domainstatus API Function
+
+          **Parameters:**:
+
+          - **directoryservice_id**: Directory Service ID
+          - **domainstatus_id**: Domain Status ID
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices/{}/domainstatus/{}".format(api_version,
+                                                                                               tenant_id,
+                                                                                               directoryservice_id,
+                                                                                               domainstatus_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "get")
+
     def directoryservices_status(self, tenant_id=None, api_version="v2.0"):
         """
         GET Directoryservices_Status API Function
 
           **Parameters:**:
 
           - **tenant_id**: Tenant ID
@@ -1131,44 +1161,14 @@
                                                                                                   site_id,
                                                                                                   element_id,
                                                                                                   dnsservice_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "get")
 
-    def directoryservices_domainstatus(self, directoryservice_id, domainstatus_id, tenant_id=None, api_version="v2.0"):
-        """
-        GET Domainstatus_Directoryservices API Function
-
-          **Parameters:**:
-
-          - **directoryservice_id**: Directory Service ID
-          - **domainstatus_id**: Domain Status ID
-          - **tenant_id**: Tenant ID
-          - **api_version**: API version to use (default v2.0)
-
-        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
-        """
-
-        if tenant_id is None and self._parent_class.tenant_id:
-            # Pull tenant_id from parent namespace cache.
-            tenant_id = self._parent_class.tenant_id
-        elif not tenant_id:
-            # No value for tenant_id.
-            raise TypeError("tenant_id is required but not set or cached.")
-        cur_ctlr = self._parent_class.controller
-
-        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices/{}/domainstatus/{}".format(api_version,
-                                                                                               tenant_id,
-                                                                                               directoryservice_id,
-                                                                                               domainstatus_id)
-
-        api_logger.debug("URL = %s", url)
-        return self._parent_class.rest_call(url, "get")
-
     def element_bgppeers_status(self, site_id, element_id, bgppeer_id, tenant_id=None, api_version="v2.1"):
         """
         GET Element_Bgppeers_Status API Function
 
           **Parameters:**:
 
           - **site_id**: Site ID
@@ -7719,15 +7719,15 @@
     correlationevents_waninterfaces = wantinterfaces_correlationevents
     """ Backwards-compatibility alias of `correlationevents_waninterfaces` to `wantinterfaces_correlationevents`"""
 
     discoveredprefixes_bgppeers = bgppeers_discoveredprefixes
     """ Backwards-compatibility alias of `discoveredprefixes_bgppeers` to `bgppeers_discoveredprefixes`"""
 
     domainstatus_directoryservices = directoryservices_domainstatus
-    """ Backwards-compatibility alias of `discoveredprefixes_bgppeers` to `bgppeers_discoveredprefixes`"""
+    """ Backwards-compatibility alias of `domainstatus_directoryservices` to `directoryservices_domainstatus`"""
 
     elementpassageconfigs_e = elementpassageconfigs
     """ Backwards-compatibility alias of `elementpassageconfigs_e` to `elementpassageconfigs`"""
 
     elementpassageconfigs_t = tenant_elementpassageconfigs
     """ Backwards-compatibility alias of `elementpassageconfigs_t` to `tenant_elementpassageconfigs`"""
```

### Comparing `cloudgenix-6.2.1b1/cloudgenix/interactive.py` & `cloudgenix-6.2.2b1/cloudgenix/interactive.py`

 * *Files identical despite different names*

### Comparing `cloudgenix-6.2.1b1/cloudgenix/patch_api.py` & `cloudgenix-6.2.2b1/cloudgenix/patch_api.py`

 * *Files identical despite different names*

### Comparing `cloudgenix-6.2.1b1/cloudgenix/post_api.py` & `cloudgenix-6.2.2b1/cloudgenix/post_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1268,14 +1268,74 @@
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices".format(api_version,
                                                                             tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
+    def directoryservices_deltasync(self, data, tenant_id=None, api_version="v2.0"):
+        """
+        POST Directoryservices_Deltasync API Function
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices/deltasync".format(api_version,
+                                                                                      tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
+    def directoryservices_sync(self, data, tenant_id=None, api_version="v2.0"):
+        """
+        POST Directoryservices_Sync API Function
+
+          **Parameters:**:
+
+          - **data**: Dictionary containing data to POST as JSON
+          - **tenant_id**: Tenant ID
+          - **api_version**: API version to use (default v2.0)
+
+          **Payload Attributes:** 
+
+
+        **Returns:** requests.Response object extended with cgx_status and cgx_content properties.
+        """
+
+        if tenant_id is None and self._parent_class.tenant_id:
+            # Pull tenant_id from parent namespace cache.
+            tenant_id = self._parent_class.tenant_id
+        elif not tenant_id:
+            # No value for tenant_id.
+            raise TypeError("tenant_id is required but not set or cached.")
+        cur_ctlr = self._parent_class.controller
+
+        url = str(cur_ctlr) + "/{}/api/tenants/{}/directoryservices/sync".format(api_version,
+                                                                                 tenant_id)
+
+        api_logger.debug("URL = %s", url)
+        return self._parent_class.rest_call(url, "post", data=data)
+
     def directoryusergroups_query(self, data, tenant_id=None, api_version="v2.0"):
         """
         POST Directoryusergroups_Query API Function
 
           **Parameters:**:
 
           - **data**: Dictionary containing data to POST as JSON
@@ -2862,32 +2922,38 @@
                    - **csum:**  Type: boolean 
                    - **keepalive_enable:**  Type: boolean 
                    - **keepalive_fail_count:**  Type: integer 
                    - **keepalive_interval:**  Type: integer 
                - **ipsec_config:**           
                    - **authentication:**           
                        - **certificate:**  Type: string 
+                       - **certificate_profile_id:**  Type: string 
+                       - **comment:**  Type: string 
                        - **ikev1_params:**           
                            - **xauth_id:**  Type: string 
                            - **xauth_secret:**  Type: string 
                            - **xauth_secret_encrypted:**  Type: string 
                            - **xauth_secret_hash:**  Type: string 
                            - **xauth_type:**  Type: string 
                        - **local_ca_certificate:**  Type: string 
                        - **local_id:**  Type: string 
                        - **local_id_custom:**  Type: string 
+                       - **pa_master_key_id:**  Type: string 
                        - **passphrase:**  Type: string 
                        - **passphrase_encrypted:**  Type: string 
+                       - **peer_id_check:**  Type: string 
+                       - **permit_peer_id_mismatch:**  Type: boolean 
                        - **private_key:**  Type: string 
                        - **private_key_encrypted:**  Type: string 
                        - **remote_ca_certificate:**  Type: string 
                        - **remote_id:**  Type: string 
                        - **secret:**  Type: string 
                        - **secret_encrypted:**  Type: string 
                        - **secret_hash:**  Type: string 
+                       - **strict_validation_peer_extended_key_use:**  Type: boolean 
                        - **type:**  Type: string 
                        - **x509Objects:**           
                            - **certHolder:**  Type: object 
                            - **certificate:**  Type: string 
                            - **is_local_ca_cert_set:**  Type: boolean 
                            - **is_remote_ca_cert_set:**  Type: boolean 
                            - **keyPair:**  Type: object 
@@ -3588,32 +3654,38 @@
           - **tenant_id**: Tenant ID
           - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **authentication:**           
                - **certificate:**  Type: string 
+               - **certificate_profile_id:**  Type: string 
+               - **comment:**  Type: string 
                - **ikev1_params:**           
                    - **xauth_id:**  Type: string 
                    - **xauth_secret:**  Type: string 
                    - **xauth_secret_encrypted:**  Type: string 
                    - **xauth_secret_hash:**  Type: string 
                    - **xauth_type:**  Type: string 
                - **local_ca_certificate:**  Type: string 
                - **local_id:**  Type: string 
                - **local_id_custom:**  Type: string 
+               - **pa_master_key_id:**  Type: string 
                - **passphrase:**  Type: string 
                - **passphrase_encrypted:**  Type: string 
+               - **peer_id_check:**  Type: string 
+               - **permit_peer_id_mismatch:**  Type: boolean 
                - **private_key:**  Type: string 
                - **private_key_encrypted:**  Type: string 
                - **remote_ca_certificate:**  Type: string 
                - **remote_id:**  Type: string 
                - **secret:**  Type: string 
                - **secret_encrypted:**  Type: string 
                - **secret_hash:**  Type: string 
+               - **strict_validation_peer_extended_key_use:**  Type: boolean 
                - **type:**  Type: string 
                - **x509Objects:**           
                    - **certHolder:**  Type: object 
                    - **certificate:**  Type: string 
                    - **is_local_ca_cert_set:**  Type: boolean 
                    - **is_remote_ca_cert_set:**  Type: boolean 
                    - **keyPair:**  Type: object 
@@ -3625,24 +3697,34 @@
                    - **remote_ca_certs_set:**  [Type: object] 
            - **description:**  Type: string 
            - **dpd_delay:**  Type: integer 
            - **dpd_enable:**  Type: boolean 
            - **dpd_timeout:**  Type: integer 
            - **esp_group:**           
                - **force_encapsulation:**  Type: boolean 
+               - **lifesize:**           
+                   - **units:**  Type: string 
+                   - **value:**  Type: integer 
                - **lifetime:**  Type: integer 
+               - **lifetime_units:**  Type: string 
                - **mode:**  Type: string 
                - **proposals:**           
                    - **dh_groups:**  Type: string 
                    - **encryption:**  Type: string 
                    - **hash:**  Type: string 
+               - **responder_sase_proposals:**           
+                   - **dh_group:**  [Type: string] 
+                   - **encryption:**  [Type: string] 
+                   - **hash:**  [Type: string] 
            - **ike_group:**           
                - **aggressive:**  Type: boolean 
+               - **authentication_multiple:**  Type: integer 
                - **key_exchange:**  Type: string 
                - **lifetime:**  Type: integer 
+               - **lifetime_units:**  Type: string 
                - **port:**  Type: integer 
                - **proposals:**           
                    - **dh_groups:**  Type: string 
                    - **encryption:**  Type: string 
                    - **hash:**  Type: string 
                - **reauth:**  Type: boolean 
            - **name:**  Type: string 
@@ -3675,32 +3757,38 @@
           - **tenant_id**: Tenant ID
           - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **authentication:**           
                - **certificate:**  Type: string 
+               - **certificate_profile_id:**  Type: string 
+               - **comment:**  Type: string 
                - **ikev1_params:**           
                    - **xauth_id:**  Type: string 
                    - **xauth_secret:**  Type: string 
                    - **xauth_secret_encrypted:**  Type: string 
                    - **xauth_secret_hash:**  Type: string 
                    - **xauth_type:**  Type: string 
                - **local_ca_certificate:**  Type: string 
                - **local_id:**  Type: string 
                - **local_id_custom:**  Type: string 
+               - **pa_master_key_id:**  Type: string 
                - **passphrase:**  Type: string 
                - **passphrase_encrypted:**  Type: string 
+               - **peer_id_check:**  Type: string 
+               - **permit_peer_id_mismatch:**  Type: boolean 
                - **private_key:**  Type: string 
                - **private_key_encrypted:**  Type: string 
                - **remote_ca_certificate:**  Type: string 
                - **remote_id:**  Type: string 
                - **secret:**  Type: string 
                - **secret_encrypted:**  Type: string 
                - **secret_hash:**  Type: string 
+               - **strict_validation_peer_extended_key_use:**  Type: boolean 
                - **type:**  Type: string 
                - **x509Objects:**           
                    - **certHolder:**  Type: object 
                    - **certificate:**  Type: string 
                    - **is_local_ca_cert_set:**  Type: boolean 
                    - **is_remote_ca_cert_set:**  Type: boolean 
                    - **keyPair:**  Type: object 
@@ -3712,24 +3800,34 @@
                    - **remote_ca_certs_set:**  [Type: object] 
            - **description:**  Type: string 
            - **dpd_delay:**  Type: integer 
            - **dpd_enable:**  Type: boolean 
            - **dpd_timeout:**  Type: integer 
            - **esp_group:**           
                - **force_encapsulation:**  Type: boolean 
+               - **lifesize:**           
+                   - **units:**  Type: string 
+                   - **value:**  Type: integer 
                - **lifetime:**  Type: integer 
+               - **lifetime_units:**  Type: string 
                - **mode:**  Type: string 
                - **proposals:**           
                    - **dh_groups:**  Type: string 
                    - **encryption:**  Type: string 
                    - **hash:**  Type: string 
+               - **responder_sase_proposals:**           
+                   - **dh_group:**  [Type: string] 
+                   - **encryption:**  [Type: string] 
+                   - **hash:**  [Type: string] 
            - **ike_group:**           
                - **aggressive:**  Type: boolean 
+               - **authentication_multiple:**  Type: integer 
                - **key_exchange:**  Type: string 
                - **lifetime:**  Type: integer 
+               - **lifetime_units:**  Type: string 
                - **port:**  Type: integer 
                - **proposals:**           
                    - **dh_groups:**  Type: string 
                    - **encryption:**  Type: string 
                    - **hash:**  Type: string 
                - **reauth:**  Type: boolean 
            - **name:**  Type: string 
@@ -4675,15 +4773,15 @@
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
         elif not tenant_id:
             # No value for tenant_id.
             raise TypeError("tenant_id is required but not set or cached.")
-        cur_ctlr = self._parent_class.cdl_url
+        cur_ctlr = self._parent_class.controller
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/insights".format(api_version,
                                                                            tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
@@ -4705,15 +4803,15 @@
 
         if tenant_id is None and self._parent_class.tenant_id:
             # Pull tenant_id from parent namespace cache.
             tenant_id = self._parent_class.tenant_id
         elif not tenant_id:
             # No value for tenant_id.
             raise TypeError("tenant_id is required but not set or cached.")
-        cur_ctlr = self._parent_class.cdl_url
+        cur_ctlr = self._parent_class.controller
 
         url = str(cur_ctlr) + "/{}/api/tenants/{}/monitor/insightslist".format(api_version,
                                                                                tenant_id)
 
         api_logger.debug("URL = %s", url)
         return self._parent_class.rest_call(url, "post", data=data)
 
@@ -12043,14 +12141,17 @@
 
     change_password = password_change
     """ Backwards-compatibility alias of `change_password` to `password_change`"""
 
     configs_sdwanapps = sdwanapps_configs
     """ Backwards-compatibility alias of `configs_sdwanapps` to `sdwanapps_configs`"""
 
+    deltasync_directoryservices = directoryservices_deltasync
+    """ Backwards-compatibility alias of `deltasync_directoryservices` to `directoryservices_deltasync`"""
+
     extensions_i = element_extensions
     """ Backwards-compatibility alias of `extensions_i` to `element_extensions`"""
 
     extensions_s = site_extensions
     """ Backwards-compatibility alias of `extensions_s` to `site_extensions`"""
 
     extensions_ws = ws_extensions
@@ -12541,14 +12642,17 @@
 
     rquery_vfflicensesstatus = vfflicensesstatus_rquery
     """ Backwards-compatibility alias of `rquery_vfflicensesstatus` to `vfflicensesstatus_rquery`"""
 
     summary_events = events_summary
     """ Backwards-compatibility alias of `summary_events` to `events_summary`"""
 
+    sync_directoryservices = directoryservices_sync
+    """ Backwards-compatibility alias of `sync_directoryservices` to `directoryservices_sync`"""
+
     sys_metrics_monitor = monitor_sys_metrics
     """ Backwards-compatibility alias of `sys_metrics_monitor` to `monitor_sys_metrics`"""
 
     sys_point_metrics_monitor = monitor_sys_point_metrics
     """ Backwards-compatibility alias of `sys_point_metrics_monitor` to `monitor_sys_point_metrics`"""
 
     tokens_vfflicenses = vfflicense_tokens
```

### Comparing `cloudgenix-6.2.1b1/cloudgenix/put_api.py` & `cloudgenix-6.2.2b1/cloudgenix/put_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1882,32 +1882,38 @@
                    - **csum:**  Type: boolean 
                    - **keepalive_enable:**  Type: boolean 
                    - **keepalive_fail_count:**  Type: integer 
                    - **keepalive_interval:**  Type: integer 
                - **ipsec_config:**           
                    - **authentication:**           
                        - **certificate:**  Type: string 
+                       - **certificate_profile_id:**  Type: string 
+                       - **comment:**  Type: string 
                        - **ikev1_params:**           
                            - **xauth_id:**  Type: string 
                            - **xauth_secret:**  Type: string 
                            - **xauth_secret_encrypted:**  Type: string 
                            - **xauth_secret_hash:**  Type: string 
                            - **xauth_type:**  Type: string 
                        - **local_ca_certificate:**  Type: string 
                        - **local_id:**  Type: string 
                        - **local_id_custom:**  Type: string 
+                       - **pa_master_key_id:**  Type: string 
                        - **passphrase:**  Type: string 
                        - **passphrase_encrypted:**  Type: string 
+                       - **peer_id_check:**  Type: string 
+                       - **permit_peer_id_mismatch:**  Type: boolean 
                        - **private_key:**  Type: string 
                        - **private_key_encrypted:**  Type: string 
                        - **remote_ca_certificate:**  Type: string 
                        - **remote_id:**  Type: string 
                        - **secret:**  Type: string 
                        - **secret_encrypted:**  Type: string 
                        - **secret_hash:**  Type: string 
+                       - **strict_validation_peer_extended_key_use:**  Type: boolean 
                        - **type:**  Type: string 
                        - **x509Objects:**           
                            - **certHolder:**  Type: object 
                            - **certificate:**  Type: string 
                            - **is_local_ca_cert_set:**  Type: boolean 
                            - **is_remote_ca_cert_set:**  Type: boolean 
                            - **keyPair:**  Type: object 
@@ -2260,32 +2266,38 @@
           - **tenant_id**: Tenant ID
           - **api_version**: API version to use (default v2.1)
 
           **Payload Attributes:** 
 
            - **authentication:**           
                - **certificate:**  Type: string 
+               - **certificate_profile_id:**  Type: string 
+               - **comment:**  Type: string 
                - **ikev1_params:**           
                    - **xauth_id:**  Type: string 
                    - **xauth_secret:**  Type: string 
                    - **xauth_secret_encrypted:**  Type: string 
                    - **xauth_secret_hash:**  Type: string 
                    - **xauth_type:**  Type: string 
                - **local_ca_certificate:**  Type: string 
                - **local_id:**  Type: string 
                - **local_id_custom:**  Type: string 
+               - **pa_master_key_id:**  Type: string 
                - **passphrase:**  Type: string 
                - **passphrase_encrypted:**  Type: string 
+               - **peer_id_check:**  Type: string 
+               - **permit_peer_id_mismatch:**  Type: boolean 
                - **private_key:**  Type: string 
                - **private_key_encrypted:**  Type: string 
                - **remote_ca_certificate:**  Type: string 
                - **remote_id:**  Type: string 
                - **secret:**  Type: string 
                - **secret_encrypted:**  Type: string 
                - **secret_hash:**  Type: string 
+               - **strict_validation_peer_extended_key_use:**  Type: boolean 
                - **type:**  Type: string 
                - **x509Objects:**           
                    - **certHolder:**  Type: object 
                    - **certificate:**  Type: string 
                    - **is_local_ca_cert_set:**  Type: boolean 
                    - **is_remote_ca_cert_set:**  Type: boolean 
                    - **keyPair:**  Type: object 
@@ -2297,24 +2309,34 @@
                    - **remote_ca_certs_set:**  [Type: object] 
            - **description:**  Type: string 
            - **dpd_delay:**  Type: integer 
            - **dpd_enable:**  Type: boolean 
            - **dpd_timeout:**  Type: integer 
            - **esp_group:**           
                - **force_encapsulation:**  Type: boolean 
+               - **lifesize:**           
+                   - **units:**  Type: string 
+                   - **value:**  Type: integer 
                - **lifetime:**  Type: integer 
+               - **lifetime_units:**  Type: string 
                - **mode:**  Type: string 
                - **proposals:**           
                    - **dh_groups:**  Type: string 
                    - **encryption:**  Type: string 
                    - **hash:**  Type: string 
+               - **responder_sase_proposals:**           
+                   - **dh_group:**  [Type: string] 
+                   - **encryption:**  [Type: string] 
+                   - **hash:**  [Type: string] 
            - **ike_group:**           
                - **aggressive:**  Type: boolean 
+               - **authentication_multiple:**  Type: integer 
                - **key_exchange:**  Type: string 
                - **lifetime:**  Type: integer 
+               - **lifetime_units:**  Type: string 
                - **port:**  Type: integer 
                - **proposals:**           
                    - **dh_groups:**  Type: string 
                    - **encryption:**  Type: string 
                    - **hash:**  Type: string 
                - **reauth:**  Type: boolean 
            - **name:**  Type: string
```

### Comparing `cloudgenix-6.2.1b1/cloudgenix/ws_api.py` & `cloudgenix-6.2.2b1/cloudgenix/ws_api.py`

 * *Files identical despite different names*

### Comparing `cloudgenix-6.2.1b1/cloudgenix.egg-info/PKG-INFO` & `cloudgenix-6.2.2b1/cloudgenix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudgenix
-Version: 6.2.1b1
+Version: 6.2.2b1
 Summary: Python2 and Python3 SDK for the CloudGenix AppFabric
 Home-page: https://github.com/CloudGenix/sdk-python
 Author: CloudGenix Developer Support
 Author-email: developers@cloudgenix.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,27 +19,28 @@
 [![CloudGenix Logo](https://raw.githubusercontent.com/CloudGenix/sdk-python/master/docs/CloudGenix_Logo.png)](https://www.cloudgenix.com)
 
 [![image](https://img.shields.io/pypi/v/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![image](https://img.shields.io/pypi/pyversions/cloudgenix.svg)](https://pypi.org/project/cloudgenix/)
 [![Downloads](https://pepy.tech/badge/cloudgenix)](https://pepy.tech/project/cloudgenix)
 [![License: MIT](https://img.shields.io/pypi/l/cloudgenix.svg?color=brightgreen)](https://pypi.org/project/cloudgenix/)
 [![GitHub issues open](https://img.shields.io/github/issues/CloudGenix/sdk-python.svg)](https://github.com/CloudGenix/sdk-python/issues)
-# CloudGenix Python SDK v6.2.1b1
+# CloudGenix Python SDK v6.2.2b1
 Python2 and Python3 SDK for the CloudGenix AppFabric
 
 #### Synopsis
 Intended to be a small, lightweight SDK wrapper around the CloudGenix API for easy use. 
 Initial version requires knowledge of JSON/Dict objects for POST/PUT/PATCH operations.
 
 #### Requirements
 * Active CloudGenix Account
 * Python >= 2.7 or >=3.6
 * Python modules:
     * Requests + Security Extras >= 2.22.0 - <http://docs.python-requests.org/en/master/>
     * Websockets (if Python >= 3.6) >= 8.1 - <https://websockets.readthedocs.io/en/stable/index.html>
+    * urllib3 == 1.26.16 - <https://urllib3.readthedocs.io/en/stable/>
 
 #### Code Example
 Comes with `example.py` that shows usage to get a JSON list of sites.
 
 Super-simplified example code (rewrite of example.py in ~4 lines of code):
 ```python
 # Import the CloudGenix SDK API constructor and JSON response pretty printer
@@ -57,14 +58,15 @@
 
 #### License
 MIT
 
 #### Version
 | Version | Build | Changes |
 | ------- | ----- | ------- |
+| **6.2.2** | **b1** | Support for June 2023 Controller release. |
 | **6.2.1** | **b1** | Support for April 2023 Controller release. |
 | **6.1.2** | **b1** | Support for January 2023 Controller release. |
 | **6.1.1** | **b1** | Support for November 2022 Controller release. |
 | **6.0.2** | **b1** | Support for August 2022 Controller release. |
 | **6.0.1** | **b1** | Support for June 2022 Controller release. |
 | **5.6.1** | **b2** | Minor bugfix. |
 |           | **b1** | Support for Sept 2021 Controller release. |
```

### Comparing `cloudgenix-6.2.1b1/setup.py` & `cloudgenix-6.2.2b1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='cloudgenix',
-      version='6.2.1b1',
+      version='6.2.2b1',
       description='Python2 and Python3 SDK for the CloudGenix AppFabric',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/CloudGenix/sdk-python',
       author='CloudGenix Developer Support',
       author_email='developers@cloudgenix.com',
       license='MIT',
       install_requires=[
             'requests[security] >= 2.22.0',
-            'websockets >= 8.1; python_version >= "3.6"'
+            'websockets >= 8.1; python_version >= "3.6"',
+            'urllib3 == 1.26.16'
       ],
       packages=['cloudgenix'],
       classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Intended Audience :: Developers",
             "License :: OSI Approved :: MIT License",
             "Programming Language :: Python :: 2.7",
```

