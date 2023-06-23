# Comparing `tmp/skeletonkey-0.1.1.tar.gz` & `tmp/skeletonkey-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeletonkey-0.1.1.tar", last modified: Fri Jun 23 20:08:30 2023, max compression
+gzip compressed data, was "skeletonkey-0.1.2.tar", last modified: Fri Jun 23 21:42:25 2023, max compression
```

## Comparing `skeletonkey-0.1.1.tar` & `skeletonkey-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 20:08:30.091232 skeletonkey-0.1.1/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-05-01 03:35:36.000000 skeletonkey-0.1.1/LICENSE
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-06-23 20:08:30.079231 skeletonkey-0.1.1/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     3814 2023-05-01 05:00:51.000000 skeletonkey-0.1.1/README.md
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-06-23 20:08:30.155235 skeletonkey-0.1.1/setup.cfg
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      758 2023-06-23 20:07:35.000000 skeletonkey-0.1.1/setup.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 20:08:29.827219 skeletonkey-0.1.1/skeletonkey/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      562 2023-05-01 04:36:26.000000 skeletonkey-0.1.1/skeletonkey/__init__.py
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)    10442 2023-06-23 19:57:18.000000 skeletonkey-0.1.1/skeletonkey/config.py
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4684 2023-06-23 19:41:37.000000 skeletonkey-0.1.1/skeletonkey/core.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 20:08:30.035229 skeletonkey-0.1.1/skeletonkey.egg-info/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-06-23 20:08:28.000000 skeletonkey-0.1.1/skeletonkey.egg-info/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      266 2023-06-23 20:08:28.000000 skeletonkey-0.1.1/skeletonkey.egg-info/SOURCES.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-06-23 20:08:28.000000 skeletonkey-0.1.1/skeletonkey.egg-info/dependency_links.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       14 2023-06-23 20:08:28.000000 skeletonkey-0.1.1/skeletonkey.egg-info/requires.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-06-23 20:08:28.000000 skeletonkey-0.1.1/skeletonkey.egg-info/top_level.txt
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 21:42:25.239363 skeletonkey-0.1.2/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-05-01 03:35:36.000000 skeletonkey-0.1.2/LICENSE
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-06-23 21:42:25.219362 skeletonkey-0.1.2/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     3814 2023-05-01 05:00:51.000000 skeletonkey-0.1.2/README.md
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-06-23 21:42:25.251364 skeletonkey-0.1.2/setup.cfg
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      758 2023-06-23 21:40:28.000000 skeletonkey-0.1.2/setup.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 21:42:24.711337 skeletonkey-0.1.2/skeletonkey/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      562 2023-05-01 04:36:26.000000 skeletonkey-0.1.2/skeletonkey/__init__.py
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)    10442 2023-06-23 19:57:18.000000 skeletonkey-0.1.2/skeletonkey/config.py
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4691 2023-06-23 21:37:29.000000 skeletonkey-0.1.2/skeletonkey/core.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 21:42:25.123357 skeletonkey-0.1.2/skeletonkey.egg-info/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-06-23 21:42:22.000000 skeletonkey-0.1.2/skeletonkey.egg-info/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      266 2023-06-23 21:42:23.000000 skeletonkey-0.1.2/skeletonkey.egg-info/SOURCES.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-06-23 21:42:22.000000 skeletonkey-0.1.2/skeletonkey.egg-info/dependency_links.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       14 2023-06-23 21:42:22.000000 skeletonkey-0.1.2/skeletonkey.egg-info/requires.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-06-23 21:42:22.000000 skeletonkey-0.1.2/skeletonkey.egg-info/top_level.txt
```

### Comparing `skeletonkey-0.1.1/LICENSE` & `skeletonkey-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.1/PKG-INFO` & `skeletonkey-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.1.1
+Version: 0.1.2
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `skeletonkey-0.1.1/README.md` & `skeletonkey-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.1/setup.py` & `skeletonkey-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="skeletonkey",
-    version="0.1.1",
+    version="0.1.2",
     description="A bare-bones configuration managment tool.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sizemore0125/skeletonkey",
     author="Logan Sizemore",
     author_email="sizemore0125@gmail.com",
```

### Comparing `skeletonkey-0.1.1/skeletonkey/__init__.py` & `skeletonkey-0.1.2/skeletonkey/__init__.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.1/skeletonkey/config.py` & `skeletonkey-0.1.2/skeletonkey/config.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.1/skeletonkey/core.py` & `skeletonkey-0.1.2/skeletonkey/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 
     Returns:
         Any: An instance of the specified class.
 
     Raises:
         AssertionError: If the class is missing specific parameters.
     """
-    kwargs = vars(namespace)
+    kwargs = vars(namespace).copy()
     target_keyword = "_target_"
     class_obj = import_class(kwargs[target_keyword])
     del kwargs[target_keyword]
 
     obj_parameters = list(inspect.signature(class_obj).parameters)
     valid_parameters = {k: v for k, v in kwargs.items() if k in obj_parameters}
     missing_parameters = [k for k in obj_parameters if k not in valid_parameters.keys()]
```

### Comparing `skeletonkey-0.1.1/skeletonkey.egg-info/PKG-INFO` & `skeletonkey-0.1.2/skeletonkey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.1.1
+Version: 0.1.2
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

