# Comparing `tmp/molgenis_emx2_pyclient-8.196.0.tar.gz` & `tmp/molgenis_emx2_pyclient-8.197.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgenis_emx2_pyclient-8.196.0.tar", last modified: Thu Jun 22 08:38:06 2023, max compression
+gzip compressed data, was "molgenis_emx2_pyclient-8.197.0.tar", last modified: Thu Jun 22 10:48:18 2023, max compression
```

## Comparing `molgenis_emx2_pyclient-8.196.0.tar` & `molgenis_emx2_pyclient-8.197.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:38:06.802900 molgenis_emx2_pyclient-8.196.0/
--rw-r--r--   0 root         (0) root         (0)     7631 2023-06-22 08:31:12.000000 molgenis_emx2_pyclient-8.196.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1337 2023-06-22 08:38:06.802900 molgenis_emx2_pyclient-8.196.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      953 2023-06-22 08:31:13.000000 molgenis_emx2_pyclient-8.196.0/README.md
--rw-r--r--   0 root         (0) root         (0)      634 2023-06-22 08:31:13.000000 molgenis_emx2_pyclient-8.196.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-22 08:31:13.000000 molgenis_emx2_pyclient-8.196.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 08:38:06.802900 molgenis_emx2_pyclient-8.196.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:38:06.802900 molgenis_emx2_pyclient-8.196.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:38:06.802900 molgenis_emx2_pyclient-8.196.0/src/molgenis_emx2_client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 08:31:13.000000 molgenis_emx2_pyclient-8.196.0/src/molgenis_emx2_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2781 2023-06-22 08:31:13.000000 molgenis_emx2_pyclient-8.196.0/src/molgenis_emx2_client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:38:06.802900 molgenis_emx2_pyclient-8.196.0/src/molgenis_emx2_pyclient.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1337 2023-06-22 08:38:06.000000 molgenis_emx2_pyclient-8.196.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 08:38:06.000000 molgenis_emx2_pyclient-8.196.0/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 08:38:06.000000 molgenis_emx2_pyclient-8.196.0/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-22 08:38:06.000000 molgenis_emx2_pyclient-8.196.0/src/molgenis_emx2_pyclient.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-22 08:38:06.000000 molgenis_emx2_pyclient-8.196.0/src/molgenis_emx2_pyclient.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 08:32:30.000000 molgenis_emx2_pyclient-8.196.0/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:48:18.412006 molgenis_emx2_pyclient-8.197.0/
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-06-22 10:41:16.000000 molgenis_emx2_pyclient-8.197.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-06-22 10:48:18.412006 molgenis_emx2_pyclient-8.197.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      953 2023-06-22 10:41:16.000000 molgenis_emx2_pyclient-8.197.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      634 2023-06-22 10:41:16.000000 molgenis_emx2_pyclient-8.197.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-22 10:41:16.000000 molgenis_emx2_pyclient-8.197.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 10:48:18.412006 molgenis_emx2_pyclient-8.197.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:48:18.408007 molgenis_emx2_pyclient-8.197.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:48:18.412006 molgenis_emx2_pyclient-8.197.0/src/molgenis_emx2_client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 10:41:16.000000 molgenis_emx2_pyclient-8.197.0/src/molgenis_emx2_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-06-22 10:41:16.000000 molgenis_emx2_pyclient-8.197.0/src/molgenis_emx2_client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:48:18.412006 molgenis_emx2_pyclient-8.197.0/src/molgenis_emx2_pyclient.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-06-22 10:48:18.000000 molgenis_emx2_pyclient-8.197.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 10:48:18.000000 molgenis_emx2_pyclient-8.197.0/src/molgenis_emx2_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 10:48:18.000000 molgenis_emx2_pyclient-8.197.0/src/molgenis_emx2_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-22 10:48:18.000000 molgenis_emx2_pyclient-8.197.0/src/molgenis_emx2_pyclient.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-22 10:48:18.000000 molgenis_emx2_pyclient-8.197.0/src/molgenis_emx2_pyclient.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 10:42:39.000000 molgenis_emx2_pyclient-8.197.0/version.txt
```

### Comparing `molgenis_emx2_pyclient-8.196.0/LICENSE` & `molgenis_emx2_pyclient-8.197.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.196.0/PKG-INFO` & `molgenis_emx2_pyclient-8.197.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis_emx2_pyclient
-Version: 8.196.0
+Version: 8.197.0
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `molgenis_emx2_pyclient-8.196.0/README.md` & `molgenis_emx2_pyclient-8.197.0/README.md`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.196.0/pyproject.toml` & `molgenis_emx2_pyclient-8.197.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.196.0/src/molgenis_emx2_client/client.py` & `molgenis_emx2_pyclient-8.197.0/src/molgenis_emx2_client/client.py`

 * *Files identical despite different names*

### Comparing `molgenis_emx2_pyclient-8.196.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO` & `molgenis_emx2_pyclient-8.197.0/src/molgenis_emx2_pyclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgenis-emx2-pyclient
-Version: 8.196.0
+Version: 8.197.0
 Summary: Python client for the Molgenis EMX2 API
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

