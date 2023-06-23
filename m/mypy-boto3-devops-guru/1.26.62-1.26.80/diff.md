# Comparing `tmp/mypy-boto3-devops-guru-1.26.62.tar.gz` & `tmp/mypy-boto3-devops-guru-1.26.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-devops-guru-1.26.62.tar", last modified: Wed Feb  1 20:26:24 2023, max compression
+gzip compressed data, was "mypy-boto3-devops-guru-1.26.80.tar", last modified: Mon Feb 27 20:35:29 2023, max compression
```

## Comparing `mypy-boto3-devops-guru-1.26.62.tar` & `mypy-boto3-devops-guru-1.26.80.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:26:24.127657 mypy-boto3-devops-guru-1.26.62/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-02-01 20:26:24.127657 mypy-boto3-devops-guru-1.26.62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:26:24.127657 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31157 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-02-01 20:25:59.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    61082 2023-02-01 20:25:58.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:26:24.127657 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-02-01 20:26:23.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-02-01 20:26:23.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:26:23.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:26:23.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-01 20:26:23.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-01 20:26:23.000000 mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 20:26:24.127657 mypy-boto3-devops-guru-1.26.62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-02-01 20:25:57.000000 mypy-boto3-devops-guru-1.26.62/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.132040 mypy-boto3-devops-guru-1.26.80/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-02-27 20:35:29.124040 mypy-boto3-devops-guru-1.26.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21340 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.124040 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31157 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13686 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61203 2023-02-27 20:35:03.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61138 2023-02-27 20:35:02.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.124040 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22842 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-27 20:35:28.000000 mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:35:29.132040 mypy-boto3-devops-guru-1.26.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-02-27 20:35:01.000000 mypy-boto3-devops-guru-1.26.80/setup.py
```

### Comparing `mypy-boto3-devops-guru-1.26.62/LICENSE` & `mypy-boto3-devops-guru-1.26.80/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.62/PKG-INFO` & `mypy-boto3-devops-guru-1.26.80/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.26.62
-Summary: Type annotations for boto3.DevOpsGuru 1.26.62 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.80
+Summary: Type annotations for boto3.DevOpsGuru 1.26.80 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devops-guru?color=blue)](https://pypistats.org/packages/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.26.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-devops-guru-1.26.62/README.md` & `mypy-boto3-devops-guru-1.26.80/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devops-guru?color=blue)](https://pypistats.org/packages/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.26.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/__init__.py` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/__init__.pyi` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/__main__.py` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DevOpsGuru 1.26.62\nVersion:         1.26.62\nBuilder version:"
-        " 7.12.3\nDocs:           "
+        "Type annotations for boto3.DevOpsGuru 1.26.80\nVersion:         1.26.80\nBuilder version:"
+        " 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.62")
+    print("1.26.80")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/client.py` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/client.pyi` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/literals.py` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,14 +340,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -516,14 +517,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/literals.pyi` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -338,14 +338,15 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -514,14 +515,15 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
     "waf",
     "waf-regional",
     "wafv2",
```

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/paginator.py` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/paginator.pyi` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/type_defs.py` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2093,14 +2093,15 @@
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
         "ResourceCollection": ResourceCollectionTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
+        "Description": str,
     },
     total=False,
 )
 
 ProactiveAnomalyTypeDef = TypedDict(
     "ProactiveAnomalyTypeDef",
     {
@@ -2113,14 +2114,15 @@
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
         "ResourceCollection": ResourceCollectionTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
+        "Description": str,
     },
     total=False,
 )
 
 ReactiveAnomalySummaryTypeDef = TypedDict(
     "ReactiveAnomalySummaryTypeDef",
     {
```

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru/type_defs.pyi` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2028,14 +2028,15 @@
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
         "ResourceCollection": ResourceCollectionTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
+        "Description": str,
     },
     total=False,
 )
 
 ProactiveAnomalyTypeDef = TypedDict(
     "ProactiveAnomalyTypeDef",
     {
@@ -2048,14 +2049,15 @@
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
         "ResourceCollection": ResourceCollectionTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
+        "Description": str,
     },
     total=False,
 )
 
 ReactiveAnomalySummaryTypeDef = TypedDict(
     "ReactiveAnomalySummaryTypeDef",
     {
```

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru.egg-info/PKG-INFO` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-devops-guru
-Version: 1.26.62
-Summary: Type annotations for boto3.DevOpsGuru 1.26.62 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.80
+Summary: Type annotations for boto3.DevOpsGuru 1.26.80 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-devops-guru.svg?color=blue)](https://pypi.org/project/mypy-boto3-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-devops-guru?color=blue)](https://pypistats.org/packages/mypy-boto3-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DevOpsGuru 1.26.62](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
+[boto3.DevOpsGuru 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-devops-guru docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_devops_guru/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-devops-guru-1.26.62/mypy_boto3_devops_guru.egg-info/SOURCES.txt` & `mypy-boto3-devops-guru-1.26.80/mypy_boto3_devops_guru.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-devops-guru-1.26.62/setup.py` & `mypy-boto3-devops-guru-1.26.80/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-devops-guru",
-    version="1.26.62",
+    version="1.26.80",
     packages=["mypy_boto3_devops_guru"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DevOpsGuru 1.26.62 service generated with mypy-boto3-builder"
-        " 7.12.3"
+        "Type annotations for boto3.DevOpsGuru 1.26.80 service generated with mypy-boto3-builder"
+        " 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

