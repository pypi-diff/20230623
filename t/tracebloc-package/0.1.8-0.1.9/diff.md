# Comparing `tmp/tracebloc_package-0.1.8.tar.gz` & `tmp/tracebloc_package-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-0.1.8.tar", last modified: Fri Jul  8 06:49:26 2022, max compression
+gzip compressed data, was "tracebloc_package-0.1.9.tar", last modified: Fri Jul  8 07:09:10 2022, max compression
```

## Comparing `tracebloc_package-0.1.8.tar` & `tracebloc_package-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2022-07-08 06:49:26.781392 tracebloc_package-0.1.8/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-0.1.8/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      569 2022-07-08 06:49:26.781449 tracebloc_package-0.1.8/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-0.1.8/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2022-07-08 06:49:26.781643 tracebloc_package-0.1.8/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      727 2022-07-08 06:48:32.000000 tracebloc_package-0.1.8/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2022-07-08 06:49:26.780603 tracebloc_package-0.1.8/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       46 2022-05-16 08:30:43.000000 tracebloc_package-0.1.8/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)    35773 2022-06-30 10:58:44.000000 tracebloc_package-0.1.8/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2022-06-30 11:01:57.000000 tracebloc_package-0.1.8/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)     5953 2022-07-08 06:44:54.000000 tracebloc_package-0.1.8/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)     8901 2022-07-05 09:00:33.000000 tracebloc_package-0.1.8/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     3174 2022-07-05 08:41:58.000000 tracebloc_package-0.1.8/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3203 2022-06-09 05:22:24.000000 tracebloc_package-0.1.8/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2022-07-08 06:49:26.781305 tracebloc_package-0.1.8/tracebloc_package.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      569 2022-07-08 06:49:26.000000 tracebloc_package-0.1.8/tracebloc_package.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      492 2022-07-08 06:49:26.000000 tracebloc_package-0.1.8/tracebloc_package.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2022-07-08 06:49:26.000000 tracebloc_package-0.1.8/tracebloc_package.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2022-07-08 06:49:26.000000 tracebloc_package-0.1.8/tracebloc_package.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)       24 2022-07-08 06:49:26.000000 tracebloc_package-0.1.8/tracebloc_package.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2022-07-08 06:49:26.000000 tracebloc_package-0.1.8/tracebloc_package.egg-info/top_level.txt
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2022-07-08 07:09:10.514214 tracebloc_package-0.1.9/
+-rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-0.1.9/LICENSE.txt
+-rw-r--r--   0 hasan      (501) staff       (20)      569 2022-07-08 07:09:10.514277 tracebloc_package-0.1.9/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-0.1.9/README.md
+-rw-r--r--   0 hasan      (501) staff       (20)       78 2022-07-08 07:09:10.514490 tracebloc_package-0.1.9/setup.cfg
+-rw-r--r--   0 hasan      (501) staff       (20)      727 2022-07-08 07:07:49.000000 tracebloc_package-0.1.9/setup.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2022-07-08 07:09:10.513283 tracebloc_package-0.1.9/tracebloc_package/
+-rw-r--r--   0 hasan      (501) staff       (20)       46 2022-05-16 08:30:43.000000 tracebloc_package-0.1.9/tracebloc_package/__init__.py
+-rw-r--r--   0 hasan      (501) staff       (20)    35773 2022-06-30 10:58:44.000000 tracebloc_package-0.1.9/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7100 2022-06-30 11:01:57.000000 tracebloc_package-0.1.9/tracebloc_package/messages.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5953 2022-07-08 06:44:54.000000 tracebloc_package-0.1.9/tracebloc_package/upload.py
+-rw-r--r--   0 hasan      (501) staff       (20)     8928 2022-07-08 07:05:00.000000 tracebloc_package-0.1.9/tracebloc_package/user.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3174 2022-07-05 08:41:58.000000 tracebloc_package-0.1.9/tracebloc_package/utils.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3203 2022-06-09 05:22:24.000000 tracebloc_package-0.1.9/tracebloc_package/weights.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2022-07-08 07:09:10.513984 tracebloc_package-0.1.9/tracebloc_package.egg-info/
+-rw-r--r--   0 hasan      (501) staff       (20)      569 2022-07-08 07:09:10.000000 tracebloc_package-0.1.9/tracebloc_package.egg-info/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      492 2022-07-08 07:09:10.000000 tracebloc_package-0.1.9/tracebloc_package.egg-info/SOURCES.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2022-07-08 07:09:10.000000 tracebloc_package-0.1.9/tracebloc_package.egg-info/dependency_links.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2022-07-08 07:09:10.000000 tracebloc_package-0.1.9/tracebloc_package.egg-info/not-zip-safe
+-rw-r--r--   0 hasan      (501) staff       (20)       24 2022-07-08 07:09:10.000000 tracebloc_package-0.1.9/tracebloc_package.egg-info/requires.txt
+-rw-r--r--   0 hasan      (501) staff       (20)       18 2022-07-08 07:09:10.000000 tracebloc_package-0.1.9/tracebloc_package.egg-info/top_level.txt
```

### Comparing `tracebloc_package-0.1.8/LICENSE.txt` & `tracebloc_package-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.1.8/PKG-INFO` & `tracebloc_package-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc_package
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package
 Author: Tracebloc
 Author-email: lukas-wutke@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-0.1.8/setup.py` & `tracebloc_package-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package",
-    version="0.1.8",
+    version="0.1.9",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="lukas-wutke@tracebloc.io",
```

### Comparing `tracebloc_package-0.1.8/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-0.1.9/tracebloc_package/linkModelDataSet.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.1.8/tracebloc_package/messages.py` & `tracebloc_package-0.1.9/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.1.8/tracebloc_package/upload.py` & `tracebloc_package-0.1.9/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.1.8/tracebloc_package/user.py` & `tracebloc_package-0.1.9/tracebloc_package/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
     def __checkmodel(self, datasetId):
         try:
             header = {"Authorization": f"Token {self.__token}"}
             re = requests.post(
                 f"{self.__url}check-model/",
                 headers=header,
-                data={"datasetId": datasetId, "modelName": self.__modelId},
+                data={"datasetId": datasetId, "modelName": self.__modelId, "type": 'linking_dataset'},
             )
             if re.status_code == 403 or re.status_code == 400:
                 text = colored(
                     f"There is no dataset with ID: {datasetId} in your dataset table.\n"
                     f"Please check your dataset ID.",
                     "red",
                 )
```

### Comparing `tracebloc_package-0.1.8/tracebloc_package/utils.py` & `tracebloc_package-0.1.9/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.1.8/tracebloc_package/weights.py` & `tracebloc_package-0.1.9/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-0.1.8/tracebloc_package.egg-info/PKG-INFO` & `tracebloc_package-0.1.9/tracebloc_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tracebloc-package
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package
 Author: Tracebloc
 Author-email: lukas-wutke@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

