# Comparing `tmp/renalsegmentor-1.3.6.tar.gz` & `tmp/renalsegmentor-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renalsegmentor-1.3.6.tar", last modified: Thu Feb 16 18:17:30 2023, max compression
+gzip compressed data, was "renalsegmentor-1.3.7.tar", last modified: Fri Jun 23 11:22:00 2023, max compression
```

## Comparing `renalsegmentor-1.3.6.tar` & `renalsegmentor-1.3.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:17:30.003758 renalsegmentor-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-02-16 18:17:30.003758 renalsegmentor-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:17:29.991758 renalsegmentor-1.3.6/renalsegmentor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-02-16 18:17:29.000000 renalsegmentor-1.3.6/renalsegmentor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-16 18:17:29.000000 renalsegmentor-1.3.6/renalsegmentor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 18:17:29.000000 renalsegmentor-1.3.6/renalsegmentor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-16 18:17:29.000000 renalsegmentor-1.3.6/renalsegmentor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-16 18:17:29.000000 renalsegmentor-1.3.6/renalsegmentor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:17:29.991758 renalsegmentor-1.3.6/segment/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:17:29.991758 renalsegmentor-1.3.6/segment/data/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:17:30.003758 renalsegmentor-1.3.6/segment/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_01.PAR
--rw-r--r--   0 runner    (1001) docker     (123)  1497600 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_01.REC
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_01.hdr
--rw-r--r--   0 runner    (1001) docker     (123)  1497600 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_01.img
--rw-r--r--   0 runner    (1001) docker     (123)  1497952 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_01.nii
--rw-r--r--   0 runner    (1001) docker     (123)  1106508 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_01.nii.gz
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_02.PAR
--rw-r--r--   0 runner    (1001) docker     (123)  2228224 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_02.REC
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_02.hdr
--rw-r--r--   0 runner    (1001) docker     (123)  2228224 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_02.img
--rw-r--r--   0 runner    (1001) docker     (123)  2228576 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_02.nii
--rw-r--r--   0 runner    (1001) docker     (123)  1331514 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/test_data/test_sub_02.nii.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:17:30.003758 renalsegmentor-1.3.6/segment/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/data/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 18:17:30.003758 renalsegmentor-1.3.6/segment/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/tests/test_tkv.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/segment/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 18:17:30.003758 renalsegmentor-1.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-16 18:16:57.000000 renalsegmentor-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:22:00.627787 renalsegmentor-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-23 11:22:00.627787 renalsegmentor-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:22:00.611787 renalsegmentor-1.3.7/renalsegmentor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-23 11:22:00.000000 renalsegmentor-1.3.7/renalsegmentor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-23 11:22:00.000000 renalsegmentor-1.3.7/renalsegmentor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:22:00.000000 renalsegmentor-1.3.7/renalsegmentor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-23 11:22:00.000000 renalsegmentor-1.3.7/renalsegmentor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 11:22:00.000000 renalsegmentor-1.3.7/renalsegmentor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:22:00.611787 renalsegmentor-1.3.7/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:22:00.611787 renalsegmentor-1.3.7/segment/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:22:00.623787 renalsegmentor-1.3.7/segment/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_01.PAR
+-rw-r--r--   0 runner    (1001) docker     (123)  1497600 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_01.REC
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_01.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)  1497600 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_01.img
+-rw-r--r--   0 runner    (1001) docker     (123)  1497952 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_01.nii
+-rw-r--r--   0 runner    (1001) docker     (123)  1106508 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_01.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_02.PAR
+-rw-r--r--   0 runner    (1001) docker     (123)  2228224 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_02.REC
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_02.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)  2228224 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_02.img
+-rw-r--r--   0 runner    (1001) docker     (123)  2228576 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_02.nii
+-rw-r--r--   0 runner    (1001) docker     (123)  1331514 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/test_data/test_sub_02.nii.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:22:00.627787 renalsegmentor-1.3.7/segment/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/data/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:22:00.627787 renalsegmentor-1.3.7/segment/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/tests/test_tkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/segment/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 11:22:00.627787 renalsegmentor-1.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-23 11:21:17.000000 renalsegmentor-1.3.7/setup.py
```

### Comparing `renalsegmentor-1.3.6/LICENSE.txt` & `renalsegmentor-1.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/PKG-INFO` & `renalsegmentor-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renalsegmentor
-Version: 1.3.6
+Version: 1.3.7
 Summary: Segment kidneys from MRI data
 Home-page: https://github.com/alexdaniel654/Renal_Segmentor
 License: GPL-3.0
 Description: # Renal Segmentor
         [![Python CI](https://github.com/alexdaniel654/Renal_Segmentor/actions/workflows/python_ci.yml/badge.svg?branch=master)](https://github.com/alexdaniel654/Renal_Segmentor/actions/workflows/python_ci.yml)
         [![codecov](https://codecov.io/gh/alexdaniel654/Renal_Segmentor/branch/master/graph/badge.svg?token=6oSiDfrFpJ)](https://codecov.io/gh/alexdaniel654/Renal_Segmentor)
         [![Downloads](https://static.pepy.tech/badge/renalsegmentor)](https://pepy.tech/project/renalsegmentor)
```

### Comparing `renalsegmentor-1.3.6/README.md` & `renalsegmentor-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/renalsegmentor.egg-info/PKG-INFO` & `renalsegmentor-1.3.7/renalsegmentor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renalsegmentor
-Version: 1.3.6
+Version: 1.3.7
 Summary: Segment kidneys from MRI data
 Home-page: https://github.com/alexdaniel654/Renal_Segmentor
 License: GPL-3.0
 Description: # Renal Segmentor
         [![Python CI](https://github.com/alexdaniel654/Renal_Segmentor/actions/workflows/python_ci.yml/badge.svg?branch=master)](https://github.com/alexdaniel654/Renal_Segmentor/actions/workflows/python_ci.yml)
         [![codecov](https://codecov.io/gh/alexdaniel654/Renal_Segmentor/branch/master/graph/badge.svg?token=6oSiDfrFpJ)](https://codecov.io/gh/alexdaniel654/Renal_Segmentor)
         [![Downloads](https://static.pepy.tech/badge/renalsegmentor)](https://pepy.tech/project/renalsegmentor)
```

### Comparing `renalsegmentor-1.3.6/renalsegmentor.egg-info/SOURCES.txt` & `renalsegmentor-1.3.7/renalsegmentor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/fetch.py` & `renalsegmentor-1.3.7/segment/data/fetch.py`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/test_data/test_sub_01.PAR` & `renalsegmentor-1.3.7/segment/data/test_data/test_sub_01.PAR`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/test_data/test_sub_01.REC` & `renalsegmentor-1.3.7/segment/data/test_data/test_sub_01.REC`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/test_data/test_sub_01.img` & `renalsegmentor-1.3.7/segment/data/test_data/test_sub_01.img`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/test_data/test_sub_01.nii` & `renalsegmentor-1.3.7/segment/data/test_data/test_sub_01.nii`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/test_data/test_sub_01.nii.gz` & `renalsegmentor-1.3.7/segment/data/test_data/test_sub_01.nii.gz`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/test_data/test_sub_02.PAR` & `renalsegmentor-1.3.7/segment/data/test_data/test_sub_02.PAR`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/test_data/test_sub_02.REC` & `renalsegmentor-1.3.7/segment/data/test_data/test_sub_02.REC`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/test_data/test_sub_02.img` & `renalsegmentor-1.3.7/segment/data/test_data/test_sub_02.img`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/test_data/test_sub_02.nii` & `renalsegmentor-1.3.7/segment/data/test_data/test_sub_02.nii`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/test_data/test_sub_02.nii.gz` & `renalsegmentor-1.3.7/segment/data/test_data/test_sub_02.nii.gz`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/data/tests/test_fetch.py` & `renalsegmentor-1.3.7/segment/data/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/segment.py` & `renalsegmentor-1.3.7/segment/segment.py`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/segment/tests/test_tkv.py` & `renalsegmentor-1.3.7/segment/tests/test_tkv.py`

 * *Files identical despite different names*

### Comparing `renalsegmentor-1.3.6/setup.py` & `renalsegmentor-1.3.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     requirements_gui = f.read().splitlines()
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="renalsegmentor",
-    version="1.3.6",
+    version="1.3.7",
     description="Segment kidneys from MRI data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alexdaniel654/Renal_Segmentor",
     license="GPL-3.0",
 
     python_requires='>=3.8, <4',
```

