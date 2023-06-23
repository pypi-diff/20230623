# Comparing `tmp/scipion-app-3.0.9.tar.gz` & `tmp/scipion-app-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-app-3.0.9.tar", last modified: Wed Aug 18 09:51:12 2021, max compression
+gzip compressed data, was "scipion-app-3.1.0.tar", last modified: Fri Jun 23 12:44:37 2023, max compression
```

## Comparing `scipion-app-3.0.9.tar` & `scipion-app-3.1.0.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 09:51:12.354902 scipion-app-3.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)      383 2021-08-18 09:51:04.000000 scipion-app-3.0.9/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2021-08-18 09:51:04.000000 scipion-app-3.0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-08-18 09:51:04.000000 scipion-app-3.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2021-08-18 09:51:12.354902 scipion-app-3.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2021-08-18 09:51:04.000000 scipion-app-3.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-08-18 09:51:04.000000 scipion-app-3.0.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 09:51:12.350902 scipion-app-3.0.9/scipion/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    17823 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/guiplugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 09:51:12.350902 scipion-app-3.0.9/scipion/install/
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3224 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/change_rpath.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      883 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/clean.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4144 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/find_deps.py
--rw-r--r--   0 runner    (1001) docker     (121)    30469 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6873 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/inspect-plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)    14977 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/install_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)    19797 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/plugin_funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)    50631 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/plugin_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1785 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/tar.py
--rw-r--r--   0 runner    (1001) docker     (121)     6124 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/update_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1613 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/install/upgrade_release.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 09:51:12.350902 scipion-app-3.0.9/scipion/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20856 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7415 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/scripts/fontbrowser.py
--rw-r--r--   0 runner    (1001) docker     (121)    15307 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/scripts/kickoff.py
--rw-r--r--   0 runner    (1001) docker     (121)     4127 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/scripts/tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 09:51:12.354902 scipion-app-3.0.9/scipion/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/templates/hosts.template
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/templates/protocols.template
--rw-r--r--   0 runner    (1001) docker     (121)     4292 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/templates/scipion.template
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/templates/scipionbox.template
--rw-r--r--   0 runner    (1001) docker     (121)     4197 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/templates/workflow_betagal1.json
--rw-r--r--   0 runner    (1001) docker     (121)     3016 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/templates/workflow_betagal2.json
--rw-r--r--   0 runner    (1001) docker     (121)     6076 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/templates/workflow_tutorial_intro.json
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2021-08-18 09:51:04.000000 scipion-app-3.0.9/scipion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-18 09:51:12.354902 scipion-app-3.0.9/scipion_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2021-08-18 09:51:12.000000 scipion-app-3.0.9/scipion_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2021-08-18 09:51:12.000000 scipion-app-3.0.9/scipion_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-18 09:51:12.000000 scipion-app-3.0.9/scipion_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-08-18 09:51:12.000000 scipion-app-3.0.9/scipion_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-08-18 09:51:12.000000 scipion-app-3.0.9/scipion_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-08-18 09:51:12.000000 scipion-app-3.0.9/scipion_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-18 09:51:12.354902 scipion-app-3.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2021-08-18 09:51:04.000000 scipion-app-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:44:37.642852 scipion-app-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-23 12:44:25.000000 scipion-app-3.1.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-23 12:44:25.000000 scipion-app-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 12:44:25.000000 scipion-app-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-23 12:44:37.642852 scipion-app-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-23 12:44:25.000000 scipion-app-3.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 12:44:25.000000 scipion-app-3.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:44:37.638852 scipion-app-3.1.0/scipion/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18676 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/guiplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:44:37.642852 scipion-app-3.1.0/scipion/install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/install/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3224 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/install/change_rpath.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/install/clean.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4144 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/install/find_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55639 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/install/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/install/inspect_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15708 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/install/install_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20214 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/install/plugin_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50672 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/install/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/install/update_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:44:37.642852 scipion-app-3.1.0/scipion/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18200 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/scripts/fontbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19092 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/scripts/kickoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/scripts/tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:44:37.642852 scipion-app-3.1.0/scipion/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/templates/hosts.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/templates/protocols.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/templates/scipion.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/templates/scipionbox.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/templates/workflow_betagal1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/templates/workflow_betagal2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/templates/workflow_tutorial_intro.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-23 12:44:25.000000 scipion-app-3.1.0/scipion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:44:37.642852 scipion-app-3.1.0/scipion_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-23 12:44:37.000000 scipion-app-3.1.0/scipion_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-23 12:44:37.000000 scipion-app-3.1.0/scipion_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:44:37.000000 scipion-app-3.1.0/scipion_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-23 12:44:37.000000 scipion-app-3.1.0/scipion_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 12:44:37.000000 scipion-app-3.1.0/scipion_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 12:44:37.000000 scipion-app-3.1.0/scipion_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 12:44:37.642852 scipion-app-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-23 12:44:25.000000 scipion-app-3.1.0/setup.py
```

### Comparing `scipion-app-3.0.9/LICENSE.txt` & `scipion-app-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/PKG-INFO` & `scipion-app-3.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: scipion-app
-Version: 3.0.9
+Version: 3.1.0
 Summary: Scipion application. For processing cryo electron microscopy images and hybrid modelling
 Home-page: https://github.com/scipion-em/scipion-app
 Author: Scipion team
 Author-email: scipion@cnb.csic.es
-License: UNKNOWN
-Description: ===========
-        Scipion app
-        ===========
-        
-        **Scipion** is an image processing framework to obtain 3D models of
-        macromolecular complexes using Electron Microscopy (3DEM). It integrates
-        several software packages and presents an unified interface for both biologists
-        and developers. Scipion allows to execute workflows combining different
-        software tools, while taking care of formats and conversions. Additionally,
-        all steps are tracked and can be reproduced later on.
-        
-        Want to learn more? [Go to our web site.](http://scipion.i2pc.es)
-        
-        
-        .. figure:: https://travis-ci.org/I2PC/scipion.svg?branch=devel
-           :align: left
-           :alt: Build Status
-        
-        .. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=alert_status
-           :align: left
-           :alt: Quality Gate
-        
-        .. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=sqale_index
-           :align: left
-           :alt: Technical debt
-        
-        .. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=bugs
-           :align: left
-           :alt: Bugs
-        
 Keywords: scipion cryoem imageprocessing scipion-3.0
-Platform: UNKNOWN
+License-File: LICENSE.txt
+
+===========
+Scipion app
+===========
+
+**Scipion** is an image processing framework to obtain 3D models of
+macromolecular complexes using Electron Microscopy (3DEM). It integrates
+several software packages and presents an unified interface for both biologists
+and developers. Scipion allows to execute workflows combining different
+software tools, while taking care of formats and conversions. Additionally,
+all steps are tracked and can be reproduced later on.
+
+Want to learn more? [Go to our web site.](http://scipion.i2pc.es)
+
+
+.. figure:: https://travis-ci.org/I2PC/scipion.svg?branch=devel
+   :align: left
+   :alt: Build Status
+
+.. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=alert_status
+   :align: left
+   :alt: Quality Gate
+
+.. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=sqale_index
+   :align: left
+   :alt: Technical debt
+
+.. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=bugs
+   :align: left
+   :alt: Bugs
```

### Comparing `scipion-app-3.0.9/README.rst` & `scipion-app-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/scipion/__main__.py` & `scipion-app-3.1.0/scipion/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,27 +30,28 @@
 """
 Main entry point to scipion. It launches the gui, tests, etc.
 """
 import sys
 import os
 from os.path import join, exists, expanduser, expandvars
 
-from configparser import ConfigParser  # Python 3
+from configparser import ConfigParser
 from threading import Thread
 
 from scipion.constants import *
 from scipion.utils import (getScipionHome, getInstallPath,
                            getScriptsPath, getTemplatesPath, getModuleFolder)
-from scipion.scripts.config import getConfigPathFromConfigFile, PROTOCOLS, HOSTS
+from scipion.scripts.config import getConfigPathFromConfigFile, HOSTS
 from scipion.constants import MODE_UPDATE
 from scipion import __version__
 
 __nickname__ = "Eugenius"
 
 # *********************  Helper functions *****************************
+
 def getVersion(long=True):
     if long:
         return "v%s - %s" % (__version__, __nickname__)
     else:
         return __version__
 
 
@@ -72,15 +73,17 @@
         config.read(configFile)
 
         # For each section
         for sectionName, section in config.items():
             for variable, value in section.items():
                 # Expanding user and avoiding comments
                 cleanValue = value.split('#')[0]
-                varDict[variable] = expandvars(cleanValue).strip()
+
+                # Give priority to environment variables
+                varDict[variable] = os.environ.get(variable, default=expandvars(cleanValue).strip())
 
     return varDict
 
 
 def envOn(varName):
     value = os.environ.get(varName, '').lower()
     return value in ['1', 'true', 'on', 'yes']
@@ -152,18 +155,14 @@
             # Here we can react differently,instead of exiting, may be continuing warning about
             # the missing config file?
             sys.exit('Config file missing: %s' % scipionConfig)
 
     else:
         sys.exit('Unknown argument: %s' % arg)
 
-# Protocols.conf and hosts.conf, fallback to the template.
-protocols = getConfigPathFromConfigFile(scipionConfig, PROTOCOLS)
-if not exists(protocols):
-    protocols = join(getTemplatesPath(), "protocols.template")
 
 hosts = getConfigPathFromConfigFile(scipionConfig, HOSTS)
 if not exists(hosts):
     hosts = join(getTemplatesPath(), "hosts.template")
 
 
 # *********************** STORE VARIABLES ********************
@@ -178,25 +177,27 @@
     SCIPION_SCRIPTS = getScriptsPath()
     # Scipion path to install
     SCIPION_INSTALL = getInstallPath()
 
     # Config files
     SCIPION_CONFIG = scipionConfig
     SCIPION_LOCAL_CONFIG = scipionLocalConfig
-    SCIPION_PROTOCOLS = protocols
     SCIPION_HOSTS = os.environ.get('SCIPION_HOSTS', hosts)
 
     # Paths to apps or scripts
     PW_APPS = join(getModuleFolder("pyworkflow"), 'apps')
     SCIPION_TEMPLATES = getTemplatesPath()
 
     SCIPION_VERSION = getVersion()
     SCIPION_PYTHON = PYTHON
     SCIPION_TESTS_CMD = os.environ.get("SCIPION_TESTS_CMD", '%s %s' % (SCIPION_EP, MODE_TESTS))
 
+    # Priority package list
+    SCIPION_PRIORITY_PACKAGE_LIST = "pwem tomo pwchem"
+
 
 # *********************** READ CONFIG FILES ***********************
 try:
     VARS = dict()
 
     # Load variables from Vars class into VARS dict
 
@@ -206,17 +207,17 @@
         # PYTHONPATH_LIST.insert(0, join(pyworkflow.Config.getPyworkflowPath(), 'gui', 'no-tkinter'))
         print("SCIPION_NOGUI variable not implemented for this version. Please contact us if you need this.")
 
     # Load VARS dictionary, all items here will go to the environment
     VARS['SCIPION_DOMAIN'] = Vars.SCIPION_DOMAIN
     VARS['SCIPION_CONFIG'] = Vars.SCIPION_CONFIG
     VARS['SCIPION_LOCAL_CONFIG'] = Vars.SCIPION_LOCAL_CONFIG
-    VARS['SCIPION_PROTOCOLS'] = Vars.SCIPION_PROTOCOLS
     VARS['SCIPION_HOSTS'] = Vars.SCIPION_HOSTS
     VARS['SCIPION_VERSION'] = Vars.SCIPION_VERSION
+    VARS['SCIPION_PRIORITY_PACKAGE_LIST'] = Vars.SCIPION_PRIORITY_PACKAGE_LIST
 
     # Read main config file
     config2Dict(Vars.SCIPION_CONFIG, VARS)
 
     # Load the local config
     if Vars.SCIPION_LOCAL_CONFIG != Vars.SCIPION_CONFIG:
         config2Dict(Vars.SCIPION_LOCAL_CONFIG, VARS)
@@ -237,15 +238,25 @@
     mode = getMode()
 
     # Prepare the environment
     os.environ.update(VARS)
 
     # Set default VIEWERS value for scipion if not defined:
     if not os.environ.get("VIEWERS", None):
-        os.environ["VIEWERS"] = '{"Volume":["pwem.viewers.DataViewer"], "VolumeMask":["pwem.viewers.DataViewer"]}'
+        defaultViewers = []
+        defaultViewers.append('"Volume":["pwem.viewers.DataViewer"]')
+        defaultViewers.append('"VolumeMask":["pwem.viewers.DataViewer"]')
+        defaultViewers.append('"SetOfTiltSeries":["imod.viewers.ImodViewer"]')
+        defaultViewers.append('"SetOfLandmarkModels":["imod.viewers.ImodViewer"]')
+        defaultViewers.append('"SetOfTomograms":["imod.viewers.ImodViewer"]')
+        defaultViewers.append('"SetOfSubTomograms":["pwem.viewers.DataViewer"]')
+        defaultViewers.append('"SetOfVolumes":["pwem.viewers.DataViewer"]')
+        defaultViewers.append('"SetOfParticles":["pwem.viewers.DataViewer"]')
+
+        os.environ["VIEWERS"] = '{%s}' % ','.join(defaultViewers)
 
     # Trigger Config initialization once environment is ready
     import pyworkflow
     pwVARS = pyworkflow.Config.getVars()
     VARS.update(pwVARS)
 
     # Update the environment now with pyworkflow values.
@@ -258,15 +269,15 @@
 
         # Check update status in a thread.
         thread = Thread(target=lambda: UpdateManager.getPackagesStatus(printAll=False))
         thread.start()
 
         ProjectManagerWindow().show()
 
-    elif mode in [ MODE_LAST, MODE_HERE, MODE_PROJECT]:
+    elif mode in [MODE_LAST, MODE_HERE, MODE_PROJECT]:
         os.environ.update(VARS)
         from pyworkflow.utils.log import LoggingConfigurator
         LoggingConfigurator.setUpGUILogging()
         from pyworkflow.apps.pw_project import openProject
         arg = sys.argv[2] if mode == MODE_PROJECT else mode
         openProject(arg)
 
@@ -334,14 +345,18 @@
 
         sys.exit(0)
 
     elif mode == MODE_RUN:
         # Run any command with the environment of scipion loaded.
         runCmd('emprogram ' + ' '.join(['"%s"' % arg for arg in sys.argv[2:]]))
 
+    elif mode == MODE_PIP:
+        # Runs pip command inside scipion's environment.
+        runCmd('pip ' + ' '.join(['"%s"' % arg for arg in sys.argv[2:]]))
+
     elif mode == MODE_PYTHON:
         runScript(' '.join(['"%s"' % arg for arg in sys.argv[2:]]),
                   chdir=False)
 
     elif mode == MODE_TUTORIAL:
         runApp(join(Vars.SCIPION_SCRIPTS, 'tutorial.py'), sys.argv[2:])
 
@@ -359,37 +374,37 @@
           mode.startswith('sx') or
           mode.startswith('b')):
         # To avoid Ghost activation warning
         from pwem import EM_PROGRAM_ENTRY_POINT
         runCmd(EM_PROGRAM_ENTRY_POINT, sys.argv[1:])
 
     elif mode == MODE_INSPECT:
-        runScript(join(Vars.SCIPION_INSTALL, 'inspect-plugins.py'), sys.argv[2:])
+        runScript(join(Vars.SCIPION_INSTALL, 'inspect_plugins.py'), sys.argv[2:])
 
     elif mode == MODE_UPDATE:
-        # Once more: local import to avoid importing pyworkflow, trigerred by install.__init__ (Plugin Manager)
+        # Once more: local import to avoid importing pyworkflow, triggered by install.__init__ (Plugin Manager)
         from scipion.install.update_manager import updateManagerParser
         updateManagerParser(sys.argv[:])
     # Else HELP or wrong argument
     else:
         sys.stdout.write("""\
 Usage: scipion [--config PATH] [MODE] [ARGUMENTS]
 
-    --config               Path to a full config file
+    --config               Full path to a config file.
                     
 MODE can be:
     %s                   Prints this help message.
 
     %s                 Checks and/or writes Scipion's global and local configuration.
     
     %s                Launches the plugin manager window.
     
-    %s               Installs Scipion plugins from a terminal. Use flag --help to see usage.
+    %s, %s      Installs Scipion plugins from a terminal. Use flag --help to see usage.
     
-    %s             Uninstalls Scipion plugins from a terminal. Use with flag --help to see usage.
+    %s, %s  Uninstalls Scipion plugins from a terminal. Use with flag --help to see usage.
     
     %s               Installs Plugin Binaries. Use with flag --help to see usage.
     
     %s             Uninstalls Plugin Binaries. Use with flag --help to see usage.
 
     %s                Opens the manager with a list of all projects.
 
@@ -399,19 +414,21 @@
     
     %s              Displays a list of the available Scipion protocols.
         
     %s [ARGS ...] Run the specified Scipion protocol.
 
     %s NAME           Opens the specified project. The name 'last' opens the last project.
     
-    %s                   Same as 'project last'
+    %s                   Same as 'project last'.
 
     %s COMMAND [ARG ...]  Runs COMMAND within the Scipion environment.
     
-    %s [ARG ...]       Shortcut for 'scipion run python ...'
+    %s [PIP ARGS ...]     Runs pip within the Scipion environment.
+    
+    %s [ARG ...]       Shortcut for 'scipion run python ...'.
 
     %s OPTION            Runs/Lists test(s).
                            OPTION can be:
                              <name>: name of the test to run
                              --show: list the available tests
                              --help: show all the available options
                              --grep <pattern> : filter the list using the <pattern> 
@@ -427,17 +444,17 @@
                              --list: list the datasets in the local computer and in the server
                              --help: show all the available options
                            For example, to download the dataset xmipp_tutorial:
                              scipion testdata --download xmipp_tutorial
                            Or to upload it:
                              scipion testdata --upload xmipp_tutorial
                              
-    %s                Prints main packages version
+    %s                Prints main packages version.
     
-    %s | %s         Displays a GUI which allows to run the available Scipion workflow demos 
+    %s | %s        Displays a GUI which allows to run the available Scipion workflow demos. 
     
     %s [NAME]        Creates a new protocol with a tutorial workflow loaded.
                            If NAME is empty, the list of available tutorials are shown.
 
     %s | %s FILE       Opens a file with Scipion's showj, or a directory with Browser.
     
     %s [TEMPLATE]    Shows all the *.json.template files found in the config folder
@@ -447,29 +464,31 @@
 
     %s [ARGS]          Check for updates of scipion-em, scipion-pyworkflow 
                            and scipion-app and updates them. OPTIONS can be:
                               -h or --help: to see usage.
                               -dry : only check the status of scipion-em, scipion-pyworkflow 
                                      and scipion-app
 
-""" % (MODE_HELP, MODE_CONFIG, MODE_PLUGINS, MODE_INSTALL_PLUGIN, MODE_UNINSTALL_PLUGIN,
+""" % (MODE_HELP, MODE_CONFIG,
+       MODE_PLUGINS,
+       MODE_INSTALL_PLUGIN[1], MODE_INSTALL_PLUGIN[0],
+       MODE_UNINSTALL_PLUGIN[1], MODE_UNINSTALL_PLUGIN[0],
        MODE_INSTALL_BINS, MODE_UNINSTALL_BINS, MODE_MANAGER, MODE_INSPECT,
        MODE_ENV, MODE_PROTOCOLS, MODE_RUNPROTOCOL, MODE_PROJECT, MODE_LAST,
-       MODE_RUN, MODE_PYTHON, MODE_TEST, MODE_TEST_DATA, MODE_VERSION,
-       *MODE_DEMO, MODE_TUTORIAL, MODE_VIEWER[1], MODE_VIEWER[2],
+       MODE_RUN, MODE_PIP, MODE_PYTHON, MODE_TEST, MODE_TEST_DATA, MODE_VERSION,
+       MODE_DEMO[0], MODE_DEMO[1], MODE_TUTORIAL, MODE_VIEWER[1], MODE_VIEWER[2],
        MODE_DEMO[1], MODE_UPDATE))
 
         if mode == MODE_HELP:
             sys.exit(0)
         else:
             print("Unknown mode: %s." % mode)
             sys.exit(1)
 
 
 if __name__ == '__main__':
     try:
         main()
     except Exception as e:
         import traceback
-
         traceback.print_exc()
         sys.exit('Error at main: %s\n' % e)
```

### Comparing `scipion-app-3.0.9/scipion/constants.py` & `scipion-app-3.1.0/scipion/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,31 +10,34 @@
 MODE_TEST = 'test'  # also allow 'test', in singular
 MODE_TEST_DATA = 'testdata'
 MODE_HELP = 'help'
 MODE_VIEWER = ['viewer', 'view', 'show']
 
 # Installation modes
 MODE_PLUGINS = 'plugins'
-MODE_INSTALL_PLUGIN = 'installp'
-MODE_UNINSTALL_PLUGIN = 'uninstallp'
+MODE_INSTALL_PLUGIN = ['installp', "install"]
+MODE_UNINSTALL_PLUGIN = ['uninstallp', 'uninstall']
 MODE_INSTALL_BINS = 'installb'
 MODE_UNINSTALL_BINS = 'uninstallb'
 MODE_CONFIG = 'config'
 MODE_VERSION = 'version'
 MODE_RUNPROTOCOL = 'runprotocol'
 MODE_PROTOCOLS = 'protocols'
 MODE_ENV = 'printenv'
 MODE_RUN = 'run'
 MODE_PYTHON = 'python'
 MODE_TUTORIAL = 'tutorial'
 MODE_DEMO = ['demo', 'template']
 MODE_INSPECT = "inspect"
 MODE_UPDATE = 'update'
-PLUGIN_MODES = [MODE_UNINSTALL_PLUGIN, MODE_INSTALL_PLUGIN,
-                MODE_INSTALL_BINS, MODE_UNINSTALL_BINS]
+MODE_PIP = 'pip'
+PLUGIN_MODES = [MODE_UNINSTALL_PLUGIN[0], MODE_UNINSTALL_PLUGIN[1],
+                MODE_INSTALL_PLUGIN[1], MODE_INSTALL_PLUGIN[0],
+                MODE_INSTALL_BINS,
+                MODE_UNINSTALL_BINS]
 
 # Entry points
 SCIPION_EP = "scipion"
 
 # python file name: at install or scripts
 PLUGIN_MANAGER_PY = 'plugin_manager.py'
 PYTHON = 'python'
```

### Comparing `scipion-app-3.0.9/scipion/install/__init__.py` & `scipion-app-3.1.0/scipion/install/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-from .funcs import Environment
+from .funcs import Environment
```

### Comparing `scipion-app-3.0.9/scipion/install/change_rpath.py` & `scipion-app-3.1.0/scipion/install/change_rpath.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/scipion/install/clean.py` & `scipion-app-3.1.0/scipion/install/clean.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/scipion/install/find_deps.py` & `scipion-app-3.1.0/scipion/install/find_deps.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/scipion/install/inspect-plugins.py` & `scipion-app-3.1.0/scipion/install/inspect_plugins.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,35 +28,35 @@
 
 import sys
 from os.path import join, exists, dirname
 import importlib
 import inspect
 import traceback
 from collections import OrderedDict
-from future.utils import iteritems
 
 from pwem.protocols import (Prot3D, Prot2D, ProtParticles,
                             ProtMicrographs, ProtImport)
 from pwem import Domain
 from pyworkflow.protocol import Protocol
 import pyworkflow.utils as pwutils
 
 from scipion.install.plugin_funcs import PluginInfo
 
+ERROR_PREFIX = " error -> %s"
 
 exitWithErrors = False
 
 
 def usage(error=""):
 
     if error:
         error = "ERROR: %s\n" % error
 
     print("""%s
-    Usage: scipion python scripts/inspect-plugins.py [PLUGIN-NAME] [info] [--showBase]
+    Usage: scipion python scripts/inspect_plugins.py [PLUGIN-NAME] [info] [--showBase]
         This script loads all Scipion plugins found.
         If a PLUGIN-NAME is passed, it will inspect that plugin
         in more detail.
         'info' argument will print plugin summary,
         '-showBase' will print Base class protocols (hidden by default).
     """ % error)
     sys.exit(1)
@@ -79,15 +79,15 @@
         moduleExists = (exists(join(dirname(plugin.__file__), "%s.py" % subName)) or
                         exists(join(dirname(plugin.__file__), subName)))
         r = (None, None if msg == noModuleMsg and not moduleExists else traceback.format_exc())
     return r
 
 
 def getFirstLine(doc):
-    """ Get the first non empty line from doc. """
+    """ Get the first non-empty line from doc. """
     if doc:
         for lines in doc.split('\n'):
             l = lines.strip()
             if l:
                 return l
     return ''
 
@@ -96,15 +96,15 @@
 
 if n > 4:
     usage("Incorrect number of input parameters")
 
 if n == 1:  # List all plugins
     plugins = Domain.getPlugins()
     print("Plugins:")
-    for k, v in iteritems(plugins):
+    for k, v in plugins.items():
         print("-", k)
 
     print("Objects")
     pwutils.prettyDict(Domain.getObjects())
 
     print("Protocols")
     pwutils.prettyDict(Domain.getProtocols())
@@ -125,15 +125,15 @@
         sub, error = getSubmodule(plugin, pluginName, subName)
 
         if sub is None:
             if error is None:
                 msg = " missing"
             else:
                 exitWithErrors = True
-                msg = " error -> %s" % error
+                msg = ERROR_PREFIX % error
 
         else:
             msg = " loaded"
 
         print("   >>> %s: %s" % (subName, msg))
 
 elif n > 2:
@@ -149,38 +149,36 @@
 
         plugin = Domain.getPlugin(pluginName)
         version = PluginInfo('scipion-em-%s' % pluginName).pipVersion
         bin = PluginInfo('scipion-em-%s' % pluginName).printBinInfoStr()
         print("Plugin name: %s, version: %s" % (pluginName, version))
         print("Plugin binaries: %s" % bin)
 
-        # print bibtex
         bib, error2 = getSubmodule(plugin, pluginName, 'bibtex')
         if bib is None:
             if error2 is None:
                 msg = " missing bibtex"
             else:
                 exitWithErrors = True
-                msg = " error -> %s" % error2
+                msg = ERROR_PREFIX % error2
         else:
             print("Plugin references:")
             bibtex = pwutils.parseBibTex(bib.__doc__)
 
             for citeStr in bibtex:
                 text = Protocol()._getCiteText(bibtex[citeStr])
                 print(text)
 
-        # print protocols
         sub, error = getSubmodule(plugin, pluginName, 'protocols')
         if sub is None:
             if error is None:
                 msg = " missing protocols"
             else:
                 exitWithErrors = True
-                msg = " error -> %s" % error
+                msg = ERROR_PREFIX % error
 
         else:
             for name in dir(sub):
                 attr = getattr(sub, name)
                 if inspect.isclass(attr) and issubclass(attr, Protocol):
                     # Set this special property used by Scipion
                     attr._package = plugin
```

### Comparing `scipion-app-3.0.9/scipion/install/install_plugin.py` & `scipion-app-3.1.0/scipion/install/install_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,29 +24,27 @@
 # *
 # **************************************************************************
 
 import sys
 import argparse
 import os
 import re
-from future.utils import iteritems
 
+from scipion.constants import MODE_INSTALL_PLUGIN, MODE_UNINSTALL_PLUGIN
 from scipion.install import Environment
-from scipion.install.plugin_funcs import PluginRepository, PluginInfo
+from scipion.install.plugin_funcs import PluginRepository, PluginInfo, installBinsDefault
 from pyworkflow.utils import redStr
 
 #  ************************************************************************
 #  *                                                                      *
 #  *                       External (EM) Plugins                          *
 #  *                                                                      *
 #  ************************************************************************
 from pyworkflow import Config
 
-MODE_INSTALL_PLUGIN = 'installp'
-MODE_UNINSTALL_PLUGIN = 'uninstallp'
 MODE_LIST_BINS = 'listb'
 MODE_INSTALL_BINS = 'installb'
 MODE_UNINSTALL_BINS = 'uninstallb'
 
 # For now let's use scipion hard coded as example for the help
 SCIPION_CMD = "scipion"
 
@@ -57,24 +55,25 @@
     # Trigger plugin's variable definition
     Config.getDomain().getPlugins()
 
     invokeCmd = SCIPION_CMD + " " + sys.argv[1]
     pluginRepo = PluginRepository()
 
     parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter)
-    subparsers = parser.add_subparsers(help='mode "installp", "uninstallp" or "listb"',
+    subparsers = parser.add_subparsers(help='mode "%s", "%s" or "listb"' % (MODE_INSTALL_PLUGIN[1], MODE_UNINSTALL_PLUGIN[1]),
                                        dest='mode',
                                        title='Mode',
-                                       description='available modes are "installp" or "uninstallp"')
+                                       description='available modes are "%s" or "%s"' % (MODE_INSTALL_PLUGIN[1], MODE_UNINSTALL_PLUGIN[1]))
 
     ############################################################################
     #                               Install parser                             #
     ############################################################################
 
-    installParser = subparsers.add_parser("installp", formatter_class=argparse.RawTextHelpFormatter,
+
+    installParser = subparsers.add_parser(MODE_INSTALL_PLUGIN[1], aliases=[MODE_INSTALL_PLUGIN[0]], formatter_class=argparse.RawTextHelpFormatter,
                                           usage="%s  [-h] [--noBin] [-p pluginName [pipVersion ...]]" %
                                                 invokeCmd,
                                           epilog="Example: %s -p scipion-em-motioncorr 1.0.6 "
                                                  "-p scipion-em-relion -p scipion-em-eman2 \n\n" %
                                                  invokeCmd,
                                           add_help=False)
     installParser.add_argument('-h', '--help', action='store_true', help='show help')
@@ -93,26 +92,26 @@
 
     installParser.add_argument('--devel', action='store_true',
                                help='Optional flag to indicate that we will pass install sources instead\n'
                                     'of pip names. Sources might be local paths or git urls. With local\n'
                                     'paths, will do pip install -e (editable mode). It is expected to find\n'
                                     'the plugin name in the basename of the path or in the repo name. \n'
                                     '(i.e. it needs to match the one specified in setup.py). E.g:\n'
-                                    'scipion installp -p path/to/pluginName --devel \n'
-                                    'scipion installp -p https://github.com/someOrg/pluginName.git --devel')
+                                    'scipion install -p path/to/pluginName --devel \n'
+                                    'scipion install -p https://github.com/someOrg/pluginName.git --devel')
     installParser.add_argument('-j',
                                default='1',
                                metavar='j',
                                help='Number of CPUs to use for compilation \n')
 
     ############################################################################
     #                             Uninstall parser                             #
     ############################################################################
 
-    uninstallParser = subparsers.add_parser("uninstallp", formatter_class=argparse.RawTextHelpFormatter,
+    uninstallParser = subparsers.add_parser(MODE_UNINSTALL_PLUGIN[1], aliases=[MODE_UNINSTALL_PLUGIN[0]], formatter_class=argparse.RawTextHelpFormatter,
                                             usage="%s  [-h] [-p pluginName [binVersion ...]]" % invokeCmd,
                                             epilog="Example: %s -p scipion-em-eman2 scipion-em-motioncorr \n\n" %
                                                    invokeCmd,
                                             add_help=False)
     uninstallParser.add_argument('-h', '--help', action='store_true', help='show help')
     uninstallParser.add_argument('--noBin', action='store_true',
                                  help='Optional flag to uninstall plugins only as a python module,\n'
@@ -159,42 +158,45 @@
                                     metavar='binName(s)',
                                     help='The name(s) of the bins we want to uninstall\n'
                                          '(optionally with version in the form name-version). \n'
                                          'If no version is specified, will uninstall the last one.\n')
 
     modeToParser = {MODE_INSTALL_BINS: installBinParser,
                     MODE_UNINSTALL_BINS: uninstallBinParser,
-                    MODE_INSTALL_PLUGIN: installParser,
-                    MODE_UNINSTALL_PLUGIN: uninstallParser}
+                    MODE_INSTALL_PLUGIN[0]: installParser,
+                    MODE_INSTALL_PLUGIN[1]: installParser,
+                    MODE_UNINSTALL_PLUGIN[0]: uninstallParser,
+                    MODE_UNINSTALL_PLUGIN[1]: uninstallParser}
 
     parsedArgs = parser.parse_args(sys.argv[1:])
     mode = parsedArgs.mode
     parserUsed = modeToParser[mode]
     exitWithErrors = False
 
+
     if parsedArgs.help or (mode in [MODE_INSTALL_BINS, MODE_UNINSTALL_BINS]
                            and len(parsedArgs.binName) == 0):
 
         if mode not in [MODE_INSTALL_BINS, MODE_UNINSTALL_BINS]:
             parserUsed.epilog += pluginRepo.printPluginInfoStr()
         else:
             env = Environment()
             env.setDefault(False)
             installedPlugins = Config.getDomain().getPlugins()
-            for p, pobj in iteritems(installedPlugins):
+            for p, pobj in installedPlugins.items():
                 try:
                     pobj.Plugin.defineBinaries(env)
                 except Exception as e:
                     print(
                         redStr("Error retrieving plugin %s binaries: " % str(p)), e)
             parserUsed.epilog += env.printHelp()
         parserUsed.print_help()
         parserUsed.exit(0)
 
-    elif mode == MODE_INSTALL_PLUGIN:
+    elif mode in MODE_INSTALL_PLUGIN:
         if parsedArgs.checkUpdates:
             print(pluginRepo.printPluginInfoStr(withUpdates=True))
             installParser.exit(0)
 
         if parsedArgs.devel:
             for p in parsedArgs.plugin:
                 pluginSrc = p[0]
@@ -208,15 +210,16 @@
                 if not pluginName:
                     print("ERROR: Couldn't find pluginName for source %s" % pluginSrc)
                     exitWithErrors = True
                 else:
                     plugin = PluginInfo(pipName=pluginName, pluginSourceUrl=pluginSrc, remote=False)
                     numberProcessor = parsedArgs.j
                     installed = plugin.installPipModule()
-                    if installed and not parsedArgs.noBin:
+                    if installed and installBinsDefault() and not parsedArgs.noBin:
+                        plugin.getPluginClass()._defineVariables()
                         plugin.installBin({'args': ['-j', numberProcessor]})
         else:
             pluginsToInstall = list(zip(*parsedArgs.plugin))[0]
             pluginDict = pluginRepo.getPlugins(pluginList=pluginsToInstall,
                                                getPipData=True)
             if not pluginDict:
                 exitWithErrors = True
@@ -224,30 +227,35 @@
                 for cmdTarget in parsedArgs.plugin:
                     pluginName = cmdTarget[0]
                     pluginVersion = "" if len(cmdTarget) == 1 else cmdTarget[1]
                     numberProcessor = parsedArgs.j
                     plugin = pluginDict.get(pluginName, None)
                     if plugin:
                         installed = plugin.installPipModule(version=pluginVersion)
-                        if installed and not parsedArgs.noBin:
+                        if installed and installBinsDefault() and not parsedArgs.noBin:
+                            plugin.getPluginClass()._defineVariables()
                             plugin.installBin({'args': ['-j', numberProcessor]})
                     else:
                         print("WARNING: Plugin %s does not exist." % pluginName)
                         exitWithErrors = True
 
-    elif parsedArgs.mode == MODE_UNINSTALL_PLUGIN:
+    elif parsedArgs.mode in MODE_UNINSTALL_PLUGIN:
 
-        for pluginName in parsedArgs.plugin:
-            plugin = PluginInfo(pluginName, pluginName, remote=False)
-            if plugin.isInstalled():
-                if not parsedArgs.noBin:
-                    plugin.uninstallBins()
-                plugin.uninstallPip()
-            else:
-                print("WARNING: Plugin %s is not installed." % pluginName)
+        if parsedArgs.plugin:
+            for pluginName in parsedArgs.plugin:
+                plugin = PluginInfo(pluginName, pluginName, remote=False)
+                if plugin.isInstalled():
+                    if installBinsDefault() and not parsedArgs.noBin:
+                        plugin.uninstallBins()
+                    plugin.uninstallPip()
+                else:
+                    print("WARNING: Plugin %s is not installed." % pluginName)
+        else:
+            print("Incorrect usage of command 'uninstallp'. Execute 'scipion3 uninstallp --help' or "
+                  "'scipion3 help' for more details.")
 
     elif parsedArgs.mode == MODE_INSTALL_BINS:
         binToInstallList = parsedArgs.binName
         binToPlugin = pluginRepo.getBinToPluginDict()
         for binTarget in binToInstallList:
             pluginTargetName = binToPlugin.get(binTarget, None)
             if pluginTargetName is None:
```

### Comparing `scipion-app-3.0.9/scipion/install/plugin_funcs.py` & `scipion-app-3.1.0/scipion/install/plugin_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import re
 import sys
 import json
 import pkg_resources
 from pkg_resources import parse_version
 
-from .funcs import Environment, VOID_TGZ
+from .funcs import Environment
 from pwem import Domain
 from pyworkflow.utils import redStr, yellowStr
 from pyworkflow.utils.path import cleanPath
 from pyworkflow import LAST_VERSION, CORE_VERSION, OLD_VERSIONS, Config
 from importlib import reload
 
 NULL_VERSION = "0.0.0"
@@ -95,15 +95,15 @@
 
     def hasPipPackage(self):
         """Checks if the current plugin is installed via pip"""
         return self._getDistribution() is not None
 
     def isInstalled(self):
         """Checks if the current plugin is installed (i.e. has pip package).
-        NOTE: we might wanna change definition of isInstalled, hence the extra function."""
+        NOTE: we might want to change definition of isInstalled, hence the extra function."""
         reload(pkg_resources)
         return self.hasPipPackage()
 
     def installPipModule(self, version=""):
         """Installs the version specified of the pip plugin, as long as it is compatible
         with the current Scipion version. If no version specified, will install latest
         compatible one."""
@@ -128,15 +128,15 @@
 
         if self.pluginSourceUrl:
             if os.path.exists(self.pluginSourceUrl):
                 # install from dir in editable mode
                 installSrc = '-e %s' % self.pluginSourceUrl
                 target = "%s*" % self.pipName
             else:
-                # path doesnt exist, we assume is git and force install
+                # path doesn't exist, we assume is git and force install
                 installSrc = '--upgrade git+%s' % self.pluginSourceUrl
                 target = "%s*" % self.pipName.replace('-', '_')
         else:
             # install from pypi
             installSrc = "%s==%s" % (self.pipName, version)
             target = "%s*" % self.pipName.replace('-', '_')
 
@@ -163,26 +163,31 @@
         """Install binaries of the plugin. Args is the list of args to be
            passed to the install environment."""
         environment = self.getInstallenv(envArgs=args)
         environment.execute()
 
     def uninstallBins(self, binList=None):
         """Uninstall binaries of the plugin.
-        - binList: if  given, will uninstall the binaries in it. The binList
-                   may contain strings with only the name of the binary or
-                   name and version in the format name-version"""
+
+        :param binList: if  given, will uninstall the binaries in it. The binList
+        may contain strings with only the name of the binary or
+        name and version in the format name-version
+
+        :returns None
+
+        """
         if binList is None:
             binList = self.binVersions
 
         binFolder = Environment.getEmFolder()
         for binVersion in binList:
             f = os.path.join(binFolder, binVersion)
             if os.path.exists(f):
                 print('Removing %s binaries...' % binVersion)
-                realPath = os.path.realpath(f)  # in case its a link
+                realPath = os.path.realpath(f)  # in case it's a link
                 cleanPath(f, realPath)
                 print('Binary %s has been uninstalled successfully ' % binVersion)
             else:
                 print('The binary %s does not exist ' % binVersion)
         return
 
     def uninstallPip(self):
@@ -325,14 +330,16 @@
 
         plugin = self.getPluginClass()
         if plugin is not None:
             try:
                 plugin.defineBinaries(env)
             except Exception as e:
                 print("Couldn't get binaries definition of %s plugin: %s" % (self.name, e))
+                import traceback
+                traceback.print_exc()
             return env
         else:
             return None
 
     def getBinVersions(self):
         """Get list with names of binaries of this plugin"""
         env = Environment()
@@ -477,17 +484,19 @@
             if pluginInfo.getLatestRelease() != NULL_VERSION:
                 self.plugins[pluginName] = pluginInfo
 
         return self.plugins
 
     def printPluginInfoStr(self, withBins=False, withUpdates=False):
         """Returns string to print in console which plugins are installed.
-        - withBins: If true, will add binary info for the plugins installed
-        - with Updates: If true, will check if the installed plugins have new
-                    releases."""
+
+        :param withBins: If true, will add binary info for the plugins installed
+        :param withUpdates: If true, will check if the installed plugins have new releases.
+
+        :return A string with the plugin information summarized"""
 
         def ansi(n):
             """Return function that escapes text with ANSI color n."""
             return lambda txt: '\x1b[%dm%s\x1b[0m' % (n, txt)
 
         black, red, green, yellow, blue, magenta, cyan, white = map(ansi,
                                                                     range(30, 38))
@@ -512,7 +521,14 @@
                         printStr += yellow('\t(%s available)' % plugin.latestRelease)
                 printStr += "\n"
                 if withBins:
                     printStr += green(plugin.printBinInfoStr())
         else:
             printStr = "List of available plugins in plugin repository inaccessible at this time."
         return printStr
+
+
+def installBinsDefault():
+    """ Returns the default behaviour for installing binaries
+    By default it is TRUE, define "SCIPION_DONT_INSTALL_BINARIES" to anything to deactivate binaries installation"""
+
+    return os.environ.get("SCIPION_DONT_INSTALL_BINARIES", True) == True
```

### Comparing `scipion-app-3.0.9/scipion/install/plugin_manager.py` & `scipion-app-3.1.0/scipion/install/plugin_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-import logging
 from logging.handlers import RotatingFileHandler
 from tkinter import *
 import threading
 
+from pyworkflow import Config
 from pyworkflow.gui.project import ProjectManagerWindow
 from pyworkflow.project import MenuConfig
 from pyworkflow.gui import *
 import pyworkflow.gui.dialog as pwgui
 from scipion.install.plugin_funcs import PluginRepository, PluginInfo, NULL_VERSION
 
 from pyworkflow.utils.properties import *
@@ -216,15 +216,15 @@
         """
         Set the object status
         """
         self.objStatus = status
 
     def getObjParent(self):
         """
-        Get the object parent in the tree. If the object is a bynary, this
+        Get the object parent in the tree. If the object is a binary, this
         method return None
         """
         return self.objParent
 
     def runOperation(self, processors, handleBins=True):
         """
         This method install or uninstall a plugin/binary operation
@@ -252,15 +252,15 @@
                 plugin.installBin({'args': [self.objText, '-j', processors]})
             else:
                 plugin.uninstallBins([self.objText])
 
 
 class OperationList:
     """
-    This class contain a plugins/binaries operations list and allow execute it
+    This class contains a plugins/binaries operations list and allows to execute it
     """
     def __init__(self):
         self.operationList = []
 
     def insertOperation(self, operation):
         """
         This method insert into the list a given operation. If the operation was
@@ -395,15 +395,15 @@
 
         # Bottom Panel
         # This section show the plugin operation and a console
         bottomPanel = ttk.Frame(rightPanel)
         tabControl = ttk.Notebook(bottomPanel)  # Create Tab Control
         tabControl.grid(row=1, column=0, sticky='news')
 
-        operationTab = ttk.Frame(tabControl)  # Create a operation tab
+        operationTab = ttk.Frame(tabControl)  # Create an operation tab
         operationTab.grid(row=0, column=0, padx=0, pady=0)
         self._fillRightBottomOperationsPanel(operationTab)
         consoleTab = ttk.Frame(tabControl)  # Create a console
         self._fillRightBottomOutputLogPanel(consoleTab)
 
         tabControl.add(operationTab, text='Operations')  # Add the Operation tab
         tabControl.add(consoleTab, text='Output Log')
@@ -447,15 +447,14 @@
         self._col += 1
         self.numberProcessors = tk.StringVar()
         self.numberProcessors.set('4')
         processorsEntry = tk.Entry(frame, textvariable=self.numberProcessors,
                                    font=getDefaultFont())
         processorsEntry.grid(row=0, column=self._col, sticky='ew', padx=5)
 
-
     def _addButton(self, frame, text, image, tooltip, state, command):
         btn = IconButton(frame, text, image, command=command,
                          tooltip=tooltip, bg=None)
         btn.config(relief="flat", activebackground=None, compound='left',
                    fg='black', overrelief="raised",
                    state=state)
         btn.bind('<Button-1>', command)
@@ -594,15 +593,15 @@
         self.showOperationList()
 
     def _createRightTopPanel(self, topPanel):
         """
         Create a right top panel
         """
         self.topPanelTree = PluginTree(topPanel, show='tree', cursor='hand2',
-                                         style=self._getStandardTreeStyle())
+                                       style=self._getStandardTreeStyle())
         self.topPanelTree.grid(row=0, column=0, sticky='news')
 
         # configure vertical scroollbar
         ysb = ttk.Scrollbar(topPanel, orient='vertical',
                             command=self.topPanelTree.yview)
         ysb.grid(row=0, column=1, sticky='news')
         self.topPanelTree.configure(yscrollcommand=ysb.set)
@@ -661,39 +660,40 @@
         self.file_errors_path = os.path.join(Config.getLogsFolder(),
                                              pluginErrorsLogName)
 
         self.fileLog = open(self.file_log_path, 'w')
         self.fileLogErr = open(self.file_errors_path, 'w')
         self.plug_log = getRotatingFileLogger("plugins_stdout", self.file_log_path)
         self.plug_errors_log = getRotatingFileLogger("plugin_strerr", self.file_errors_path)
-        # Create two tabs where the log and errors will appears
+        # Create two tabs where the log and errors will appear
         self.Textlog.createWidgets([self.file_log_path, self.file_errors_path])
 
     def _onPluginTreeClick(self, event):
         """ check or uncheck a plugin or binary box when clicked """
         if self.tree.is_enabled():
             self.popup_menu.unpost()
             x, y, widget = event.x, event.y, event.widget
             elem = widget.identify("element", x, y)
-            self.tree.selectedItem = self.tree.identify_row(y)
-            if "image" in elem:
-                # a box was clicked
-                self._treeOperation()
-            else:
-                if self.tree.selectedItem is not None:
-                    if self.isPlugin(self.tree.item(self.tree.selectedItem,
-                                                    "values")[0]):
-                        self.showPluginInformation(self.tree.selectedItem)
-                    else:
-                        parent = self.tree.parent(self.tree.selectedItem)
-                        self.showPluginInformation(parent)
-            if len(self.operationList.getOperations(None)):
-                self.executeOpsBtn.config(state='normal')
-            else:
-                self.executeOpsBtn.config(state='disable')
+            if elem:
+                self.tree.selectedItem = self.tree.identify_row(y)
+                if "image" in elem:
+                    # a box was clicked
+                    self._treeOperation()
+                else:
+                    if self.tree.selectedItem is not None:
+                        item = self.tree.selectedItem
+                        if not self.isPlugin(self.tree.item(item, "values")[0]):
+                            item = self.tree.parent(item)
+
+                        self.showPluginInformation(item)
+
+                if len(self.operationList.getOperations(None)):
+                    self.executeOpsBtn.config(state='normal')
+                else:
+                    self.executeOpsBtn.config(state='disable')
 
     def _deleteSelectedOperation(self, e=None):
         """
         Delete a selected operation
         """
         if self.operationTree.selectedItem:
             item = self.operationTree.selectedItem
@@ -715,15 +715,15 @@
                 if not len(self.operationList.getOperations(None)):
                     self.executeOpsBtn.config(state='disable')
 
     def _applyAllOperations(self, event=None):
         """
         Execute the operation list
         """
-        # Disable the execute and cancel button
+        # Disable execute and cancel buttons
         self.executeOpsBtn.config(state='disable')
         self.cancelOpsBtn.config(state='disable')
         # Disable the TreeView
         self.tree.disable()
         if event is not None:
             self.threadOp = threading.Thread(name="plugin-manager",
                                              target=self._applyOperations,
@@ -884,15 +884,15 @@
                                      tags=('pluginName',))
             if PluginStates.AVAILABLE_RELEASE in self.tree.item(pluginName,
                                                                 'tags'):
                 pluginVersion = (plugin.getPipVersion() + '  *(Version ' +
                                  plugin.latestRelease + ' available. Right-click on the '
                                                         'plugin to update it)')
                 self.topPanelTree.tag_configure('pluginVersion',
-                                                foreground=Color.RED_COLOR)
+                                                foreground=Config.SCIPION_MAIN_COLOR)
             else:
                 self.topPanelTree.tag_configure('pluginVersion', foreground='black')
             self.topPanelTree.insert('', 'end', pluginVersion,
                                      text='  ' + pluginVersion,
                                      values='pluginVersion',
                                      tags=('pluginVersion',))
             self.topPanelTree.insert('', 'end', pluginUploadedDate,
@@ -1118,28 +1118,34 @@
         btn.grid(row=5, column=1, sticky='sw', padx=0, pady=5)
 
         btn = Label(helpFrame, text='(Right Click)   ')
         btn.grid(row=6, column=0, sticky='sw', padx=10, pady=5)
         btn = Label(helpFrame, text='Apply an operation to the selected plugin')
         btn.grid(row=6, column=1, sticky='sw', padx=0, pady=5)
 
+
 def getRotatingFileLogger(name, path):
     logger = logging.getLogger(name)
     makeFilePath(path)
     handler = RotatingFileHandler(filename=path, maxBytes=100000)
     handler.setLevel(Config.SCIPION_LOG_LEVEL)
     return logger
 
+
 class PluginManager(PluginManagerWindow):
     """
     Windows to hold a frame inside.
     """
     def __init__(self, title, master=None, **kwargs):
+
+        # Trigger plugin's variable definition
+        Config.getDomain().getPlugins()
+
         PluginManagerWindow.__init__(self, title, master, **kwargs)
-        browser = PluginBrowser(self.root, **kwargs)
+        PluginBrowser(self.root, **kwargs)
 
 
 def main():
     PluginManager("Plugin manager", None).show()
 
 
 if __name__ == '__main__':
```

### Comparing `scipion-app-3.0.9/scipion/install/update_manager.py` & `scipion-app-3.1.0/scipion/install/update_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 # *
 # **************************************************************************
 """
 This module is responsible for updating scipion-em, scipion-pyworkflow and
 scipion-app if a higher version of these is released
 """
 import argparse
-from threading import Thread
-
 from pip._internal.commands import create_command
 
 from pyworkflow.utils import redStr, greenStr, os
 from scipion.constants import MODE_UPDATE
 
 DRY_COMMAND = '-dry'
 SCIPION_NAME = 'Scipion'
@@ -101,23 +99,24 @@
                 print(greenStr('The package %s is up to date.  Your version '
                                'is %s' % (package[0], version)))
 
         return outdatedPackages
 
     @classmethod
     def getPackageState(cls, packageName, version):
-        """
-        Check if a package needs to be updated or not
-        args: packageName: the package name
-              version: version of the installed package
-        return: (True, version) if the the package needs to be updated, otherwise
+        """ Check if a package needs to be updated or not
+
+        :param packageName: the package name
+        :param version: version of the installed package
+
+        :return (True, version) if the package needs to be updated, otherwise
                 (False, version)
 
         """
-        # Ignore autocheck of outdated package that happens at import time
+        # Ignore auto-check of outdated package that happens at import time
         os.environ["OUTDATED_IGNORE"] = "1"
         from outdated import check_outdated
         from requests.exceptions import ConnectionError
         try:
             checkOutdated = check_outdated(packageName, version)
         except ConnectionError as connError:
             print("Cannot check update status of %s (%s)" % (packageName, version))
```

### Comparing `scipion-app-3.0.9/scipion/scripts/config.py` & `scipion-app-3.1.0/scipion/scripts/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 # **************************************************************************
 """
 Check the local configuration files, and/or create them if requested
 or if they do not exist.
 """
 import sys
 import os
+from datetime import datetime
 from os.path import join, exists, basename
 import time
 import optparse
 from pathlib import Path
 
-from configparser import ConfigParser  # Python 3
+from configparser import ConfigParser
 from shutil import copyfile
 
 from scipion.utils import getTemplatesPath
 
 PYWORKFLOW_SECTION = "PYWORKFLOW"
 SCIPION_CONF = 'scipion'
 BACKUPS = 'backups'
 HOSTS = 'hosts'
-PROTOCOLS = 'protocols'
 MISSING_VAR = "None"
 SCIPION_NOTIFY = 'SCIPION_NOTIFY'
 SCIPION_CONFIG = 'SCIPION_CONFIG'
 SCIPION_LOCAL_CONFIG = 'SCIPION_LOCAL_CONFIG'
 
 UPDATE_PARAM = '--update'
 COMPARE_PARAM = '--compare'
@@ -99,14 +99,20 @@
             plugin._defineVariables()
 
             print("Variables defined by plugin '%s':\n" % pluginName)
             for k, v in plugin._vars.items():
                 print("%s = %s" % (k, v))
             print("\nThese variables can be added/edited in '%s'"
                   % os.environ[SCIPION_CONFIG])
+            url = plugin.getUrl()
+
+            if url != "":
+                print("\nMore information these variables might be found at '%s'"
+                  % url)
+
         else:
             print("No plugin found with name '%s'. Module name is expected,\n"
                   "i.e. 'scipion3 config -p xmipp3' shows the config variables "
                   "defined in 'scipion-em-xmipp' plugin." % pluginName)
 
         sys.exit(0)
     elif options.show:
@@ -119,17 +125,20 @@
         sys.exit(0)
     try:
         # where templates are
         templates_dir = getTemplatesPath()
 
         scipionConfigFile = os.environ[SCIPION_CONFIG]
         # Global installation configuration files.
+
+        # NOTE: generating a protocols.conf from the template does not make much sense
+        # Plugins are dynamically creating sections and the template is currently quite
+        # outdated. It doesn't either make sense to update protocols template regularly.
         for fpath, tmplt in [
             (scipionConfigFile, SCIPION_CONF),
-            (getConfigPathFromConfigFile(scipionConfigFile, PROTOCOLS), PROTOCOLS),
             (getConfigPathFromConfigFile(scipionConfigFile, HOSTS), HOSTS)]:
             if not exists(fpath) or options.overwrite:
                 print(fpath, tmplt)
                 createConf(fpath, join(templates_dir, getTemplateName(tmplt)),
                            unattended=unattended)
             else:
                 checkConf(fpath, join(templates_dir, getTemplateName(tmplt)),
@@ -178,25 +187,15 @@
 
 
 def createConf(fpath, ftemplate, unattended=False):
     """Create config file in fpath following the template in ftemplate"""
     # Remove from the template the sections in "remove", and if "keep"
     # is used only keep those sections.
 
-    # Create directory and backup if necessary.
-    dname = os.path.dirname(fpath)
-    if not exists(dname):
-        os.makedirs(dname)
-    elif exists(fpath):
-        if not exists(join(dname, BACKUPS)):
-            os.makedirs(join(dname, BACKUPS))
-        backup = join(dname, BACKUPS,
-                      '%s.%d' % (basename(fpath), int(time.time())))
-        print(yellow("* Creating backup: %s" % backup))
-        os.rename(fpath, backup)
+    backup(fpath)
 
     # Read the template configuration file.
     print(yellow("* Creating configuration file: %s" % fpath))
     print("Please edit it to reflect the configuration of your system.\n")
 
     if not os.path.exists(ftemplate):
         raise FileNotFoundError('Missing file: %s' % ftemplate)
@@ -216,14 +215,36 @@
         # Create the actual configuration file.
         cf.write(open(fpath, 'w'))
     else:
         # For host.conf and protocols.conf, just copy files
         copyfile(ftemplate, fpath)
 
 
+def backup(fpath):
+    """
+    Create directory "backup" if necessary and back up the file.
+
+    :param fpath:
+    :return: None
+
+    """
+    dname = os.path.dirname(fpath)
+
+    if not exists(dname):
+        os.makedirs(dname)
+
+    elif exists(fpath):
+        if not exists(join(dname, BACKUPS)):
+            os.makedirs(join(dname, BACKUPS))
+        backupFn = join(dname, BACKUPS,
+                      '%s.%s' % (basename(fpath), datetime.now().strftime("%Y%m%d%H%M%S")))
+        print(yellow("* Creating backup: %s" % backupFn))
+        os.rename(fpath, backupFn)
+
+
 def addVariablesToSection(cf, section, vars, exclude=[]):
     """ Add all the variables in vars to the config "cf" at the section passed
     it cleans the path to avoid long absolute repetitive paths"""
 
     def cleanVarPath(varValue):
         """ Clean variable to avoid long paths and relate them to SCIPION_HOME or EM_ROOT"""
         import pwem
@@ -234,14 +255,18 @@
             varValue = varValue.replace(pwem.Config.SCIPION_HOME, "")
             if varValue.startswith(os.path.sep):
                 varValue = varValue[1:]
 
         elif varValue.startswith(pwem.Config.EM_ROOT):
             varValue = varValue.replace(pwem.Config.EM_ROOT, "%(EM_ROOT)s")
 
+        # duplicate %
+        elif "%" in varValue:
+            varValue = varValue.replace("%", "%%")
+
         # If value contains SCIPION_HOME and is not scipion home
         if varValue.startswith(pw.Config.SCIPION_HOME) and varValue != pw.Config.SCIPION_HOME:
             varValue = varValue.replace(pwem.Config.SCIPION_HOME, "${SCIPION_HOME}")
 
         # Replace HOME paths with ~
         home = str(Path.home())
         if varValue.startswith(home):
@@ -318,28 +343,29 @@
     :parameter update: flag, default to false. if true, values from the template will be written to the config file
     :parameter unattended: avoid questions, default to false.
     :parameter compare: make a comparison with the template"""
     # Remove from the checks the sections in "remove", and if "keep"
     # is used only check those sections.
 
     # Read the config file fpath and the template ftemplate
-    cf = ConfigParser()
+    cf = ConfigParser(interpolation=None)
     cf.optionxform = str  # keep case (stackoverflow.com/questions/1611799)
     assert cf.read(fpath) != [], 'Missing file %s' % fpath
 
-    ct = ConfigParser()
+    ct = ConfigParser(interpolation=None)
     ct.optionxform = str
 
     suggestUpdate = True  # Flag to suggest --update
 
     # Special case for scipion config... get values from objects
     if getTemplateName(SCIPION_CONF) in ftemplate:
         # This will be the place to "exclude some variables"
         addPyworkflowVariables(ct)
         addPluginsVariables(ct)
+        ftemplate = ":MEMORY:"
     else:
         # Cancel update for others than SCIPION_CONF
         update = False
         suggestUpdate = False
         assert ct.read(ftemplate) != [], 'Missing file %s' % ftemplate
 
     df = dict([(s, set(cf.options(s))) for s in cf.sections()])
@@ -352,65 +378,69 @@
 
     confChanged = False
 
     if df == dt:
         print(green("All the expected sections and options found in " + fpath))
     else:
         print("Found differences between the configuration file\n  %s\n"
-              "and the template file\n  %s" % (fpath, ftemplate))
+              "and the current defined variables.\n  %s" % (fpath, ftemplate))
         sf = set(df.keys())
         st = set(dt.keys())
         for s in sf - st:
             print("Section %s exists in the configuration file but "
                   "not in the template." % red(s))
 
         for s in st - sf:
-            print("Section %s exists in the template but not in the configuration file. Use %s parameter to update  "
+            print("Section %s is defined but not in the configuration file. Use %s parameter to update  "
                   "local config files." % (yellow(s), UPDATE_PARAM))
 
             if update:
                 # Update config file with missing section
                 cf.add_section(s)
                 # add it to the keys
                 sf.add(s)
                 df[s] = set()
                 print("Section %s added to your config file."
                       % green(s))
                 confChanged = True
 
         for s in st & sf:
             for o in df[s] - dt[s]:
-                print("In section %s, option %s exists in the configuration "
-                      "file but not in the template." % (red(s), red(o)))
+                print("In section %s, variable %s exists in the configuration "
+                      "file but not defined by any package." % (red(s), red(o)))
             for o in dt[s] - df[s]:
                 suggestion = "" if not suggestUpdate else " Use %s parameter to update local config files." % UPDATE_PARAM
-                print("In section %s, option %s exists in the template but not in the configuration file.%s" % (
-                yellow(s), yellow(o), suggestion))
+                print("In section %s, variable %s is defined by a package but not in the configuration file.%s" % (
+                    yellow(s), yellow(o), suggestion))
 
                 if update:
                     if o == 'SCIPION_NOTIFY':
                         checkNotify(ct, fpath, unattended)
                     # Update config file with missing variable
                     value = ct.get(s, o)
                     cf.set(s, o, value)
                     confChanged = True
                     print("Variable %s -> %s added and set to %s in your config file."
                           % (s, green(o), value))
 
     if update:
-        if confChanged:
-            print("Changes detected: writing changes into %s. Please check values." % fpath)
-        else:
+        if not confChanged:
             print("Update requested no changes detected for %s." % fpath)
+        else:
 
-        try:
-            with open(fpath, 'w') as f:
-                cf.write(f)
-        except Exception as e:
-            print("Could not update the config: ", e)
+            print("Changes detected: writing changes into %s.")
+
+            try:
+                # Make a back up
+                backup(fpath)
+
+                with open(fpath, 'w') as f:
+                    cf.write(f)
+            except Exception as e:
+                print("Could not update the config: ", e)
 
 
 def compareConfig(cf, ct, fPath, fTemplate):
     """ Compare configuration against template values"""
 
     print(magenta("COMPARING %s to %s" % (fPath, fTemplate)))
     print(magenta("We expect values to follow the <package>-<version> pattern."
@@ -438,100 +468,14 @@
 
     if valueInConfig != valueInTemplate:
         print("%s at %s section (%s) differs from the default value in the "
               "template: %s" % (red(variableName), section, red(valueInConfig),
                                 yellow(valueInTemplate)))
 
 
-def guessJava():
-    """Guess the system's Java installation, return a dict with the Java keys"""
-
-    options = {}
-    candidates = []
-
-    # First check if the system has a favorite one.
-    if 'JAVA_HOME' in os.environ:
-        candidates.append(os.environ['JAVA_HOME'])
-
-    # Add also all the ones related to a "javac" program.
-    for d in os.environ.get('PATH', '').split(':'):
-        if not os.path.isdir(d) or 'javac' not in os.listdir(d):
-            continue
-        javaBin = os.path.realpath(join(d, 'javac'))
-        if javaBin.endswith('/bin/javac'):
-            javaHome = javaBin[:-len('/bin/javac')]
-            candidates.append(javaHome)
-            if javaHome.endswith('/jre'):
-                candidates.append(javaHome[:-len('/jre')])
-
-    # Check in order if for any of our candidates, all related
-    # directories and files exist. If they do, that'd be our best guess.
-    for javaHome in candidates:
-        allExist = True
-        for path in ['include', join('bin', 'javac'), join('bin', 'jar')]:
-            if not exists(join(javaHome, path)):
-                allExist = False
-        if allExist:
-            options['JAVA_HOME'] = javaHome
-            break
-            # We could instead check individually for JAVA_BINDIR, JAVAC
-            # and so on, as we do with MPI options, but we go for an
-            # easier and consistent case instead: everything must be under
-            # JAVA_HOME, which is the most common case for Java.
-
-    if not options:
-        print(red("Warning: could not detect a suitable JAVA_HOME."))
-        if candidates:
-            print(red("Our candidates were:\n  %s" % '\n  '.join(candidates)))
-
-    return options
-
-
-def guessMPI():
-    """Guess the system's MPI installation, return a dict with MPI keys"""
-    # Returns MPI_LIBDIR, MPI_INCLUDE and MPI_BINDIR as a dictionary.
-
-    options = {}
-    candidates = []
-
-    # First check if the system has a favorite one.
-    for prefix in ['MPI_', 'MPI', 'OPENMPI_', 'OPENMPI']:
-        if '%sHOME' % prefix in os.environ:
-            candidates.append(os.environ['%sHOME' % prefix])
-
-    # Add also all the ones related to a "mpicc" program.
-    for d in os.environ.get('PATH', '').split(':'):
-        if not os.path.isdir(d) or 'mpicc' not in os.listdir(d):
-            continue
-        mpiBin = os.path.realpath(join(d, 'mpicc'))
-        if 'MPI_BINDIR' not in options:
-            options['MPI_BINDIR'] = os.path.dirname(mpiBin)
-        if mpiBin.endswith('/bin/mpicc'):
-            mpiHome = mpiBin[:-len('/bin/mpicc')]
-            candidates.append(mpiHome)
-
-    # Add some extra directories that are commonly around.
-    candidates += ['/usr/lib/openmpi', '/usr/lib64/mpi/gcc/openmpi']
-
-    # Check in order if for any of our candidates, all related
-    # directories and files exist. If they do, that'd be our best guess.
-    for mpiHome in candidates:
-        if (exists(join(mpiHome, 'include', 'mpi.h')) and
-                'MPI_INCLUDE' not in options):
-            options['MPI_INCLUDE'] = join(mpiHome, 'include')
-        if (exists(join(mpiHome, 'lib', 'libmpi.so')) and
-                'MPI_LIBDIR' not in options):
-            options['MPI_LIBDIR'] = join(mpiHome, 'lib')
-        if (exists(join(mpiHome, 'bin', 'mpicc')) and
-                'MPI_BINDIR' not in options):
-            options['MPI_BINDIR'] = join(mpiHome, 'bin')
-
-    return options
-
-
 def getConfigPathFromConfigFile(scipionConfigFile, configFile):
     """
     :param scipionConfigFile path to the config file to derive the folder name from
     :param configFile: name of the template: protocols or hosts so far
     :return theoretical path for the template at the same path as the config file"""
     return os.path.join(os.path.dirname(scipionConfigFile), configFile + ".conf")
```

### Comparing `scipion-app-3.0.9/scipion/scripts/fontbrowser.py` & `scipion-app-3.1.0/scipion/scripts/fontbrowser.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/scipion/scripts/kickoff.py` & `scipion-app-3.1.0/scipion/scripts/kickoff.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 import tkinter.font as tkFont
 import traceback
 import time
 
 import pyworkflow as pw
 import pyworkflow.utils as pwutils
 from pyworkflow.gui import Message, dialog
-from pyworkflow.plugin import SCIPION_JSON_TEMPLATES, Template
+from pyworkflow.plugin import Template
 from pyworkflow.project import ProjectSettings, Project
 import pyworkflow.gui as pwgui
 from pyworkflow.gui.project.base import ProjectBaseWindow
 from pyworkflow.gui.widgets import HotButton, Button
 from pyworkflow.template import TemplateList
 from scipion.constants import SCIPION_EP, MODE_PROJECT
 
@@ -62,15 +62,15 @@
 NO = "No"
 
 FLAG_PARAM = "--"
 NOGUI_FLAG = FLAG_PARAM + "nogui"
 NOSCHEDULE_FLAG = FLAG_PARAM + "noschedule"
 
 
-START_BUTTON = "Start"
+ACCEPT_BUTTON = "Accept"
 LEN_LABEL_IN_CHARS = 30
 LABEL_ALIGN_PATTERN = '{:>%s}' % LEN_LABEL_IN_CHARS
 LEN_BUTTON_IN_CHARS = 12
 BUTTON_ALIGN_PATTERN = "{:^%s}" % LEN_BUTTON_IN_CHARS
 
 FIELD_SEP = '~'
 VIEW_WIZARD = 'wizardview'
@@ -84,63 +84,89 @@
 PROJECT_PATTERN = "^\w{2}\d{4,6}-\d+$"
 PROJECT_REGEX = re.compile(PROJECT_PATTERN)
 
 
 class KickoffWindow(ProjectBaseWindow):
     """ Windows to manage all projects. """
 
-    def __init__(self, **kwargs):
+    def __init__(self, template, argsList, showScheduleOption, schedule,
+                 showProjectOption, showProject, showProjectName):
         try:
             title = '%s (%s on %s)' % ('Workflow template customizer',
                                        pwutils.getLocalUserName(),
                                        pwutils.getLocalHostName())
         except Exception:
             title = Message.LABEL_PROJECTS
 
         settings = ProjectSettings()
         self.generalCfg = settings.getConfig()
 
-        ProjectBaseWindow.__init__(self, title, minsize=(800, 350), **kwargs)
+        ProjectBaseWindow.__init__(self, title, minsize=(800, 350))
+        self.template = template
+        self.argsList = argsList
+        self.showScheduleOption = showScheduleOption
+        self.schedule = schedule
+        self.showProjectOption = showProjectOption
+        self.showProject = showProject
+        self.showProjectName = showProjectName
+
         self.viewFuncs = {VIEW_WIZARD: KickoffView}
-        self.template = kwargs.get('template', None)
         self.action = Message.LABEL_BUTTON_CANCEL
-        self.switchView(VIEW_WIZARD, **kwargs)
-
-    def close(self, e=None):
-        self.root.destroy()
-        sys.exit(0)
+        self.switchView(VIEW_WIZARD)
 
     def getTemplate(self):
         return self.template
 
     def getAction(self):
         return self.action
 
     def switchView(self, newView, **kwargs):
         # Destroy the previous view if exists:
         if self.viewWidget:
             self.viewWidget.grid_forget()
             self.viewWidget.destroy()
         # Create the new view: Instantiates KickoffView HERE!.
-        self.viewWidget = self.viewFuncs[newView](self.footer, self, template=self.template)
+        self.viewWidget = self.viewFuncs[newView](self.footer, self,
+                                                  template=self.template,
+                                                  argsList=self.argsList,
+                                                  showScheduleOption=self.showScheduleOption,
+                                                  schedule=self.schedule,
+                                                  showProjectOption=self.showProjectOption,
+                                                  showProject=self.showProject,
+                                                  showProjectName=self.showProjectName)
+
         # Grid in the second row (1)
         self.viewWidget.grid(row=0, column=0, columnspan=10, sticky='news')
         self.footer.rowconfigure(0, weight=1)
         self.footer.columnconfigure(0, weight=1)
         self.view = newView
 
+    def _onClosing(self):
+        self.root.destroy()
+        if self.showScheduleOption and self.showProjectOption:
+            sys.exit()
+
 
 class KickoffView(tk.Frame):
-    def __init__(self, parent, windows, template=None, **kwargs):
+    def __init__(self, parent, windows, template=None, argsList=[],
+                 showScheduleOption=True, schedule=True, showProjectOption=True,
+                 showProject=True, showProjectName=True, **kwargs):
+
         tk.Frame.__init__(self, parent, bg='white', **kwargs)
         self.windows = windows
         self.root = windows.root
         self.vars = {}
         self.checkvars = []
         self.template = template
+        self.argsList = argsList
+        self.showScheduleOption = showScheduleOption
+        self.schedule = schedule
+        self.showProjectOption = showProjectOption
+        self.showProject = showProject
+        self.showProjectName = showProjectName
 
         bigSize = pwgui.cfgFontSize + 2
         smallSize = pwgui.cfgFontSize - 2
         fontName = pwgui.cfgFontName
 
         self.bigFont = tkFont.Font(size=bigSize, family=fontName)
         self.bigFontBold = tkFont.Font(size=bigSize, family=fontName,
@@ -154,16 +180,15 @@
         bodyFrame.columnconfigure(0, minsize=120)
         bodyFrame.columnconfigure(1, minsize=120, weight=1)
         bodyFrame.grid(row=0, column=0, sticky='news')
         self._fillContent(bodyFrame)
 
         # Add the create project button
         btnFrame = tk.Frame(self, bg='white')
-
-        btn = HotButton(btnFrame, text=START_BUTTON,
+        btn = HotButton(btnFrame, text=ACCEPT_BUTTON,
                         font=self.bigFontBold,
                         command=self._onReadDataFromTemplateForm)
         btn.grid(row=0, column=1, sticky='ne', padx=10, pady=10)
 
         # Add the Import project button
         btn = Button(btnFrame, Message.LABEL_BUTTON_CANCEL,
                      font=self.bigFontBold,
@@ -173,54 +198,67 @@
         btnFrame.columnconfigure(0, weight=1)
         btnFrame.grid(row=1, column=0, sticky='news')
 
         self.columnconfigure(0, weight=1)
 
     def _closeCallback(self):
         self.root.destroy()
-        sys.exit()
+        if self.showScheduleOption and self.showProjectOption:
+            sys.exit()
 
     def _fillContent(self, frame):
         # Add project name
         self.template.genProjectName()
-        self._addPair(PROJECT_NAME, PROJECT_NAME, 1, frame, value=self.template.projectName)
-        self._addPair(DO_NOT_SCHEDULE, DO_NOT_SCHEDULE, 2, frame, widget=CHECKBUTTON, value=flag2Value(NOSCHEDULE_FLAG))
-        self._addPair(DO_NOT_SHOW_GUI, DO_NOT_SHOW_GUI, 3, frame, widget=CHECKBUTTON, value=flag2Value(NOGUI_FLAG), pady=(5, 30))
+        self._addPair(PROJECT_NAME, PROJECT_NAME, 1, frame, value=self.template.projectName,
+                      visible=self.showProjectName)
+
+        self._addPair(DO_NOT_SCHEDULE, DO_NOT_SCHEDULE, 2, frame,
+                      widget=CHECKBUTTON, value=not self.schedule,
+                      visible=self.showScheduleOption)
+
+        self._addPair(DO_NOT_SHOW_GUI, DO_NOT_SHOW_GUI, 3, frame,
+                      widget=CHECKBUTTON, value=not self.showProject,
+                      pady=(5, 30), visible=self.showProjectOption)
 
         # Add template params
         self._addTemplateFieldsToForm(frame)
 
-    def _addPair(self, text, title, r, lf, widget=ENTRY, traceCallback=None, mouseBind=False, value=None, pady=2):
-        label = tk.Label(lf, text=text, bg='white', font=self.bigFont)
-        label.grid(row=r, column=0, padx=(10, 5), pady=pady, sticky='nes')
+    def _addPair(self, text, title, r, lf, widget=ENTRY, traceCallback=None,
+                 mouseBind=False, value=None, pady=2, visible=True):
+
+        if visible:
+            label = tk.Label(lf, text=text, bg='white', font=self.bigFont)
+            label.grid(row=r, column=0, padx=(10, 5), pady=pady, sticky='nes')
 
         if not widget:
             return
 
         var = tk.StringVar()
 
         if value is not None:
             var.set(value)
 
-        if widget == ENTRY:
-            widget = tk.Entry(lf, width=30, font=self.bigFont,
-                              textvariable=var)
-            if traceCallback:
-                if mouseBind:  # call callback on click
-                    widget.bind("<Button-1>", traceCallback, "eee")
-                else:  # call callback on type
-                    var.trace('w', traceCallback)
-        elif widget == LABEL:
-            widget = tk.Label(lf, font=self.bigFont, textvariable=var)
-        elif widget == CHECKBUTTON:
-            widget = tk.Checkbutton(lf, text="", font=self.bigFont, variable=var,
-                        onvalue=YES, offvalue=NO, bg="white")
-
         self.vars[title] = var
-        widget.grid(row=r, column=1, sticky='news', padx=(5, 10), pady=pady)
+        if visible:
+            if widget == ENTRY:
+                widget = tk.Entry(lf, width=30, font=self.bigFont,
+                                  textvariable=var)
+                if traceCallback:
+                    if mouseBind:  # call callback on click
+                        widget.bind("<Button-1>", traceCallback, "eee")
+                    else:  # call callback on type
+                        var.trace('w', traceCallback)
+            elif widget == LABEL:
+                widget = tk.Label(lf, font=self.bigFont, textvariable=var)
+            elif widget == CHECKBUTTON:
+                var.set(YES if value else NO)
+                widget = tk.Checkbutton(lf, text="", font=self.bigFont, variable=var,
+                                        onvalue=YES, offvalue=NO, bg=pw.Config.SCIPION_BG_COLOR)
+
+            widget.grid(row=r, column=1, sticky='news', padx=(5, 10), pady=pady)
 
     def _addTemplateFieldsToForm(self, labelFrame):
         row = 5
         for field in self.template.params.values():
             alias = field.getAlias()
             text = field.getTitle() if alias is None else "%s (%s)" % (field.getTitle(), alias)
 
@@ -245,202 +283,251 @@
             newValue = self._getValue(field.getTitle())
             field.setValue(newValue)
             if not field.validate():
                 errors.append("%s value does not validate. Value: %s, Type: %s"
                               % (field.getTitle(), field.getValue(),
                                  field.getType()))
 
-        # Do more checks only if there are not previous errors
+        # Do more checks only if there are no previous errors
         if errors:
             errors.insert(0, "*Errors*:")
             self.windows.showError("\n  - ".join(errors))
         else:
             self.template.projectName = self._getValue(PROJECT_NAME)
 
             # Set parent with the data
             self.windows.template = self.template
-            if self._getValue(DO_NOT_SCHEDULE) == YES :
-                sys.argv.append(NOSCHEDULE_FLAG)
-
-            if self._getValue(DO_NOT_SHOW_GUI) == YES :
-                sys.argv.append(NOGUI_FLAG)
+            if self._getValue(DO_NOT_SCHEDULE) == YES:
+                self.argsList.append(NOSCHEDULE_FLAG)
+            if self._getValue(DO_NOT_SHOW_GUI) == YES:
+                self.argsList.append(NOGUI_FLAG)
 
-            self.windows.action = START_BUTTON
+            self.windows.action = ACCEPT_BUTTON
             self.windows.root.quit()
             self.windows.root.withdraw()
             return
 
 
-def getTemplates():
+def getTemplates(templateName=None):
     """ Get a template or templates either from arguments
         or from the templates directory.
         If more than one template is found or passed, a dialog is raised
         to choose one.
     """
-    templateFolder = getExternalJsonTemplates()
-    customTemplates = len(sys.argv) > 1
     tempList = TemplateList()
     tempId = None
-    if customTemplates:
-        fileTemplate = sys.argv[1]
-        if os.path.isfile(fileTemplate) and os.path.exists(fileTemplate):
-            t = Template("custom_template", fileTemplate)
+    if templateName:
+        if os.path.isfile(templateName) and os.path.exists(templateName):
+            t = Template("custom_template", templateName)
             tempList.addTemplate(t)
         else:
-            tempId = sys.argv[1]
+            tempId = templateName
+
     # Try to find all templates from the template folder and the plugins
     if len(tempList.templates) == 0:
         tempList.addScipionTemplates(tempId)
         if not (tempId is not None and len(tempList.templates) == 1):
             tempList.addPluginTemplates(tempId)
 
     if not len(tempList.templates):
         raise Exception("No valid file found (*.json.template).\n"
                         "Please, add (at least one) at %s "
-                        "or pass it/them as argument(s).\n"
+                        "or pass it as argument(s).\n"
                         "\n -> Usage: scipion template [PATH.json.template]\n"
-                        "\n see 'scipion help'\n" % templateFolder)
+                        "\n see 'scipion help'\n" % getExternalJsonTemplates())
 
     return tempList.sortListByPluginName().templates
 
 
-def chooseTemplate(templates):
+def chooseTemplate(templates, parentWindow=None):
+    chosenTemplate = None
     if len(templates) == 1:
         chosenTemplate = templates[0]
     else:
         provider = pwgui.tree.ListTreeProviderTemplate(templates)
-        dlg = dialog.ListDialog(None, "Workflow templates", provider,
+        dlg = dialog.ListDialog(parentWindow, "Workflow templates", provider,
                                 "Select one of the templates.",
                                 selectOnDoubleClick=True)
 
-        if dlg.result == dialog.RESULT_CANCEL:
-            sys.exit()
-        chosenTemplate = dlg.values[0]
+        if dlg.result == dialog.RESULT_YES:
+            chosenTemplate = dlg.values[0]
 
-    print("Template to use: %s" % chosenTemplate)
-    # Replace environment variables
-    chosenTemplate.replaceEnvVariables()
+    if chosenTemplate is not None:
+        print("Template to use: %s" % chosenTemplate)
+        # Replace environment variables
+        chosenTemplate.replaceEnvVariables()
 
     return chosenTemplate
 
 
-def resolveTemplate(template):
+def resolveTemplate(template, argsList, showScheduleOption=True, schedule=True,
+                    showProjectOption=True, showProject=True, showProjectName=True):
     """ Resolve a template assigning CML params to the template.
     if not enough, a window will pop pup to ask for missing ones only"""
-    if not assignAllParams(template):
-        wizWindow = KickoffWindow(template=template)
+
+    if not assignAllParams(argsList, template):
+        wizWindow = KickoffWindow(template=template,
+                                  argsList=argsList,
+                                  showScheduleOption=showScheduleOption,
+                                  schedule=schedule,
+                                  showProjectOption=showProjectOption,
+                                  showProject=showProject,
+                                  showProjectName=showProjectName)
         wizWindow.show()
-        return wizWindow.action == START_BUTTON
+        return wizWindow.action == ACCEPT_BUTTON
     else:
         # All parameters have been assigned and template is fully populated
+        # Add schedule and showProject flags back: removed at flag2value
+        if not schedule:
+            argsList.append(NOSCHEDULE_FLAG)
+
+        if not showProject:
+            argsList.append(NOGUI_FLAG)
+
         return True
 
 
-def assignAllParams(template):
+def assignAllParams(argsList, template):
     """
     Assign CML params to the template, if missing params after assignment
     return False
     """
     paramsSetted = 0
     template.parseContent()
-    if len(sys.argv) > 2:
-        attrList = sys.argv[2:]
+    if argsList:
 
-        for attr in attrList:
+        for attr in argsList:
             # skipp --params
             if attr.startswith(FLAG_PARAM):
                 continue
 
             aliasAttr, valAttr = attr.split('=')
             try:
                 paramsSetted += template.setParamValue(aliasAttr, valAttr)
             except Exception as e:
                 print(pwutils.redStr(e))
                 sys.exit(os.EX_DATAERR)
 
-        return len(template.params) == paramsSetted
-    return False
+    return len(template.params) == paramsSetted
 
 
-def launchTemplate(template):
-    """ Launches a resolved template"""
+def createTemplateFile(template):
     try:
         workflow = template.createTemplateFile()
     except Exception as e:
         workflow = None
         errorStr = "Couldn't create the template.\n" + str(e)
         print(errorStr)
         traceback.print_exc()
+    return workflow
+
 
+def launchTemplate(argsList, template):
+    """ Launches a resolved template"""
+    workflow = createTemplateFile(template)
     if workflow is not None:
         # Create the project
         if not template.projectName:
             template.genProjectName()
-        createProjectFromWorkflow(workflow, template.projectName)
+        createProjectFromWorkflow(workflow, template.projectName, argsList)
 
 
-def createProjectFromWorkflow(workflow, projectName):
+def importTemplate(template, window):
+    """
+    Import a resolved template
+    """
+    workflow = createTemplateFile(template)
+    if workflow is not None:
+        try:
+            window.getViewWidget().info('Importing workflow %s' % workflow)
+            window.project.loadProtocols(workflow)
+            window.getViewWidget().updateRunsGraph(True)
+            window.getViewWidget().cleanInfo()
+        except Exception as ex:
+            window.showError(str(ex), exception=ex)
+
+
+def createProjectFromWorkflow(workflow, projectName, argsList):
     scipion = SCIPION_EP
     scriptsPath = pw.join('project', 'scripts')
 
     # Clean the project name as pyworkflow will do
     projectName = Project.cleanProjectName(projectName)
 
     # Create the project
     print("Creating project %s" % projectName)
     createProjectScript = os.path.join(scriptsPath, 'create.py')
     os.system("python -m %s  python %s %s %s" % (scipion, createProjectScript, projectName, workflow))
     # Wait 2 seconds to avoid activity
     time.sleep(2)
 
-    if scheduleProject():
-
+    if scheduleProject(argsList):
 
         # Schedule the project
         scheduleProjectScript = os.path.join(scriptsPath, 'schedule.py')
         print("Scheduling project %s" % projectName)
         subprocess.Popen(["python", "-m", scipion, "python", scheduleProjectScript, projectName])
         # Wait 5 seconds to avoid activity
         time.sleep(5)
 
-    if launchGUI():
+    if launchGUI(argsList):
 
         print("Showing project %s" % projectName)
         # Launch scipion
         subprocess.Popen(["python", "-m", scipion, MODE_PROJECT, projectName])
 
-def flag2Value(flag):
+
+def flag2Value(argsList, flag):
     # Remove the flag from sys.argsv
-    value = getFlagArg(flag)
+    value = getFlagArg(argsList, flag)
 
     if value:
-        sys.argv.remove(flag)
+        argsList.remove(flag)
 
-    return YES if value else NO
+    return value
 
-def launchGUI():
-    """Checks if project GUI has to be launched. Only if --noGUI param is found in sys.argv it will return False"""
-    return not getFlagArg(NOGUI_FLAG)
 
-def scheduleProject():
-    return not getFlagArg(NOSCHEDULE_FLAG)
+def launchGUI(argsList):
+    """Checks if project GUI has to be launched. Only if --noGUI param is
+       found in the argument List it will return False"""
+    return not getFlagArg(argsList, NOGUI_FLAG)
 
-def getFlagArg(flag):
+
+def scheduleProject(argsList):
+    return not getFlagArg(argsList, NOSCHEDULE_FLAG)
+
+
+def getFlagArg(argsList, flag):
     """Checks if a flag exists (True) or not (False)"""
-    for arg in sys.argv:
+    for arg in argsList:
         if flag == arg.lower():
             return True
 
     # Flag not found
     return False
 
+
 def main():
-    templates = getTemplates()
+    """ Resolves command line arguments for scipion template"""
+
+    # Remove "template"
+    argsList = sys.argv[1:]
+
+    # Now, there 2 cases:
+    # 1.- it comes with a template name (full path) or id (name)
+    # 2.- is empty
+    templateName = argsList[0] if argsList else None
+    templates = getTemplates(templateName)
+
+    # Remove the name from the args, in case it is passed
+    argsList = argsList[1:]
+
     chosenTemplate = chooseTemplate(templates)
-    if resolveTemplate(chosenTemplate):
-        launchTemplate(chosenTemplate)
-    else:
-        sys.exit(3)
+
+    if chosenTemplate is not None and resolveTemplate(chosenTemplate, argsList,
+                                                      schedule=not flag2Value(argsList, NOSCHEDULE_FLAG),
+                                                      showProject=not flag2Value(argsList, NOGUI_FLAG)):
+        launchTemplate(argsList, chosenTemplate)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `scipion-app-3.0.9/scipion/scripts/tutorial.py` & `scipion-app-3.1.0/scipion/scripts/tutorial.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 Launch main project window 
 """
 
 import os
 import sys
 from collections import OrderedDict
 
-import pyworkflow as pw
 import pyworkflow.tests as tests
 from pyworkflow.project import Manager
 from pyworkflow.gui.project import ProjectWindow
 from scipion.utils import getTemplatesPath
 from abc import ABC, abstractmethod
```

### Comparing `scipion-app-3.0.9/scipion/templates/hosts.template` & `scipion-app-3.1.0/scipion/templates/hosts.template`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/scipion/templates/protocols.template` & `scipion-app-3.1.0/scipion/templates/protocols.template`

 * *Files 0% similar despite different names*

```diff
@@ -57,10 +57,10 @@
 	{"tag": "section", "text": "Imports", "icon": "bookmark.gif", "children": []},
 	{"tag": "section", "text": "Preprocess map", "icon": "bookmark.gif", "children": []},
 	{"tag": "section", "text": "Initial model", "icon": "bookmark.gif", "children": []},
 	{"tag": "section", "text": "Rigid fitting", "icon": "bookmark.gif", "children": []},
 	{"tag": "section", "text": "Flexible fitting", "icon": "bookmark.gif", "children": []},
 	{"tag": "section", "text": "Validation", "icon": "bookmark.gif", "children": []},
 	{"tag": "section", "text": "Tools-Calculators", "icon": "bookmark.gif", "children": []},
-	{"tag": "section", "text": "Others", "icon": "bookmark.gif", "children": []},
-	{"tag": "section", "text": "Exports", "icon": "bookmark.gif", "children": []}
+	{"tag": "section", "text": "Exports", "icon": "bookmark.gif", "children": []},
+	{"tag": "section", "text": "Others", "icon": "bookmark.gif", "children": []}
 	]
```

### Comparing `scipion-app-3.0.9/scipion/templates/scipion.template` & `scipion-app-3.1.0/scipion/templates/scipion.template`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/scipion/templates/scipionbox.template` & `scipion-app-3.1.0/scipion/templates/scipionbox.template`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/scipion/templates/workflow_betagal1.json` & `scipion-app-3.1.0/scipion/templates/workflow_betagal1.json`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/scipion/templates/workflow_betagal2.json` & `scipion-app-3.1.0/scipion/templates/workflow_betagal2.json`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/scipion/templates/workflow_tutorial_intro.json` & `scipion-app-3.1.0/scipion/templates/workflow_tutorial_intro.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5606851392335264%*

 * *Differences: {'0': "{'_useQueue': False, '_prerequisites': '', '_queueParams': None, 'dataStreaming': False, "*

 * *      "'timeout': 43200, 'fileTimeout': 30, 'blacklistDateFrom': None, 'blacklistDateTo': None, "*

 * *      "'useRegexps': True, 'blacklistFile': None}",*

 * * '1': "{'object.id': '57', '_useQueue': False, '_prerequisites': '', '_queueParams': None, "*

 * *      "'doDenoise': False, 'maxIteration': 50, 'doHighPass': False, 'highCutoff': 0.002, "*

 * *      "'highRaised': 0.001, 'doLowPass': False, 'lowCutoff': 0.4, 'lowRaised': 0 […]*

```diff
@@ -1,13 +1,21 @@
 [
     {
+        "_prerequisites": "",
+        "_queueParams": null,
+        "_useQueue": false,
         "acquisitionWizard": null,
         "amplitudeContrast": 0.1,
+        "blacklistDateFrom": null,
+        "blacklistDateTo": null,
+        "blacklistFile": null,
         "copyFiles": false,
+        "dataStreaming": false,
         "emxFile": null,
+        "fileTimeout": 30,
         "filesPath": "",
         "filesPattern": "",
         "haveDataBeenPhaseFlipped": false,
         "importFrom": 0,
         "magnification": 56588,
         "mdFile": null,
         "object.className": "ProtImportMicrographs",
@@ -17,115 +25,165 @@
         "runMode": 0,
         "runName": null,
         "samplingRate": 1.237,
         "samplingRateMode": 0,
         "scannedPixelSize": 7.0,
         "sphericalAberration": 2.0,
         "sqliteFile": null,
+        "timeout": 43200,
+        "useRegexps": true,
         "voltage": 300.0
     },
     {
+        "_prerequisites": "",
+        "_queueParams": null,
+        "_useQueue": false,
         "cropPixels": 10,
         "doCrop": false,
+        "doDenoise": false,
         "doDownsample": true,
+        "doHighPass": false,
         "doInvert": true,
         "doLog": false,
+        "doLowPass": false,
         "doNormalize": false,
         "doRemoveBadPix": false,
         "doSmooth": false,
         "downFactor": 5.0,
+        "highCutoff": 0.002,
+        "highRaised": 0.001,
         "hostName": "localhost",
         "inputMicrographs": "2.outputMicrographs",
         "logA": 4.431,
         "logB": 0.4018,
         "logC": 336.6,
+        "lowCutoff": 0.4,
+        "lowRaised": 0.001,
+        "maxIteration": 50,
         "mulStddev": 5,
         "numberOfMpi": 1,
         "numberOfThreads": 1,
         "object.className": "XmippProtPreprocessMicrographs",
         "object.comment": "",
-        "object.id": "43",
+        "object.id": "57",
         "object.label": "2. downsample x5",
         "orderComment": null,
         "runMode": 0,
         "runName": null,
         "sigmaConvolution": 2.0
     },
     {
+        "_prerequisites": "",
+        "_queueParams": null,
+        "_useQueue": false,
         "astigmatism": 100.0,
-        "ctfDownFactor": 1.0,
+        "avgFrames": 3,
         "findPhaseShift": false,
-        "highRes": 0.46,
+        "fixAstig": true,
+        "highRes": 10.0,
         "hostName": "localhost",
-        "inputMicrographs": "43.outputMicrographs",
-        "lowRes": 0.14,
-        "maxDefocus": 4.0,
-        "minDefocus": 0.5,
+        "inputMicrographs": "57.outputMicrographs",
+        "inputType": 1,
+        "lowRes": 50.0,
+        "maxDefocus": 40000.0,
+        "maxPhaseShift": 180.0,
+        "minDefocus": 500.0,
+        "minPhaseShift": 0.0,
         "numberOfMpi": 1,
         "numberOfThreads": 4,
-        "object.className": "ProtCTFFind",
+        "object.className": "CistemProtCTFFind",
         "object.comment": "",
-        "object.id": "85",
-        "object.label": "3. ctffind3",
+        "object.id": "112",
+        "object.label": "3. ctffind4",
         "recalculate": false,
         "runMode": 0,
         "runName": null,
+        "slowSearch": false,
         "sqliteFile": null,
-        "useCftfind4": true,
-        "windowSize": 256
+        "stepDefocus": 500.0,
+        "stepPhaseShift": 10.0,
+        "streamingBatchSize": 1,
+        "streamingSleepOnWait": 0,
+        "streamingWarning": null,
+        "usePowerSpectra": false,
+        "windowSize": 512
     },
     {
-        "inputMicrographs": "43.outputMicrographs",
-        "memory": 2.0,
+        "_prerequisites": "",
+        "_queueParams": null,
+        "_useQueue": false,
+        "doInteractive": true,
+        "inputMicrographs": "57.outputMicrographs",
         "object.className": "XmippProtParticlePicking",
         "object.comment": "",
-        "object.id": "126",
+        "object.id": "170",
         "object.label": "4a. xmipp picking",
         "runMode": 0,
-        "runName": null
+        "runName": null,
+        "saveDiscarded": false
     },
     {
+        "_prerequisites": "",
+        "_queueParams": null,
+        "_useQueue": false,
         "backRadius": -1,
         "boxSize": 110,
-        "ctfRelations": "85.outputCTF",
+        "ctfRelations": "112.outputCTF",
+        "doBorders": false,
         "doFlip": true,
         "doInvert": false,
         "doNormalize": true,
         "doRemoveDust": true,
-        "doSort": true,
+        "downFactor": 1.0,
+        "downsampleType": 0,
         "hostName": "localhost",
-        "maxZscore": 3,
-        "micsSource": 0,
+        "inputCoordinates": "170.outputCoordinates",
         "normType": 2,
         "numberOfMpi": 1,
         "numberOfThreads": 4,
         "object.className": "XmippProtExtractParticles",
         "object.comment": "",
-        "object.id": "155",
+        "object.id": "205",
         "object.label": "5. extract particles",
-        "percentage": 5,
-        "rejectionMethod": 0,
+        "patchSize": -1,
         "runMode": 0,
         "runName": null,
         "thresholdDust": 3.5
     },
     {
+        "_prerequisites": "",
+        "_queueParams": null,
+        "_useQueue": false,
         "copyFiles": false,
+        "dataStreaming": false,
+        "emdbId": null,
+        "fileTimeout": 30,
         "filesPath": "",
         "filesPattern": "",
+        "half1map": null,
+        "half2map": null,
         "importFrom": 0,
         "object.className": "ProtImportVolumes",
         "object.comment": "",
-        "object.id": "200",
+        "object.id": "253",
         "object.label": "6. import vol",
         "runMode": 0,
         "runName": null,
-        "samplingRate": 6.185
+        "samplingRate": 6.185,
+        "setHalfMaps": false,
+        "setOrigCoord": false,
+        "timeout": 43200,
+        "x": null,
+        "y": null,
+        "z": null
     },
     {
+        "_prerequisites": "",
+        "_queueParams": null,
+        "_useQueue": false,
         "align2DIterNr": "4",
         "align2dMaxChangeOffset": "2x1000 2x10",
         "align2dMaxChangeRot": "2x1000 2x20",
         "angSamplingRateDeg": "3 2 1 0.5",
         "artLambda": "0.2",
         "artReconstructionExtraCommand": "-k 0.5 -n 10 ",
         "availableMemory": 2,
@@ -143,31 +201,32 @@
         "doComputeResolution": true,
         "doLowPassFilter": true,
         "doRestricSearchbyTiltAngle": false,
         "doScale": false,
         "doSplitReferenceImages": "1",
         "fourierMaxFrequencyOfInterest": 0.25,
         "fourierReconstructionExtraCommand": "",
+        "gpuList": "0",
         "hostName": "localhost",
         "innerRadius": "28",
-        "input3DReferences": "200.outputVolume",
-        "inputParticles": "155.outputParticles",
+        "input3DReferences": "253.outputVolume",
+        "inputParticles": "205.outputParticles",
         "kernelAngularProjection": 2,
         "maskRadius": 55,
         "maskType": 1,
         "maxChangeInAngles": "1000 8 4 2",
         "maxChangeOffset": "2x1000 5",
         "minimumCrossCorrelation": "0.1",
         "mpiJobSize": 8,
         "numberOfIterations": 3,
         "numberOfMpi": 4,
         "numberOfThreads": 1,
         "object.className": "XmippProtProjMatch",
         "object.comment": "\n",
-        "object.id": "230",
+        "object.id": "299",
         "object.label": "7. projection matching",
         "onlyWinner": "0",
         "outerRadius": "55",
         "paddingAngularProjection": 1.0,
         "paddingFactor": 2.0,
         "performAlign2D": false,
         "perturbProjectionDirections": "0",
@@ -182,21 +241,31 @@
         "search5DStep": "2",
         "setOfDefocus": "",
         "symmetry": "i1",
         "symmetryGroupNeighbourhood": "",
         "tilt0": -91.0,
         "tiltF": -91.0,
         "useFscForFilter": true,
+        "useGpu": true,
         "useInitialAngles": false,
         "wbpReconstructionExtraCommand": "",
         "wienerConstant": -1.0
     },
     {
-        "inputMicrographs": "43.outputMicrographs",
+        "_prerequisites": "",
+        "_queueParams": null,
+        "_useQueue": false,
+        "boxSize": -1,
+        "device": "cpu",
+        "hostName": "localhost",
+        "inputMicrographs": "57.outputMicrographs",
+        "invertY": false,
+        "numberOfThreads": 1,
         "object.className": "EmanProtBoxing",
         "object.comment": "\n",
-        "object.id": "319",
+        "object.id": "395",
         "object.label": "4b Eman boxer",
+        "particleSize": -1,
         "runMode": 0,
         "runName": null
     }
 ]
```

### Comparing `scipion-app-3.0.9/scipion/utils.py` & `scipion-app-3.1.0/scipion/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.0.9/scipion_app.egg-info/PKG-INFO` & `scipion-app-3.1.0/scipion_app.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: scipion-app
-Version: 3.0.9
+Version: 3.1.0
 Summary: Scipion application. For processing cryo electron microscopy images and hybrid modelling
 Home-page: https://github.com/scipion-em/scipion-app
 Author: Scipion team
 Author-email: scipion@cnb.csic.es
-License: UNKNOWN
-Description: ===========
-        Scipion app
-        ===========
-        
-        **Scipion** is an image processing framework to obtain 3D models of
-        macromolecular complexes using Electron Microscopy (3DEM). It integrates
-        several software packages and presents an unified interface for both biologists
-        and developers. Scipion allows to execute workflows combining different
-        software tools, while taking care of formats and conversions. Additionally,
-        all steps are tracked and can be reproduced later on.
-        
-        Want to learn more? [Go to our web site.](http://scipion.i2pc.es)
-        
-        
-        .. figure:: https://travis-ci.org/I2PC/scipion.svg?branch=devel
-           :align: left
-           :alt: Build Status
-        
-        .. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=alert_status
-           :align: left
-           :alt: Quality Gate
-        
-        .. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=sqale_index
-           :align: left
-           :alt: Technical debt
-        
-        .. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=bugs
-           :align: left
-           :alt: Bugs
-        
 Keywords: scipion cryoem imageprocessing scipion-3.0
-Platform: UNKNOWN
+License-File: LICENSE.txt
+
+===========
+Scipion app
+===========
+
+**Scipion** is an image processing framework to obtain 3D models of
+macromolecular complexes using Electron Microscopy (3DEM). It integrates
+several software packages and presents an unified interface for both biologists
+and developers. Scipion allows to execute workflows combining different
+software tools, while taking care of formats and conversions. Additionally,
+all steps are tracked and can be reproduced later on.
+
+Want to learn more? [Go to our web site.](http://scipion.i2pc.es)
+
+
+.. figure:: https://travis-ci.org/I2PC/scipion.svg?branch=devel
+   :align: left
+   :alt: Build Status
+
+.. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=alert_status
+   :align: left
+   :alt: Quality Gate
+
+.. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=sqale_index
+   :align: left
+   :alt: Technical debt
+
+.. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=bugs
+   :align: left
+   :alt: Bugs
```

### Comparing `scipion-app-3.0.9/scipion_app.egg-info/SOURCES.txt` & `scipion-app-3.1.0/scipion_app.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,19 @@
 scipion/guiplugin.py
 scipion/utils.py
 scipion/install/__init__.py
 scipion/install/change_rpath.py
 scipion/install/clean.py
 scipion/install/find_deps.py
 scipion/install/funcs.py
-scipion/install/inspect-plugins.py
+scipion/install/inspect_plugins.py
 scipion/install/install_plugin.py
 scipion/install/plugin_funcs.py
 scipion/install/plugin_manager.py
-scipion/install/tar.py
 scipion/install/update_manager.py
-scipion/install/upgrade_release.py
 scipion/scripts/__init__.py
 scipion/scripts/config.py
 scipion/scripts/fontbrowser.py
 scipion/scripts/kickoff.py
 scipion/scripts/tutorial.py
 scipion/templates/hosts.template
 scipion/templates/protocols.template
```

### Comparing `scipion-app-3.0.9/setup.py` & `scipion-app-3.1.0/setup.py`

 * *Files identical despite different names*

