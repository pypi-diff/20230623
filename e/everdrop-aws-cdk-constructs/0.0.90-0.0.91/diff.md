# Comparing `tmp/everdrop-aws-cdk-constructs-0.0.90.tar.gz` & `tmp/everdrop-aws-cdk-constructs-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "everdrop-aws-cdk-constructs-0.0.90.tar", last modified: Thu Jun 22 00:34:04 2023, max compression
+gzip compressed data, was "everdrop-aws-cdk-constructs-0.0.91.tar", last modified: Fri Jun 23 00:36:06 2023, max compression
```

## Comparing `everdrop-aws-cdk-constructs-0.0.90.tar` & `everdrop-aws-cdk-constructs-0.0.91.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:34:04.902305 everdrop-aws-cdk-constructs-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-22 00:33:50.000000 everdrop-aws-cdk-constructs-0.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 00:33:50.000000 everdrop-aws-cdk-constructs-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-22 00:34:04.902305 everdrop-aws-cdk-constructs-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 00:33:50.000000 everdrop-aws-cdk-constructs-0.0.90/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 00:33:50.000000 everdrop-aws-cdk-constructs-0.0.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 00:34:04.906304 everdrop-aws-cdk-constructs-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-22 00:33:50.000000 everdrop-aws-cdk-constructs-0.0.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:34:04.902305 everdrop-aws-cdk-constructs-0.0.90/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:34:04.902305 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-06-22 00:33:50.000000 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:34:04.902305 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-22 00:33:50.000000 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21421 2023-06-22 00:33:50.000000 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs/_jsii/everdrop-aws-cdk-constructs@0.0.90.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:33:50.000000 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:34:04.902305 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-22 00:34:04.000000 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-22 00:34:04.000000 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:34:04.000000 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-22 00:34:04.000000 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 00:34:04.000000 everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:36:06.914227 everdrop-aws-cdk-constructs-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-23 00:35:52.000000 everdrop-aws-cdk-constructs-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 00:35:52.000000 everdrop-aws-cdk-constructs-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-23 00:36:06.914227 everdrop-aws-cdk-constructs-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 00:35:52.000000 everdrop-aws-cdk-constructs-0.0.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-23 00:35:52.000000 everdrop-aws-cdk-constructs-0.0.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 00:36:06.914227 everdrop-aws-cdk-constructs-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-23 00:35:52.000000 everdrop-aws-cdk-constructs-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:36:06.910227 everdrop-aws-cdk-constructs-0.0.91/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:36:06.914227 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-06-23 00:35:52.000000 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:36:06.914227 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-23 00:35:52.000000 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-06-23 00:35:52.000000 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs/_jsii/everdrop-aws-cdk-constructs@0.0.91.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 00:35:52.000000 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:36:06.914227 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-23 00:36:06.000000 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-23 00:36:06.000000 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 00:36:06.000000 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 00:36:06.000000 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 00:36:06.000000 everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs.egg-info/top_level.txt
```

### Comparing `everdrop-aws-cdk-constructs-0.0.90/LICENSE` & `everdrop-aws-cdk-constructs-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `everdrop-aws-cdk-constructs-0.0.90/PKG-INFO` & `everdrop-aws-cdk-constructs-0.0.91/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everdrop-aws-cdk-constructs
-Version: 0.0.90
+Version: 0.0.91
 Summary: Package provides opinionated constrcuts for common patterns used in everdrop infrastructure
 Home-page: https://github.com/everdropde/ed-aws-cdk-constructs.git
 Author: Fabian Bosler<FBosler@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/everdropde/ed-aws-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `everdrop-aws-cdk-constructs-0.0.90/setup.py` & `everdrop-aws-cdk-constructs-0.0.91/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "everdrop-aws-cdk-constructs",
-    "version": "0.0.90",
+    "version": "0.0.91",
     "description": "Package provides opinionated constrcuts for common patterns used in everdrop infrastructure",
     "license": "Apache-2.0",
     "url": "https://github.com/everdropde/ed-aws-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Fabian Bosler<FBosler@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "everdrop_aws_cdk_constructs",
         "everdrop_aws_cdk_constructs._jsii"
     ],
     "package_data": {
         "everdrop_aws_cdk_constructs._jsii": [
-            "everdrop-aws-cdk-constructs@0.0.90.jsii.tgz"
+            "everdrop-aws-cdk-constructs@0.0.91.jsii.tgz"
         ],
         "everdrop_aws_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs/__init__.py` & `everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs.egg-info/PKG-INFO` & `everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everdrop-aws-cdk-constructs
-Version: 0.0.90
+Version: 0.0.91
 Summary: Package provides opinionated constrcuts for common patterns used in everdrop infrastructure
 Home-page: https://github.com/everdropde/ed-aws-cdk-constructs.git
 Author: Fabian Bosler<FBosler@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/everdropde/ed-aws-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `everdrop-aws-cdk-constructs-0.0.90/src/everdrop_aws_cdk_constructs.egg-info/SOURCES.txt` & `everdrop-aws-cdk-constructs-0.0.91/src/everdrop_aws_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/everdrop_aws_cdk_constructs/py.typed
 src/everdrop_aws_cdk_constructs.egg-info/PKG-INFO
 src/everdrop_aws_cdk_constructs.egg-info/SOURCES.txt
 src/everdrop_aws_cdk_constructs.egg-info/dependency_links.txt
 src/everdrop_aws_cdk_constructs.egg-info/requires.txt
 src/everdrop_aws_cdk_constructs.egg-info/top_level.txt
 src/everdrop_aws_cdk_constructs/_jsii/__init__.py
-src/everdrop_aws_cdk_constructs/_jsii/everdrop-aws-cdk-constructs@0.0.90.jsii.tgz
+src/everdrop_aws_cdk_constructs/_jsii/everdrop-aws-cdk-constructs@0.0.91.jsii.tgz
```

