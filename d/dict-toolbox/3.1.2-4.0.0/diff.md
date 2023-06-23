# Comparing `tmp/dict-toolbox-3.1.2.tar.gz` & `tmp/dict-toolbox-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dict-toolbox-3.1.2.tar", last modified: Fri May 26 17:20:56 2023, max compression
+gzip compressed data, was "dict-toolbox-4.0.0.tar", last modified: Fri Jun 23 16:46:59 2023, max compression
```

## Comparing `dict-toolbox-3.1.2.tar` & `dict-toolbox-4.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:20:56.420105 dict-toolbox-3.1.2/
--rw-r--r--   0 root         (0) root         (0)    19053 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6418 2023-05-26 17:20:56.420105 dict-toolbox-3.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5499 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:20:56.420105 dict-toolbox-3.1.2/dict_toolbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6418 2023-05-26 17:20:56.000000 dict-toolbox-3.1.2/dict_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      479 2023-05-26 17:20:56.000000 dict-toolbox-3.1.2/dict_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 17:20:56.000000 dict-toolbox-3.1.2/dict_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-26 17:20:56.000000 dict-toolbox-3.1.2/dict_toolbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-26 17:20:56.000000 dict-toolbox-3.1.2/dict_toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 17:20:56.420105 dict-toolbox-3.1.2/dict_tools/
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5428 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/aggregation.py
--rw-r--r--   0 root         (0) root         (0)     3297 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/args.py
--rw-r--r--   0 root         (0) root         (0)    28296 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/data.py
--rw-r--r--   0 root         (0) root         (0)    15032 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/differ.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/mysql.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/trim.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/typing.py
--rw-r--r--   0 root         (0) root         (0)     9583 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/update.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/utils.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/xml.py
--rw-r--r--   0 root         (0) root         (0)    12072 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/dict_tools/yamlex.py
--rw-r--r--   0 root         (0) root         (0)      255 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-26 17:20:56.424106 dict-toolbox-3.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2687 2023-05-26 17:20:41.000000 dict-toolbox-3.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:46:59.381895 dict-toolbox-4.0.0/
+-rw-r--r--   0 root         (0) root         (0)    19053 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6368 2023-06-23 16:46:59.381895 dict-toolbox-4.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5499 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:46:59.381895 dict-toolbox-4.0.0/dict_toolbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6368 2023-06-23 16:46:59.000000 dict-toolbox-4.0.0/dict_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-23 16:46:59.000000 dict-toolbox-4.0.0/dict_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 16:46:59.000000 dict-toolbox-4.0.0/dict_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-23 16:46:59.000000 dict-toolbox-4.0.0/dict_toolbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-23 16:46:59.000000 dict-toolbox-4.0.0/dict_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:46:59.381895 dict-toolbox-4.0.0/dict_tools/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5428 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/aggregation.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/args.py
+-rw-r--r--   0 root         (0) root         (0)    28294 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/data.py
+-rw-r--r--   0 root         (0) root         (0)    15032 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/differ.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/mysql.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/trim.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/typing.py
+-rw-r--r--   0 root         (0) root         (0)     9583 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/update.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/xml.py
+-rw-r--r--   0 root         (0) root         (0)    12071 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/dict_tools/yamlex.py
+-rw-r--r--   0 root         (0) root         (0)      265 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-23 16:46:59.381895 dict-toolbox-4.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2638 2023-06-23 16:46:44.000000 dict-toolbox-4.0.0/setup.py
```

### Comparing `dict-toolbox-3.1.2/LICENSE` & `dict-toolbox-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.2/PKG-INFO` & `dict-toolbox-4.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: dict-toolbox
-Version: 3.1.2
+Version: 4.0.0
 Summary: Dict tools for Python projects
 Home-page: https://gitlab.com/saltstack/open/dict-toolbox
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 DICT-TOOLBOX
 ============
```

### Comparing `dict-toolbox-3.1.2/README.rst` & `dict-toolbox-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.2/dict_toolbox.egg-info/PKG-INFO` & `dict-toolbox-4.0.0/dict_toolbox.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: dict-toolbox
-Version: 3.1.2
+Version: 4.0.0
 Summary: Dict tools for Python projects
 Home-page: https://gitlab.com/saltstack/open/dict-toolbox
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ============
 DICT-TOOLBOX
 ============
```

### Comparing `dict-toolbox-3.1.2/dict_tools/aggregation.py` & `dict-toolbox-4.0.0/dict_tools/aggregation.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.2/dict_tools/args.py` & `dict-toolbox-4.0.0/dict_tools/args.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.2/dict_tools/data.py` & `dict-toolbox-4.0.0/dict_tools/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,15 +445,15 @@
         append_old, append_new = [], []
         if len(old) != len(new):
             min_length = min(len(old), len(new))
             # The list coercion is required for Py3
             append_old = list(old.keys())[min_length:]
             append_new = list(new.keys())[min_length:]
         # Compare ordered
-        for (key_old, key_new) in zip(old, new):
+        for key_old, key_new in zip(old, new):
             if key_old == key_new:
                 if key_old in ignore_keys:
                     del ret_old[key_old]
                     del ret_new[key_new]
                 else:
                     res = recursive_diff(
                         old[key_old],
```

### Comparing `dict-toolbox-3.1.2/dict_tools/differ.py` & `dict-toolbox-4.0.0/dict_tools/differ.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.2/dict_tools/mysql.py` & `dict-toolbox-4.0.0/dict_tools/mysql.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.2/dict_tools/trim.py` & `dict-toolbox-4.0.0/dict_tools/trim.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.2/dict_tools/typing.py` & `dict-toolbox-4.0.0/dict_tools/typing.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.2/dict_tools/update.py` & `dict-toolbox-4.0.0/dict_tools/update.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.2/dict_tools/utils.py` & `dict-toolbox-4.0.0/dict_tools/utils.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.2/dict_tools/xml.py` & `dict-toolbox-4.0.0/dict_tools/xml.py`

 * *Files identical despite different names*

### Comparing `dict-toolbox-3.1.2/dict_tools/yamlex.py` & `dict-toolbox-4.0.0/dict_tools/yamlex.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,14 @@
                 f"expected a mapping node, but found {node.id}",
                 node.start_mark,
             )
 
         self.flatten_mapping(node)
 
         for key_node, value_node in node.value:
-
             # !reset instruction applies on document only.
             # It tells to reset previous decoded value for this present key.
             reset = key_node.tag == "!reset"
 
             # even if !aggregate tag apply only to values and not keys
             # it's a reason to act as a such nazi.
             if key_node.tag == "!aggregate":
```

### Comparing `dict-toolbox-3.1.2/setup.py` & `dict-toolbox-4.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import Command
 from setuptools import setup
 
 NAME = "dict_tools"
 DESC = "Dict tools for Python projects"
 
 # Version info -- read without importing
-VERSION = "3.1.2"
+VERSION = "4.0.0"
 
 SETUP_DIRNAME = os.path.dirname(__file__)
 if not SETUP_DIRNAME:
     SETUP_DIRNAME = os.getcwd()
 
 with open("README.rst", encoding="utf-8") as f:
     LONG_DESC = f.read()
@@ -68,23 +68,22 @@
     url="https://gitlab.com/saltstack/open/dict-toolbox",
     version=VERSION,
     install_requires=REQUIREMENTS,
     extras_require=REQUIREMENTS_EXTRA,
     description=DESC,
     long_description=LONG_DESC,
     long_description_content_type="text/x-rst",
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     classifiers=[
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Development Status :: 5 - Production/Stable",
     ],
     packages=discover_packages(),
```

