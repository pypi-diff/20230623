# Comparing `tmp/ghga_connector-0.3.3.tar.gz` & `tmp/ghga_connector-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_connector-0.3.3.tar", last modified: Wed Jun 14 09:42:43 2023, max compression
+gzip compressed data, was "ghga_connector-0.3.5.tar", last modified: Fri Jun 23 14:27:12 2023, max compression
```

## Comparing `ghga_connector-0.3.3.tar` & `ghga_connector-0.3.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.225463 ghga_connector-0.3.3/ghga_connector/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.233463 ghga_connector-0.3.3/ghga_connector/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.233463 ghga_connector-0.3.3/ghga_connector/core/api_calls/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/api_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/api_calls/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/api_calls/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/api_calls/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/api_calls/work_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/batch_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/file_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/http_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/message_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/ghga_connector/core/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.229463 ghga_connector-0.3.3/ghga_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 09:42:42.000000 ghga_connector-0.3.3/ghga_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-14 09:42:43.000000 ghga_connector-0.3.3/ghga_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.221463 ghga_connector-0.3.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.233463 ghga_connector-0.3.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.233463 ghga_connector-0.3.3/tests/fixtures/mock_api/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/mock_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/mock_api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/mock_api/testcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/integration/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/integration/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/integration/test_file_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 09:42:43.237463 ghga_connector-0.3.3/tests/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/test_api_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-14 09:42:30.000000 ghga_connector-0.3.3/tests/unit/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.898450 ghga_connector-0.3.5/ghga_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.902450 ghga_connector-0.3.5/ghga_connector/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.902450 ghga_connector-0.3.5/ghga_connector/core/api_calls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/api_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/api_calls/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/api_calls/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/api_calls/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/api_calls/work_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/batch_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/file_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/http_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/ghga_connector/core/message_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.898450 ghga_connector-0.3.5/ghga_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 14:27:12.000000 ghga_connector-0.3.5/ghga_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-23 14:27:12.910450 ghga_connector-0.3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.894451 ghga_connector-0.3.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.902450 ghga_connector-0.3.5/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.902450 ghga_connector-0.3.5/tests/fixtures/mock_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/mock_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/mock_api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/mock_api/testcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/integration/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/integration/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/integration/test_file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:27:12.906450 ghga_connector-0.3.5/tests/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/test_api_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-23 14:27:01.000000 ghga_connector-0.3.5/tests/unit/test_file_operations.py
```

### Comparing `ghga_connector-0.3.3/LICENSE` & `ghga_connector-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/PKG-INFO` & `ghga_connector-0.3.5/ghga_connector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: ghga_connector
-Version: 0.3.3
+Name: ghga-connector
+Version: 0.3.5
 Summary: GHGA Connector - A CLI client application for interacting with the GHGA system.
 Home-page: https://github.com/ghga-de/ghga-connector
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.9.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 
 [![tests](https://github.com/ghga-de/ghga-connector/actions/workflows/unit_and_int_tests.yaml/badge.svg)](https://github.com/ghga-de/ghga-connector/actions/workflows/unit_and_int_tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga-connector/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga-connector?branch=main)
 
@@ -41,29 +41,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.3
+docker pull ghga/ghga-connector:0.3.5
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.3 .
+docker build -t ghga/ghga-connector:0.3.5 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.3 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.5 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_connector-0.3.3/README.md` & `ghga_connector-0.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,29 +24,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.3
+docker pull ghga/ghga-connector:0.3.5
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.3 .
+docker build -t ghga/ghga-connector:0.3.5 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.3 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.5 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_connector-0.3.3/ghga_connector/__init__.py` & `ghga_connector-0.3.5/ghga_connector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 CLI - Client to perform up- and download operations to and from a local ghga instance
 """
 
-__version__ = "0.3.3"
+__version__ = "0.3.5"
```

### Comparing `ghga_connector-0.3.3/ghga_connector/__main__.py` & `ghga_connector-0.3.5/ghga_connector/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/ghga_connector/cli.py` & `ghga_connector-0.3.5/ghga_connector/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """ CLI-specific wrappers around core functions."""
 
 import os
+from distutils.util import strtobool
 from pathlib import Path
 
 import crypt4gh.keys
 import typer
 from ghga_service_commons.utils import crypt
 
 from ghga_connector import core
@@ -53,15 +54,14 @@
         """
         typer.secho(message, fg=core.MessageColors.FAILURE, err=True)
 
 
 cli = typer.Typer()
 
 
-@cli.command()
 def upload(  # noqa C901
     *,
     file_id: str = typer.Option(..., help="The id if the file to upload"),
     file_path: Path = typer.Option(..., help="The path to the file to upload"),
     submitter_pubkey_path: Path = typer.Argument(
         "./key.pub",
         help="The path to a public key from the key pair that was announced in the "
@@ -72,27 +72,31 @@
         help="The path to a private key from the key pair that will be used to encrypt the "
         + "crypt4gh envelope. Defaults to key in the current folder.",
     ),
 ):
     """
     Command to upload a file
     """
-    core.RequestsSession.configure(CONFIG.max_retries)
+    core.HttpxClientState.configure(CONFIG.max_retries)
 
     core.upload(
         api_url=CONFIG.upload_api,
         file_id=file_id,
         file_path=file_path,
         message_display=CLIMessageDisplay(),
         server_pubkey=CONFIG.server_pubkey,
         submitter_pubkey_path=submitter_pubkey_path,
         submitter_private_key_path=submitter_private_key_path,
     )
 
 
+if strtobool(os.getenv("UPLOAD_ENABLED") or "false"):
+    cli.command()(upload)
+
+
 @cli.command()
 def download(  # pylint: disable=too-many-arguments
     *,
     output_dir: Path = typer.Option(
         ..., help="The directory to put the downloaded files into."
     ),
     submitter_pubkey_path: Path = typer.Argument(
@@ -105,15 +109,15 @@
         help="The path to a private key from the key pair that will be used to decrypt the"
         + "work package access and work order tokens. Defaults to key in the current folder.",
     ),
 ):
     """
     Command to download files
     """
-    core.RequestsSession.configure(CONFIG.max_retries)
+    core.HttpxClientState.configure(CONFIG.max_retries)
     message_display = CLIMessageDisplay()
 
     if not submitter_pubkey_path.is_file():
         message_display.failure(f"The file {submitter_pubkey_path} does not exist.")
         raise core.exceptions.PubKeyFileDoesNotExistError(
             pubkey_path=submitter_pubkey_path
         )
```

### Comparing `ghga_connector-0.3.3/ghga_connector/config.py` & `ghga_connector-0.3.5/ghga_connector/config.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/ghga_connector/core/__init__.py` & `ghga_connector-0.3.5/ghga_connector/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 This sub-package contains the main business functionality of this service.
 It should not contain any service API-related code.
 """
 
 from . import exceptions  # noqa: F401
 from .api_calls import WorkPackageAccessor  # noqa: F401
 from .batch_processing import CliIoHandler, FileStager, StagingParameters  # noqa: F401
+from .client import HttpxClientState, httpx_client  # noqa: F401
 from .constants import (  # noqa: F401
     DEFAULT_PART_SIZE,
     MAX_PART_NUMBER,
     MAX_RETRIES,
     MAX_WAIT_TIME,
 )
 from .main import decrypt_file, download, upload  # noqa: F401
 from .message_display import AbstractMessageDisplay, MessageColors  # noqa: F401
-from .session import RequestsSession  # noqa: F401
```

### Comparing `ghga_connector-0.3.3/ghga_connector/core/api_calls/__init__.py` & `ghga_connector-0.3.5/ghga_connector/core/api_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/ghga_connector/core/api_calls/download.py` & `ghga_connector-0.3.5/ghga_connector/core/api_calls/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 This file contains all api calls related to uploading files
 """
 
 import base64
 from time import sleep
 from typing import Iterator, Tuple, Union
 
-import requests
+import httpx
 from ghga_service_commons.utils.crypt import encode_key
 from requests.structures import CaseInsensitiveDict
 
 from ghga_connector.core import exceptions
 from ghga_connector.core.api_calls.work_package import WorkPackageAccessor
+from ghga_connector.core.client import httpx_client
 from ghga_connector.core.constants import TIMEOUT
 from ghga_connector.core.http_translation import ResponseExceptionTranslator
 from ghga_connector.core.message_display import AbstractMessageDisplay
-from ghga_connector.core.session import RequestsSession
 
 # Constants for clarity of return values
 NO_DOWNLOAD_URL = None
 NO_FILE_SIZE = None
 NO_RETRY_TIME = None
 
 
-def get_download_url(  # noqa: C901
+def get_download_url(  # noqa: C901 pylint: disable=too-many-locals
     *, file_id: str, work_package_accessor: WorkPackageAccessor
 ) -> Union[Tuple[None, None, int], Tuple[str, int, None]]:
     """
     Perform a RESTful API call to retrieve a presigned download URL.
     Returns:
         A tuple of three elements:
             1. the download url
@@ -64,17 +64,18 @@
             "Authorization": f"Bearer {decrypted_token}",
             "Content-Type": "application/json",
         }
     )
 
     # Make function call to get download url
     try:
-        response = RequestsSession.get(url=url, headers=headers, timeout=TIMEOUT)
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
+        with httpx_client() as client:
+            response = client.get(url=url, headers=headers, timeout=TIMEOUT)
+    except httpx.RequestError as request_error:
+        exceptions.raise_if_connection_failed(request_error=request_error, url=url)
         raise exceptions.RequestFailedError(url=url) from request_error
 
     status_code = response.status_code
     if status_code != 200:
         if status_code == 403:
             content = response.json()
             # handle both normal and httpyexpect 403 response
@@ -190,16 +191,17 @@
             "Authorization": f"Bearer {decrypted_token}",
             "Content-Type": "application/json",
         }
     )
 
     # Make function call to get download url
     try:
-        response = RequestsSession.get(url=url, headers=headers, timeout=TIMEOUT)
-    except requests.exceptions.RequestException as request_error:
+        with httpx_client() as client:
+            response = client.get(url=url, headers=headers, timeout=TIMEOUT)
+    except httpx.RequestError as request_error:
         raise exceptions.RequestFailedError(url=url) from request_error
 
     status_code = response.status_code
 
     if status_code == 200:
         return base64.b64decode(response.content)
```

### Comparing `ghga_connector-0.3.3/ghga_connector/core/api_calls/upload.py` & `ghga_connector-0.3.5/ghga_connector/core/api_calls/upload.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 import base64
 import json
 from enum import Enum
 from pathlib import Path
 from typing import Dict, Iterator, Tuple
 
 import crypt4gh.keys
-import requests
+import httpx
 
 from ghga_connector.core import exceptions
+from ghga_connector.core.client import httpx_client
 from ghga_connector.core.constants import MAX_PART_NUMBER, TIMEOUT
 from ghga_connector.core.http_translation import ResponseExceptionTranslator
-from ghga_connector.core.session import RequestsSession
 
 # Constants for clarity of return values
 NO_DOWNLOAD_URL = None
 NO_FILE_SIZE = None
 NO_RETRY_TIME = None
 
 
@@ -67,19 +67,20 @@
     public_key = base64.b64encode(crypt4gh.keys.get_public_key(pubkey_path)).decode()
 
     post_data = {"file_id": file_id, "submitter_public_key": public_key}
     serialized_data = json.dumps(post_data)
 
     # Make function call to get upload url
     try:
-        response = RequestsSession.post(
-            url=url, headers=headers, data=serialized_data, timeout=TIMEOUT
-        )
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
+        with httpx_client() as client:
+            response = client.post(
+                url=url, headers=headers, content=serialized_data, timeout=TIMEOUT
+            )
+    except httpx.RequestError as request_error:
+        exceptions.raise_if_connection_failed(request_error=request_error, url=url)
         raise exceptions.RequestFailedError(url=url) from request_error
 
     status_code = response.status_code
     if status_code != 200:
         spec = {
             400: {
                 "existingActiveUpload": lambda: exceptions.NoUploadPossibleError(
@@ -110,17 +111,18 @@
 
     # build url and headers
     url = f"{api_url}/uploads/{upload_id}/parts/{part_no}/signed_urls"
     headers = {"Accept": "application/json", "Content-Type": "application/json"}
 
     # Make function call to get upload url
     try:
-        response = RequestsSession.post(url=url, headers=headers, timeout=TIMEOUT)
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
+        with httpx_client() as client:
+            response = client.post(url=url, headers=headers, timeout=TIMEOUT)
+    except httpx.RequestError as request_error:
+        exceptions.raise_if_connection_failed(request_error=request_error, url=url)
         raise exceptions.RequestFailedError(url=url) from request_error
 
     status_code = response.status_code
     if status_code != 200:
         spec = {
             403: {
                 "noFileAccess": lambda: exceptions.UserHasNoUploadAccessError(
@@ -181,19 +183,20 @@
     # build url and headers
     url = f"{api_url}/uploads/{upload_id}"
     headers = {"Accept": "*/*", "Content-Type": "application/json"}
     post_data = {"status": upload_status}
     serialized_data = json.dumps(post_data)
 
     try:
-        response = RequestsSession.patch(
-            url=url, headers=headers, data=serialized_data, timeout=TIMEOUT
-        )
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
+        with httpx_client() as client:
+            response = client.patch(
+                url=url, headers=headers, content=serialized_data, timeout=TIMEOUT
+            )
+    except httpx.RequestError as request_error:
+        exceptions.raise_if_connection_failed(request_error=request_error, url=url)
         raise exceptions.RequestFailedError(url=url) from request_error
 
     status_code = response.status_code
     if status_code != 204:
         spec = {
             400: {
                 "uploadNotPending": lambda: exceptions.CantChangeUploadStatusError(
@@ -228,17 +231,18 @@
     """
 
     # build url and headers
     url = f"{api_url}/uploads/{upload_id}"
     headers = {"Accept": "*/*", "Content-Type": "application/json"}
 
     try:
-        response = RequestsSession.get(url=url, headers=headers, timeout=TIMEOUT)
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
+        with httpx_client() as client:
+            response = client.get(url=url, headers=headers, timeout=TIMEOUT)
+    except httpx.RequestError as request_error:
+        exceptions.raise_if_connection_failed(request_error=request_error, url=url)
         raise exceptions.RequestFailedError(url=url) from request_error
 
     status_code = response.status_code
     if status_code != 200:
         spec = {
             403: {
                 "noFileAccess": lambda: exceptions.UserHasNoUploadAccessError(
@@ -263,17 +267,18 @@
     """
 
     # build url and headers
     url = f"{api_url}/files/{file_id}"
     headers = {"Accept": "application/json", "Content-Type": "application/json"}
 
     try:
-        response = RequestsSession.get(url=url, headers=headers, timeout=TIMEOUT)
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=url)
+        with httpx_client() as client:
+            response = client.get(url=url, headers=headers, timeout=TIMEOUT)
+    except httpx.RequestError as request_error:
+        exceptions.raise_if_connection_failed(request_error=request_error, url=url)
         raise exceptions.RequestFailedError(url=url) from request_error
 
     status_code = response.status_code
     if status_code != 200:
         spec = {
             403: {
                 "noFileAccess": lambda: exceptions.UserHasNoFileAccessError(
```

### Comparing `ghga_connector-0.3.3/ghga_connector/core/api_calls/utils.py` & `ghga_connector-0.3.5/ghga_connector/core/api_calls/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 This file contains general utility api calls
 """
 
-import requests
+import httpx
 
 
 def check_url(api_url, *, wait_time=1) -> bool:
     """
     Checks, if an url is reachable within a certain time
     """
     try:
-        requests.get(url=api_url, timeout=wait_time)
-    except requests.exceptions.RequestException:
+        httpx.get(url=api_url, timeout=wait_time)
+    except httpx.RequestError:
         return False
     return True
```

### Comparing `ghga_connector-0.3.3/ghga_connector/core/api_calls/work_package.py` & `ghga_connector-0.3.5/ghga_connector/core/api_calls/work_package.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # limitations under the License.
 """
 This file contains all api calls related to obtaining work package and work order tokens
 """
 
 from dataclasses import dataclass
 
-import requests
+import httpx
 from ghga_service_commons.utils.crypt import decrypt
 
 from ghga_connector.core import exceptions
-from ghga_connector.core.session import RequestsSession
+from ghga_connector.core.client import httpx_client
 
 
 @dataclass
 class WorkPackageAccessor:
     """Wrapper for WPS associated API call parameters"""
 
     access_token: str
@@ -42,16 +42,17 @@
 
         url = f"{self.api_url}/work-packages/{self.package_id}"
 
         # send authorization header as bearer token
         headers = {"Authorization": f"Bearer {self.access_token}"}
 
         try:
-            response = RequestsSession.get(url=url, headers=headers)
-        except requests.exceptions.RequestException as request_error:
+            with httpx_client() as client:
+                response = client.get(url=url, headers=headers)
+        except httpx.RequestError as request_error:
             raise exceptions.RequestFailedError(url=url) from request_error
 
         status_code = response.status_code
         if status_code != 200:
             if status_code == 403:
                 raise exceptions.NoWorkPackageAccessError(
                     work_package_id=self.package_id
@@ -69,16 +70,17 @@
 
         url = f"{self.api_url}/work-packages/{self.package_id}/files/{file_id}/work-order-tokens"
 
         # send authorization header as bearer token
         headers = {"Authorization": f"Bearer {self.access_token}"}
 
         try:
-            response = RequestsSession.post(url=url, headers=headers)
-        except requests.exceptions.RequestException as request_error:
+            with httpx_client() as client:
+                response = client.post(url=url, headers=headers)
+        except httpx.RequestError as request_error:
             raise exceptions.RequestFailedError(url=url) from request_error
 
         status_code = response.status_code
         if status_code != 201:
             if status_code == 403:
                 raise exceptions.NoWorkPackageAccessError(
                     work_package_id=self.package_id
```

### Comparing `ghga_connector-0.3.3/ghga_connector/core/batch_processing.py` & `ghga_connector-0.3.5/ghga_connector/core/batch_processing.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/ghga_connector/core/constants.py` & `ghga_connector-0.3.5/ghga_connector/core/constants.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/ghga_connector/core/exceptions.py` & `ghga_connector-0.3.5/ghga_connector/core/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 # limitations under the License.
 #
 
 """Custom Exceptions."""
 
 from pathlib import Path
 
-import requests
-import urllib3.exceptions
+import httpx
 
 from ghga_connector.core.constants import MAX_PART_NUMBER
 
 
 class AbortBatchProcessError(RuntimeError):
     """Thrown when user selected to not proceed with batch proccesing"""
 
@@ -228,19 +227,19 @@
     exceeded."""
 
     def __init__(self, *, max_wait_time: int):
         message = f"Exceeded maximum wait time of {max_wait_time} seconds."
         super().__init__(message)
 
 
-class MaxRetriesReachedError(RuntimeError):
-    """Thrown, when the specified number of retries has been exceeded."""
+class ConnectionFailedError(RuntimeError):
+    """Thrown, when a ConnectError or ConnectTimeout error is raised by httpx"""
 
     def __init__(self, *, url: str, reason: str):
-        message = f"Exceeded maximum retries for '{url}' due to: {reason}."
+        message = f"Request to '{url}' failed to connect. Reason: {reason}"
         super().__init__(message)
 
 
 class MaxPartNoExceededError(RuntimeError):
     """
     Thrown requesting a part number larger than the maximally possible number of parts.
 
@@ -248,26 +247,21 @@
     """
 
     def __init__(self):
         message = f"No more than ({MAX_PART_NUMBER}) file parts can be up-/downloaded."
         super().__init__(message)
 
 
-def raise_if_max_retries(request_error: requests.exceptions.RequestException, url: str):
+def raise_if_connection_failed(request_error: httpx.RequestError, url: str):
     """
     Check if request exception is caused by hitting max retries and raise accordingly
     """
-    if isinstance(request_error, requests.exceptions.ConnectionError):
-        if request_error.args and isinstance(
-            request_error.args[0], urllib3.exceptions.MaxRetryError
-        ):
-            max_retry_error = request_error.args[0]
-            raise MaxRetriesReachedError(
-                url=url, reason=str(max_retry_error.reason)
-            ) from max_retry_error
+    if isinstance(request_error, (httpx.ConnectError, httpx.ConnectTimeout)):
+        connection_failure = str(request_error.args[0])
+        raise ConnectionFailedError(url=url, reason=connection_failure)
 
 
 class EnvelopeNotFoundError(RuntimeError):
     """Thrown, when the envelope requested for a file could not be retrieved"""
 
     def __init__(self, *, file_id: str):
         message = f"The request for an envelope for the file with ID {file_id} failed."
```

### Comparing `ghga_connector-0.3.3/ghga_connector/core/file_operations.py` & `ghga_connector-0.3.5/ghga_connector/core/file_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 from pathlib import Path
 from queue import Queue
 from tempfile import mkstemp
 from typing import Any, Iterator, Sequence, Tuple, Union
 
 import crypt4gh.keys
 import crypt4gh.lib
-import requests
+import httpx
 
 from ghga_connector.core import exceptions
+from ghga_connector.core.client import httpx_client
 from ghga_connector.core.constants import TIMEOUT
-from ghga_connector.core.session import RequestsSession
 
 
 class Crypt4GHEncryptor:
     """Convenience class to deal with Crypt4GH encryption"""
 
     def __init__(
         self,
@@ -101,19 +101,20 @@
     end: int,
     queue: Queue,
 ) -> None:
     """Download a specific range of a file's content using a presigned download url."""
 
     headers = {"Range": f"bytes={start}-{end}"}
     try:
-        response = RequestsSession.get(
-            download_url, headers=headers, timeout=TIMEOUT, allow_redirects=False
+        with httpx_client() as client:
+            response = client.get(download_url, headers=headers, timeout=TIMEOUT)
+    except httpx.RequestError as request_error:
+        exceptions.raise_if_connection_failed(
+            request_error=request_error, url=download_url
         )
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=download_url)
         raise exceptions.RequestFailedError(url=download_url) from request_error
 
     status_code = response.status_code
 
     # 200, if the full file was returned, 206 else.
     if status_code in (200, 206):
         queue.put((start, response.content))
@@ -197,17 +198,20 @@
         yield file_part
 
 
 def upload_file_part(*, presigned_url: str, part: bytes) -> None:
     """Upload File"""
 
     try:
-        response = RequestsSession.put(presigned_url, data=part, timeout=TIMEOUT)
-    except requests.exceptions.RequestException as request_error:
-        exceptions.raise_if_max_retries(request_error=request_error, url=presigned_url)
+        with httpx_client() as client:
+            response = client.put(presigned_url, content=part, timeout=TIMEOUT)
+    except httpx.RequestError as request_error:
+        exceptions.raise_if_connection_failed(
+            request_error=request_error, url=presigned_url
+        )
         raise exceptions.RequestFailedError(url=presigned_url) from request_error
 
     status_code = response.status_code
     if status_code == 200:
         return
 
     raise exceptions.BadResponseCodeError(url=presigned_url, response_code=status_code)
```

### Comparing `ghga_connector-0.3.3/ghga_connector/core/http_translation.py` & `ghga_connector-0.3.5/ghga_connector/core/http_translation.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 """
 Adds wrapper classes to translate httpyexpect errors and check against
 provided exception specs for all API endpoints
 """
 
 from typing import Dict
 
-import requests
+import httpx
 from httpyexpect.client import ExceptionMapping, ResponseTranslator
 
 
 class ResponseExceptionTranslator:
     """Base class providing behaviour and injection point for spec"""
 
     def __init__(self, *, spec: Dict[int, object]) -> None:
         self._exception_map = ExceptionMapping(spec)
 
-    def handle(self, response: requests.Response):
+    def handle(self, response: httpx.Response):
         """Translate and raise error, if defined by spec"""
         translator = ResponseTranslator(response, exception_map=self._exception_map)
         translator.raise_for_error()
```

### Comparing `ghga_connector-0.3.3/ghga_connector/core/main.py` & `ghga_connector-0.3.5/ghga_connector/core/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 #
 
 """Main domain logic."""
 
 import os
 from pathlib import Path
-from queue import Queue
+from queue import Empty, Queue
 from typing import List
 
 from ghga_connector.core import exceptions
 from ghga_connector.core.api_calls import (
     UploadStatus,
     WorkPackageAccessor,
     await_download_url,
@@ -131,15 +131,15 @@
     try:
         upload_file_parts(
             api_url=api_url,
             upload_id=upload_id,
             part_size=part_size,
             file_path=Path(encrypted_file_path),
         )
-    except exceptions.MaxRetriesReachedError as error:
+    except exceptions.ConnectionFailedError as error:
         message_display.failure(
             "The upload has failed too many times. The upload was aborted."
         )
         raise error
     finally:
         # remove temporary encrypted file
         os.remove(encrypted_file_path)
@@ -247,15 +247,15 @@
             envelope=envelope,
             output_file=str(output_file_ongoing),
             file_id=file_id,
             part_size=part_size,
             file_size=download_url_tuple[1],
             work_package_accessor=work_package_accessor,
         )
-    except exceptions.MaxRetriesReachedError as error:
+    except exceptions.ConnectionFailedError as error:
         # Remove file, if the download failed.
         output_file_ongoing.unlink()
         raise error
     except exceptions.NoS3AccessMethodError as error:
         message_display.failure(
             f"The request to return information for file {file_id}"
             + " did not return an S3 access method."
@@ -313,15 +313,18 @@
 
     # Write the downloaded parts to a file
     with open(output_file, "wb") as file:
         # put envelope in file
         downloaded_size = len(envelope)
         file.write(envelope)
         while downloaded_size < file_size:
-            start, part = queue.get()
+            try:
+                start, part = queue.get(block=False)
+            except Empty:
+                continue
             file.seek(start + len(envelope))
             file.write(part)
             downloaded_size += len(part)
             queue.task_done()
 
 
 def get_wps_token(max_tries: int, message_display: AbstractMessageDisplay) -> List[str]:
```

### Comparing `ghga_connector-0.3.3/ghga_connector/core/message_display.py` & `ghga_connector-0.3.5/ghga_connector/core/message_display.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/ghga_connector.egg-info/PKG-INFO` & `ghga_connector-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
-Name: ghga-connector
-Version: 0.3.3
+Name: ghga_connector
+Version: 0.3.5
 Summary: GHGA Connector - A CLI client application for interacting with the GHGA system.
 Home-page: https://github.com/ghga-de/ghga-connector
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.9.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 
 [![tests](https://github.com/ghga-de/ghga-connector/actions/workflows/unit_and_int_tests.yaml/badge.svg)](https://github.com/ghga-de/ghga-connector/actions/workflows/unit_and_int_tests.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga-connector/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga-connector?branch=main)
 
@@ -41,29 +41,29 @@
 
 
 ## Installation
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-connector):
 ```bash
-docker pull ghga/ghga-connector:0.3.3
+docker pull ghga/ghga-connector:0.3.5
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-connector:0.3.3 .
+docker build -t ghga/ghga-connector:0.3.5 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-connector:0.3.3 --help
+docker run -p 8080:8080 ghga/ghga-connector:0.3.5 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_connector-0.3.3/ghga_connector.egg-info/SOURCES.txt` & `ghga_connector-0.3.5/ghga_connector.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 ghga_connector.egg-info/dependency_links.txt
 ghga_connector.egg-info/entry_points.txt
 ghga_connector.egg-info/not-zip-safe
 ghga_connector.egg-info/requires.txt
 ghga_connector.egg-info/top_level.txt
 ghga_connector/core/__init__.py
 ghga_connector/core/batch_processing.py
+ghga_connector/core/client.py
 ghga_connector/core/constants.py
 ghga_connector/core/exceptions.py
 ghga_connector/core/file_operations.py
 ghga_connector/core/http_translation.py
 ghga_connector/core/main.py
 ghga_connector/core/message_display.py
-ghga_connector/core/session.py
 ghga_connector/core/api_calls/__init__.py
 ghga_connector/core/api_calls/download.py
 ghga_connector/core/api_calls/upload.py
 ghga_connector/core/api_calls/utils.py
 ghga_connector/core/api_calls/work_package.py
 tests/fixtures/__init__.py
 tests/fixtures/config.py
```

### Comparing `ghga_connector-0.3.3/setup.cfg` & `ghga_connector-0.3.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 include_package_data = True
 packages = find:
 install_requires = 
 	typer==0.7.0
 	crypt4gh==1.6
 	ghga-service-commons[api, crypt]==0.4.2
 	hexkit[s3]==0.10.0
-python_requires = >= 3.9.10
+python_requires = >= 3.9
 
 [options.entry_points]
 console_scripts = 
 	ghga-connector = ghga_connector.__main__:run
 
 [options.packages.find]
 exclude = tests
```

### Comparing `ghga_connector-0.3.3/setup.py` & `ghga_connector-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/fixtures/__init__.py` & `ghga_connector-0.3.5/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/fixtures/config.py` & `ghga_connector-0.3.5/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/fixtures/mock_api/__init__.py` & `ghga_connector-0.3.5/tests/fixtures/mock_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/fixtures/mock_api/app.py` & `ghga_connector-0.3.5/tests/fixtures/mock_api/app.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/fixtures/mock_api/testcontainer.py` & `ghga_connector-0.3.5/tests/fixtures/mock_api/testcontainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # limitations under the License.
 #
 
 """A testcontainer for running the mock app in the background."""
 
 from pathlib import Path
 
-import requests
+import httpx
 from testcontainers.core.container import DockerContainer
 from testcontainers.core.waiting_utils import wait_container_is_ready
 
 APP_MODULE_PATH = Path(__file__).parent.resolve() / "app.py"
 
 
 class MockAPIContainer(DockerContainer):
@@ -70,15 +70,15 @@
         port = self.get_exposed_port(self._port)
         return f"http://{ip}:{port}"
 
     @wait_container_is_ready()
     def readiness_probe(self):
         """Test if the RabbitMQ broker is ready."""
         connection_url = self.get_connection_url()
-        request = requests.get(f"{connection_url}/ready", timeout=0.5)
+        request = httpx.get(f"{connection_url}/ready", timeout=0.5)
 
         if request.status_code != 204:
             raise RuntimeError("Mock API server not ready.")
 
     def start(self):
         """Start the test container."""
         super().start()
```

### Comparing `ghga_connector-0.3.3/tests/fixtures/s3.py` & `ghga_connector-0.3.5/tests/fixtures/s3.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/fixtures/state.py` & `ghga_connector-0.3.5/tests/fixtures/state.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/fixtures/utils.py` & `ghga_connector-0.3.5/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/integration/__init__.py` & `ghga_connector-0.3.5/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/integration/fixtures/__init__.py` & `ghga_connector-0.3.5/tests/integration/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/integration/fixtures/utils.py` & `ghga_connector-0.3.5/tests/integration/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/integration/test_cli.py` & `ghga_connector-0.3.5/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/integration/test_file_operations.py` & `ghga_connector-0.3.5/tests/integration/test_file_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Test file operations"""
 
-from queue import Queue
+from queue import Empty, Queue
 from typing import Any, Iterator, Tuple, Union
 
 import pytest
 
 from ghga_connector.core.file_operations import (
     calc_part_ranges,
     download_content_range,
@@ -106,13 +106,16 @@
     }
 
     # donwload file parts with dedicated function:
     download_file_parts(**kwargs)
 
     obtained = 0
     while obtained < len(expected_bytes):
-        start, obtained_bytes = queue.get()
+        try:
+            start, obtained_bytes = queue.get(block=False)
+        except Empty:
+            continue
         obtained += len(obtained_bytes)
         queue.task_done()
         assert expected_bytes[start : start + part_size] == obtained_bytes
 
     assert obtained == len(expected_bytes)
```

### Comparing `ghga_connector-0.3.3/tests/unit/__init__.py` & `ghga_connector-0.3.5/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/unit/fixtures/__init__.py` & `ghga_connector-0.3.5/tests/unit/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/unit/fixtures/utils.py` & `ghga_connector-0.3.5/tests/unit/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/unit/test_core.py` & `ghga_connector-0.3.5/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `ghga_connector-0.3.3/tests/unit/test_file_operations.py` & `ghga_connector-0.3.5/tests/unit/test_file_operations.py`

 * *Files identical despite different names*

