# Comparing `tmp/wozoxutils-0.2.5.tar.gz` & `tmp/wozoxutils-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wozoxutils-0.2.5.tar", last modified: Sun May 14 09:17:32 2023, max compression
+gzip compressed data, was "wozoxutils-0.2.6.tar", last modified: Fri Jun 23 00:00:31 2023, max compression
```

## Comparing `wozoxutils-0.2.5.tar` & `wozoxutils-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:17:32.915646 wozoxutils-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 09:17:32.915646 wozoxutils-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 09:17:32.915646 wozoxutils-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:17:32.911646 wozoxutils-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/tests/test_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:17:32.915646 wozoxutils-0.2.5/wozoxutils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/wozoxutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/wozoxutils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/wozoxutils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/wozoxutils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-14 09:17:15.000000 wozoxutils-0.2.5/wozoxutils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:17:32.915646 wozoxutils-0.2.5/wozoxutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 09:17:32.000000 wozoxutils-0.2.5/wozoxutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-14 09:17:32.000000 wozoxutils-0.2.5/wozoxutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:17:32.000000 wozoxutils-0.2.5/wozoxutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 09:17:32.000000 wozoxutils-0.2.5/wozoxutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 09:17:32.000000 wozoxutils-0.2.5/wozoxutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:00:31.227660 wozoxutils-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-23 00:00:31.227660 wozoxutils-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 00:00:31.227660 wozoxutils-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:00:31.227660 wozoxutils-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:00:31.227660 wozoxutils-0.2.6/wozoxutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/wozoxutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/wozoxutils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/wozoxutils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/wozoxutils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-23 00:00:20.000000 wozoxutils-0.2.6/wozoxutils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:00:31.227660 wozoxutils-0.2.6/wozoxutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-23 00:00:31.000000 wozoxutils-0.2.6/wozoxutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-23 00:00:31.000000 wozoxutils-0.2.6/wozoxutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 00:00:31.000000 wozoxutils-0.2.6/wozoxutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 00:00:31.000000 wozoxutils-0.2.6/wozoxutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 00:00:31.000000 wozoxutils-0.2.6/wozoxutils.egg-info/top_level.txt
```

### Comparing `wozoxutils-0.2.5/LICENSE` & `wozoxutils-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.5/PKG-INFO` & `wozoxutils-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wozoxutils
-Version: 0.2.5
+Version: 0.2.6
 Summary: general-purpose library for Python that contains various commonly used functional modules
 Home-page: https://github.com/wozox/wozoxutils-py
 Author: illiten
 Author-email: admin@leelib.com
 Keywords: wozox utils
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `wozoxutils-0.2.5/README.md` & `wozoxutils-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.5/setup.py` & `wozoxutils-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name="wozoxutils",
-    version="0.2.5",
+    version="0.2.6",
     packages=find_packages(),
     install_requires=[
         'pyyaml>=6.0',
     ],
     author="illiten",
     author_email="admin@leelib.com",
     description="general-purpose library for Python that contains various commonly used functional modules",
```

### Comparing `wozoxutils-0.2.5/wozoxutils/file.py` & `wozoxutils-0.2.6/wozoxutils/file.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """
     Ensure that the directory of the given path exists.
 
     :param path: Path to a file or directory.
     """
     if not os.path.isdir(path):
         path = os.path.dirname(path)
-    if not os.path.exists(path):
+    if path != '' and not os.path.exists(path):
         os.makedirs(path)
 
 
 def save_text(filename: str, content: str):
     """
     Save text to file. If the directory does not exist, it will be created.
```

### Comparing `wozoxutils-0.2.5/wozoxutils/hash.py` & `wozoxutils-0.2.6/wozoxutils/hash.py`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.5/wozoxutils/json.py` & `wozoxutils-0.2.6/wozoxutils/json.py`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.5/wozoxutils/yaml.py` & `wozoxutils-0.2.6/wozoxutils/yaml.py`

 * *Files identical despite different names*

### Comparing `wozoxutils-0.2.5/wozoxutils.egg-info/PKG-INFO` & `wozoxutils-0.2.6/wozoxutils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wozoxutils
-Version: 0.2.5
+Version: 0.2.6
 Summary: general-purpose library for Python that contains various commonly used functional modules
 Home-page: https://github.com/wozox/wozoxutils-py
 Author: illiten
 Author-email: admin@leelib.com
 Keywords: wozox utils
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

