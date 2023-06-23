# Comparing `tmp/pyxecm-0.0.18.tar.gz` & `tmp/pyxecm-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.0.18.tar", last modified: Mon May 22 11:45:37 2023, max compression
+gzip compressed data, was "pyxecm-0.0.19.tar", last modified: Fri Jun 23 05:26:26 2023, max compression
```

## Comparing `pyxecm-0.0.18.tar` & `pyxecm-0.0.19.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:37.626434 pyxecm-0.0.18/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-22 11:45:09.000000 pyxecm-0.0.18/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1680 2023-05-22 11:45:37.625434 pyxecm-0.0.18/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-05-22 11:45:09.000000 pyxecm-0.0.18/README.md
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-22 11:45:22.000000 pyxecm-0.0.18/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:37.623434 pyxecm-0.0.18/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    33694 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)    15046 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/llm.py
--rw-rw-rw-   0 root         (0) root         (0)    77524 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/m365.py
--rw-rw-rw-   0 root         (0) root         (0)    50994 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/main.py
--rw-rw-rw-   0 root         (0) root         (0)     9554 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   256092 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   117829 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1627 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10240 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)   250685 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/payload.py
--rw-rw-rw-   0 root         (0) root         (0)     5986 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/sap.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/translate.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:37.625434 pyxecm-0.0.18/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1680 2023-05-22 11:45:37.000000 pyxecm-0.0.18/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-22 11:45:37.000000 pyxecm-0.0.18/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 11:45:37.000000 pyxecm-0.0.18/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-22 11:45:37.000000 pyxecm-0.0.18/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 11:45:37.000000 pyxecm-0.0.18/pyxecm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 11:45:37.626434 pyxecm-0.0.18/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-22 11:45:09.000000 pyxecm-0.0.18/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:26:26.130016 pyxecm-0.0.19/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-06-23 05:25:58.000000 pyxecm-0.0.19/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-06-23 05:26:26.130016 pyxecm-0.0.19/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      854 2023-06-23 05:25:58.000000 pyxecm-0.0.19/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2023-06-23 05:26:16.000000 pyxecm-0.0.19/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:26:26.127016 pyxecm-0.0.19/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/assoc.py
+-rw-rw-rw-   0 root         (0) root         (0)    33694 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)    77794 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/m365.py
+-rw-rw-rw-   0 root         (0) root         (0)    51479 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     9554 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   256466 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   129349 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1627 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    10240 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)   297179 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/payload.py
+-rw-rw-rw-   0 root         (0) root         (0)     5986 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/sap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/translate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    21850 2023-06-23 05:25:58.000000 pyxecm-0.0.19/pyxecm/xml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 05:26:26.129016 pyxecm-0.0.19/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-06-23 05:26:26.000000 pyxecm-0.0.19/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      424 2023-06-23 05:26:26.000000 pyxecm-0.0.19/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 05:26:26.000000 pyxecm-0.0.19/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-06-23 05:26:26.000000 pyxecm-0.0.19/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-23 05:26:26.000000 pyxecm-0.0.19/pyxecm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 05:26:26.130016 pyxecm-0.0.19/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-23 05:25:58.000000 pyxecm-0.0.19/setup.py
```

### Comparing `pyxecm-0.0.18/LICENSE` & `pyxecm-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.18/PKG-INFO` & `pyxecm-0.0.19/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.18
+Version: 0.0.19
 Summary: A Python library to interact with Opentext Extended ECM REST API
-Home-page: https://pypi.org/project/pyxecm/
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
-Project-URL: Homepage, https://github.com/opentext/pyxecm
-Keywords: opentext extendedecm contentserver otds appworks archivecenter
+Project-URL: Homepage, https://gitlab.otxlab.net/ecm/pyxecm
+Keywords: opentext,extendedecm,contentserver,otds,appworks,archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PYXECM
 
-A python library to interact with Opentext Extended ECM REST API.
+A python library to interact with Opentext Extended ECM REST API. 
 API documentation is available on [OpenText Developer](https://developer.opentext.com/ce/products/extendedecm)
 
 
 # Disclaimer
 
 Copyright © 2023 Open Text Corporation, All Rights Reserved.
 The above copyright notice and this permission notice shall be included in all
```

### Comparing `pyxecm-0.0.18/README.md` & `pyxecm-0.0.19/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PYXECM
 
-A python library to interact with Opentext Extended ECM REST API.
+A python library to interact with Opentext Extended ECM REST API. 
 API documentation is available on [OpenText Developer](https://developer.opentext.com/ce/products/extendedecm)
 
 
 # Disclaimer
 
 Copyright © 2023 Open Text Corporation, All Rights Reserved.
 The above copyright notice and this permission notice shall be included in all
```

### Comparing `pyxecm-0.0.18/pyproject.toml` & `pyxecm-0.0.19/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,28 @@
   build-backend = "setuptools.build_meta"
   requires = ["setuptools >= 61.0"]
 
 [project]
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
   dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "python-hcl2", "zipfile36", "suds"]
   description = "A Python library to interact with Opentext Extended ECM REST API"
+  keywords = ["opentext", "extendedecm", "contentserver", "otds", "appworks", "archivecenter"]
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.0.18"
+  version = "0.0.19"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
     name = "Dr. Marc Diefenbruch"
 
   [project.urls]
-    Homepage = "https://github.com/opentext/pyxecm"
+    Homepage = "https://gitlab.otxlab.net/ecm/pyxecm"
+
+[tool]
+
+  [tool.setuptools]
+    packages = ["pyxecm"]
```

### Comparing `pyxecm-0.0.18/pyxecm/k8s.py` & `pyxecm-0.0.19/pyxecm/k8s.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.18/pyxecm/m365.py` & `pyxecm-0.0.19/pyxecm/m365.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
            not set or is empty it just converts the response_object to a dict using
            the vars() built-in method.
 
         Args:
             response_object (object): this is reponse object delivered by the request call
             additional_error_message (string, optional): use a more specific error message
                                                          in case of an error
-            show_error (boolean): True: write an error to the log file 
+            show_error (boolean): True: write an error to the log file
                                   False: write a warning to the log file
         Returns:
             dictionary: response information or None in case of an error
         """
 
         if not response_object:
             return None
@@ -492,15 +492,15 @@
                     )
                 else:
                     logger.info("User -> {} not found.".format(user_email))
                 return None
 
     # end method definition
 
-    def getGroups(self):
+    def getGroups(self, max_number: int = 250):
         """Get list all all groups in M365 tenant
 
         Args:
             None
         Returns:
             List of all groups.
         """
@@ -508,15 +508,17 @@
         request_url = self.config()["groupsUrl"]
         request_header = self.requestHeader()
 
         logger.info("Get list of all groups; calling -> {}".format(request_url))
 
         retries = 0
         while True:
-            response = requests.get(request_url, headers=request_header)
+            response = requests.get(
+                request_url, headers=request_header, params={"$top": str(max_number)}
+            )
             if response.ok:
                 return self.parseRequestResponse(response)
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 request_header = self.requestHeader()
@@ -986,18 +988,23 @@
             pattern_list (list): list of patterns for group names to be deleted
                                  (regular expression)
         Returns:
             boolean: True if teams have been deleted, False otherwise.
         """
 
         # Get list of all existing M365 groups/teams:
-        response = self.getGroups()
+        response = self.getGroups(max_number=500)
         if not "value" in response or not response["value"]:
             return False
         groups = response["value"]
+        logger.info(
+            "Found -> {} existing M365 groups. Checking which ones should be deleted...".format(
+                len(groups)
+            )
+        )
 
         # Process all groups and check if the< should be
         # deleted:
         for group in groups:
             group_name = group["displayName"]
             # Check if group is in exception list:
             if group_name in exception_list:
```

### Comparing `pyxecm-0.0.18/pyxecm/main.py` & `pyxecm-0.0.19/pyxecm/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,14 @@
 
 # Global variables for OTCS replicas
 otcs_replicas_frontend = 0
 otcs_replicas_backend = 0
 
 # global Logging LEVEL environment variable
 # This produces debug-level output in pod logging
-# and also activates stop_on_error parameter
-# in processTransportPackages()
 LOGLEVEL = os.environ.get("LOGLEVEL", "INFO")
 
 # The following CUST artifacts are created by the main.tf in the python module:
 CUST_BASE_DIR = ""  # change this if you run / test locally
 CUST_APP_DIR = CUST_BASE_DIR + "/app/"
 CUST_SETTINGS_DIR = CUST_BASE_DIR + "/settings/"
 CUST_PAYLOAD_DIR = CUST_BASE_DIR + "/payload/"
@@ -91,28 +89,28 @@
 OTCS_PUBLIC_PROTOCOL = os.environ.get("OTCS_PUBLIC_PROTOCOL", "https")
 OTCS_HOSTNAME = OTCS_HOSTNAME_BACKEND = os.environ.get("OTCS_HOSTNAME", "otcs-admin-0")
 OTCS_HOSTNAME_FRONTEND = os.environ.get("OTCS_HOSTNAME_FRONTEND", "otcs-frontend")
 OTCS_PUBLIC_URL = os.environ.get("OTCS_PUBLIC_URL", "otcs.xecm.dev")
 OTCS_PORT = OTCS_PORT_BACKEND = os.environ.get("OTCS_SERVICE_PORT_OTCS", 8080)
 OTCS_PORT_FRONTEND = 80
 OTCS_ADMIN = os.environ.get("OTCS_ADMIN", "admin")
+OTCS_PASSWORD = os.environ.get("OTCS_PASSWORD", "Opentext1!")
 OTCS_PARTITION = os.environ.get("OTCS_PARTITION", "Content Server Members")
 OTCS_RESOURCE_NAME = "cs"
 OTCS_K8S_STATEFUL_SET_FRONTEND = "otcs-frontend"
 OTCS_K8S_STATEFUL_SET_BACKEND = "otcs-admin"
 OTCS_K8S_INGRESS = "otxecm-ingress"
 OTCS_MAINTENANCE_MODE = (
     os.environ.get("OTCS_MAINTENANCE_MODE", "true").lower() == "true"
 )
 OTCS_LICENSE_FEATURE = "X3"
 
 # K8s service name for maintenance pod
 OTCS_MAINTENANCE_SERVICE_NAME = "maintenance"
 OTCS_MAINTENANCE_SERVICE_PORT = 80  # K8s service name for maintenance pod
-OTCS_PASSWORD = os.environ.get("OTCS_PASSWORD", "Opentext1!")
 
 # Archive Center constants:
 OTAC_ENABLED = os.environ.get("OTAC_ENABLED", True)
 OTAC_HOSTNAME = os.environ.get("OTAC_SERVICE_HOST", "otac-0")
 OTAC_PORT = os.environ.get("OTAC_SERVICE_PORT", 8080)
 OTAC_PROTOCOL = os.environ.get("OTAC_PROTOCOL", "http")
 OTAC_PUBLIC_URL = os.environ.get("OTAC_PUBLIC_URL", "otcs.xecm.dev")
@@ -472,14 +470,17 @@
         otcs_resource[
             "logoutURL"
         ] = f"{OTAWP_PUBLIC_PROTOCOL}://{OTAWP_PUBLIC_URL}/home/system/wcp/sso/sso_logout.htm"
         otcs_resource["logoutMethod"] = "GET"
 
         otds_object.updateResource(name="cs", resource=otcs_resource)
 
+    # Allow impersonation of the resource for all users:
+    otds_object.impersonateResource(resource_name)
+
     return otcs_object
 
     # end function definition
 
 
 def initOTIV(otds_object: object) -> object:
     """Initialize the OTIV (Intelligent Viewing) object and its OTDS settings.
@@ -831,15 +832,15 @@
             )
         )
 
     awp_resource_id = awp_resource["resourceID"]
 
     logger.info("OTDS resource ID for AppWorks Platform -> {}".format(awp_resource_id))
 
-    placeholder_values["OTAWP_RESSOURCE_ID"] = str(awp_resource_id)
+    placeholder_values["OTAWP_RESOURCE_ID"] = str(awp_resource_id)
 
     logger.debug("Placeholder values after OTAWP init = {}".format(placeholder_values))
 
     logger.info("Update AppWorks Kubernetes Config Map with OTDS resource IDs...")
 
     config_map = k8s_object.getConfigMap(OTAWP_K8S_CONFIGMAP)
     if not config_map:
@@ -929,14 +930,16 @@
     Returns:
         None
     """
 
     global otcs_replicas_frontend
     global otcs_replicas_backend
 
+    logger.info("Restart OTCS frontend and backend pods...")
+
     # Restart all frontends:
     for x in range(0, otcs_replicas_frontend):
         pod_name = OTCS_K8S_STATEFUL_SET_FRONTEND + "-" + str(x)
 
         logger.info("Deactivate Liveness probe for pod -> {}".format(pod_name))
         k8s_object.execPodCommand(pod_name, ["/bin/sh", "-c", "touch /tmp/keepalive"])
         logger.info("Restarting pod -> {}".format(pod_name))
@@ -978,24 +981,26 @@
 
     for x in range(0, otcs_replicas_backend):
         pod_name = OTCS_K8S_STATEFUL_SET_BACKEND + "-" + str(x)
 
         logger.info("Reactivate Liveness probe for pod -> {}".format(pod_name))
         k8s_object.execPodCommand(pod_name, ["/bin/sh", "-c", "rm /tmp/keepalive"])
 
+    logger.info("Restart OTCS frontend and backend pods has been completed.")
+
     # end function definition
 
 
 def restartOTACPod(k8s_object: object) -> bool:
     """Restart the Archive Center spawner service in OTAC pod
 
     Args:
         k8s_object (object): Kubernetes object
     Returns:
-        boolean: True if restart was done, False if error occured 
+        boolean: True if restart was done, False if error occured
     """
 
     if not OTAC_ENABLED:
         return False
 
     logger.info(
         "Restarting spawner service in Archive Center pod -> {}".format(
@@ -1131,15 +1136,15 @@
 
     if OTAWP_ENABLED == "true":  # is AppWorks Platform deployed?
         logger.info("========== Initialize OTAWP =============")
 
         # Configure required OTDS resources as AppWorks doesn't do this on its own:
         initOTAWP(otds_object, k8s_object)
     else:
-        placeholder_values["OTAWP_RESSOURCE_ID"] = ""
+        placeholder_values["OTAWP_RESOURCE_ID"] = ""
 
     if O365_ENABLED == "true":  # is M365 enabled?
         logger.info("======== Initialize MS Graph API ========")
 
         # Initialize the M365 object and connection to M365 Graph API:
         m365_object = initM365()
     else:
@@ -1247,25 +1252,26 @@
         # Open the payload file. If this fails we bail out:
         logger.info("Starting processing of payload -> {}".format(cust_payload))
 
         # Set startTime for duration calculation
         totalStartTime = datetime.now()
 
         payload_object = payload.Payload(
-            cust_payload,
-            CUST_SETTINGS_DIR,
-            k8s_object,
-            otds_object,
-            otac_object,
-            otcs_backend_object,
-            otcs_frontend_object,
-            otiv_object,
-            m365_object,
-            placeholder_values,
-            True if LOGLEVEL == "DEBUG" else False,
+            payload_source=cust_payload,
+            custom_settings_dir=CUST_SETTINGS_DIR,
+            k8s_object=k8s_object,
+            otds_object=otds_object,
+            otac_object=otac_object,
+            otcs_backend_object=otcs_backend_object,
+            otcs_frontend_object=otcs_frontend_object,
+            otcs_restart_callback=restartOTCSPods,
+            otiv_object=otiv_object,
+            m365_object=m365_object,
+            placeholder_values=placeholder_values, # this dict includes placeholder replacements for the Ressource IDs of OTAWP and OTCS
+            stop_on_error=True if LOGLEVEL == "DEBUG" else False,
         )
         # Load the payload file and initialize the payload sections:
         if not payload_object.initPayload():
             logger.error(
                 "Failed to initialize payload -> {} - skipping...".format(cust_payload)
             )
             continue
@@ -1328,19 +1334,19 @@
             "otcs",
             OTCS_HOSTNAME_FRONTEND,
             OTCS_PORT_FRONTEND,
         )
         logger.info("OTCS frontend is now back in Production Mode!")
 
     # Restart OTCS frontend and backend pods:
-    logger.info("Restart OTCS frontend and backend pods...")
-    restartOTCSPods(otcs_backend_object, k8s_object)
-    # give some additional time to make sure service is responsive
-    time.sleep(30)
-    logger.info("Restart OTCS frontend and backend pods has been completed.")
+    # logger.info("Restart OTCS frontend and backend pods...")
+    # restartOTCSPods(otcs_backend_object, k8s_object)
+    # # give some additional time to make sure service is responsive
+    # time.sleep(30)
+    # logger.info("Restart OTCS frontend and backend pods has been completed.")
 
     # Restart AppWorksPlatform pod if it is deployed (to make settings effective):
     if OTAWP_ENABLED == "true":  # is AppWorks Platform deployed?
         logger.info("Restart OTAWP pod...")
         restartOTAWPPod(k8s_object)
 
     # Upload log file for later review to "Deployment" folder in "Administration" folder
```

### Comparing `pyxecm-0.0.18/pyxecm/otac.py` & `pyxecm-0.0.19/pyxecm/otac.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.18/pyxecm/otcs.py` & `pyxecm-0.0.19/pyxecm/otcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,14 @@
 addExternalSystemConnection: Add Extended ECM external system connection
 
 createTransportWorkbench: Create a Workbench in the Transport Volume
 unpackTransportPackage: Unpack an existing Transport Package into an existing Workbench
 deployWorkbench: Deploy an existing Workbench
 deployTransport: Main method to deploy a transport. This uses subfunctions to upload,
                  unpackage and deploy the transport, and creates the required workbench
-replaceInXmlFiles: Replace all occurrences of the search pattern with the replace string in all
-                   XML files in the directory and its subdirectories.
 replaceTransportPlaceholders: Search and replace strings in the XML files of the transport packlage
 
 getWorkspaceTypes: Get all workspace types configured in Extended ECM
 getBusinessObjectType: Get information for a specific business object type
 getWorkspaceCreateForm: Get the Workspace create form
 getWorkspace: Get a workspace node
 getWorkspaceInstances: Get all instances of a given workspace type 
@@ -150,15 +148,15 @@
 import os
 import logging
 import requests
 import json
 import urllib.parse
 from datetime import datetime
 import zipfile
-import re
+from pyxecm.xml import *
 
 logger = logging.getLogger(os.path.basename(__file__))
 
 requestJsonHeaders = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/json",
 }
@@ -1702,30 +1700,37 @@
                     )
                 )
                 return None
 
     # end method definition
 
     def getNodeByParentAndName(
-        self, parent_id: int, name: str, show_error: bool = False
+        self,
+        parent_id: int,
+        name: str,
+        fields: str = "properties",
+        show_error: bool = False,
     ) -> dict:
         """Get a node based on the parent ID and name. This method does basically
            a query with "where_name" and the "result" is a list.
 
         Args:
             parent_id (integer) is the node Id of the parent node
             name (string) is the name of the node to get
+            fields (string): which fields to retrieve. This can have a big impact on performance!
             show_error (boolean, optional): treat as error if node is not found
         Returns:
             dictionary: Node information or None if no node with this name is found in parent.
                         Access to node ID with: response["results"][0]["data"]["properties"]["id"]
         """
 
         # Add query parameters (these are NOT passed via JSon body!)
         query = {"where_name": name}
+        if fields:
+            query["fields"] = fields
         encoded_query = urllib.parse.urlencode(query, doseq=True)
 
         request_url = (
             self.config()["nodesUrlv2"]
             + "/"
             + str(parent_id)
             + "/nodes?{}".format(encoded_query)
@@ -1805,15 +1810,15 @@
                 )
             )
 
         return node
 
     # end method definition
 
-    def getNodeByVolumeAndPath(self, volume_type: int, path: list) -> dict:
+    def getNodeByVolumeAndPath(self, volume_type: int, path: list = []) -> dict:
         """Get a node based on the volume and path (list of container items).
 
         Args:
             volume_type (integer): Volume type ID (default is 141 = Enterprise Workspace)
                 "Records Management"                = 550
                 "Content Server Document Templates" = 20541
                 "O365 Office Online Volume"         = 1296
@@ -1826,14 +1831,15 @@
                 "Transport Warehouse Package"       = 531
                 "Event Action Center Configuration" = 898
                 "Classification Volume"             = 198
                 "Support Asset Volume"              = 1309
                 "Physical Objects Workspace"        = 413
                 "Extended ECM"                      = 882
                 "Enterprise Workspace"              = 141
+                "Personal Workspace"                = 142
                 "Business Workspaces"               = 862
             path (list): list of container items (top down), last item is name of to be retrieved item.
                          If path is empty the node of the volume is returned.
         Returns:
             dictionary: Node information or None if no node with this path is found.
         """
 
@@ -1914,27 +1920,29 @@
         self,
         parent_node_id: int,
         filter_node_types: int = -2,
         filter_name: str = "",
         show_hidden: bool = False,
         limit: int = 100,
         page: int = 1,
+        fields: str = "properties",  # per default we just get the most important information
     ) -> dict:
         """Get a subnodes of a parent node ID.
 
         Args:
             parent_node_id (integer) is the node Id of the node
             filter_node_types (integer, optional):
                 -1 get all containers
                 -2 get all searchable objects (default)
                 -3 get all non-containers
             filter_name (string, optional): filter nodes for specific name (dfault = no filter)
             show_hidden (boolean, optional): list also hidden items (default = False)
             limit (integer, optional): maximum number of results (default = 100)
             page (integer, optional): number of result page (default = 1 = 1st page)
+            fields (string): which fields to retrieve. This can have a big impact on performance!
         Returns:
             dictionary: Subnodes information or None if no node with this parent ID is found.
         """
 
         # Add query parameters (these are NOT passed via JSon body!)
         query = {
             "where_type": filter_node_types,
@@ -1942,14 +1950,16 @@
         }
         if filter_name:
             query["where_name"] = filter_name
         if show_hidden:
             query["show_hidden"] = show_hidden
         if page > 1:
             query["page"] = page
+        if fields:
+            query["fields"] = fields
 
         encodedQuery = urllib.parse.urlencode(query, doseq=True)
 
         request_url = (
             self.config()["nodesUrlv2"]
             + "/"
             + str(parent_node_id)
@@ -2570,25 +2580,28 @@
         if not os.path.exists(directory):
             logger.error("Directory -> {} does not exist".format(directory))
             return False
 
         if not version_number:
             response = self.getLatestDocumentVersion(node_id)
             if not response:
-                logger.error("Cannot get latest version of document with ID -> {}".format(node_id))
+                logger.error(
+                    "Cannot get latest version of document with ID -> {}".format(
+                        node_id
+                    )
+                )
             version_number = response["data"]["version_number"]
 
         request_url = (
             self.config()["nodesUrlv2"]
             + "/"
             + str(node_id)
             + "/versions/"
             + str(version_number)
-            + "/content/"
-            + str(node_id)
+            + "/content"
         )
         request_header = self.requestDownloadHeader()
 
         logger.info(
             "Download document with node ID -> {}; calling -> {}".format(
                 node_id, request_url
             )
@@ -3190,15 +3203,15 @@
             )
         )
 
         # Step 4: Deploy Workbench
         logger.info("Deploy workbench -> {} ({})".format(workbench_name, workbench_id))
         response = self.deployWorkbench(workbench_id)
         if response == None:
-            logger.warning("Failed to to deploy workbench -> {}".format(workbench_name))
+            logger.error("Failed to deploy workbench -> {}".format(workbench_name))
             return None
 
         logger.info(
             "Successfully deployed workbench -> {} ({})".format(
                 workbench_name, workbench_id
             )
         )
@@ -3208,60 +3221,14 @@
             package_description,
         )
 
         return response
 
     # end method definition
 
-    def replaceInXmlFiles(
-        self, directory: str, search_pattern: str, replace_string: str
-    ) -> bool:
-        """Replaces all occurrences of the search pattern with the replace string in all XML files
-            in the directory and its subdirectories.
-
-        Args:
-            directory (string): directory to traverse for XML files
-            search_pattern (sting): string to search in the XML file
-            replace_string (string): replacement string
-        Returns:
-            boolean: True if a replacement happened, False otherwise
-        """
-        # Define the regular expression pattern to search for
-        pattern = re.compile(search_pattern)
-        found = False
-
-        # Traverse the directory and its subdirectories
-        for subdir, dirs, files in os.walk(directory):
-            for file in files:
-                # Check if the file is an XML file
-                if file.endswith(".xml"):
-                    # Read the contents of the file
-                    file_path = os.path.join(subdir, file)
-                    with open(file_path, "r") as f:
-                        contents = f.read()
-
-                    # Replace all occurrences of the search pattern with the replace string
-                    new_contents = pattern.sub(replace_string, contents)
-
-                    # Write the updated contents to the file if there were replacements
-                    if contents != new_contents:
-                        logger.info(
-                            "Found search string -> {} in XML file -> {}. Updating content...".format(
-                                search_pattern, file_path
-                            )
-                        )
-                        # Write the updated contents to the file
-                        with open(file_path, "w") as f:
-                            f.write(new_contents)
-                        found = True
-
-        return found
-
-        # end method definition
-
     def replaceTransportPlaceholders(
         self, zip_file_path: str, replacements: list
     ) -> bool:
         """Search and replace strings in the XML files of the transport packlage
 
         Args:
             zip_file_path (string): path to transport zip file
@@ -3281,46 +3248,85 @@
         with zipfile.ZipFile(zip_file_path, "r") as zfile:
             zfile.extractall(zip_file_folder)
 
         modified = False
 
         # Replace search pattern with replace string in all XML files in the directory and its subdirectories
         for replacement in replacements:
-            if replacement["placeholder"] == replacement["value"]:
+            if not "value" in replacement:
+                logger.error("Replacement needs a value but it is not specified. Skipping...")
+                continue
+            if "enabled" in replacement and not replacement["enabled"]:
                 logger.info(
-                    "Placeholder and replacement are identical -> {}. Skipping...".format(
-                        replacement["value"]
-                    )
+                    "Replacement for transport -> {} is disabled. Skipping...".format(zip_file_path)
                 )
                 continue
-            logger.info(
-                "Replace -> {} with -> {} in Transport package -> {}".format(
-                    replacement["placeholder"], replacement["value"], zip_file_folder
+            # there are two types of replacements:
+            # 1. XPath - more elegant and powerful
+            # 2. Search & Replace - basically treat the XML file like a like file and do a search & replace
+            if "xpath" in replacement:
+                logger.info(
+                    "Using xpath -> {} to narrow down the replacement".format(
+                        replacement["xpath"]
+                    )
                 )
-            )
-            found = self.replaceInXmlFiles(
-                zip_file_folder, replacement["placeholder"], replacement["value"]
+                if "setting" in replacement:
+                    logger.info(
+                        "Looking up setting -> {} in XML element".format(
+                            replacement["setting"]
+                        )
+                    )
+                if "assoc_elem" in replacement:
+                    logger.info(
+                        "Looking up assoc element -> {} in XML element".format(
+                            replacement["assoc_elem"]
+                        )
+                    )
+            else: # we have a simple "search & replace" replacement
+                if not "placeholder" in replacement:
+                    logger.error("Replacement without an xpath needs a placeholder value but it is not specified. Skipping...")
+                    continue
+                if replacement.get("placeholder") == replacement["value"]:
+                    logger.info(
+                        "Placeholder and replacement are identical -> {}. Skipping...".format(
+                            replacement["value"]
+                        )
+                    )
+                    continue
+                logger.info(
+                    "Replace -> {} with -> {} in Transport package -> {}".format(
+                        replacement["placeholder"], replacement["value"], zip_file_folder
+                    )
+                )
+
+            found = XML.replaceInXmlFiles(
+                zip_file_folder,
+                replacement.get("placeholder"),
+                replacement["value"],
+                replacement.get("xpath"),
+                replacement.get("setting"),
+                replacement.get("assoc_elem"),
             )
             if found:
                 logger.info(
-                    "Found replacement string -> {} in Transport package -> {}".format(
-                        replacement["placeholder"], zip_file_folder
+                    "Replacement -> {} has been completed successfully for Transport package -> {}".format(
+                        replacement, zip_file_folder
                     )
                 )
                 modified = True
             else:
                 logger.warning(
-                    "Did not find replacement string -> {} in Transport package -> {}".format(
-                        replacement["placeholder"], zip_file_folder
+                    "Replacement -> {} failed for Transport package -> {}".format(
+                        replacement, zip_file_folder
                     )
                 )
 
         if not modified:
             logger.warning(
-                "None of the replacements have been found in transport -> {}".format(
+                "None of the specified replacements have been successful for Transport package -> {}. No need to create a new transport package.".format(
                     zip_file_folder
                 )
             )
             return False
 
         # Create the new zip file and add all files from the directory to it
         new_zip_file_path = (
@@ -4155,21 +4161,21 @@
         Returns:
             dictionary: Node information or None if REST call fails.
         """
 
         if not os.path.exists(file_path):
             logger.error("Workdpace icon file does not exist -> {}".format(file_path))
             return None
-        
-#        icon_file = open(file_path, "rb")
+
+        #        icon_file = open(file_path, "rb")
 
         updateWorkspaceIconPutBody = {
             "file_content_type": file_mimetype,
             "file_filename": os.path.basename(file_path),
-            "file": file_path #icon_file
+            "file": file_path,  # icon_file
         }
 
         request_url = (
             self.config()["businessworkspaces"] + "/" + str(workspace_id) + "/icons"
         )
         request_header = self.requestFormHeader()
```

### Comparing `pyxecm-0.0.18/pyxecm/otds.py` & `pyxecm-0.0.19/pyxecm/otds.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,20 @@
 authenticate : authenticates at OTDS server
 
 addLicenseToResource : Add (or update) a product license to OTDS
 getLicensesForResource : Get list of licenses for a resource
 deleteLicenseFromResource : Delete a license from a resource
 assignUserToLicense : Assign an OTDS user to a product license (feature) in OTDS.
 assignPartitionToLicense: Assign an OTDS user partition to a license (feature) in OTDS.
+getLicensedObjects: Return the licensed objects (users, groups, partitions) an OTDS for a
+                    license + license feature associated with an OTDS resource (like "cs").
+isUserLicensed: Check if a user is licensed for a license and license feature associated
+                with a particular OTDS resource.
+isPartitionLicensed: Check if a user partition is licensed for a license and license feature
+                     associated with a particular OTDS resource.
 
 addPartition : Add an OTDS partition
 getPartition : Get a partition with a specific name
 addUser : Add a user to a partion
 getUser : Get a user with a specific user ID (= login name @ partition)
 updateUser : Update attributes of on OTDS user
 deleteUser : Delete a user with a specific ID in a specific partition
@@ -401,18 +407,19 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add product license -> {} for product -> {}; error -> {}".format(
+                    "Failed to add product license -> {} for product -> {}; error -> {} ({})".format(
                         path_to_license_file,
                         product_description,
                         response.text,
+                        response.status_code,
                     )
                 )
                 return None
 
     # end method definition
 
     def getLicensesForResource(self, resource_id: str):
@@ -450,16 +457,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to get license for resource -> {}; error -> {}".format(
-                        resource_id, response.text
+                    "Failed to get license for resource -> {}; error -> {} ({})".format(
+                        resource_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def deleteLicenseFromResource(self, resource_id: str, license_id: str) -> bool:
@@ -490,16 +497,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to delete license -> {} for resource -> {}; error -> {}".format(
-                        license_id, resource_id, response.text
+                    "Failed to delete license -> {} for resource -> {}; error -> {} ({})".format(
+                        license_id, resource_id, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
     def assignUserToLicense(
@@ -580,18 +587,19 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add license feature -> {} associated with resource -> {} for user -> {}; status code -> {}".format(
+                    "Failed to add license feature -> {} associated with resource -> {} to user -> {}; error -> {} ({})".format(
                         license_feature,
                         resource_id,
                         user_id,
+                        response.text,
                         response.status_code,
                     )
                 )
                 return False
 
     # end method definition
 
@@ -612,15 +620,34 @@
             license_name (string): name of the license to assign, e.g. "EXTENDED_ECM" or "INTELLGENT_VIEWIMG"
             license_type (string, optional): deault is "Full", Extended ECM also has "Occasional"
         Returns:
             boolean: True if successful or False if the REST call fails or the license is not found
         """
 
         licenses = self.getLicensesForResource(resource_id)
+        if not licenses:
+            logger.error(
+                "Resource with ID -> {} does not exist or has no licenses".format(
+                    resource_id
+                )
+            )
+            return False
 
+        # licenses have this format:
+        # {
+        #   '_oTLicenseType': 'NON-PRODUCTION',
+        #   '_oTLicenseResource': '7382094f-a434-4714-9696-82864b6803da',
+        #   '_oTLicenseResourceName': 'cs',
+        #   '_oTLicenseProduct': 'EXTENDED_ECM',
+        #   'name': 'EXTENDED_ECM¹7382094f-a434-4714-9696-82864b6803da',
+        #   'location': 'cn=EXTENDED_ECM¹7382094f-a434-4714-9696-82864b6803da,ou=Licenses,dc=identity,dc=opentext,dc=net',
+        #   'id': 'cn=EXTENDED_ECM¹7382094f-a434-4714-9696-82864b6803da,ou=Licenses,dc=identity,dc=opentext,dc=net',
+        #   'description': 'CS license',
+        #   'values': [{...}, {...}, {...}, {...}, {...}, {...}, {...}, {...}, {...}, ...]
+        # }
         for lic in licenses:
             if lic["_oTLicenseProduct"] == license_name:
                 license_location = lic["id"]
 
         try:
             license_location
         except UnboundLocalError:
@@ -638,15 +665,19 @@
             "values": [{"name": "counter", "values": [license_feature]}],
         }
 
         request_url = self.licenseUrl() + "/object/" + license_location
 
         logger.info(
             "Assign license feature -> {} of license -> {} associated with resource -> {} to partition -> {}; calling -> {}".format(
-                license_feature, license_location, resource_id, partition_name, request_url
+                license_feature,
+                license_location,
+                resource_id,
+                partition_name,
+                request_url,
             )
         )
 
         retries = 0
         while True:
             response = requests.post(
                 request_url,
@@ -664,25 +695,266 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add license feature -> {} associated with resource -> {} for partition -> {}; status code -> {}".format(
+                    "Failed to add license feature -> {} associated with resource -> {} to partition -> {}; error -> {} ({})".format(
                         license_feature,
                         resource_id,
                         partition_name,
+                        response.text,
                         response.status_code,
                     )
                 )
                 return False
 
     # end method definition
 
+    def getLicensedObjects(
+        self,
+        resource_id: str,
+        license_feature: str,
+        license_name: str,
+    ):
+        """Return the licensed objects (users, groups, partitions) in OTDS for a license + license feature
+           associated with an OTDS resource (like "cs").
+
+        Args:
+            resource_id (string): OTDS resource ID (this is ID not the resource name!)
+            license_feature (string): name of the license feature, e.g. "X2" or "ADDON_ENGINEERING"
+            license_name (string): name of the license to assign, e.g. "EXTENDED_ECM" or "INTELLGENT_VIEWIMG"
+        Returns:
+            dict: data structure of licensed objects
+
+            Example return value:
+            {
+                'status': 0,
+                'displayString': 'Success',
+                'exceptions': None,
+                'retValue': 0,
+                'listGroupsResults': {'groups': [...], 'actualPageSize': 0, 'nextPageCookie': None, 'requestedPageSize': 250},
+                'listUsersResults': {'users': [...], 'actualPageSize': 53, 'nextPageCookie': None, 'requestedPageSize': 250},
+                'listUserPartitionResult': {'_userPartitions': [...], 'warningMessage': None, 'actualPageSize': 0, 'nextPageCookie': None, 'requestedPageSize': 250},
+                'version': 1
+            }
+        """
+
+        licenses = self.getLicensesForResource(resource_id)
+        if not licenses:
+            logger.error(
+                "Resource with ID -> {} does not exist or has no licenses".format(
+                    resource_id
+                )
+            )
+            return False
+
+        # licenses have this format:
+        # {
+        #   '_oTLicenseType': 'NON-PRODUCTION',
+        #   '_oTLicenseResource': '7382094f-a434-4714-9696-82864b6803da',
+        #   '_oTLicenseResourceName': 'cs',
+        #   '_oTLicenseProduct': 'EXTENDED_ECM',
+        #   'name': 'EXTENDED_ECM¹7382094f-a434-4714-9696-82864b6803da',
+        #   'location': 'cn=EXTENDED_ECM¹7382094f-a434-4714-9696-82864b6803da,ou=Licenses,dc=identity,dc=opentext,dc=net',
+        #   'id': 'cn=EXTENDED_ECM¹7382094f-a434-4714-9696-82864b6803da,ou=Licenses,dc=identity,dc=opentext,dc=net',
+        #   'description': 'CS license',
+        #   'values': [{...}, {...}, {...}, {...}, {...}, {...}, {...}, {...}, {...}, ...]
+        # }
+        for lic in licenses:
+            if lic["_oTLicenseProduct"] == license_name:
+                license_location = lic["location"]
+
+        try:
+            license_location
+        except UnboundLocalError:
+            logger.error(
+                "Cannot find license -> {} for resource -> {}".format(
+                    license_name, resource_id
+                )
+            )
+            return False
+
+        request_url = (
+            self.licenseUrl()
+            + "/object/"
+            + license_location
+            + "?counter="
+            + license_feature
+        )
+
+        logger.info(
+            "Get licensed objects for license -> {} and license feature -> {} associated with resource -> {}; calling -> {}".format(
+                license_name,
+                license_feature,
+                resource_id,
+                request_url,
+            )
+        )
+
+        retries = 0
+        while True:
+            response = requests.get(
+                request_url,
+                headers=requestHeaders,
+                cookies=self.cookie(),
+            )
+            if response.ok:
+                return self.parseRequestResponse(response)
+            # Check if Session has expired - then re-authenticate and try once more
+            elif response.status_code == 401 and retries == 0:
+                logger.warning("Session has expired - try to re-authenticate...")
+                self.authenticate(True)
+                retries += 1
+            else:
+                logger.error(
+                    "Failed to get licensed objects for license -> {} and license feature -> {} associated with resource -> {}; error -> {} ({})".format(
+                        license_name,
+                        license_feature,
+                        resource_id,
+                        response.text,
+                        response.status_code,
+                    )
+                )
+                return None
+
+    # end method definition
+
+    def isUserLicensed(self, user_name: str, resource_id: str, license_feature: str, license_name: str) -> bool:
+        """Check if a user is licensed for a license and license feature associated with a particular OTDS resource.
+
+        Args:
+            user_name (str): login name of the OTDS user
+            resource_id (string): OTDS resource ID (this is ID not the resource name!)
+            license_feature (string): name of the license feature, e.g. "X2" or "ADDON_ENGINEERING"
+            license_name (string): name of the license to assign, e.g. "EXTENDED_ECM" or "INTELLGENT_VIEWIMG"
+
+        Returns:
+            bool: True if the user is licensed and False otherwise
+        """
+
+        response = self.getLicensedObjects(
+            resource_id=resource_id,
+            license_feature=license_feature,
+            license_name=license_name,
+        )
+
+        if not response or not response["listUsersResults"]:
+            return False
+
+        users = response["listUsersResults"]["users"]
+
+        if not users:
+            return False
+
+        user = next(
+            (
+                item
+                for item in users
+                if item["name"] == user_name
+            ),
+            None,
+        )
+
+        if user:
+            return True
+        
+        return False
+
+    # end method definition
+
+    def isGroupLicensed(self, group_name: str, resource_id: str, license_feature: str, license_name: str) -> bool:
+        """Check if a group is licensed for a license and license feature associated with a particular OTDS resource.
+
+        Args:
+            group_name (str): name of the OTDS user group
+            resource_id (string): OTDS resource ID (this is ID not the resource name!)
+            license_feature (string): name of the license feature, e.g. "X2" or "ADDON_ENGINEERING"
+            license_name (string): name of the license to assign, e.g. "EXTENDED_ECM" or "INTELLGENT_VIEWIMG"
+
+        Returns:
+            bool: True if the group is licensed and False otherwise
+        """
+
+        response = self.getLicensedObjects(
+            resource_id=resource_id,
+            license_feature=license_feature,
+            license_name=license_name,
+        )
+
+        if not response or not response["listGroupsResults"]:
+            return False
+
+        groups = response["listGroupsResults"]["groups"]
+
+        if not groups:
+            return False
+
+        group = next(
+            (
+                item
+                for item in groups
+                if item["name"] == group_name
+            ),
+            None,
+        )
+
+        if group:
+            return True
+        
+        return False
+
+    # end method definition
+
+    def isPartitionLicensed(
+        self, partition_name: str, resource_id: str, license_feature: str, license_name: str
+    ):
+        """Check if a user is licensed for a license and license feature associated with a particular OTDS resource.
+
+        Args:
+            partition_name (str): name of the OTDS user partition, e.g. "Content Server Members"
+            resource_id (string): OTDS resource ID (this is ID not the resource name!)
+            license_feature (string): name of the license feature, e.g. "X2" or "ADDON_ENGINEERING"
+            license_name (string): name of the license to assign, e.g. "EXTENDED_ECM" or "INTELLGENT_VIEWIMG"
+
+        Returns:
+            bool: True if the partition is licensed and False otherwise
+        """
+
+        response = self.getLicensedObjects(
+            resource_id=resource_id,
+            license_feature=license_feature,
+            license_name=license_name,
+        )
+
+        if not response or not response["listUserPartitionResult"]:
+            return False
+
+        partitions = response["listUserPartitionResult"]["_userPartitions"]
+
+        if not partitions:
+            return False
+
+        partition = next(
+            (
+                item
+                for item in partitions
+                if item["name"] == partition_name
+            ),
+            None,
+        )
+
+        if partition:
+            return True
+        
+        return False
+
+    # end method definition
+
     def addPartition(self, name: str, description: str) -> dict:
         """Add a new user partition to OTDS
 
         Args:
             name (string): name of the new partition
         Returns:
             dictionary: Request response or None if the creation fails.
@@ -711,16 +983,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add user partition -> {}; error -> {}".format(
-                        name, response.text
+                    "Failed to add user partition -> {}; error -> {} ({})".format(
+                        name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def getPartition(self, name: str, show_error: bool = True) -> dict:
@@ -750,16 +1022,16 @@
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
-                        "Failed to get partition -> {}; warning -> {}".format(
-                            name, response.text
+                        "Failed to get partition -> {}; warning -> {} ({})".format(
+                            name, response.text, response.status_code
                         )
                     )
                 return None
 
     # end method definition
 
     def addUser(
@@ -817,15 +1089,17 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add user -> {}; error -> {}".format(name, response.text)
+                    "Failed to add user -> {}; error -> {} ({})".format(
+                        name, response.text, response.status_code
+                    )
                 )
                 return None
 
     # end method definition
 
     def getUser(self, partition: str, user_id: str) -> dict:
         """Get a user by its partition and user ID
@@ -855,16 +1129,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to get user -> {}; error -> {}".format(
-                        user_id, response.text
+                    "Failed to get user -> {}; error -> {} ({})".format(
+                        user_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def updateUser(
@@ -907,16 +1181,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to update user -> {}; error -> {}".format(
-                        user_id, response.text
+                    "Failed to update user -> {}; error -> {} ({})".format(
+                        user_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def deleteUser(self, partition: str, user_id: str) -> bool:
@@ -947,16 +1221,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to delete user -> {}; error -> {}".format(
-                        user_id, response.text
+                    "Failed to delete user -> {}; error -> {} ({})".format(
+                        user_id, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
     def resetUserPassword(self, user_id: str, password: str) -> bool:
@@ -992,16 +1266,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to reset password for user -> {}; error -> {}".format(
-                        user_id, response.text
+                    "Failed to reset password for user -> {}; error -> {} ({})".format(
+                        user_id, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
     def addGroup(self, partition: str, name: str, description: str) -> dict:
@@ -1043,15 +1317,17 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add group -> {}; error -> {}".format(name, response.text)
+                    "Failed to add group -> {}; error -> {} ({})".format(
+                        name, response.text, response.status_code
+                    )
                 )
                 return None
 
     # end method definition
 
     def getGroup(self, group: str) -> dict:
         """Get a OTDS group by its group name
@@ -1092,16 +1368,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to get group -> {}; error -> {}".format(
-                        group, response.text
+                    "Failed to get group -> {}; error -> {} ({})".format(
+                        group, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def addUserToGroup(self, user: str, group: str) -> bool:
@@ -1137,16 +1413,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add user -> {} to group -> {}; error -> {}".format(
-                        user, group, response.text
+                    "Failed to add user -> {} to group -> {}; error -> {} ({})".format(
+                        user, group, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
     def addGroupToParentGroup(self, group: str, parent_group: str) -> bool:
@@ -1183,16 +1459,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add group -> {} to parent group -> {}; error -> {}".format(
-                        group, parent_group, response.text
+                    "Failed to add group -> {} to parent group -> {}; error -> {} ({})".format(
+                        group, parent_group, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
     def addResource(
@@ -1245,16 +1521,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add resource -> {}; error -> {}".format(
-                        name, response.text
+                    "Failed to add resource -> {}; error -> {} ({})".format(
+                        name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def getResource(self, name: str, show_error: bool = False) -> dict:
@@ -1296,15 +1572,17 @@
                     )
                 else:
                     logger.info("Resource -> {} not found.".format(name))
                 return None
 
     # end method definition
 
-    def updateResource(self, name: str, resource: object, show_error: bool = True) -> dict:
+    def updateResource(
+        self, name: str, resource: object, show_error: bool = True
+    ) -> dict:
         """Update an existing OTDS resource
 
         Args:
             name (string): name of the new OTDS resource
             resource (object): updated resource object of getResource called before
             show_error (boolean, optional): treat as error if resource is not found
         Returns:
@@ -1375,16 +1653,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to activate resource -> {}; error -> {}".format(
-                        resource_id, response.text
+                    "Failed to activate resource -> {}; error -> {} ({})".format(
+                        resource_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def getAccessRoles(self) -> dict:
@@ -1409,15 +1687,17 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to retrieve access roles; error -> {}".format(response.text)
+                    "Failed to retrieve access roles; error -> {} ({})".format(
+                        response.text, response.status_code
+                    )
                 )
                 return None
 
     # end method definition
 
     def getAccessRole(self, name: str) -> dict:
         """Get an OTDS access role
@@ -1444,16 +1724,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to retrieve access role -> {}; error -> {}".format(
-                        name, response.text
+                    "Failed to retrieve access role -> {}; error -> {} ({})".format(
+                        name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def addPartitionToAccessRole(
@@ -1497,23 +1777,25 @@
                 return True
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add partition -> {} to access role -> {}; error -> {}".format(
-                        partition, access_role, response.text
+                    "Failed to add partition -> {} to access role -> {}; error -> {} ({})".format(
+                        partition, access_role, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
-    def addUserToAccessRole(self, access_role: str, user_id: str, location: str = "") -> bool:
+    def addUserToAccessRole(
+        self, access_role: str, user_id: str, location: str = ""
+    ) -> bool:
         """Add an OTDS user to an OTDS access role
 
         Args:
             access_role (string): name of the OTDS access role
             user_id (string): ID of the user (= login name)
             location (string, optional): this is kind of a unique identifier DN (Distinguished Name)
                                          most of the times you will want to keep it to empty string ("")
@@ -1570,23 +1852,25 @@
                 return True
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add user -> {} to access role -> {}; error -> {}".format(
-                        user_id, access_role, response.text
+                    "Failed to add user -> {} to access role -> {}; error -> {} ({})".format(
+                        user_id, access_role, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
-    def addGroupToAccessRole(self, access_role: str, group: str, location: str = "") -> bool:
+    def addGroupToAccessRole(
+        self, access_role: str, group: str, location: str = ""
+    ) -> bool:
         """Add an OTDS group to an OTDS access role
 
         Args:
             access_role (string): name of the OTDS access role
             group (string): name of the group
             location (string, optional): this is kind of a unique identifier DN (Distinguished Name)
                                          most of the times you will want to keep it to empty string ("")
@@ -1642,16 +1926,16 @@
                 return True
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add group -> {} to access role -> {}; error -> {}".format(
-                        group, access_role, response.text
+                    "Failed to add group -> {} to access role -> {}; error -> {} ({})".format(
+                        group, access_role, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
 
     def updateAccessRoleAttributes(self, name: str, attribute_list: list) -> dict:
@@ -1699,16 +1983,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to update access role -> {}; error -> {}".format(
-                        name, response.text
+                    "Failed to update access role -> {}; error -> {} ({})".format(
+                        name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def addSystemAttribute(self, name: str, value: str, description: str = "") -> dict:
@@ -1756,16 +2040,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add system attribute -> {} with value -> {}; error -> {}".format(
-                        name, value, response.text
+                    "Failed to add system attribute -> {} with value -> {}; error -> {} ({})".format(
+                        name, value, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def getTrustedSites(self) -> dict:
@@ -1791,16 +2075,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to retrieve trusted sites; error -> {}".format(
-                        response.text
+                    "Failed to retrieve trusted sites; error -> {} ({})".format(
+                        response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def addTrustedSite(self, trusted_site: str) -> dict:
@@ -1833,20 +2117,20 @@
             request_url,
             json=trustedSitePostBodyJson,
             headers=requestHeaders,
             cookies=self.cookie(),
         )
         if not response.ok:
             logger.error(
-                "Failed to add trusted site -> {}; error -> {}".format(
-                    trusted_site, response.text
+                "Failed to add trusted site -> {}; error -> {} ({})".format(
+                    trusted_site, response.text, response.status_code
                 )
             )
             return None
-        return response # don't parse it!
+        return response  # don't parse it!
 
     # end method definition
 
     def enableAudit(self):
         """enable Audit
 
         Args:
@@ -1917,15 +2201,19 @@
         response = requests.put(
             request_url,
             json=auditPutBodyJson,
             headers=requestHeaders,
             cookies=self.cookie(),
         )
         if not response.ok:
-            logger.error("Failed to enable audit; error -> {}".format(response.text))
+            logger.error(
+                "Failed to enable audit; error -> {} ({})".format(
+                    response.text, response.status_code
+                )
+            )
         return response
 
     # end method definition
 
     def addOauthClient(
         self,
         client_id: str,
@@ -1989,16 +2277,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add OAuth client -> {}; error -> {}".format(
-                        client_id, response.text
+                    "Failed to add OAuth client -> {}; error -> {} ({})".format(
+                        client_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def getOauthClient(self, client_id: str, show_error: bool = True):
@@ -2028,16 +2316,16 @@
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 if show_error:
                     logger.error(
-                        "Failed to get oauth client -> {}; error -> {}".format(
-                            client_id, response.text
+                        "Failed to get oauth client -> {}; error -> {} ({})".format(
+                            client_id, response.text, response.status_code
                         )
                     )
                 return None
 
     # end method definition
 
     def updateOauthClient(self, client_id, updates: dict):
@@ -2064,16 +2352,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to update OAuth client -> {}; error -> {}".format(
-                        client_id, response.text
+                    "Failed to update OAuth client -> {}; error -> {} ({})".format(
+                        client_id, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def addOauthClientsToAccessRole(self, access_role_name: str):
@@ -2104,16 +2392,19 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to retrieve role -> {}; url -> {} : error -> {}".format(
-                        access_role_name, accessRolesUrl, response.text
+                    "Failed to retrieve role -> {}; url -> {} : error -> {} ({})".format(
+                        access_role_name,
+                        accessRolesUrl,
+                        response.text,
+                        response.status_code,
                     )
                 )
                 return None
 
         # Checking if OAuthClients partition already added to access role
         userPartitions = accessRolesJson["accessRoleMembers"]["userPartitions"]
         for userPartition in userPartitions:
@@ -2134,16 +2425,16 @@
         if partitionsResponse.ok:
             response_dict = self.parseRequestResponse(partitionsResponse)
             if not response_dict:
                 return None
             oauthClientLocation = response_dict["location"]
         else:
             logger.error(
-                "Failed to get partition info for OAuthClients; url -> {} : error -> {}".format(
-                    oauthPartitionsUrl, partitionsResponse.text
+                "Failed to get partition info for OAuthClients; url -> {} : error -> {} ({})".format(
+                    oauthPartitionsUrl, partitionsResponse.text, response.status_code
                 )
             )
             return None
 
         # adding OAuthClients info to acess roles organizational units
         oauthClientsOuBlock = {
             "location": oauthClientLocation,
@@ -2324,16 +2615,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add SAML auth handler -> {}; error -> {}".format(
-                        name, response.text
+                    "Failed to add SAML auth handler -> {}; error -> {} ({})".format(
+                        name, response.text, response.status_code
                     )
                 )
                 return None
 
     # end method definition
 
     def addAuthHandlerSAP(
@@ -2421,16 +2712,16 @@
             request_url,
             json=authHandlerPostBodyJson,
             headers=requestHeaders,
             cookies=self.cookie(),
         )
         if not response.ok:
             logger.error(
-                "Failed to add SAP auth handler -> {}; error -> {}".format(
-                    name, response.text
+                "Failed to add SAP auth handler -> {}; error -> {} ({})".format(
+                    name, response.text, response.status_code
                 )
             )
             return None
 
         # 3. Upload the certificate file:
 
         # Check that the certificate (PSE) file is readable:
@@ -2518,16 +2809,16 @@
             request_url,
             data=authHandlerPostData,
             files=authHandlerPostFiles,
             cookies=self.cookie(),
         )
         if not response.ok:
             logger.error(
-                "Failed to upload certificate file -> {} for SAP auth handler -> {}; error -> {}".format(
-                    certificate_file, name, response.text
+                "Failed to upload certificate file -> {} for SAP auth handler -> {}; error -> {} ({})".format(
+                    certificate_file, name, response.text, response.status_code
                 )
             )
             return None
 
         return response
 
     # end method definition
@@ -2923,16 +3214,16 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to add OAuth auth handler -> {}; error -> {}".format(
-                        name, response.text
+                    "Failed to add OAuth auth handler -> {}; error -> {} ({})".format(
+                        name, response.text, response.status_code
                     )
                 )
                 return None
 
         # end method definition
 
     def consolidate(self, resource_name: str) -> bool:
@@ -2943,16 +3234,16 @@
         Returns:
             boolean: True if the consolidation succeeded or False if it failed.
         """
 
         resource = self.getResource(resource_name)
         if not resource:
             logger.error(
-                "Resource -> {} not found - cannot consolidate; error -> {}".format(
-                    resource_name
+                "Resource -> {} not found - cannot consolidate; error -> {} ({})".format(
+                    resource_name, response.text, response.status_code
                 )
             )
             return False
 
         resourceDN = resource["resourceDN"]
         if not resourceDN:
             logger.error("Resource DN is empty - cannot consolidate")
@@ -2985,15 +3276,19 @@
                 return True
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
-                logger.error("Failed to consolidate; error -> {}".format(response.text))
+                logger.error(
+                    "Failed to consolidate; error -> {} ({})".format(
+                        response.text, response.status_code
+                    )
+                )
                 return False
 
     # end method definition
 
     def impersonateResource(
         self,
         resource_name: str,
@@ -3090,14 +3385,14 @@
             # Check if Session has expired - then re-authenticate and try once more
             elif response.status_code == 401 and retries == 0:
                 logger.warning("Session has expired - try to re-authenticate...")
                 self.authenticate(True)
                 retries += 1
             else:
                 logger.error(
-                    "Failed to set impersonation for OAuth Client -> {}; error -> {}".format(
-                        client_id, response.text
+                    "Failed to set impersonation for OAuth Client -> {}; error -> {} ({})".format(
+                        client_id, response.text, response.status_code
                     )
                 )
                 return False
 
     # end method definition
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyxecm-0.0.18/pyxecm/otiv.py` & `pyxecm-0.0.19/pyxecm/otiv.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.18/pyxecm/otpd.py` & `pyxecm-0.0.19/pyxecm/otpd.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.18/pyxecm/payload.py` & `pyxecm-0.0.19/pyxecm/payload.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,32 +26,39 @@
 Class: Payload
 Methods:
 
 __init__ : class initializer
 replacePlaceholders: replace placeholder in admin config files
 initPayload: load and initialize the YAML payload
 getPayloadSection: delivers a section of the payload as a list of settings
+getAllGroupNames: construct a list of all group name
+checkStatusFile: check if the payload section has been processed before
+writeStatusFile: Write a status file into the Admin Personal Workspace in Extended ECM
+                 to indicate that the payload section has been deployed successfully
+determineGroupID: determine the id of a group - either from payload or from OTCS
+determineUserID: determine the id of a user - either from payload or from OTCS
+determineWorkspaceID: determine the nodeID of a workspace - either from payload or from OTCS
 
 processPayload: process payload (main method)
 processWebHooks: process list of web hooks
 processPartitions: process the OTDS partitions
+processPartitionLicenses: process the licenses that should be assigned to OTDS partitions (this includes existing partitions)
 processOAuthClients: process the OTDS OAuth clients
 processTrustedSites: process the OTDS trusted sites
 processSystemAttributes: process the OTDS system attributes
 processGroups: process Extended ECM user groups
 processGroupsM365: process M365 user groups
 processUsers: process Extended ECM users
 processUsersM365: process M365 users
 processAdminSettings: process Extended ECM administration settings (LLConfig)
 processExternalSystems: process Extended ECM external systems
 processTransportPackages: process Extended ECM transport packages
 processUserPhotos: process Extended ECM user photos (user profile)
 processUserPhotosM365: process user photos in payload and assign them to Microsoft 365 users.
 processWorkspaceTypes: process Extended ECM workspace types (needs to run after processTransportPackages)
-processWorkspaceTemplateRegistrations: register workspace templates as projects for Extended ECM for Engineering (deprecated)
 processWorkspaces: process Extended ECM workspace instances
 processWorkspaceRelationships: process Extended ECM workspace relationships
 processWorkspaceMembers: process Extended ECM workspace members (users and groups)
 processWebReports: process Extended ECM Web Reports (starts them with parameters)
 processCSApplications: process Extended ECM CS Applications
 processUserSettings: Process user settings in payload and apply themin OTDS.
 processUserFavoritesAndProfile: Process user favorites in payload and create them in Extended ECM
@@ -90,35 +97,41 @@
 __email__ = "mdiefenb@opentext.com"
 
 import os
 import logging
 import yaml
 import hcl2
 import re
+import time
+import json
 
 from urllib.parse import urlparse
 
 # OpenText specific modules:
 import pyxecm.web as web
 import pyxecm.sap as sap
 
+from pyxecm.otcs import OTCS
+from pyxecm.otds import OTDS
+from pyxecm.otac import OTAC
+
 logger = logging.getLogger(os.path.basename(__file__))
 
 
 class Payload(object):
     """Used to process Terrarium payload."""
 
     # _debug controls whether or not transport processing is
     # stopped if one transport fails:
-    _debug = False
-    _otcs = None
-    _otcs_backend = None
-    _otcs_frontend = None
-    _otac = None
-    _otds = None
+    _debug: bool = False
+    _otcs: OTCS = None
+    _otcs_backend: OTCS = None
+    _otcs_frontend: OTCS = None
+    _otac: OTAC = None
+    _otds: OTDS = None
     _otiv = None
     _k8s = None
     _web = None
     _m365 = None
     _custom_settings_dir = ""
 
     # _payload_source (string): This is either path + filename of the yaml payload
@@ -193,37 +206,41 @@
     _supplemental_markings = []
     _records_management_settings = []
     _holds = []
     _doc_generators = []
 
     _placeholder_values = {}
 
+    _otcs_restart_callback = None
+
     def __init__(
         self,
         payload_source: str,
         custom_settings_dir: str,
         k8s_object: object,
-        otds_object: object,
-        otac_object: object,
-        otcs_backend_object: object,
-        otcs_frontend_object: object,
+        otds_object: OTDS,
+        otac_object: OTAC,
+        otcs_backend_object: OTCS,
+        otcs_frontend_object: OTCS,
+        otcs_restart_callback: callable,
         otiv_object: object,
         m365_object: object,
         placeholder_values: dict = {},
         stop_on_error: bool = False,
     ):
         """Initialize the Payload object
 
         Args:
             payload_source (string): path or URL to payload source file
             k8s_object (object): Kubernetes object
-            otds_object (object): OTDS object
-            otac_object (object): OTAC object
-            otcs_backend_object (object): OTCS backend object
-            otcs_frontend_object (object): OTCS frontend object
+            otds_object (OTDS): OTDS object
+            otac_object (OTAC): OTAC object
+            otcs_backend_object (OTCS): OTCS backend object
+            otcs_frontend_object (OTCS): OTCS frontend object
+            otcs_restart_callback (callable): function to call if OTCS service needs a restart
             otiv_object (object): OTIV object
             m365_object (object): M365 object to talk to Microsoft Graph API
             placeholder_values (dict): dictionary of placeholder values to be replaced in admin settings
             stop_on_error (bool): controls if transport deployment should stop if one transport fails
         """
 
         self._stop_on_error = stop_on_error
@@ -234,14 +251,15 @@
         self._otcs = otcs_backend_object
         self._otcs_backend = otcs_backend_object
         self._otcs_frontend = otcs_frontend_object
         self._otiv = otiv_object
         self._m365 = m365_object
         self._custom_settings_dir = custom_settings_dir
         self._placeholder_values = placeholder_values
+        self._otcs_restart_callback = otcs_restart_callback
 
         self._http_object = web.HTTP()
 
     # end method definition
 
     def replacePlaceholders(self, content: str):
         # https://stackoverflow.com/questions/63502218/replacing-placeholders-in-a-text-file-with-python
@@ -353,17 +371,14 @@
         )
         self._renamings = self.getPayloadSection("renamings")
         self._items = self.getPayloadSection("items")
         self._items_post = self.getPayloadSection("itemsPost")
         self._permissions = self.getPayloadSection("permissions")
         self._permissions_post = self.getPayloadSection("permissionsPost")
         self._assignments = self.getPayloadSection("assignments")
-        self._workspace_template_registrations = self.getPayloadSection(
-            "workspaceTemplateRegistrations",
-        )
         self._security_clearances = self.getPayloadSection("securityClearances")
         self._supplemental_markings = self.getPayloadSection("supplementalMarkings")
         self._records_management_settings = self.getPayloadSection(
             "recordsManagementSettings"
         )
         self._holds = self.getPayloadSection("holds")
         self._doc_generators = self.getPayloadSection("documentGenerators")
@@ -399,16 +414,277 @@
                 return []
 
         return self._payload[payload_section_name]
 
         # end method definition
 
     def getAllGroupNames(self) -> list:
+        """Construct a list of all group name
+
+        Returns:
+            list: list of all group names
+        """
         return [group.get("name") for group in self._groups]
 
+        # end method definition
+
+    def checkStatusFile(
+        self, payload_section_name: str, payload_specific: bool = True
+    ) -> bool:
+        """Check if the payload section has been processed before. This is
+           done by checking the existance of a text file in the Admin Personal
+           workspace in Extended ECM with the name of the payload section.
+
+        Args:
+            payload_section_name (str): name of the payload section. This
+                                        is used to construct the file name
+            payload_specific (bool): whether or not the success should be specific for
+                                     each payload file or if success is "global" - like for the deletion
+                                     of the existing M365 teams (which we don't want to execute per
+                                     payload file)
+        Returns:
+            bool: True if the payload has been processed successfully before, False otherwise
+        """
+
+        logger.info(
+            "Check if payload section -> {} has been processed successfully before...".format(
+                payload_section_name
+            )
+        )
+
+        response = self._otcs.getNodeByVolumeAndPath(
+            142
+        )  # write to Personal Workspace of Admin
+        target_folder_id = self._otcs.getResultValue(response, "id")
+        if not target_folder_id:
+            target_folder_id = 2004  # use Personal Workspace of Admin as fallback
+
+        # Some sections are actually not payload specific like teamsM365Cleanup
+        # we don't want external payload runs to re-apply this processing:
+        if payload_specific:
+            file_name = os.path.basename(self._payload_source)  # remove directories
+            file_name = os.path.splitext(file_name)[0]  # remove file suffix
+            file_name = "success_" + file_name + "_" + payload_section_name + ".txt"
+        else:
+            file_name = "success_" + payload_section_name + ".txt"
+
+        status_document = self._otcs.getNodeByParentAndName(
+            parent_id=target_folder_id, name=file_name, show_error=False
+        )
+        if status_document and status_document["results"]:
+            name = self._otcs.getResultValue(status_document, "name")
+            if name == file_name:
+                logger.info(
+                    "Payload section -> {} has been processed successfully before. Skipping...".format(
+                        payload_section_name
+                    )
+                )
+                return True
+        logger.info(
+            "Payload section -> {} has not been processed successfully before. Processing...".format(
+                payload_section_name
+            )
+        )
+        return False
+
+        # end method definition
+
+    def writeStatusFile(
+        self,
+        payload_section_name: str,
+        payload_section: list,
+        payload_specific: bool = True,
+    ) -> bool:
+        """Write a status file into the Admin Personal Workspace in Extended ECM
+           to indicate that the payload section has been deployed successfully.
+           This speeds up the customizing process in case the customizer pod
+           is restarted.
+
+        Args:
+            payload_section_name (str): name of the payload section
+            payload_section (list): payload section content - this is written as JSon into the file
+            payload_specific (bool): whether or not the success should be specific for
+                                     each payload file or if success is "global" - like for the deletion
+                                     of the existing M365 teams (which we don't want to execute per
+                                     payload file)
+        Returns:
+            bool: True if the status file as been upladed to Extended ECM successfully, False otherwise
+        """
+
+        response = self._otcs.getNodeByVolumeAndPath(
+            142
+        )  # write to Personal Workspace of Admin (with Volume Type ID = 142)
+        target_folder_id = self._otcs.getResultValue(response, "id")
+        if not target_folder_id:
+            target_folder_id = 2004  # use Personal Workspace of Admin as fallback
+
+        # Some sections are actually not payload specific like teamsM365Cleanup
+        # we don't want external payload runs to re-apply this processing:
+        if payload_specific:
+            file_name = os.path.basename(self._payload_source)  # remove directories
+            file_name = os.path.splitext(file_name)[0]  # remove file suffix
+            file_name = "success_" + file_name + "_" + payload_section_name + ".txt"
+        else:
+            file_name = "success_" + payload_section_name + ".txt"
+        full_path = "/tmp/" + file_name
+
+        with open(full_path, mode="w") as localfile:
+            localfile.write(json.dumps(payload_section, indent=2))
+
+        response = self._otcs.uploadFileToParent(
+            file_url=full_path,
+            file_name=file_name,
+            mime_type="text/plain",
+            parent_id=target_folder_id,
+        )
+
+        if response:
+            logger.info(
+                "Payload section -> {} has been completed successfully!".format(
+                    payload_section_name
+                )
+            )
+            return True
+
+        return False
+
+        # end method definition
+
+    def determineGroupID(self, group: dict) -> int:
+        """Determine the id of a group - either from payload or from OTCS.
+           If the group is found in OTCS write back the ID into the payload.
+
+        Args:
+            group (dict): group payload element
+
+        Returns:
+            int: group ID
+        Side Effects:
+            the group items are modified by adding an "id" dict element that
+            includes the technical ID of the group in Extended ECM
+        """
+
+        if "id" in group:
+            return group["id"]
+
+        if not "name" in group:
+            logger.error("Group needs a name to lookup the ID.")
+            return 0
+        group_name = group["name"]
+
+        existing_groups = self._otcs.getGroup(name=group_name)
+        if not existing_groups or not existing_groups["data"]:
+            logger.info(
+                "Cannot find an existing group with name -> {}".format(group_name)
+            )
+            return 0
+
+        # Get list of all matching groups:
+        existing_groups_list = existing_groups["data"]
+        # Find the group with the exact match of the name:
+        existing_group = next(
+            (item for item in existing_groups_list if item["name"] == group_name),
+            None,
+        )
+        # Have we found an exact match?
+        if existing_group:
+            group["id"] = existing_group["id"]
+            return group["id"]
+        else:
+            logger.info(
+                "Did not find an existing group with name -> {}".format(group_name)
+            )
+            return 0
+
+        # end method definition
+
+    def determineUserID(self, user: dict):
+        """Determine the id of a group - either from payload or from OTCS
+           If the user is found in OTCS write back the ID into the payload.
+
+        Args:
+            user (dict): user payload element
+
+        Returns:
+            int: user ID
+        Side Effects:
+            the user items are modified by adding an "id" dict element that
+            includes the technical ID of the user in Extended ECM
+        """
+
+        if "id" in user:
+            return user["id"]
+
+        if not "name" in user:
+            logger.error("User needs a login name to lookup the ID.")
+            return 0
+        user_name = user["name"]
+
+        existing_users = self._otcs.getUser(name=user_name)
+        if not existing_users or not existing_users["data"]:
+            logger.info(
+                "Cannot find an existing user with name -> {}".format(user_name)
+            )
+            return 0
+
+        # Get list of all matching users:
+        existing_users_list = existing_users["data"]
+        # Find the group with the exact match of the name:
+        existing_user = next(
+            (item for item in existing_users_list if item["name"] == user_name),
+            None,
+        )
+        # Have we found an exact match?
+        if existing_user:
+            user["id"] = existing_user["id"]
+            return user["id"]
+        else:
+            logger.info(
+                "Did not find an existing user with name -> {}".format(user_name)
+            )
+            return 0
+
+        # end method definition
+
+    def determineWorkspaceID(self, workspace: dict):
+        """Determine the nodeID of a workspace - either from payload or from OTCS"""
+
+        """Determine the id of a group - either from payload or from OTCS
+           If the user is found in OTCS write back the ID into the payload.
+
+        Args:
+            workspace (dict): workspace payload element
+
+        Returns:
+            int: workspace Node ID
+        Side Effects:
+            the workspace items are modified by adding an "nodeId" dict element that
+            includes the node ID of the workspace in Extended ECM
+        """
+
+        if "nodeId" in workspace:
+            return workspace["nodeId"]
+
+        response = self._otcs.getWorkspaceByTypeAndName(
+            workspace["type_name"], workspace["name"]
+        )
+        workspace_id = self._otcs.getResultValue(response, "id")
+        if workspace_id:
+            workspace["nodeId"] = workspace_id
+            return workspace_id
+        else:
+            logger.warning(
+                "Workspace of type -> {} and name -> {} does not exist.".format(
+                    workspace["type_name"], workspace["name"]
+                )
+            )
+            return 0
+
+        # end method definition
+
     def processPayload(self):
         """Main method to process a payload file.
 
         Args:
             None
         Returns:
             None
@@ -426,20 +702,24 @@
                         "========== Process Web Hooks ==========================="
                     )
                     self.processWebHooks(self._webhooks)
                 case "webHooksPost":
                     logger.info(
                         "========== Process Web Hooks (post) ===================="
                     )
-                    self.processWebHooks(self._webhooks_post)
+                    self.processWebHooks(self._webhooks_post, "webHooksPost")
                 case "partitions":
                     logger.info(
                         "========== Process OTDS Partitions ====================="
                     )
                     self.processPartitions()
+                    logger.info(
+                        "========== Assign OTCS Licenses to Partitions =========="
+                    )
+                    self.processPartitionLicenses()
                 case "oauthClients":
                     logger.info(
                         "========== Process OTDS OAuth Clients =================="
                     )
                     self.processOAuthClients()
                 case "trustedSites":
                     logger.info(
@@ -452,28 +732,38 @@
                     )
                     self.processSystemAttributes()
                 case "groups":
                     logger.info(
                         "========== Process OTCS Groups ========================="
                     )
                     self.processGroups()
+                    # Add all groups with ID the a lookup dict for placeholder replacements
+                    # in adminSetting. This also updates the payload with group IDs from OTCS
+                    # if the group already exists in Extended ECM. This is important especially
+                    # if the customizer pod is restarted / run multiple times:
+                    self.processGroupPlaceholders()
                     if self._m365:
                         logger.info(
                             "========== Cleanup existing MS Teams ==================="
                         )
                         self.cleanupAllTeamsM365()
                         logger.info(
                             "========== Process M365 Groups ========================="
                         )
                         self.processGroupsM365()
                 case "users":
                     logger.info(
                         "========== Process OTCS Users =========================="
                     )
                     self.processUsers()
+                    # Add all users with ID the a lookup dict for placeholder replacements
+                    # in adminSetting. This also updates the payload with user IDs from OTCS
+                    # if the user already exists in Extended ECM. This is important especially
+                    # if the cutomizer pod is restarted / run multiple times:
+                    self.processUserPlaceholders()
                     logger.info(
                         "========== Assign OTCS Licenses to Users ==============="
                     )
                     self.processUserLicenses(
                         self._otcs.config()["resource"],
                         self._otcs.config()["license"],
                         "EXTENDED_ECM",
@@ -501,36 +791,42 @@
                         # the M365 users as we require Group Owners to create teams
                         logger.info(
                             "========== Process M365 Teams =========================="
                         )
                         self.processTeamsM365()
                 case "adminSettings":
                     logger.info(
-                        "========== Process OTCS LLConfig Settings (1) =========="
+                        "========== Process Administration Settings (1) ========="
                     )
                     self.processAdminSettings(self._admin_settings)
                 case "adminSettingsPost":
                     logger.info(
-                        "========== Process OTCS LLConfig Settings (2) =========="
+                        "========== Process Administration Settings (2) ========="
+                    )
+                    self.processAdminSettings(
+                        self._admin_settings_post, "adminSettingsPost"
                     )
-                    self.processAdminSettings(self._admin_settings_post)
                 case "execPodCommands":
                     logger.info(
                         "========== Process Pod Commands ========================"
                     )
                     self.processExecPodCommands()
                 case "csApplications":
                     logger.info(
                         "========== Process CS Apps (backend) ==================="
                     )
-                    self.processCSApplications()
+                    self.processCSApplications(
+                        self._otcs_backend, section_name="csApplicationsBackend"
+                    )
                     logger.info(
                         "========== Process CS Apps (frontend) =================="
                     )
-                    self.processCSApplications(self._otcs_frontend)
+                    self.processCSApplications(
+                        self._otcs_frontend, section_name="csApplicationsFrontend"
+                    )
                 case "externalSystems":
                     logger.info(
                         "========== Process External System Connections ========="
                     )
                     self.processExternalSystems()
                 case "transportPackages":
                     logger.info(
@@ -543,30 +839,29 @@
                         "========== Process Workspace Types ====================="
                     )
                     workspace_types = self.processWorkspaceTypes()
                 case "contentTransportPackages":
                     logger.info(
                         "========== Process Content Transport Packages =========="
                     )
-                    self.processTransportPackages(self._content_transport_packages)
+                    self.processTransportPackages(
+                        self._content_transport_packages, "contentTransportPackages"
+                    )
                 case "transportPackagesPost":
                     # if self._m365:
                     #     logger.info(
                     #         "========== Cleanup stale MS Teams ======================"
                     #     )
                     #     self.cleanupStaleTeamsM365(workspace_types)
                     logger.info(
                         "========== Process Transport Packages (post) ==========="
                     )
-                    self.processTransportPackages(self._transport_packages_post)
-                case "workspaceTemplateRegistrations":
-                    logger.info(
-                        "========== Register Workspace Templates ================"
+                    self.processTransportPackages(
+                        self._transport_packages_post, "transportPackagesPost"
                     )
-                    self.processWorkspaceTemplateRegistrations()
                 case "workspaces":
                     logger.info(
                         "========== Process Workspaces =========================="
                     )
                     self.processWorkspaces()
                     logger.info(
                         "========== Process Workspace Relationships ============="
@@ -582,15 +877,16 @@
                     )
 
                     if self._external_systems:
                         sap_external_system = next(
                             (
                                 item
                                 for item in self._external_systems
-                                if item["external_system_type"] == "SAP"
+                                if item.get("external_system_type")
+                                and item["external_system_type"] == "SAP"
                             ),
                             None,
                         )
                     if not sap_external_system:
                         logger.warning(
                             "SAP RFC in payload but SAP external system is configured. RFCs will not be processed."
                         )
@@ -611,15 +907,15 @@
                         "========== Process Web Reports ========================="
                     )
                     self.processWebReports(self._web_reports)
                 case "webReportsPost":
                     logger.info(
                         "========== Process Web Reports (post) =================="
                     )
-                    self.processWebReports(self._web_reports_post)
+                    self.processWebReports(self._web_reports_post, "webReportsPost")
                 case "additionalGroupMemberships":
                     logger.info(
                         "========== Process additional group members for OTDS ==="
                     )
                     self.processAdditionalGroupMembers()
                 case "additionalAccessRoleMemberships":
                     logger.info(
@@ -636,15 +932,15 @@
                         "========== Process Items ==============================="
                     )
                     self.processItems(self._items)
                 case "itemsPost":
                     logger.info(
                         "========== Process Items (post) ========================"
                     )
-                    self.processItems(self._items_post)
+                    self.processItems(self._items_post, "itemsPost")
                 case "permissions":
                     logger.info(
                         "========== Process Permissions ========================="
                     )
                     self.processPermissions(self._permissions)
                 case "permissionsPost":
                     logger.info(
@@ -683,44 +979,74 @@
                     self.processDocumentGenerators()
                 case other:
                     logger.error(
                         "Illegal payload section name -> {} in payloadSections!".format(
                             payload_section["name"]
                         )
                     )
+            payload_section_restart = payload_section.get("restart", False)
+            if payload_section_restart:
+                logger.info(
+                    "Payload section -> {} requests a restart of OTCS services...".format(
+                        payload_section["name"]
+                    )
+                )
+                # Restart OTCS frontend and backend pods:
+                self._otcs_restart_callback(self._otcs_backend, self._k8s)
+                # give some additional time to make sure service is responsive
+                time.sleep(30)
+            else:
+                logger.info(
+                    "Payload section -> {} does not require a restart of OTCS services".format(
+                        payload_section["name"]
+                    )
+                )
 
         if self._users:
             logger.info("========== Process User Profile Photos =================")
             self.processUserPhotos()
             if self._m365:
                 logger.info("========== Process M365 User Profile Photos ============")
                 self.processUserPhotosM365()
             logger.info("========== Process User Favorites and Profiles =========")
             self.processUserFavoritesAndProfiles()
             logger.info("========== Process User Security =======================")
             self.processUserSecurity()
 
         # end method definition
 
-    def processWebHooks(self, webhooks: list):
+    def processWebHooks(self, webhooks: list, section_name: str = "webHooks") -> bool:
         """Process Web Hooks in payload and do HTTP requests.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
         if not webhooks:
-            return None
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+
+        # WE LET THIS RUN EACH TIME!
+        #        if self.checkStatusFile(section_name):
+        #            return True
+
+        success: bool = True
 
         for webhook in webhooks:
             url = webhook.get("url")
             if not url:
                 logger.info("Web Hook does not have a url - skipping...")
+                success = False
                 continue
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in webhook and not webhook["enabled"]:
                 logger.info(
                     "Payload for Web Hook -> {} is disabled. Skipping...".format(url)
@@ -740,29 +1066,48 @@
                     "Calling Web Hook -> {}: {} ({})".format(method, url, description)
                 )
             else:
                 logger.info("Calling Web Hook -> {}: {}".format(method, url))
 
             self._http_object.httpRequest(url, method, payload, headers)
 
+        #        if success:
+        #            self.writeStatusFile(section_name, webhooks)
+
+        return success
+
         # end method definition
 
-    def processPartitions(self):
+    def processPartitions(self, section_name: str = "partitions") -> bool:
         """Process OTDS partitions in payload and create them in OTDS.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._partitions:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for partition in self._partitions:
             partition_name = partition.get("name")
             if not partition_name:
                 logger.error("Partition does not have a name - skipping...")
+                success = False
                 continue
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in partition and not partition["enabled"]:
                 logger.info(
                     "Payload for Partition -> {} is disabled. Skipping...".format(
@@ -796,14 +1141,15 @@
             response = self._otds.addPartition(partition_name, partition_description)
             if response:
                 logger.info("Added OTDS partition -> {}".format(partition_name))
             else:
                 logger.error(
                     "Failed to add OTDS partition -> {}".format(partition_name)
                 )
+                success = False
                 continue
 
             access_role = partition.get("access_role")
             if access_role:
                 response = self._otds.addPartitionToAccessRole(
                     access_role, partition_name
                 )
@@ -815,66 +1161,192 @@
                     )
                 else:
                     logger.error(
                         "Failed to add OTDS partition -> {} to access role -> {}".format(
                             partition_name, access_role
                         )
                     )
+                    success = False
                     continue
 
             # Partions may have an optional list of licenses in
             # the payload. Assign the partition to all these licenses:
             partition_specific_licenses = partition.get("licenses")
             if partition_specific_licenses:
                 # We assume these licenses are Extended ECM licenses!
                 otcs_resource_name = self._otcs.config()["resource"]
                 otcs_resource = self._otds.getResource(otcs_resource_name)
                 if not otcs_resource:
                     logger.error(
                         "Cannot find OTCS resource -> {}".format(otcs_resource_name)
                     )
+                    success = False
                     continue
                 otcs_resource_id = otcs_resource["resourceID"]
-                license_name = "Extended ECM"
+                license_name = "EXTENDED_ECM"
                 for license_feature in partition_specific_licenses:
                     assigned_license = self._otds.assignPartitionToLicense(
                         partition_name,
                         otcs_resource_id,
                         license_feature,
                         license_name,
                     )
 
                     if not assigned_license:
                         logger.error(
                             "Failed to assign partition -> {} to license feature -> {} of license -> {}!".format(
                                 partition_name, license_feature, license_name
                             )
                         )
+                        success = False
                     else:
                         logger.info(
                             "Successfully assigned partition -> {} to license feature -> {} of license -> {}".format(
                                 partition_name, license_feature, license_name
                             )
                         )
 
+        if success:
+            self.writeStatusFile(section_name, self._partitions)
+
+        return success
+
         # end method definition
 
-    def processOAuthClients(self):
-        """Process OTDS OAuth clients in payload and create them in OTDS.
+    def processPartitionLicenses(self, section_name: str = "partitionLicenses") -> bool:
+        """Process the licenses that should be assigned to OTDS partitions
+           (this includes existing partitions).
 
         Args:
             None
         Returns:
+            bool: True if payload has been processed without errors, False otherwise
+        """
+
+        if not self._partitions:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
+        for partition in self._partitions:
+            partition_name = partition.get("name")
+            if not partition_name:
+                logger.error("Partition does not have a name - skipping...")
+                success = False
+                continue
+
+            # Check if element has been disabled in payload (enabled = false).
+            # In this case we skip the element:
+            if "enabled" in partition and not partition["enabled"]:
+                logger.info(
+                    "Payload for Partition -> {} is disabled. Skipping...".format(
+                        partition_name
+                    )
+                )
+                continue
+
+            response = self._otds.getPartition(partition_name, show_error=True)
+            if not response:
+                logger.error(
+                    "Partition -> {} does not exist. Skipping...".format(partition_name)
+                )
+                success = False
+                continue
+
+            # Partions may have an optional list of licenses in
+            # the payload. Assign the partition to all these licenses:
+            partition_specific_licenses = partition.get("licenses")
+            if partition_specific_licenses:
+                # We assume these licenses are Extended ECM licenses!
+                otcs_resource_name = self._otcs.config()["resource"]
+                otcs_resource = self._otds.getResource(otcs_resource_name)
+                if not otcs_resource:
+                    logger.error(
+                        "Cannot find OTCS resource -> {}".format(otcs_resource_name)
+                    )
+                    success = False
+                    continue
+                otcs_resource_id = otcs_resource["resourceID"]
+                license_name = "EXTENDED_ECM"
+                for license_feature in partition_specific_licenses:
+                    if self._otds.isPartitionLicensed(
+                        partition_name=partition_name,
+                        resource_id=otcs_resource_id,
+                        license_feature=license_feature,
+                        license_name=license_name,
+                    ):
+                        logger.info(
+                            "Partition -> {} is already licensed for -> {} ({})".format(
+                                partition_name, license_name, license_feature
+                            )
+                        )
+                        continue
+                    assigned_license = self._otds.assignPartitionToLicense(
+                        partition_name,
+                        otcs_resource_id,
+                        license_feature,
+                        license_name,
+                    )
+
+                    if not assigned_license:
+                        logger.error(
+                            "Failed to assign partition -> {} to license feature -> {} of license -> {}!".format(
+                                partition_name, license_feature, license_name
+                            )
+                        )
+                        success = False
+                    else:
+                        logger.info(
+                            "Successfully assigned partition -> {} to license feature -> {} of license -> {}".format(
+                                partition_name, license_feature, license_name
+                            )
+                        )
+
+        if success:
+            self.writeStatusFile(section_name, self._partitions)
+
+        return success
+
+        # end method definition
+
+    def processOAuthClients(self, section_name: str = "oauthClients") -> bool:
+        """Process OTDS OAuth clients in payload and create them in OTDS.
+
+        Args:
             None
+        Returns:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._oauth_clients:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for oauth_client in self._oauth_clients:
             client_name = oauth_client.get("name")
             if not client_name:
                 logger.error("OAuth client does not have a name - skipping...")
+                success = False
                 continue
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in oauth_client and not oauth_client["enabled"]:
                 logger.info(
                     "Payload for OAuthClient -> {} is disabled. Skipping...".format(
@@ -925,60 +1397,102 @@
             )
             if response:
                 logger.info("Added OTDS OAuth client -> {}".format(client_name))
             else:
                 logger.error(
                     "Failed to add OTDS OAuth client -> {}".format(client_name)
                 )
+                success = False
                 continue
 
             client_secret = response.get("secret")
             if not client_secret:
                 logger.error(
                     "OAuth client -> {} does not have a secret!".format(client_name)
                 )
                 continue
 
             client_description += " Client Secret Key: " + str(client_secret)
             response = self._otds.updateOauthClient(
                 client_name, {"description": client_description}
             )
 
+        if success:
+            self.writeStatusFile(section_name, self._oauth_clients)
+
+        return success
+
     #        self._otds.addOauthClientsToAccessRole()
 
     # end method definition
 
-    def processTrustedSites(self):
+    def processTrustedSites(self, section_name: str = "trustedSites") -> bool:
         """Process OTDS trusted sites in payload and create them in OTDS.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._trusted_sites:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for trusted_site in self._trusted_sites:
-            self._otds.addTrustedSite(trusted_site)
-            logger.info("Added OTDS trusted site -> {}".format(trusted_site))
+            response = self._otds.addTrustedSite(trusted_site)
+            if response:
+                logger.info("Added OTDS trusted site -> {}".format(trusted_site))
+            else:
+                logger.error("Failed to add trusted site -> {}".format(trusted_site))
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._trusted_sites)
+
+        return success
 
         # end method definition
 
-    def processSystemAttributes(self):
+    def processSystemAttributes(self, section_name: str = "systemAttributes") -> bool:
         """Process OTDS system attributes in payload and create them in OTDS.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._system_attributes:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for system_attribute in self._system_attributes:
             # Check if there's a matching formal parameter defined on the Web Report node:
             if not system_attribute.get("name"):
                 logger.error("OTDS System Attribute needs a name. Skipping...")
+                success = False
                 continue
             attribute_name = system_attribute["name"]
 
             if "enabled" in system_attribute and not system_attribute["enabled"]:
                 logger.info(
                     "Payload for OTDS System Attribute -> {} is disabled. Skipping...".format(
                         attribute_name
@@ -988,42 +1502,159 @@
 
             if not system_attribute.get("value"):
                 logger.error("OTDS System Attribute needs a value. Skipping...")
                 continue
 
             attribute_value = system_attribute["value"]
             attribute_description = system_attribute.get("description")
-            self._otds.addSystemAttribute(
+            response = self._otds.addSystemAttribute(
                 attribute_name, attribute_value, attribute_description
             )
-            logger.info(
-                "Added OTDS system attribute -> {} with value -> {}".format(
-                    attribute_name, attribute_value
+            if response:
+                logger.info(
+                    "Added OTDS system attribute -> {} with value -> {}".format(
+                        attribute_name, attribute_value
+                    )
                 )
-            )
+            else:
+                logger.error(
+                    "Failed to add OTDS system attribute -> {} with value -> {}".format(
+                        attribute_name, attribute_value
+                    )
+                )
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._system_attributes)
+
+        return success
 
         # end method definition
 
-    def processGroups(self):
+    def processGroupPlaceholders(self):
+        """For some adminSettings we may need to replace a placeholder (sourrounded by %%...%%)
+        with the actual ID of the Extended ECM group. For this we prepare a lookup dict.
+        The dict self._placeholder_values already includes lookups for the OTCS and OTAWP
+        OTDS resource IDs (see main.py)
+        """
+
+        for group in self._groups:
+            if not "name" in group:
+                logger.error(
+                    "Group needs a name for placeholder definition. Skipping..."
+                )
+                continue
+            group_name = group["name"]
+            # Check if group has been disabled in payload (enabled = false).
+            # In this case we skip the element:
+            if "enabled" in group and not group["enabled"]:
+                logger.info(
+                    "Payload for Group -> {} is disabled. Skipping...".format(
+                        group_name
+                    )
+                )
+                continue
+
+            # Now we determine the ID. Either it is in the payload section from
+            # the current customizer run or we try to look it up in the system.
+            # The latter case may happen if the custiomuer pod got restarted.
+            group_id = self.determineGroupID(group)
+            if not group_id:
+                logger.warning(
+                    "Group needs an ID for placeholder definition. Skipping..."
+                )
+                continue
+
+            # Add Group with its ID to the dict self._placeholder_values:
+            self._placeholder_values[
+                "OTCS_GROUP_ID_{}".format(
+                    group_name.upper().replace(" & ", "_").replace(" ", "_")
+                )
+            ] = str(group_id)
+
+        logger.debug(
+            "Placeholder values after group processing = {}".format(
+                self._placeholder_values
+            )
+        )
+
+    def processUserPlaceholders(self):
+        """For some adminSettings we may need to replace a placeholder (sourrounded by %%...%%)
+        with the actual ID of the Extended ECM user. For this we prepare a lookup dict.
+        The dict self._placeholder_values already includes lookups for the OTCS and OTAWP
+        OTDS resource IDs (see main.py)
+        """
+
+        for user in self._users:
+            if not "name" in user:
+                logger.error(
+                    "User needs a name for placeholder definition. Skipping..."
+                )
+                continue
+            user_name = user["name"]
+            # Check if group has been disabled in payload (enabled = false).
+            # In this case we skip the element:
+            if "enabled" in user and not user["enabled"]:
+                logger.info(
+                    "Payload for User -> {} is disabled. Skipping...".format(user_name)
+                )
+                continue
+
+            # Now we determine the ID. Either it is in the payload section from
+            # the current customizer run or we try to look it up in the system.
+            # The latter case may happen if the custiomuer pod got restarted.
+            user_id = self.determineUserID(user)
+            if not user_id:
+                logger.warning(
+                    "User needs an ID for placeholder definition. Skipping..."
+                )
+                continue
+
+            # Add Group with its ID to the dict self._placeholder_values:
+            self._placeholder_values["OTCS_USER_ID_{}".format(user_name.upper())] = str(
+                user_id
+            )
+
+        logger.debug(
+            "Placeholder values after user processing = {}".format(
+                self._placeholder_values
+            )
+        )
+
+    def processGroups(self, section_name: str = "groups") -> bool:
         """Process groups in payload and create them in Extended ECM.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         Side Effects:
             the group items are modified by adding an "id" dict element that
             includes the technical ID of the group in Extended ECM
         """
 
+        if not self._groups:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         # First run through groups: create all groups in payload
         # and store the IDs of the created groups:
         for group in self._groups:
             if not "name" in group:
                 logger.error("Group needs a name. Skipping...")
+                success = False
                 continue
             group_name = group["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in group and not group["enabled"]:
                 logger.info(
@@ -1031,78 +1662,43 @@
                         group_name
                     )
                 )
                 continue
 
             # Check if the group does already exist (e.g. if job is restarted)
             # as this is a pattern search it could return multiple groups:
-            existing_groups = self._otcs.getGroup(group_name)
-            if existing_groups and existing_groups["data"]:
-                logger.debug(
-                    "Found existing groups -> {}".format(existing_groups["data"])
-                )
-                # Get list of all matching groups:
-                existing_groups_list = existing_groups["data"]
-                # Find the group with the exact match of the name:
-                existing_group = next(
-                    (
-                        item
-                        for item in existing_groups_list
-                        if item["name"] == group_name
-                    ),
-                    None,
-                )
-                # Have we found an exact match?
-                if existing_group is not None:
-                    logger.info(
-                        "Found existing group -> {} ({}) - skipping to next group...".format(
-                            existing_group["name"], existing_group["id"]
-                        )
+            group_id = self.determineGroupID(group)
+            if group_id:
+                logger.info(
+                    "Found existing group -> {} ({}) - skipping to next group...".format(
+                        group_name, group_id
                     )
-                    group["id"] = existing_group["id"]
+                )
+                continue
+
+            logger.info("Did not find an existing group - creating a new group...")
 
-                    # Add Group with its ID to the class dict _placeholder_values:
-                    self._placeholder_values[
-                        "OTCS_GROUP_ID_{}".format(
-                            group_name.upper().replace(" & ", "_").replace(" ", "_")
-                        )
-                    ] = str(group["id"])
-                    continue
-                else:
-                    logger.info(
-                        "Did not find an exact match for the group - creating a new group..."
-                    )
-            else:
-                logger.info("Did not find any matching group - creating a new group...")
             # Now we know it is a new group...
             new_group = self._otcs.addGroup(group_name)
             if new_group is not None:
                 logger.debug("New group -> {}".format(new_group))
                 group["id"] = new_group["id"]
-
-            # Add Group with its ID to the global dict with placeholder values:
-            self._placeholder_values[
-                "OTCS_GROUP_ID_{}".format(
-                    group_name.upper().replace(" & ", "_").replace(" ", "_")
-                )
-            ] = str(group["id"])
+            else:
+                logger.error("Failed to create group -> {}".format(new_group))
+                success = False
+                continue
 
         logger.debug("Groups = {}".format(self._groups))
 
-        logger.debug(
-            "Placeholder values after group processing = {}".format(
-                self._placeholder_values
-            )
-        )
-
         # Second run through groups: create all group memberships
         # (nested groups) based on the IDs created in first run:
         for group in self._groups:
             if not "id" in group:
                 logger.error("Group -> {} does not have an ID.".format(group["name"]))
+                success = False
                 continue
             parent_group_names = group["parent_groups"]
             for parent_group_name in parent_group_names:
                 # First, try to find parent group in payload by parent group name:
                 parent_group = next(
                     (
                         item
@@ -1118,22 +1714,24 @@
                     parent_group = self._otcs.getGroup(parent_group_name)
                     if not parent_group:
                         logger.error(
                             "Parent Group -> {} not found. Skipping...".format(
                                 parent_group_name
                             )
                         )
+                        success = False
                         continue
                     parent_group = parent_group["data"][0]
                 elif not "id" in parent_group:
                     logger.error(
                         "Parent Group -> {} does not have an ID. Skipping...".format(
                             parent_group["name"]
                         )
                     )
+                    success = False
                     continue
 
                 # retrieve all members of the parent group (1 = get only groups)
                 members = self._otcs.getGroupMembers(parent_group["id"], 1)
                 if self._otcs.existResultItem(members, "id", group["id"]):
                     #                if existing_member:
                     logger.info(
@@ -1151,30 +1749,49 @@
                             group["id"],
                             parent_group["name"],
                             parent_group["id"],
                         )
                     )
                     self._otcs.addGroupMember(group["id"], parent_group["id"])
 
+        if success:
+            self.writeStatusFile(section_name, self._groups)
+
+        return success
+
         # end method definition
 
-    def processGroupsM365(self):
+    def processGroupsM365(self, section_name: str = "groupsM365") -> bool:
         """Process groups in payload and create them in Microsoft 365.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._groups:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         # First run through groups: create all groups in payload
         # and store the IDs of the created groups:
         for group in self._groups:
             if not "name" in group:
                 logger.error("Group needs a name. Skipping...")
+                success = False
                 continue
             group_name = group["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in group and not group["enabled"]:
                 logger.info(
@@ -1235,35 +1852,56 @@
                 # Store the Microsoft 365 group ID in payload:
                 group["m365_id"] = new_group["id"]
                 logger.info(
                     "New Microsoft 365 group -> {} with ID -> {} has been created".format(
                         group_name, group["m365_id"]
                     )
                 )
+            else:
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._groups)
+
+        return success
 
         # end method definition
 
-    def processUsers(self):
+    def processUsers(self, section_name: str = "users") -> bool:
         """Process users in payload and create them in Extended ECM.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         Side Effects:
             the user items are modified by adding an "id" dict element that
             includes the technical ID of the user in Extended ECM
         """
 
+        if not self._users:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         # Add all users in payload and establish membership in
         # specified groups:
         for user in self._users:
             # Sanity checks:
             if not "name" in user:
                 logger.error("User is missing a login - skipping to next user...")
+                success = False
                 continue
             user_name = user["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
                 logger.info(
@@ -1274,61 +1912,45 @@
             # Sanity checks:
             if not "password" in user:
                 logger.error(
                     "User -> {} is missing a password - skipping to next user...".format(
                         user_name
                     )
                 )
+                success = False
                 continue
 
             # Sanity checks:
             if not "base_group" in user:
                 logger.warning(
                     "User -> {} is missing a base group - setting to default group".format(
                         user_name
                     )
                 )
                 user["base_group"] = "DefaultGroup"
 
             # Check if the user does already exist (e.g. if job is restarted)
-            # As this is a pattern search it could return multiple users:
-            existing_users = self._otcs.getUser(user_name)
-            if existing_users and existing_users["data"]:
-                logger.debug(
-                    "Found existing users -> {}".format(existing_users["data"])
-                )
-                # Get list of all matching users:
-                existing_users_list = existing_users["data"]
-                # Find the user with the exact match of the name:
-                existing_user = next(
-                    (item for item in existing_users_list if item["name"] == user_name),
-                    None,
-                )
-                # Have we found an exact match?
-                if existing_user is not None:
-                    logger.info(
-                        "Found existing user -> {} ({}) - skipping to next user...".format(
-                            existing_user["name"], existing_user["id"]
-                        )
-                    )
-                    user["id"] = existing_user["id"]
-                    continue
-                else:
-                    logger.info(
-                        "Did not find an exact match for the user - creating a new user..."
+            # determineUserID() also writes back the user ID into the payload
+            # if it has gathered it from OTCS.
+            user_id = self.determineUserID(user)
+            if user_id:
+                logger.info(
+                    "Found existing user -> {} ({}) - skipping to next user...".format(
+                        user_name, user_id
                     )
-            else:
-                logger.info("Did not find any matching user - creating a new user...")
+                )
+                continue
+            logger.info("Did not find an existing user - creating a new user...")
 
             # Find the base group of the user. Assume 'Default Group' (= 1001) if not found:
             base_group = next(
                 (
                     item["id"]
                     for item in self._groups
-                    if item["name"] == user["base_group"]
+                    if item["name"] == user["base_group"] and item.get("id")
                 ),
                 1001,
             )
 
             # Now we know it is a new user...
             new_user = self._otcs.addUser(
                 name=user_name,
@@ -1361,79 +1983,107 @@
                         # if group is not in payload try to find group in OTCS
                         # in case it is a pre-existing group:
                         group = self._otcs.getGroup(group_name)
                         if group is None:
                             logger.error(
                                 "Group -> {} not found. Skipping...".format(group_name)
                             )
+                            success = False
                             continue
                         group = group["data"][0]
 
                     if group["id"] is None:
                         logger.error(
                             "Group -> {} does not have an ID. Skipping...".format(
                                 group["name"]
                             )
                         )
+                        success = False
                         continue
 
                     logger.info(
                         "Add user -> {} ({}) to group -> {} ({})".format(
                             user["name"], user["id"], group["name"], group["id"]
                         )
                     )
-                    self._otcs.addGroupMember(user["id"], group["id"])
+                    response = self._otcs.addGroupMember(user["id"], group["id"])
+                    if not response:
+                        success = False
                 # for some unclear reason the user is not added to its base group in OTDS
                 # so we do this explicitly:
-                self._otds.addUserToGroup(user["name"], user["base_group"])
+                response = self._otds.addUserToGroup(user["name"], user["base_group"])
+                if not response:
+                    success = False
 
                 # Extra OTDS attributes for the user can be provided in "extra_attributes"
                 # as part of the user payload.
                 if "extra_attributes" in user:
                     extra_attributes = user["extra_attributes"]
                     for extra_attribute in extra_attributes:
                         attribute_name = extra_attribute.get("name")
                         attribute_value = extra_attribute.get("value")
                         if not attribute_name or not attribute_value:
                             logger.error(
                                 "User attribute is missing a name or value. Skipping..."
                             )
+                            success = False
                             continue
                         logger.info(
                             "Set user attribute -> {} to -> {}".format(
                                 attribute_name, attribute_value
                             )
                         )
                         user_partition = self._otcs.config()["partition"]
                         if not user_partition:
                             logger.error("User partition not found!")
+                            success = False
+                            continue
                         self._otds.updateUser(
                             user_partition,
                             user["name"],
                             attribute_name,
                             attribute_value,
                         )
 
+        if success:
+            self.writeStatusFile(section_name, self._users)
+
+        return success
+
         # end method definition
 
-    def processUsersM365(self):
+    def processUsersM365(self, section_name: str = "usersM365") -> bool:
         """Process users in payload and create them in Microsoft 365 via MS Graph API.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._users:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         # Add all users in payload and establish membership in
         # specified groups:
         for user in self._users:
             # Sanity checks:
             if not "name" in user:
                 logger.error("User is missing a login - skipping to next user...")
+                success = False
                 continue
             user_name = user["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
                 logger.info(
@@ -1451,14 +2101,15 @@
             # Sanity checks:
             if not "password" in user:
                 logger.error(
                     "User -> {} is missing a password - skipping to next user...".format(
                         user_name
                     )
                 )
+                success = False
                 continue
             user_password = user["password"]
             # be careful with the following fields - they could be empty
             user_department = user.get("base_group", "")
             user_first_name = user.get("firstname", "")
             user_last_name = user.get("lastname", "")
             user_location = user.get("location", "US")
@@ -1500,14 +2151,15 @@
                     )
                 else:
                     logger.error(
                         "Failed to create new Microsoft 365 user -> {}. Skipping.".format(
                             user_name
                         )
                     )
+                    success = False
                     continue
 
             # Now we assign a license to the new M365 user.
             # First we see if there's a M365 SKU list in user
             # payload - if not we wrap the default SKU configured
             # for the m365 object into a single item list:
             existing_user_licenses = self._m365.getUserLicenses(user["m365_id"])
@@ -1520,14 +2172,15 @@
                     response = self._m365.assignLicenseToUser(user["m365_id"], sku_id)
                     if not response:
                         logger.error(
                             "Failed to assign license -> {} to Microsoft 365 user -> {}".format(
                                 sku_id, user_name
                             )
                         )
+                        success = False
                     else:
                         if (
                             not "m365_skus" in user
                         ):  # this is only True if the default license from the m365 object is taken
                             user["m365_skus"] = [sku_id]
                         logger.info(
                             "License -> {} has been assigned to Microsoft 365 user -> {}".format(
@@ -1575,15 +2228,15 @@
                 if user_department:
                     group_names.append(user_department)
                 logger.info(
                     "User -> {} has these groups in payload -> {} (including base group -> {}). Checking if they are Microsoft 365 Groups...".format(
                         user_name, group_names, user_department
                     )
                 )
-                # Go through all
+                # Go through all group names:
                 for group_name in group_names:
                     # Find the group payload item to the parent group name:
                     group = next(
                         (item for item in self._groups if item["name"] == group_name),
                         None,
                     )
                     if not group:
@@ -1616,14 +2269,15 @@
                             or not response["value"]
                         ):
                             logger.error(
                                 "Microsoft 365 Group -> {} not found. Skipping...".format(
                                     group_name
                                 )
                             )
+                            success = False
                         else:
                             group_id = response["value"][0]["id"]
 
                             # Check if user is already a member. We don't want
                             # to throw an error if the user is not found as a member:
                             if self._m365.isMember(group_id, user_id, show_error=False):
                                 logger.info(
@@ -1690,14 +2344,15 @@
                             or not response["value"]
                         ):
                             logger.error(
                                 "Microsoft 365 Group -> {} not found. Skipping...".format(
                                     group_name
                                 )
                             )
+                            success = False
                             continue
                         parent_group_id = response["value"][0]["id"]
 
                         # Check if user is already a member. We don't want
                         # to throw an error if the user is not found as a member:
                         if self._m365.isMember(
                             parent_group_id, user_id, show_error=False
@@ -1718,30 +2373,49 @@
                                 user_id,
                                 parent_group_name,
                                 parent_group_id,
                             )
                         )
                         self._m365.addGroupMember(parent_group_id, user_id)
 
+        if success:
+            self.writeStatusFile(section_name, self._users)
+
+        return success
+
         # end method definition
 
-    def processTeamsM365(self):
+    def processTeamsM365(self, section_name: str = "teamsM365") -> bool:
         """Process groups in payload and create matching Teams in Microsoft 365.
            We need to do this after the creation of the M365 users as wie require
            Group Owners to create teams.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._groups:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for group in self._groups:
             if not "name" in group:
                 logger.error("Team needs a name. Skipping...")
+                success = False
                 continue
             group_name = group["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in group and not group["enabled"]:
                 logger.info(
@@ -1762,31 +2436,39 @@
             if not "m365_id" in group:
                 # The "m365_id" value is set by the method processGroupsM365()
                 logger.error(
                     "No M365 Group exist for group -> {} (M365 Group creation may have failed). Skipping...".format(
                         group_name
                     )
                 )
+                success = False
                 continue
 
             if not self._m365.hasTeam(group_name):
                 logger.info(
                     "Create M365 Team -> {} for existing M365 Group -> {}...".format(
                         group_name, group_name
                     )
                 )
                 # Now "upgrading" this group to a MS Team:
                 new_team = self._m365.addTeam(group_name)
+                if not new_team:
+                    success = False
             else:
                 logger.info(
                     "M365 group -> {} already has an MS Team connected. Skipping...".format(
                         group_name
                     )
                 )
 
+        if success:
+            self.writeStatusFile(section_name, self._groups)
+
+        return success
+
         # end method definition
 
     def cleanupStaleTeamsM365(self, workspace_types: list):
         """Delete Microsoft Teams that are left-overs from former deployments.
            This method is currently not used.
 
         Args:
@@ -1821,43 +2503,94 @@
                         workspace_name
                     )
                 )
                 response = self._m365.deleteTeams(workspace_name)
 
         # end method definition
 
-    def cleanupAllTeamsM365(self) -> bool:
+    def cleanupAllTeamsM365(self, section_name: str = "teamsM365Cleanup") -> bool:
         """Delete Microsoft Teams that are left-overs from former deployments
 
         Args:
             None
         Returns:
-            boolean: True if teams have been deleted, False otherwise
+            bool: True if teams have been deleted, False otherwise
         """
 
+        # We want this cleanup to only run once even if we have
+        # multiple payload files - so we pass payload_specific=False here:
+        if self.checkStatusFile(
+            payload_section_name=section_name, payload_specific=False
+        ):
+            logger.info(
+                "Payload section -> {} has been processed successfully before. Skip cleanup of M365 teams...".format(
+                    section_name
+                )
+            )
+            return True
+        else:
+            logger.info("Processing payload section -> {}...".format(section_name))
+
+        # We don't want to delete MS Teams that are matching the regular OTCS Group Names (like "Sales")
         exception_list = self.getAllGroupNames()
-        pattern_list = [r"\(\d+\)", r"\d+\s-\s"]
+
+        # These are the patterns that each MS Teams needs to match at least one of to be deleted
+        # Pattern 1: all MS teams with a name that has a number in brackets, line "(1234)"
+        # Pattern 2: all MS Teams with a name that starts with a number followed by a space,
+        #            followed by a "- and followed by another space
+        # Pattern 3: all MS Teams with a name that starts with "WS" and a 1-4 digit number
+        #            (these are the workspaces for Purchase Contracts generated for Intelligent Filing)
+        # Pattern 4: all MS Teams with a name that ends with a 1-2 character + a number in brackets, like (US-1000)
+        #            this is a specialization of pattern 1
+        pattern_list = [
+            r"\(\d+\)",
+            r"\d+\s-\s",
+            r"^WS\d{1,4}$",
+            r"^.+?\s\(.{1,2}-\d+\)$",
+        ]
 
         result = self._m365.deleteAllTeams(exception_list, pattern_list)
 
+        # We want this cleanup to only run once even if we have
+        # multiple payload files - so we pass payload_specific=False here:
+        self.writeStatusFile(
+            payload_section_name=section_name,
+            payload_section=exception_list + pattern_list,
+            payload_specific=False,
+        )
+
         return result
 
         # end method definition
 
-    def processAdminSettings(self, admin_settings: list) -> bool:
+    def processAdminSettings(
+        self, admin_settings: list, section_name: str = "adminSettings"
+    ) -> bool:
         """Process admin settings in payload and import them to Extended ECM.
 
         Args:
             admin_settings (list): list of admin settings. We need this parameter
                                    as we process two different lists.
         Returns:
-            boolean: True if a restart of the OTCS pods is required. False otherwise.
+            bool: True if a restart of the OTCS pods is required. False otherwise.
         """
 
-        restart_required = False
+        if not admin_settings:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        restart_required: bool = False
+        success: bool = True
 
         for admin_setting in admin_settings:
             # Sanity checks:
             if not "filename" in admin_setting:
                 logger.error("Filename is missing - skipping to next admin setting...")
                 continue
             filename = admin_setting["filename"]
@@ -1899,48 +2632,67 @@
                 if response and response["results"]["data"]["restart"]:
                     logger.info("A restart of Extended ECM service is required.")
                     restart_required = True
             else:
                 logger.error(
                     "Admin settings file -> {} not found.".format(settings_file)
                 )
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, admin_settings)
 
         return restart_required
 
         # end method definition
 
-    def processExternalSystems(self):
+    def processExternalSystems(self, section_name: str = "externalSystems") -> bool:
         """Process external systems in payload and create them in Extended ECM.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         Side Effects:
             - based on system_type different other settings in the dict are set
             - reachability is tested and a flag is set in the dict are set
         """
 
+        if not self._external_systems:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for external_system in self._external_systems:
             #
             # 1: Do sanity checks for the payload:
             #
             if not "external_system_name" in external_system:
                 logger.error(
                     "External System connection needs a logical system name! Skipping to next external system..."
                 )
+                success = False
                 continue
             system_name = external_system["external_system_name"]
 
             if not "external_system_type" in external_system:
                 logger.error(
                     "External System connection -> {} needs a type (SAP, Salesfoce, SuccessFactors, AppWorks Platform)! Skipping to next external system...".format(
                         system_name
                     )
                 )
+                success = False
                 continue
             system_type = external_system["external_system_type"]
 
             if "enabled" in external_system and not external_system["enabled"]:
                 logger.info(
                     "Payload for External System -> {} ({}) is disabled. Skipping...".format(
                         system_name, system_type
@@ -1950,14 +2702,23 @@
 
             description = (
                 external_system["description"]
                 if external_system.get("description")
                 else ""
             )
 
+            # Possible Connection Types for external systems:
+            # "Business Scenario Sample" (Business Scenarios Sample Adapter)
+            # "ot.sap.c4c.SpiAdapter" (SAP C4C SPI Adapter)
+            # "ot.sap.c4c.SpiAdapterV2" (C4C SPI Adapter V2)
+            # "HTTP" (Default WebService Adapter)
+            # "ot.sap.S4HANAAdapter" (S/4HANA SPI Adapter)
+            # "SF" (SalesForce Adapter)
+            # "SFInstance" (SFWebService)
+
             # Set the default settings for the different system types:
             match system_type:
                 # Check if we have a SuccessFactors system:
                 case "SuccessFactors":
                     connection_type = "SFInstance"
                     auth_method = "OAUTH"
                     provider_name = system_type
@@ -1989,14 +2750,15 @@
 
             if not "as_url" in external_system:
                 logger.warning(
                     "External System connection -> {} needs an Application Server URL! Skipping to next external system...".format(
                         system_name
                     )
                 )
+                success = False
                 continue
             as_url = external_system["as_url"]
 
             # Extract the hostname:
             external_system_hostname = urlparse(as_url).hostname
             # Write this information back into the data structure:
             external_system["external_system_hostname"] = external_system_hostname
@@ -2041,21 +2803,23 @@
                 case "OAUTH":
                     if not "oauth_client_id" in external_system:
                         logger.error(
                             "External System connection -> {} is missing OAuth client ID! Skipping to next external system...".format(
                                 system_name
                             )
                         )
+                        success = False
                         continue
                     if not "oauth_client_secret" in external_system:
                         logger.error(
                             "External System connection -> {} is missing OAuth client secret! Skipping to next external system...".format(
                                 system_name
                             )
                         )
+                        success = False
                         continue
                     oauth_client_id = external_system["oauth_client_id"]
                     oauth_client_secret = external_system["oauth_client_secret"]
                     # For backward compatibility we also read username/password
                     # with OAuth settings:
                     username = (
                         external_system["username"]
@@ -2104,14 +2868,15 @@
             )
             if response == None:
                 logger.error(
                     "Failed to create external system -> {}; type -> {}".format(
                         system_name, connection_type
                     )
                 )
+                success = False
             else:
                 logger.info(
                     "Successfully created external system -> {}".format(system_name)
                 )
 
             #
             # 3: Create Authentication Handler for external system:
@@ -2123,37 +2888,40 @@
                     if not "saml_url" in external_system:
                         logger.error(
                             "SuccessFactors system -> {} ({}) is missing the SAML URL!".format(
                                 system_name,
                                 connection_type,
                             )
                         )
+                        success = False
                         continue
                     saml_url = external_system["saml_url"]
                     if not "otds_sp_endpoint" in external_system:
                         logger.error(
                             "SuccessFactors system -> {} ({}) is missing the OTDS endpoint!".format(
                                 system_name,
                                 connection_type,
                             )
                         )
+                        success = False
                         continue
                     otds_sp_endpoint = external_system["otds_sp_endpoint"]
 
                     response = self._otds.addAuthHandlerSAML(
                         name=system_name,
                         description=description,
                         provider_name=provider_name,
                         saml_url=saml_url,
                         otds_url=otds_sp_endpoint,
                     )
                     if response:
                         logger.info("Successfully added SAML authentication handler.")
                     else:
                         logger.error("Failed to add SAML authentication handler.")
+                        success = False
                 case "SAP":
                     # Configure a certificate-based SAP authentication handler:
                     if not "certificate_file" in external_system:
                         logger.error(
                             "External system -> {}; type -> {}; is missing the certificate file!".format(
                                 system_name, system_type
                             )
@@ -2163,28 +2931,30 @@
                         logger.error(
                             "External system -> {}; type -> {}; has a certificate file -> {} but it is missing the certificate password!".format(
                                 system_name,
                                 connection_type,
                                 external_system["certificate_file"],
                             )
                         )
+                        success = False
                         continue
                     certificate_file = external_system["certificate_file"]
                     certificate_password = external_system["certificate_password"]
                     certificate_description = external_system["description"]
                     response = self._otds.addAuthHandlerSAP(
                         name=system_name,
                         description=certificate_description,
                         certificate_file=certificate_file,
                         certificate_password=certificate_password,
                     )
                     if response:
                         logger.info("Successfully added SAP authentication handler.")
                     else:
                         logger.error("Failed to add SAP authentication handler.")
+                        success = False
                     # Upload and enable certificate file for Archive Center that is required for SAP scenarios
                     # we only do this if the necessary information is in payload and if OTAC is enabled:
                     if (
                         "archive_logical_name" in external_system
                         and "archive_certificate_file" in external_system
                         and self._otac
                     ):
@@ -2215,23 +2985,25 @@
                     if not "authorization_endpoint" in external_system:
                         logger.error(
                             "Salesforce system -> {} ({}) is missing the authorization endpoint!".format(
                                 system_name,
                                 connection_type,
                             )
                         )
+                        success = False
                         continue
                     authorization_endpoint = external_system["authorization_endpoint"]
                     if not "token_endpoint" in external_system:
                         logger.error(
                             "Salesforce system -> {} ({}) is missing the token endpoint!".format(
                                 system_name,
                                 connection_type,
                             )
                         )
+                        success = False
                         continue
                     token_endpoint = external_system["token_endpoint"]
                     response = self._otds.addAuthHandlerOAuth(
                         name=system_name,
                         description=description,
                         provider_name=provider_name,
                         client_id=oauth_client_id,
@@ -2240,35 +3012,57 @@
                         authorization_endpoint=authorization_endpoint,
                         token_endpoint=token_endpoint,
                         scope_string="id",
                     )
                     if response:
                         logger.info("Successfully added OAuth authentication handler.")
                     else:
+                        success = False
                         logger.error("Failed to add OAuth authentication handler.")
 
+        if success:
+            self.writeStatusFile(section_name, self._external_systems)
+
+        return success
+
         # end method definition
 
-    def processTransportPackages(self, transport_packages: list):
+    def processTransportPackages(
+        self, transport_packages: list, section_name: str = "transportPackages"
+    ) -> bool:
         """Process transport packages in payload and import them to Extended ECM.
 
         Args:
             transport_packages (list): list of transport packages. As we
                                        have three different lists (transport,
                                        content_transport, transport_post) so
                                        we need a parameter
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not transport_packages:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for transport_package in transport_packages:
             if not "name" in transport_package:
                 logger.error(
                     "Transport Package needs a name! Skipping to next transport..."
                 )
+                success = False
                 continue
             name = transport_package["name"]
 
             if "enabled" in transport_package and not transport_package["enabled"]:
                 logger.info(
                     "Payload for Transport Package -> {} is disabled. Skipping...".format(
                         name
@@ -2278,14 +3072,15 @@
 
             if not "url" in transport_package:
                 logger.error(
                     "Transport Package -> {} needs a URL! Skipping to next transport...".format(
                         name
                     )
                 )
+                success = False
                 continue
             if not "description" in transport_package:
                 logger.warning(
                     "Transport Package -> {} is missing a description".format(name)
                 )
             url = transport_package["url"]
             description = transport_package["description"]
@@ -2307,30 +3102,49 @@
                     "Deploy transport -> {}; URL -> {}".format(description, url)
                 )
                 response = self._otcs.deployTransport(url, name, description)
             if response == None:
                 logger.error(
                     "Failed to deploy transport -> {}; URL -> {}".format(name, url)
                 )
+                success = False
                 if self._stop_on_error:
-                    return
+                    break
             else:
                 logger.info("Successfully deployed transport -> {}".format(name))
 
+        if success:
+            self.writeStatusFile(section_name, transport_packages)
+
+        return success
+
         # end method definition
 
-    def processUserPhotos(self):
+    def processUserPhotos(self, section_name: str = "userPhotos") -> bool:
         """Process user photos in payload and assign them to Extended ECM users.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._users:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         # we assume the nickname of the photo item equals the login name of the user
         # we also assume that the photos have been uploaded / transported into the target system
         for user in self._users:
             user_name = user["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
@@ -2342,66 +3156,87 @@
 
             if not "id" in user:
                 logger.error(
                     "User -> {} does not have an ID. The user creation may have failed before. Skipping...".format(
                         user_name
                     )
                 )
+                success = False
                 continue
 
             user_id = user["id"]
 
             response = self._otcs.getNodeFromNickname(user_name)
             if response == None:
                 logger.warning(
                     "Missing photo for user -> {} - nickname not found. Skipping...".format(
                         user_name
                     )
                 )
                 continue
             photo_id = self._otcs.getResultValue(response, "id")
             response = self._otcs.updateUserPhoto(user_id, photo_id)
-            if response == None:
-                logger.warning("Failed to add photo for user -> {}".format(user_name))
+            if not response:
+                logger.error("Failed to add photo for user -> {}".format(user_name))
+                success = False
             else:
                 logger.info("Successfully added photo for user -> {}".format(user_name))
 
         # Check if Admin has a photo as well (nickname needs to be "admin"):
         response = self._otcs.getNodeFromNickname("admin")
         if response == None:
             logger.warning("Missing photo for admin - nickname not found. Skipping...")
-            return
-        photo_id = self._otcs.getResultValue(response, "id")
-        response = self._otcs.updateUserPhoto(1000, photo_id)
-        if response == None:
-            logger.warning("Failed to add photo for admin")
         else:
-            logger.info("Successfully added photo for admin")
+            photo_id = self._otcs.getResultValue(response, "id")
+            response = self._otcs.updateUserPhoto(1000, photo_id)
+            if response == None:
+                logger.warning("Failed to add photo for admin")
+            else:
+                logger.info("Successfully added photo for admin")
+
+        if success:
+            self.writeStatusFile(section_name, self._users)
+
+        return success
 
         # end method definition
 
-    def processUserPhotosM365(self):
+    def processUserPhotosM365(self, section_name: str = "userPhotosM365") -> bool:
         """Process user photos in payload and assign them to Microsoft 365 users.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._users:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         # we assume the nickname of the photo item equals the login name of the user
         # we also assume that the photos have been uploaded / transported into the target system
         for user in self._users:
             user_name = user["name"]
             if not "id" in user:
                 logger.error(
                     "User -> {} does not have an ID. The user creation may have failed before. Skipping...".format(
                         user_name
                     )
                 )
+                success = False
                 continue
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
                 logger.info(
                     "Payload for User -> {} is disabled. Skipping...".format(user_name)
@@ -2416,14 +3251,15 @@
                 continue
             if not "m365_id" in user:
                 logger.error(
                     "Office 365 user -> {} has not been created. Skipping...".format(
                         user_name
                     )
                 )
+                success = False
                 continue
 
             user_m365_id = user["m365_id"]
 
             if self._m365.getUserPhoto(user_m365_id, show_error=False):
                 logger.info(
                     "User -> {} ({}) has already a photo in Microsoft 365. Skipping...".format(
@@ -2452,14 +3288,15 @@
             response = self._otcs.downloadDocument(photo_id, photo_path)
             if response == None:
                 logger.warning(
                     "Failed to download photo for user -> {} from Extended ECM".format(
                         user_name
                     )
                 )
+                success = False
             else:
                 logger.info(
                     "Successfully downloaded photo for user -> {} from Extended ECM to file -> {}".format(
                         user_name, photo_path
                     )
                 )
 
@@ -2467,37 +3304,48 @@
             response = self._m365.updateUserPhoto(user_m365_id, photo_path)
             if response == None:
                 logger.error(
                     "Failed to upload photo for user -> {} to Microsoft 365".format(
                         user_name
                     )
                 )
+                success = False
             else:
                 logger.info(
                     "Successfully uploaded photo for user -> {} to Microsoft 365".format(
                         user_name
                     )
                 )
 
+        if success:
+            self.writeStatusFile(section_name, self._users)
+
+        return success
+
         # end method definition
 
-    def processWorkspaceTypes(self) -> list:
+    def processWorkspaceTypes(self, section_name: str = "workspaceTypes") -> list:
         """Create a data structure for all workspace types in the Extended ECM system.
 
         Args:
             None
         Returns:
             list: list of workspace types. Each list element is a dict with these values:
                 - id (string)
                 - name (string)
                 - templates (list)
                     + name
                     + id
         """
 
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
         # get all workspace types (these have been created by the transports and are not in the payload!):
         response = self._otcs.getWorkspaceTypes()
         if response == None:
             logger.error("No workspace types found!")
             self._workspace_types = []
         else:
             self._workspace_types = response["results"]
@@ -2565,121 +3413,44 @@
                 logger.warning(
                     "Workspace Types Name -> {} has no templates!".format(
                         workspace_type_name
                     )
                 )
                 continue
 
+        self.writeStatusFile(section_name, self._workspace_types)
+
         return self._workspace_types
 
         # end method definition
 
-    def processWorkspaceTemplateRegistrations(self):
-        """Process workspace template registrations for Extended ECM for Engineering.
-        This has been a work-around for a transport issue in 22.4. This code is not required
-        for 23.1 or newer. Right now we just disabled the payload. We may consider to remove
-        the code in future versions.
-
-        Args: None
-        Return: None
-        """
-
-        # loop through the workspace template registrations in the payload:
-        for workspace_template_registration in self._workspace_template_registrations:
-            # Do some sanity checks first and read the workspace type name
-            # and workspace template name from the payload:
-            if not "workspace_type_name" in workspace_template_registration:
-                logger.error(
-                    "Workspace template registration needs a workspace type name! Skipping to next workspace template registration..."
-                )
-                continue
-            type_name = workspace_template_registration["workspace_type_name"]
-
-            if (
-                "enabled" in workspace_template_registration
-                and not workspace_template_registration["enabled"]
-            ):
-                logger.info(
-                    "Payload for Workspace Template Registration for Workspace Type -> {} is disabled. Skipping...".format(
-                        type_name
-                    )
-                )
-                continue
-
-            if not "workspace_template_name" in workspace_template_registration:
-                logger.error(
-                    "Workspace template registration needs a workspace template name! Skipping to next workspace template registration..."
-                )
-                continue
-            template_name = workspace_template_registration["workspace_template_name"]
-
-            # now we have the template type name and the template name from the
-            # payload. We can now proceed to find these items in the workspace types
-            # data structure. First we lookup the workspace type:
-            workspace_type = next(
-                (item for item in self._workspace_types if item["name"] == type_name),
-                None,
-            )
-            if workspace_type is None:
-                logger.error(
-                    "Workspace Type with name -> {} not found.".format(type_name)
-                )
-                continue
+    def processWorkspaces(self, section_name: str = "workspaces") -> bool:
+        """Process workspaces in payload and create them in Extended ECM.
 
-            # now we use the template list in the workspace type datastructure
-            # to find the workspace template:
-            workspace_template_list = workspace_type["templates"]
-            if workspace_template_list is []:
-                logger.error(
-                    "Workspace Type with name -> {} has no templates.".format(type_name)
-                )
-                continue
+        Args:
+            None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
 
-            workspace_template = next(
-                (
-                    item
-                    for item in workspace_template_list
-                    if item["name"] == template_name
-                ),
-                None,
-            )
-            if workspace_template is None:
-                logger.error(
-                    "Workspace Type with name -> {} has no Template with name -> {}.".format(
-                        type_name, template_name
-                    )
-                )
-                continue
-            workspace_template_id = workspace_template["id"]
+        Side Effects:
+            Set workspace["nodeId] to the node ID of the created workspace
+        """
 
+        if not self._workspaces:
             logger.info(
-                "Register workspace template -> {} ({}) with workspace type -> {}".format(
-                    template_name, workspace_template_id, type_name
-                )
+                "Payload section -> {} is empty. Skipping...".format(section_name)
             )
+            return True
 
-            response = self._otcs.registerWorkspaceTemplate(workspace_template_id)
-            if response == None:
-                logger.error(
-                    "Failed to register workspace template -> {} with workspace type -> {}".format(
-                        template_name, type_name
-                    )
-                )
-                continue
-
-        # end method definition
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
 
-    def processWorkspaces(self):
-        """Process workspaces in payload and create them in Extended ECM.
-
-        Args: None
-        Return: None
-        Side Effects:
-            Set workspace["nodeId] to the node ID of the created workspace
-        """
+        success: bool = True
 
         for workspace in self._workspaces:
             # Read name from payload:
             if not "name" in workspace:
                 logger.error("Workspace needs a name! Skipping to next workspace...")
                 continue
             name = workspace["name"]
@@ -2704,22 +3475,18 @@
 
             # check if the workspace has been created before (effort to make the customizing code idem-potent)
             logger.info(
                 "Check if workspace -> {} of type -> {} does already exist...".format(
                     name, type_name
                 )
             )
-            response = self._otcs.getWorkspaceByTypeAndName(type_name, name)
-            logger.debug(
-                "Search for existing workspace delivered -> {}".format(response)
-            )
-            workspace_id = self._otcs.getResultValue(response, "id")
+            workspace_id = self.determineWorkspaceID(workspace)
             if workspace_id:
                 # we still want to set the nodeId as other parts of the payload depend on it:
-                workspace["nodeId"] = workspace_id
+                # workspace["nodeId"] = workspace_id
                 logger.info(
                     "Workspace -> {} of type -> {} does already exist and has ID -> {}! Skipping to next workspace...".format(
                         name, type_name, workspace_id
                     )
                 )
                 continue
 
@@ -2748,21 +3515,21 @@
                     logger.error(
                         "Parent Workspace with logical ID -> {} not found.".format(
                             parent_id
                         )
                     )
                     continue
 
-                if not "nodeId" in parent_workspace:
+                parent_workspace_node_id = self.determineWorkspaceID(parent_workspace)
+                if not parent_workspace_node_id:
                     logger.warning(
                         "Parent Workspace without node ID (parent workspace creation may have failed) - skipping to next workspace..."
                     )
                     continue
-                # now determine the actual node IDs of the parent workspace (should have been created before):
-                parent_workspace_node_id = parent_workspace["nodeId"]
+
                 logger.info(
                     "Parent Workspace with logical ID -> {} has node ID -> {}".format(
                         parent_id, parent_workspace_node_id
                     )
                 )
             else:
                 # if no parent_id is specified the workspace location is determined by the workspace type definition
@@ -3343,15 +4110,15 @@
                 continue
 
             # Now we add the node ID of the new workspace to the payload data structure
             # This will be reused when creating the workspace relationships!
             workspace["nodeId"] = self._otcs.getResultValue(response, "id")
 
             # We also get the name the workspace was finally created with.
-            # This can be different form the namein the payload as additional
+            # This can be different form the name in the payload as additional
             # naming conventions from the Workspace Type definitions may apply.
             # This is important to make the python container idem-potent.
             response = self._otcs.getWorkspace(workspace["nodeId"])
             workspace["name"] = self._otcs.getResultValue(response, "name")
 
             logger.info(
                 "Successfully created workspace with final name -> {} and node ID -> {}".format(
@@ -3411,29 +4178,51 @@
                         else:
                             logger.info(
                                 "Assigned Classification -> {} to workspace -> {}".format(
                                     classification_path[-1], name
                                 )
                             )
 
+        if success:
+            self.writeStatusFile(section_name, self._workspaces)
+
+        return success
+
         # end method definition
 
-    def processWorkspaceRelationships(self):
+    def processWorkspaceRelationships(
+        self, section_name: str = "workspaceRelationships"
+    ) -> bool:
         """Process workspaces relationships in payload and create them in Extended ECM.
 
         Relationships can only be created if all workspaces have been created before.
         Once a workspace got created, the node ID of that workspaces has been added
         to the payload["workspaces"] data structure (see processWorkspaces())
         Relationships are created between the node IDs of two business workspaces
         (and not the logical IDs in the inital payload specification)
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._workspaces:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for workspace in self._workspaces:
             # Read name from payload:
             if not "name" in workspace:
                 continue
             name = workspace["name"]
 
             # Check if element has been disabled in payload (enabled = false).
@@ -3460,21 +4249,21 @@
                     "Workspace without ID cannot have a relationship - skipping to next workspace..."
                 )
                 continue
 
             workspace_id = workspace["id"]
             logger.info("Workspace -> {} has relationships - creating...".format(name))
 
-            if not "nodeId" in workspace:
+            workspace_node_id = self.determineWorkspaceID(workspace)
+            if not workspace_node_id:
                 logger.warning(
                     "Workspace without node ID cannot have a relationship (workspace creation may have failed) - skipping to next workspace..."
                 )
                 continue
             # now determine the actual node IDs of the workspaces (have been created above):
-            workspace_node_id = workspace["nodeId"]
             logger.info(
                 "Workspace with logical ID -> {} has node ID -> {}".format(
                     workspace_id, workspace_node_id
                 )
             )
 
             for related_workspace_id in workspace["relationships"]:
@@ -3489,31 +4278,32 @@
                 )
                 if related_workspace is None:
                     logger.error(
                         "Related Workspace with logical ID -> {} not found.".format(
                             related_workspace_id
                         )
                     )
+                    success = False
                     continue
 
                 if "enabled" in related_workspace and not related_workspace["enabled"]:
                     logger.info(
                         "Payload for Related Workspace -> {} is disabled. Skipping...".format(
                             related_workspace["name"]
                         )
                     )
                     continue
 
-                if not "nodeId" in related_workspace:
+                related_workspace_node_id = self.determineWorkspaceID(related_workspace)
+                if not related_workspace_node_id:
                     logger.warning(
                         "Related Workspace without node ID (workspaces creation may have failed) - skipping to next workspace..."
                     )
                     continue
-                # now determine the actual node IDs of the related workspace (should have been created above):
-                related_workspace_node_id = related_workspace["nodeId"]
+
                 logger.info(
                     "Related Workspace with logical ID -> {} has node ID -> {}".format(
                         related_workspace_id, related_workspace_node_id
                     )
                 )
 
                 logger.info(
@@ -3535,28 +4325,49 @@
                         )
                     )
                     continue
 
                 response = self._otcs.createWorkspaceRelationship(
                     workspace_node_id, related_workspace_node_id
                 )
-                if response == None:
+                if not response:
                     logger.error("Failed to create workspace relationship.")
+                    success = False
                 else:
                     logger.info("Successfully created workspace relationship.")
 
+        if success:
+            self.writeStatusFile(section_name, self._workspaces)
+
+        return success
+
         # end method definition
 
-    def processWorkspaceMembers(self):
+    def processWorkspaceMembers(self, section_name: str = "workspaceMembers") -> bool:
         """Process workspaces members in payload and create them in Extended ECM.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._workspaces:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for workspace in self._workspaces:
             # Read name from payload (just for logging):
             if not "name" in workspace:
                 continue
             workspace_name = workspace["name"]
 
             # Check if element has been disabled in payload (enabled = false).
@@ -3582,22 +4393,22 @@
             workspace_id = workspace["id"]
             logger.info(
                 "Workspace -> {} has memberships in payload - establishing...".format(
                     workspace_name
                 )
             )
 
-            if not "nodeId" in workspace:
+            workspace_node_id = self.determineWorkspaceID(workspace)
+            if not workspace_node_id:
                 logger.warning(
                     "Workspace without node ID cannot have a members (workspaces creation may have failed) - skipping to next workspace..."
                 )
                 continue
 
             # now determine the actual node IDs of the workspaces (have been created by processWorkspaces()):
-            workspace_node_id = workspace["nodeId"]
             workspace_node = self._otcs.getNode(workspace_node_id)
             workspace_owner_id = self._otcs.getResultValue(
                 workspace_node, "owner_user_id"
             )
             workspace_owner_name = self._otcs.getResultValue(workspace_node, "owner")
 
             workspace_roles = self._otcs.getWorkspaceRoles(workspace_node_id)
@@ -3652,14 +4463,15 @@
 
                 if member_role_name == "":  # role name is required
                     logger.error(
                         "Members of workspace -> {} is missing the role name.".format(
                             workspace_name
                         )
                     )
+                    success = False
                     continue
                 if (
                     member_users == [] and member_groups == []
                 ):  # we either need users or groups (or both)
                     logger.warning(
                         "Role -> {} of workspace -> {} does not have any members (no users nor groups).".format(
                             member_role_name, workspace_name
@@ -3673,14 +4485,15 @@
                 if role_id is None:
                     #    if member_role is None:
                     logger.error(
                         "Workspace -> {} does not have a role with name -> {}".format(
                             workspace_name, member_role_name
                         )
                     )
+                    success = False
                     continue
                 logger.info("Role -> {} has ID -> {}".format(member_role_name, role_id))
 
                 # Process users as workspaces members:
                 for member_user in member_users:
                     # find member user in current payload:
                     member_user_id = next(
@@ -3722,14 +4535,15 @@
                             "Failed to add user -> {} ({}) to role -> {} of workspace -> {}".format(
                                 member_user_id["name"],
                                 user_id,
                                 member_role_name,
                                 workspace_name,
                             )
                         )
+                        success = False
                     else:
                         logger.info(
                             "Successfully added user -> {} ({}) to role -> {} of workspace -> {}".format(
                                 member_user_id["name"],
                                 user_id,
                                 member_role_name,
                                 workspace_name,
@@ -3742,14 +4556,15 @@
                         (item for item in self._groups if item["name"] == member_group),
                         None,
                     )
                     if member_group_id is None:
                         logger.error(
                             "Cannot find group with name -> {}".format(member_group)
                         )
+                        success = False
                         continue
                     group_id = member_group_id["id"]
 
                     response = self._otcs.addMemberToWorkspace(
                         workspace_node_id, role_id, group_id
                     )
                     if response == None:
@@ -3757,35 +4572,57 @@
                             "Failed to add group -> {} ({}) to role -> {} of workspace -> {}".format(
                                 member_group_id["name"],
                                 group_id,
                                 member_role_name,
                                 workspace_name,
                             )
                         )
+                        success = False
                     else:
                         logger.info(
                             "Successfully added group -> {} ({}) to role -> {} of workspace -> {}".format(
                                 member_group_id["name"],
                                 group_id,
                                 member_role_name,
                                 workspace_name,
                             )
                         )
 
+        if success:
+            self.writeStatusFile(section_name, self._workspaces)
+
+        return success
+
         # end method definition
 
-    def processWebReports(self, web_reports: list):
+    def processWebReports(
+        self, web_reports: list, section_name: str = "webReports"
+    ) -> bool:
         """Process web reports in payload and run them in Extended ECM.
 
         Args:
             web_reports (list): list of web reports. As we have two different list (pre and post)
                                 we need to pass the actual list as parameter.
-        Return: None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not web_reports:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for web_report in web_reports:
             nick_name = web_report["nickname"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in web_report and not web_report["enabled"]:
                 logger.info(
@@ -3799,14 +4636,15 @@
 
             if not self._otcs.getNodeFromNickname(nick_name):
                 logger.error(
                     "Web Report with nickname -> {} does not exist! Skipping...".format(
                         nick_name
                     )
                 )
+                success = False
                 continue
 
             # be careful to avoid key errors as Web Report parameters are optional:
             actual_params = (
                 web_report["parameters"] if web_report.get("parameters") else {}
             )
             formal_params = self._otcs.getWebReportParameters(nick_name)
@@ -3820,14 +4658,15 @@
                 # Check 1: are there formal parameters at all?
                 if not formal_params:
                     logger.error(
                         "Web Report -> {} is called with actual parameters but it does not expect parameters! Skipping...".format(
                             nick_name
                         )
                     )
+                    success = False
                     continue
                 lets_continue = False
                 # Check 2: Iterate through the actual parameters given in the payload
                 # and see if there's a matching formal parameter expected by the Web Report:
                 for key, value in actual_params.items():
                     # Check if there's a matching formal parameter defined on the Web Report node:
                     formal_param = next(
@@ -3836,14 +4675,15 @@
                     )
                     if formal_param is None:
                         logger.error(
                             "Web Report -> {} is called with parameter -> {} that is not expected! Skipping...".format(
                                 nick_name, key
                             )
                         )
+                        success = False
                         lets_continue = True  # we cannot do a "continue" here directly as we are in an inner loop
                 # Check 3: Iterate through the formal parameters and validate there's a matching
                 # actual parameter defined in the payload for each mandatory formal parameter
                 # that does not have a default value:
                 for formal_param in formal_params:
                     if (
                         (formal_param["mandatory"] == True)
@@ -3851,14 +4691,15 @@
                         and not actual_params.get(formal_param["parm_name"])
                     ):
                         logger.error(
                             "Web Report -> {} is called without mandatory parameter -> {}! Skipping...".format(
                                 nick_name, formal_param["parm_name"]
                             )
                         )
+                        success = False
                         lets_continue = True  # we cannot do a "continue" here directly as we are in an inner loop
                 # Did any of the checks fail?
                 if lets_continue:
                     continue
                 # Actual parameters are validated, we can run the Web Report:
                 response = self._otcs.runWebReport(nick_name, actual_params)
             else:
@@ -3881,37 +4722,60 @@
                     )
                     if required_param:
                         logger.error(
                             "Web Report -> {} is called without parameters but has a mandatory parameter -> {} without a default value! Skipping...".format(
                                 nick_name, required_param["parm_name"]
                             )
                         )
+                        success = False
                         continue
                     else:  # we are good to proceed!
                         logger.debug(
                             "Web Report -> {} does not have a mandatory parameter without a default value!".format(
                                 nick_name
                             )
                         )
                 response = self._otcs.runWebReport(nick_name)
             if response == None:
                 logger.error("Failed to run web report -> {}".format(nick_name))
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, web_reports)
+
+        return success
 
         # end method definition
 
-    def processCSApplications(self, otcs_object: object = None):
+    def processCSApplications(
+        self, otcs_object: object = None, section_name: str = "csApplications"
+    ) -> bool:
         """Process CS applications in payload and install them in Extended ECM.
         The CS Applications need to be installed in all frontend and backends.
 
         Args:
             otcs_object (object): this can either be the OTCS frontend or OTCS backend. If None
                                   then the otcs_backend is used.
-        Return: None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._cs_applications:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         # OTCS backend is the default:
         if not otcs_object:
             otcs_object = self._otcs_backend
 
         for cs_application in self._cs_applications:
             application_name = cs_application["name"]
 
@@ -3933,41 +4797,62 @@
                 )
             )
             response = otcs_object.installCSApplication(application_name)
             if response == None:
                 logger.error(
                     "Failed to install CS Application -> {}!".format(application_name)
                 )
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._cs_applications)
+
+        return success
 
         # end method definition
 
-    def processUserSettings(self):
+    def processUserSettings(self, section_name: str = "userSettings") -> bool:
         """Process user settings in payload and apply themin OTDS.
            This includes password settings and user display settings.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._users:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for user in self._users:
             user_name = user["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
                 logger.info(
                     "Payload for User -> {} is disabled. Skipping...".format(user_name)
                 )
                 continue
 
             user_partition = self._otcs.config()["partition"]
             if not user_partition:
                 logger.error("User partition not found!")
+                success = False
+                continue
 
             # Set the OTDS display name. Extended ECM does not use this but
             # it makes AppWorks display users correctly (and it doesn't hurt)
             # We only set this if firstname _and_ last name are in the payload:
             if "firstname" in user and "lastname" in user:
                 user_display_name = user["firstname"] + " " + user["lastname"]
                 response = self._otds.updateUser(
@@ -3981,36 +4866,59 @@
                     )
                 else:
                     logger.error(
                         "Display name for user -> {} could not be updated to -> {}".format(
                             user_name, user_display_name
                         )
                     )
+                    success = False
 
             # Don't enforce the user to reset password at first login (settings in OTDS):
             logger.info(
                 "Don't enforce password change for user -> {}...".format(user_name)
             )
             response = self._otds.updateUser(
                 user_partition, user_name, "UserMustChangePasswordAtNextSignIn", "False"
             )
+            if not response:
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._users)
+
+        return success
 
         # end method definition
 
-    def processUserFavoritesAndProfiles(self):
+    def processUserFavoritesAndProfiles(
+        self, section_name: str = "userFavoritesAndProfiles"
+    ) -> bool:
         """Process user favorites in payload and create them in Extended ECM.
            This method also simulates browsing the favorites to populate the
            widgets on the landing pages and sets personal preferences.
 
         Args:
             None
         Returns:
-            None
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._users:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         # We can only set favorites if we impersonate / authenticate as the user.
         # The following code (for loop) will change the authenticated user - we need to
         # switch it back to admin user later so we safe the admin credentials for this:
 
         if self._users:
             # save admin credentials for later switch back to admin user:
             admin_credentials = self._otcs.credentials()
@@ -4033,14 +4941,15 @@
 
             # we re-authenticate as the user:
             logger.info("Authenticate user -> {}...".format(user_name))
             # True = force new login with new user
             cookie = self._otcs.authenticate(True)
             if not cookie:
                 logger.error("Couldn't authenticate user -> {}".format(user_name))
+                success = False
                 continue
 
             # we update the user profile to activate navigation tree:
             response = self._otcs.updateUserProfile("conwsNavigationTreeView", True)
             if response is None:
                 logger.warning(
                     "Profile for user -> {} couldn't be updated!".format(user_name)
@@ -4056,42 +4965,29 @@
             favorites = user["favorites"]
             for favorite in favorites:
                 # check if favorite is a logical workspace name
                 favorite_item = next(
                     (item for item in self._workspaces if item["id"] == favorite), None
                 )
                 is_workspace = False
-                if favorite_item is not None:
+                if favorite_item:
                     logger.info(
                         "Found favorite item (workspace) in payload -> {}".format(
                             favorite_item["name"]
                         )
                     )
-                    if "nodeId" in favorite_item:
-                        favorite_id = favorite_item["nodeId"]
-                    else:
-                        logger.info(
-                            "Favorite -> {} (workspace) does not have a nodeId in payload - check if it was created by an external systems...".format(
-                                favorite
+                    favorite_id = self.determineWorkspaceID(favorite_item)
+                    if not favorite_id:
+                        logger.warning(
+                            "Workspace of type -> {} and name -> {} does not exist. Cannot create favorite. Skipping...".format(
+                                favorite_item["type_name"], favorite_item["name"]
                             )
                         )
-                        response = self._otcs.getWorkspaceByTypeAndName(
-                            favorite_item["type_name"], favorite_item["name"]
-                        )
-                        favorite_id = self._otcs.getResultValue(response, "id")
-                        if not favorite_id:
-                            logger.warning(
-                                "Workspace of type -> {} and name -> {} does not exist. Cannot create favorite. Skipping...".format(
-                                    favorite_item["type_name"], favorite_item["name"]
-                                )
-                            )
-                            continue
-                        else:
-                            # store ID in payload in case it is used again
-                            favorite_item["nodeId"] = favorite_id
+                        continue
+
                     is_workspace = True
                 else:
                     # alternatively try to find the item as a nickname:
                     favorite_item = self._otcs.getNodeFromNickname(favorite)
                     favorite_id = self._otcs.getResultValue(favorite_item, "id")
                     #                    if favorite_item is None:
                     if favorite_id is None:
@@ -4137,14 +5033,15 @@
                 )
                 if not proxy_user or not "id" in proxy_user:
                     logger.error(
                         "The proxy -> {} for user -> {} does not exist! Skipping proxy...".format(
                             proxy, user_name
                         )
                     )
+                    success = False
                     continue
                 proxy_user_id = proxy_user["id"]
 
                 # Check if the proxy is already set:
                 if not self._otcs.isProxy(proxy):
                     logger.info(
                         "Set user -> {} ({}) as proxy for user -> {}.".format(
@@ -4171,23 +5068,45 @@
                 "Authenticate as admin user -> {}...".format(
                     admin_credentials["username"]
                 )
             )
             # True = force new login with new user
             cookie = self._otcs.authenticate(True)
 
+        if success:
+            self.writeStatusFile(section_name, self._users)
+
+        return success
+
         # end method definition
 
-    def processSecurityClearances(self):
+    def processSecurityClearances(
+        self, section_name: str = "securityClearances"
+    ) -> bool:
         """Process Security Clearances for Extended ECM.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._security_clearances:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for security_clearance in self._security_clearances:
             clearance_level = security_clearance.get("level")
             clearance_name = security_clearance.get("name")
 
             if "enabled" in security_clearance and not security_clearance["enabled"]:
                 logger.info(
                     "Payload for Security Clearance -> {} is disabled. Skipping...".format(
@@ -4208,24 +5127,47 @@
                 self._otcs.runWebReport(
                     "web_report_security_clearance", security_clearance
                 )
             else:
                 logger.error(
                     "Cannot create Security Clearance - either level or name is missing!"
                 )
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._security_clearances)
+
+        return success
 
         # end method definition
 
-    def processSupplementalMarkings(self):
+    def processSupplementalMarkings(
+        self, section_name: str = "supplementalMarkings"
+    ) -> bool:
         """Process Supplemental Markings for Extended ECM.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._supplemental_markings:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for supplemental_marking in self._supplemental_markings:
             code = supplemental_marking.get("code")
 
             if (
                 "enabled" in supplemental_marking
                 and not supplemental_marking["enabled"]
             ):
@@ -4246,24 +5188,45 @@
                 self._otcs.runWebReport(
                     "web_report_supplemental_marking", supplemental_marking
                 )
             else:
                 logger.error(
                     "Cannot create Supplemental Marking - either code or description is missing!"
                 )
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._supplemental_markings)
+
+        return success
 
         # end method definition
 
-    def processUserSecurity(self):
+    def processUserSecurity(self, section_name: str = "userSecurity"):
         """Process Security Clearance and Supplemental Markings for Extended ECM users.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._users:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for user in self._users:
             user_id = user.get("id")
             user_name = user.get("name")
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
@@ -4282,120 +5245,175 @@
             # Read supplemental markings from user payload (it is optional!)
             user_supplemental_markings = user.get("supplemental_markings")
             if user_id and user_supplemental_markings:
                 response = self._otcs.assignUserSupplementalMarkings(
                     user_id, user_supplemental_markings
                 )
 
+        if success:
+            self.writeStatusFile(section_name, self._users)
+
+        return success
+
         # end method definition
 
-    def processRecordsManagementSettings(self):
+    def processRecordsManagementSettings(
+        self, section_name: str = "recordsManagementSettings"
+    ):
         """Process Records Management Settings for Extended ECM.
         The setting files need to be placed in the OTCS file system file via
         a transport into the Support Asset Volume.
 
         Args: None
         Return: None
         """
 
+        if not self._records_management_settings:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         if (
             "records_management_system_settings" in self._records_management_settings
             and self._records_management_settings["records_management_system_settings"]
             != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings[
                     "records_management_system_settings"
                 ]
             )
-            self._otcs.importRecordsManagementSettings(filename)
+            response = self._otcs.importRecordsManagementSettings(filename)
+            if not response:
+                success = False
 
         if (
             "records_management_codes" in self._records_management_settings
             and self._records_management_settings["records_management_codes"] != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["records_management_codes"]
             )
-            self._otcs.importRecordsManagementCodes(filename)
+            response = self._otcs.importRecordsManagementCodes(filename)
+            if not response:
+                success = False
 
         if (
             "records_management_rsis" in self._records_management_settings
             and self._records_management_settings["records_management_rsis"] != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["records_management_rsis"]
             )
-            self._otcs.importRecordsManagementRSIs(filename)
+            response = self._otcs.importRecordsManagementRSIs(filename)
+            if not response:
+                success = False
 
         if (
             "physical_objects_system_settings" in self._records_management_settings
             and self._records_management_settings["physical_objects_system_settings"]
             != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["physical_objects_system_settings"]
             )
-            self._otcs.importPhysicalObjectsSettings(filename)
+            response = self._otcs.importPhysicalObjectsSettings(filename)
+            if not response:
+                success = False
 
         if (
             "physical_objects_codes" in self._records_management_settings
             and self._records_management_settings["physical_objects_codes"] != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["physical_objects_codes"]
             )
-            self._otcs.importPhysicalObjectsCodes(filename)
+            response = self._otcs.importPhysicalObjectsCodes(filename)
+            if not response:
+                success = False
 
         if (
             "physical_objects_locators" in self._records_management_settings
             and self._records_management_settings["physical_objects_locators"] != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["physical_objects_locators"]
             )
-            self._otcs.importPhysicalObjectsLocators(filename)
+            response = self._otcs.importPhysicalObjectsLocators(filename)
+            if not response:
+                success = False
 
         if (
             "security_clearance_codes" in self._records_management_settings
             and self._records_management_settings["security_clearance_codes"] != ""
         ):
             filename = (
                 self._custom_settings_dir
                 + self._records_management_settings["security_clearance_codes"]
             )
-            self._otcs.importSecurityClearanceCodes(filename)
+            response = self._otcs.importSecurityClearanceCodes(filename)
+            if not response:
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._records_management_settings)
+
+        return success
 
         # end method definition
 
-    def processHolds(self):
+    def processHolds(self, section_name: str = "holds") -> bool:
         """Process Records Management Holds for Extended ECM users.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._holds:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for hold in self._holds:
             if not "name" in hold:
                 logger.error("Cannot create Hold without a name! Skipping...")
                 continue
             hold_name = hold["name"]
 
             if not "type" in hold:
                 logger.error(
                     "Cannot create Hold -> {} without a type! Skipping...".format(
                         hold_name
                     )
                 )
+                success = False
                 continue
             hold_type = hold["type"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in hold and not hold["enabled"]:
                 logger.info(
@@ -4447,24 +5465,48 @@
 
             if hold and hold["holdID"]:
                 logger.info(
                     "Successfully created hold -> {} with ID -> {}".format(
                         hold_name, hold["holdID"]
                     )
                 )
+            else:
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._holds)
+
+        return success
 
         # end method definition
 
-    def processAdditionalGroupMembers(self):
+    def processAdditionalGroupMembers(
+        self, section_name: str = "additionalGroupMemberships"
+    ) -> bool:
         """Process additional groups memberships we want to have in OTDS.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._additional_group_members:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for additional_group_member in self._additional_group_members:
             if not "parent_group" in additional_group_member:
                 logger.error("Missing parent_group! Skipping...")
                 continue
             parent_group = additional_group_member["parent_group"]
 
             if (
@@ -4480,14 +5522,15 @@
 
             if (not "user_name" in additional_group_member) and (
                 not "group_name" in additional_group_member
             ):
                 logger.error(
                     "Either group_name or user_name need to be specified! Skipping..."
                 )
+                success = False
                 continue
             if "group_name" in additional_group_member:
                 group_name = additional_group_member["group_name"]
                 logger.info(
                     "Adding group -> {} to parent group -> {} in OTDS.".format(
                         group_name, parent_group
                     )
@@ -4495,38 +5538,62 @@
                 response = self._otds.addGroupToParentGroup(group_name, parent_group)
                 if not response:
                     logger.error(
                         "Failed to add group -> {} to parent group -> {} in OTDS.".format(
                             group_name, parent_group
                         )
                     )
+                    success = False
             elif "user_name" in additional_group_member:
                 user_name = additional_group_member["user_name"]
                 logger.info(
                     "Adding user -> {} to group -> {} in OTDS.".format(
                         user_name, parent_group
                     )
                 )
                 response = self._otds.addUserToGroup(user_name, parent_group)
                 if not response:
                     logger.error(
                         "Failed to add user -> {} to group -> {} in OTDS.".format(
                             user_name, parent_group
                         )
                     )
+                    success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._additional_group_members)
+
+        return success
 
         # end method definition
 
-    def processAdditionalAccessRoleMembers(self):
+    def processAdditionalAccessRoleMembers(
+        self, section_name: str = "additionalAccessRoleMemberships"
+    ) -> bool:
         """Process additional access role memberships we want to have in OTDS.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._additional_access_role_members:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for additional_access_role_member in self._additional_access_role_members:
             if not "access_role" in additional_access_role_member:
                 logger.error("Missing access_role! Skipping...")
                 continue
             access_role = additional_access_role_member["access_role"]
 
             if (
@@ -4544,14 +5611,15 @@
                 (not "user_name" in additional_access_role_member)
                 and (not "group_name" in additional_access_role_member)
                 and (not "partition_name" in additional_access_role_member)
             ):
                 logger.error(
                     "Either group_name or user_name need to be specified! Skipping..."
                 )
+                success = False
                 continue
             if "group_name" in additional_access_role_member:
                 group_name = additional_access_role_member["group_name"]
                 logger.info(
                     "Adding group -> {} to access role -> {} in OTDS.".format(
                         group_name, access_role
                     )
@@ -4559,28 +5627,30 @@
                 response = self._otds.addGroupToAccessRole(access_role, group_name)
                 if not response:
                     logger.error(
                         "Failed to add group -> {} to access role -> {} in OTDS.".format(
                             group_name, access_role
                         )
                     )
+                    success = False
             elif "user_name" in additional_access_role_member:
                 user_name = additional_access_role_member["user_name"]
                 logger.info(
                     "Adding user -> {} to access role -> {} in OTDS.".format(
                         user_name, access_role
                     )
                 )
                 response = self._otds.addUserToAccessRole(access_role, user_name)
                 if not response:
                     logger.error(
                         "Failed to add user -> {} to access role -> {} in OTDS.".format(
                             user_name, access_role
                         )
                     )
+                    success = False
             elif "partition_name" in additional_access_role_member:
                 partition_name = additional_access_role_member["partition_name"]
                 logger.info(
                     "Adding partition -> {} to access role -> {} in OTDS.".format(
                         partition_name, access_role
                     )
                 )
@@ -4589,24 +5659,45 @@
                 )
                 if not response:
                     logger.error(
                         "Failed to add partition -> {} to access role -> {} in OTDS.".format(
                             partition_name, access_role
                         )
                     )
+                    success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._additional_access_role_members)
+
+        return success
 
         # end method definition
 
-    def processRenamings(self):
+    def processRenamings(self, section_name: str = "renamings") -> bool:
         """Process renamings specified in payload and rename existing Extended ECM items.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._renamings:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for renaming in self._renamings:
             if not "nodeid" in renaming:
                 if not "volume" in renaming:
                     logger.error(
                         "Renamings require either a node ID or a volume! Skipping to next renaming..."
                     )
                     continue
@@ -4627,27 +5718,46 @@
             )
             if not response:
                 logger.error(
                     "Failed to rename node ID -> {} to new name -> {}.".format(
                         node_id, renaming["name"]
                     )
                 )
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._renamings)
+
+        return success
 
         # end method definition
 
-    def processItems(self, items: list):
+    def processItems(self, items: list, section_name: str = "items") -> bool:
         """Process items specified in payload and create them in Extended ECM.
 
         Args:
-            otcs: OTCS object
             items: list of items to create (need this as parameter as we
                    have multiple lists)
-        Return: None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not items:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for item in items:
             if not "name" in item:
                 logger.error("Item needs a name. Skipping...")
                 continue
             item_name = item["name"]
 
             # Check if element has been disabled in payload (enabled = false).
@@ -4672,25 +5782,27 @@
                 # if not parent_node:
                 if not parent_id:
                     logger.error(
                         "Item -> {} has a parent nickname -> {} that does not exist. Skipping...".format(
                             item_name, parent_nickname
                         )
                     )
+                    success = False
                     continue
             else:  # use parent_path and Enterprise Volume
                 parent_node = self._otcs.getNodeByVolumeAndPath(141, parent_path)
                 parent_id = self._otcs.getResultValue(parent_node, "id")
                 if not parent_id:
                     # if not parent_node:
                     logger.error(
                         "Item -> {} has a parent path that does not exist. Skipping...".format(
                             item_name
                         )
                     )
+                    success = False
                     continue
 
             original_nickname = item.get("original_nickname")
             original_path = item.get("original_path")
 
             if original_nickname:
                 original_node = self._otcs.getNodeFromNickname(original_nickname)
@@ -4698,31 +5810,34 @@
                 if not original_id:
                     # if not original_node:
                     logger.error(
                         "Item -> {} has a original nickname -> {} that does not exist. Skipping...".format(
                             item_name, original_nickname
                         )
                     )
+                    success = False
                     continue
             elif original_path:
                 original_node = self._otcs.getNodeByVolumeAndPath(141, original_path)
                 original_id = self._otcs.getResultValue(original_node, "id")
                 if not original_id:
                     # if not original_node:
                     logger.error(
                         "Item -> {} has a original path that does not exist. Skipping...".format(
                             item_name
                         )
                     )
+                    success = False
                     continue
             else:
                 original_id = 0
 
             if not "type" in item:
                 logger.error("Item -> {} needs a type. Skipping...".format(item_name))
+                success = False
                 continue
 
             item_type = item.get("type")
             item_url = item.get("url")
 
             # check that we have the required information
             # for the given item type:
@@ -4730,44 +5845,56 @@
                 case 140:  # URL
                     if item_url == "":
                         logger.error(
                             "Item -> {} has type URL but the URL is not in the payload. Skipping...".format(
                                 item_name
                             )
                         )
+                        success = False
                         continue
                 case 1:  # Shortcut
                     if original_id == 0:
                         logger.error(
                             "Item -> {} has type Shortcut but the original item is not in the payload. Skipping...".format(
                                 item_name
                             )
                         )
+                        success = False
                         continue
 
             # Check if an item with the same name does already exist.
             # This can also be the case if the python container runs a 2nd time.
             # For this reason we are also not issuing an error but just an info (False):
-            response = self._otcs.getNodeByParentAndName(parent_id, item_name, False)
+            response = self._otcs.getNodeByParentAndName(
+                parent_id, item_name, show_error=False
+            )
             if self._otcs.getResultValue(response, "name") == item_name:
                 logger.info(
                     "Item with name -> {} does already exist in parent folder with ID -> {}".format(
                         item_name, parent_id
                     )
                 )
                 continue
             response = self._otcs.createItem(
                 parent_id, item_type, item_name, item_description, item_url, original_id
             )
             if not response:
                 logger.error("Failed to create item -> {}.".format(item_name))
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, items)
+
+        return success
 
         # end method definition
 
-    def processPermissions(self, permissions: list):
+    def processPermissions(
+        self, permissions: list, section_name: str = "permissions"
+    ) -> bool:
         """Process items specified in payload and upadate permissions.
 
         Args:
             permissions: list of items to apply permissions to.
                          Each list item in the payload is a dict with this structure:
                             {
                                 nodeid = "..."
@@ -4787,24 +5914,39 @@
                                     name = "..."
                                     permissions = []
                                 }
                                 ]
                                 apply_to = 2
                             }
 
-        Return: None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not permissions:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for permission in permissions:
             if (
                 not "path" in permission
                 and not "volume" in permission
                 and not "nickname" in permission
             ):
                 logger.error("Item to change permission is not specified. Skipping...")
+                success = False
                 continue
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in permission and not permission["enabled"]:
                 logger.info("Payload for Permission is disabled. Skipping...")
                 continue
@@ -4823,14 +5965,15 @@
                 node_id = self._otcs.getResultValue(volume, "id")
                 if not node_id:
                     logger.error(
                         "Illegal volume -> {} in permission specification. Skipping...".format(
                             volume_type
                         )
                     )
+                    success = False
                     continue
 
             # Check if "path" is in payload and not empty list
             # (path can be combined with volume so we need to take volume into account):
             if "path" in permission and permission["path"]:
                 path = permission["path"]
                 logger.info(
@@ -4838,33 +5981,36 @@
                         path
                     )
                 )
                 node = self._otcs.getNodeByVolumeAndPath(volume_type, path)
                 node_id = self._otcs.getResultValue(node, "id")
                 if not node_id:
                     logger.error("Path -> {} does not exist. Skipping...".format(path))
+                    success = False
                     continue
 
             # Check if "nickname" is in payload and not empty string:
             if "nickname" in permission and permission["nickname"]:
                 nickname = permission["nickname"]
                 logger.info(
                     "Found nickname -> {} in permission definition. Determine node ID...".format(
                         nickname
                     )
                 )
                 node = self._otcs.getNodeFromNickname(nickname)
                 node_id = self._otcs.getResultValue(node, "id")
                 if not node_id:
                     logger.error("Nickname -> {} does not exist. Skipping...")
+                    success = False
                     continue
 
             # Now we should have a value for node_id:
             if not node_id:
                 logger.error("No node ID found! Skipping permission...")
+                success = False
                 continue
             else:
                 node_name = self._otcs.getResultValue(node, "name")
                 logger.info(
                     "Found node -> {} with ID -> {} to apply permission to.".format(
                         node_name, node_id
                     )
@@ -4888,14 +6034,15 @@
                 )
                 if not response:
                     logger.error(
                         "Failed to update owner permissions for item -> {}.".format(
                             node_id
                         )
                     )
+                    success = False
 
             # 2. Process Owner Group Permissions
             if "owner_group_permissions" in permission:
                 permissions = permission["owner_group_permissions"]
                 logger.info(
                     "Update owner group permissions for item -> {} to -> {}".format(
                         node_id, permissions
@@ -4906,14 +6053,15 @@
                 )
                 if not response:
                     logger.error(
                         "Failed to update group permissions for item -> {}.".format(
                             node_id
                         )
                     )
+                    success = False
 
             # 3. Process Public Permissions
             if "public_permissions" in permission:
                 permissions = permission["public_permissions"]
                 logger.info(
                     "Update public permissions for item -> {} to -> {}".format(
                         node_id, permissions
@@ -4924,34 +6072,37 @@
                 )
                 if not response:
                     logger.error(
                         "Failed to update public permissions for item -> {}.".format(
                             node_id
                         )
                     )
+                    success = False
                     continue
 
             # 3. Process Assigned User Permissions (if specified and not empty)
             if "users" in permission and permission["users"]:
                 users = permission["users"]
                 for user in users:
                     if not "name" in user or not "permissions" in user:
                         logger.error(
                             "Missing user name or permissions in user permission specificiation. Cannot set user permissions. Skipping..."
                         )
+                        success = False
                         continue
                     user_name = user["name"]
                     permissions = user["permissions"]
                     otcs_user = self._otcs.getUser(user_name, True)
                     if not otcs_user or not otcs_user["data"]:
                         logger.error(
                             "Cannot find user with name -> {}; cannot set user permissions. Skipping user...".format(
                                 user_name
                             )
                         )
+                        success = False
                         continue
                     user_id = otcs_user["data"][0]["id"]
                     logger.info(
                         "Update user -> {} permissions for item -> {} to -> {}".format(
                             user_name, node_id, permissions
                         )
                     )
@@ -4960,14 +6111,15 @@
                     )
                     if not response:
                         logger.error(
                             "Failed to update assigned user permissions for item -> {}.".format(
                                 node_id
                             )
                         )
+                        success = False
 
             # 4. Process Assigned Group Permissions (if specified and not empty)
             if "groups" in permission and permission["groups"]:
                 groups = permission["groups"]
                 for group in groups:
                     if not "name" in group or not "permissions" in group:
                         logger.error(
@@ -4984,40 +6136,63 @@
                     otcs_group = self._otcs.getGroup(group_name, True)
                     if not otcs_group or not otcs_group["data"]:
                         logger.error(
                             "Cannot find group with name -> {}; cannot set group permissions. Skipping group...".format(
                                 group_name
                             )
                         )
+                        success = False
                         continue
                     group_id = otcs_group["data"][0]["id"]
                     response = self._otcs.assignPermission(
                         node_id, "custom", group_id, permissions, apply_to
                     )
                     if not response:
                         logger.error(
                             "Failed to update assigned group permissions for item -> {}.".format(
                                 node_id
                             )
                         )
+                        success = False
+
+        if success:
+            self.writeStatusFile(section_name, permissions)
+
+        return success
 
         # end method definition
 
-    def processAssignments(self):
+    def processAssignments(self, section_name: str = "assignments") -> bool:
         """Process assignments specified in payload and assign items (such as workspaces and
         items withnicknames) to users or groups.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._assignments:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for assignment in self._assignments:
             # Sanity check: we need a subject - it's mandatory:
             if not "subject" in assignment:
                 logger.error("Assignment needs a subject! Skipping assignment...")
+                success = False
                 continue
             subject = assignment["subject"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in assignment and not assignment["enabled"]:
                 logger.info(
@@ -5038,51 +6213,63 @@
             # Sanity check: we either need users or groups (or both):
             if not "groups" in assignment and not "users" in assignment:
                 logger.error(
                     "Assignment -> {} needs groups or users! Skipping assignment...".format(
                         subject
                     )
                 )
+                success = False
                 continue
             # Check if a workspace is specified for the assignment and check it does exist:
             if "workspace" in assignment and assignment["workspace"]:
                 workspace = next(
                     (
                         item
                         for item in self._workspaces
                         if item["id"] == assignment["workspace"]
                     ),
                     None,
                 )
-                if not workspace or not "nodeId" in workspace:
+                if not workspace:
+                    logger.error(
+                        "Assignment -> {} has specified a not existing workspace -> {}! Skipping assignment...".format(
+                            subject, assignment["workspace"]
+                        )
+                    )
+                    success = False
+                    continue
+                node_id = self.determineWorkspaceID(workspace)
+                if not node_id:
                     logger.error(
                         "Assignment -> {} has specified a not existing workspace -> {}! Skipping assignment...".format(
                             subject, assignment["workspace"]
                         )
                     )
+                    success = False
                     continue
-                node_id = workspace["nodeId"]
             # If we don't have a workspace then check if a nickname is specified for the assignment:
             elif "nickname" in assignment:
                 response = self._otcs.getNodeFromNickname(assignment["nickname"])
                 node_id = self._otcs.getResultValue(response, "id")
                 if not node_id:
                     # if response == None:
                     logger.error(
                         "Assignment item with nickname -> {} not found".format(
                             assignment["nickname"]
                         )
                     )
+                    success = False
                     continue
             else:
                 logger.error(
                     "Assignment -> {} needs a workspace or nickname! Skipping assignment...".format(
                         subject
                     )
                 )
+                success = False
                 continue
 
             assignees = []
 
             if "groups" in assignment:
                 group_assignees = assignment["groups"]
                 for group_assignee in group_assignees:
@@ -5097,21 +6284,23 @@
                     )
                     if not group:
                         logger.error(
                             "Assignment group -> {} does not exist! Skipping group...".format(
                                 group_assignee
                             )
                         )
+                        success = False
                         continue
                     if not "id" in group:
                         logger.error(
                             "Assignment group -> {} does not have an ID. Skipping group...".format(
                                 group_assignee
                             )
                         )
+                        success = False
                         continue
                     group_id = group["id"]
                     # add the group ID to the assignee list:
                     assignees.append(group_id)
 
             if "users" in assignment:
                 user_assignees = assignment["users"]
@@ -5123,76 +6312,100 @@
                     )
                     if not user:
                         logger.error(
                             "Assignment user -> {} does not exist! Skipping user...".format(
                                 user_assignee
                             )
                         )
+                        success = False
                         continue
                     if not "id" in user:
                         logger.error(
                             "Assignment user -> {} does not have an ID. Skipping user...".format(
                                 user_assignee
                             )
                         )
+                        success = False
                         continue
                     user_id = user["id"]
                     # add the group ID to the assignee list:
                     assignees.append(user_id)
 
             if assignees == []:
                 logger.error(
                     "Cannot add assignment -> {} for node ID -> {} because no assignee was found.".format(
                         subject, node_id
                     )
                 )
-                return
+                success = False
+                continue
 
             response = self._otcs.assignItemToUserGroup(
                 node_id, subject, instruction, assignees
             )
             if not response:
                 logger.error(
                     "Failed to add assignment -> {} for node ID -> {} with assignees -> {}.".format(
                         subject, node_id, assignees
                     )
                 )
+                success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._assignments)
+
+        return success
 
         # end method definition
 
     def processUserLicenses(
         self,
         resource_name: str,
         license_feature: str,
         license_name: str,
         user_specific_payload_field: str = "licenses",
-    ):
+        section_name: str = "userLicenses",
+    ) -> bool:
         """Assign a specific OTDS license feature to all Extended ECM users.
            This method is used for OTIV and Extended ECM licenses.
 
         Args:
             resource_name: name of the OTDS resource
             license_feature: license feature to assign to the user (product specific)
             license_name: Name of the license Key (e.g. "EXTENDED_ECM" or "INTELLIGENT_VIEWING")
             user_specific_payload_field: name of the user specific field in payload
                                          (if empty it will be ignored)
-        Return: None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._users:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         otds_resource = self._otds.getResource(resource_name)
         if not otds_resource:
             logger.error(
                 "OTDS Resource -> {} not found. Cannot assign licenses to users."
             )
-            return
+            return False
 
         user_partition = self._otcs.config()["partition"]
         if not user_partition:
             logger.error("OTCS user partition not found in OTDS!")
-            return
+            return False
 
         for user in self._users:
             user_name = user["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in user and not user["enabled"]:
@@ -5207,53 +6420,88 @@
                         user[user_specific_payload_field], user_name, license_feature
                     )
                 )
                 user_license_feature = user[user_specific_payload_field]
             else:  # use the default feature from the actual parameter
                 user_license_feature = [license_feature]
 
-            for lic_feature in user_license_feature:
+            for license_feature in user_license_feature:
+                if self._otds.isUserLicensed(
+                    user_name=user_name,
+                    resource_id=otds_resource["resourceID"],
+                    license_feature=license_feature,
+                    license_name=license_name,
+                ):
+                    logger.info(
+                        "User -> {} is already licensed for -> {} ({})".format(
+                            user_name, license_name, license_feature
+                        )
+                    )
+                    continue
                 assigned_license = self._otds.assignUserToLicense(
                     user_partition,
                     user_name,  # we want the plain login name here
                     otds_resource["resourceID"],
-                    lic_feature,
+                    license_feature,
                     license_name,
                 )
 
                 if not assigned_license:
                     logger.error(
                         "Failed to assign license feature -> {} to user -> {}!".format(
-                            lic_feature, user["name"]
+                            license_feature, user_name
                         )
                     )
+                    success = False
+
+        if success:
+            self.writeStatusFile(section_name, self._users)
+
+        return success
 
         # end method definition
 
-    def processExecPodCommands(self):
+    def processExecPodCommands(self, section_name: str = "execPodCommands") -> bool:
         """Process commands that should be executed in the Kubernetes pods.
 
-        Args: None
-        Return: None
+        Args:
+            None
+        Return:
+            None
         """
 
+        if not self._exec_pod_commands:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for exec_pod_command in self._exec_pod_commands:
             if not "pod_name" in exec_pod_command:
                 logger.error(
                     "To execute a command in a pod the pod name needs to be specified in the payload! Skipping to next pod command..."
                 )
+                success = False
                 continue
             pod_name = exec_pod_command["pod_name"]
 
             if not "command" in exec_pod_command or not exec_pod_command.get("command"):
                 logger.error(
                     "Pod command is not specified for pod -> {}! It needs to be a non-empty list! Skipping to next pod command...".format(
                         pod_name
                     )
                 )
+                success = False
                 continue
             command = exec_pod_command["command"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in exec_pod_command and not exec_pod_command["enabled"]:
                 logger.info(
@@ -5300,43 +6548,65 @@
                 # if a result is written to stdout or stderr.
                 logger.info(
                     "Execution of command -> {} in pod -> {} did not return a result.".format(
                         command, pod_name, result
                     )
                 )
 
+        if success:
+            self.writeStatusFile(section_name, self._exec_pod_commands)
+
+        return success
+
         # end method definition
 
-    def processDocumentGenerators(self):
+    def processDocumentGenerators(
+        self, section_name: str = "documentGenerators"
+    ) -> bool:
         """Generate documents for a defined workspace type based on template
 
         Args:
-            none
+            None
         Returns:
-            none
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._doc_generators:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         # save admin credentials for later switch back to admin user:
         admin_credentials = self._otcs.credentials()
         authenticated_user = "admin"
 
         for doc_generator in self._doc_generators:
             if not "workspace_type" in doc_generator:
                 logger.error(
                     "To generate documents for workspaces the workspace type needs to be specified in the payload! Skipping to next document generator..."
                 )
+                success = False
                 continue
             workspace_type = doc_generator["workspace_type"]
 
             if not "template_path" in doc_generator:
                 logger.error(
                     "To generate documents for workspaces of type -> {} the path to the document template needs to be specified in the payload! Skipping to next document generator...".format(
                         workspace_type
                     )
                 )
+                success = False
                 continue
             template_path = doc_generator["template_path"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in doc_generator and not doc_generator["enabled"]:
                 logger.info(
@@ -5348,32 +6618,35 @@
 
             if not "classification_path" in doc_generator:
                 logger.error(
                     "To generate documents for workspaces of type -> {} the path to the document classification needs to be specified in the payload! Skipping to next document generator...".format(
                         workspace_type
                     )
                 )
+                success = False
                 continue
             classification_path = doc_generator["classification_path"]
 
             if not "category_name" in doc_generator:
                 logger.error(
                     "To generate documents for workspaces of type -> {} the category name needs to be specified in the payload! Skipping to next document generator...".format(
                         workspace_type
                     )
                 )
+                success = False
                 continue
             category_name = doc_generator["category_name"]
 
             if not "attributes" in doc_generator:
                 logger.error(
                     "To generate documents for workspaces of type -> {} the attributes needs to be specified in the payload! Skipping to next document generator...".format(
                         workspace_type
                     )
                 )
+                success = False
                 continue
             attributes = doc_generator["attributes"]
 
             if not "workspace_folder_path" in doc_generator:
                 logger.info(
                     "No workspace folder path defined for workspaces of type -> {}. Documents will be stored in workspace root.".format(
                         workspace_type
@@ -5415,14 +6688,15 @@
                 else:
                     logger.error(
                         "Cannot find user with login name -> {} for executing. Executing as admin...".format(
                             exec_as_user
                         )
                     )
                     admin_context = True
+                    success = False
             else:
                 admin_context = True
 
             if admin_context and authenticated_user != "admin":
                 # Set back admin credentials:
                 self._otcs.setCredentials(
                     admin_credentials["username"], admin_credentials["password"]
@@ -5468,14 +6742,15 @@
 
                     if not user or not user["data"]:
                         logger.error(
                             "Cannot find user with login name -> {}. Skipping...".format(
                                 attribute_value
                             )
                         )
+                        success = False
                         continue
                     attribute_value = user["data"][0]["id"]
 
                 category_data[str(category_id)][attribute_id] = attribute_value
 
             logger.info(
                 "Generate documents for workspace type -> {} based on template -> {} with metadata -> {}...".format(
@@ -5528,14 +6803,15 @@
                 )
                 if not response:
                     logger.error(
                         "Failed to generate document -> {} in workspace -> {}".format(
                             document_name, workspace_name
                         )
                     )
+                    success = False
                 else:
                     logger.info(
                         "Successfully generated document -> {} in workspace -> {}".format(
                             document_name, workspace_name
                         )
                     )
 
@@ -5550,14 +6826,19 @@
                 "Authenticate as admin user -> {}...".format(
                     admin_credentials["username"]
                 )
             )
             # True = force new login with new user
             cookie = self._otcs.authenticate(True)
 
+        if success:
+            self.writeStatusFile(section_name, self._doc_generators)
+
+        return success
+
         # end method definition
 
     def initSAP(
         self, sap_external_system: dict, direct_application_server_login: bool = True
     ) -> object:
         """Initialize SAP object for RFC communication with SAP S/4HANA.
 
@@ -5616,22 +6897,36 @@
                 destination=destination,
             )
 
         return sap_object
 
         # end method definition
 
-    def processSAPRFCs(self, sap_object: object):
+    def processSAPRFCs(self, sap_object: object, section_name: str = "sapRFCs") -> bool:
         """Process SAP RFCs in payload and run them in SAP S/4HANA.
 
         Args:
             sap_object: SAP object
-        Return: None
+        Return:
+            bool: True if payload has been processed without errors, False otherwise
         """
 
+        if not self._doc_generators:
+            logger.info(
+                "Payload section -> {} is empty. Skipping...".format(section_name)
+            )
+            return True
+
+        # if this payload section has been processed successfully before we can return True
+        # and skip processing once more
+        if self.checkStatusFile(section_name):
+            return True
+
+        success: bool = True
+
         for sap_rfc in self._sap_rfcs:
             rfc_name = sap_rfc["name"]
 
             # Check if element has been disabled in payload (enabled = false).
             # In this case we skip the element:
             if "enabled" in sap_rfc and not sap_rfc["enabled"]:
                 logger.info(
@@ -5666,21 +6961,27 @@
             )
             if rfc_call_options:
                 logger.debug("Using call options -> {} ...".format(rfc_call_options))
 
             result = sap_object.call(rfc_name, rfc_call_options, rfc_params)
             if result == None:
                 logger.error("Failed to call SAP RFC -> {}".format(rfc_name))
+                success = False
             else:
                 logger.info(
                     "Successfully called RFC -> {}. Result -> {}".format(
                         rfc_name, result
                     )
                 )
 
+        if success:
+            self.writeStatusFile(section_name, self._sap_rfcs)
+
+        return success
+
         # end method definition
 
     def getPayload(self) -> dict:
         return self._payload
 
     def getUsers(self) -> list:
         return self._users
```

### Comparing `pyxecm-0.0.18/pyxecm/sap.py` & `pyxecm-0.0.19/pyxecm/sap.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.18/pyxecm/translate.py` & `pyxecm-0.0.19/pyxecm/translate.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.18/pyxecm/web.py` & `pyxecm-0.0.19/pyxecm/web.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.18/pyxecm.egg-info/PKG-INFO` & `pyxecm-0.0.19/pyxecm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.18
+Version: 0.0.19
 Summary: A Python library to interact with Opentext Extended ECM REST API
-Home-page: https://pypi.org/project/pyxecm/
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
-Project-URL: Homepage, https://github.com/opentext/pyxecm
-Keywords: opentext extendedecm contentserver otds appworks archivecenter
+Project-URL: Homepage, https://gitlab.otxlab.net/ecm/pyxecm
+Keywords: opentext,extendedecm,contentserver,otds,appworks,archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PYXECM
 
-A python library to interact with Opentext Extended ECM REST API.
+A python library to interact with Opentext Extended ECM REST API. 
 API documentation is available on [OpenText Developer](https://developer.opentext.com/ce/products/extendedecm)
 
 
 # Disclaimer
 
 Copyright © 2023 Open Text Corporation, All Rights Reserved.
 The above copyright notice and this permission notice shall be included in all
```

