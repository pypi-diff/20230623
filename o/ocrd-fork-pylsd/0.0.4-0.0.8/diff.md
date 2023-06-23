# Comparing `tmp/ocrd-fork-pylsd-0.0.4.tar.gz` & `tmp/ocrd-fork-pylsd-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocrd-fork-pylsd-0.0.4.tar", last modified: Thu Apr 22 08:54:32 2021, max compression
+gzip compressed data, was "ocrd-fork-pylsd-0.0.8.tar", last modified: Fri Jun 23 16:05:57 2023, max compression
```

## Comparing `ocrd-fork-pylsd-0.0.4.tar` & `ocrd-fork-pylsd-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 08:54:32.740089 ocrd-fork-pylsd-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     3649 2021-04-22 08:54:32.740089 ocrd-fork-pylsd-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2616 2021-04-22 08:54:26.000000 ocrd-fork-pylsd-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 08:54:32.740089 ocrd-fork-pylsd-0.0.4/ocrd_fork_pylsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3649 2021-04-22 08:54:31.000000 ocrd-fork-pylsd-0.0.4/ocrd_fork_pylsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      318 2021-04-22 08:54:32.000000 ocrd-fork-pylsd-0.0.4/ocrd_fork_pylsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-22 08:54:31.000000 ocrd-fork-pylsd-0.0.4/ocrd_fork_pylsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-04-22 08:54:31.000000 ocrd-fork-pylsd-0.0.4/ocrd_fork_pylsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-04-22 08:54:31.000000 ocrd-fork-pylsd-0.0.4/ocrd_fork_pylsd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 08:54:32.740089 ocrd-fork-pylsd-0.0.4/pylsd/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2021-04-22 08:54:26.000000 ocrd-fork-pylsd-0.0.4/pylsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 08:54:32.740089 ocrd-fork-pylsd-0.0.4/pylsd/bindings/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2021-04-22 08:54:26.000000 ocrd-fork-pylsd-0.0.4/pylsd/bindings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2021-04-22 08:54:26.000000 ocrd-fork-pylsd-0.0.4/pylsd/bindings/lsd_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2296 2021-04-22 08:54:26.000000 ocrd-fork-pylsd-0.0.4/pylsd/lsd.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-22 08:54:32.740089 ocrd-fork-pylsd-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      975 2021-04-22 08:54:26.000000 ocrd-fork-pylsd-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 08:54:32.736088 ocrd-fork-pylsd-0.0.4/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-22 08:54:32.740089 ocrd-fork-pylsd-0.0.4/source/src/
--rw-r--r--   0 runner    (1001) docker     (121)    77066 2021-04-22 08:54:26.000000 ocrd-fork-pylsd-0.0.4/source/src/lsd.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:57.070913 ocrd-fork-pylsd-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-23 16:05:55.000000 ocrd-fork-pylsd-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 16:05:55.000000 ocrd-fork-pylsd-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-23 16:05:57.066913 ocrd-fork-pylsd-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-23 16:05:55.000000 ocrd-fork-pylsd-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:57.066913 ocrd-fork-pylsd-0.0.8/ocrd_fork_pylsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-23 16:05:56.000000 ocrd-fork-pylsd-0.0.8/ocrd_fork_pylsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-23 16:05:57.000000 ocrd-fork-pylsd-0.0.8/ocrd_fork_pylsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:05:56.000000 ocrd-fork-pylsd-0.0.8/ocrd_fork_pylsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 16:05:56.000000 ocrd-fork-pylsd-0.0.8/ocrd_fork_pylsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 16:05:56.000000 ocrd-fork-pylsd-0.0.8/ocrd_fork_pylsd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:57.066913 ocrd-fork-pylsd-0.0.8/pylsd/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-23 16:05:55.000000 ocrd-fork-pylsd-0.0.8/pylsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:57.066913 ocrd-fork-pylsd-0.0.8/pylsd/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-23 16:05:55.000000 ocrd-fork-pylsd-0.0.8/pylsd/bindings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-23 16:05:55.000000 ocrd-fork-pylsd-0.0.8/pylsd/bindings/lsd_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-23 16:05:55.000000 ocrd-fork-pylsd-0.0.8/pylsd/lsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:05:57.070913 ocrd-fork-pylsd-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-23 16:05:55.000000 ocrd-fork-pylsd-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:57.066913 ocrd-fork-pylsd-0.0.8/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:57.066913 ocrd-fork-pylsd-0.0.8/source/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-23 16:05:55.000000 ocrd-fork-pylsd-0.0.8/source/include/lsd.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:57.066913 ocrd-fork-pylsd-0.0.8/source/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    77066 2023-06-23 16:05:55.000000 ocrd-fork-pylsd-0.0.8/source/src/lsd.cpp
```

### Comparing `ocrd-fork-pylsd-0.0.4/PKG-INFO` & `ocrd-fork-pylsd-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: ocrd-fork-pylsd
-Version: 0.0.4
+Version: 0.0.8
 Summary: pylsd is the python bindings for LSD - Line Segment Detector
-Home-page: https://github.com/kba/pylsd
+Home-page: https://github.com/OCR-D/pylsd
 Author: Gefu Tang
 Author-email: tanggefu@gmail.com
-Maintainer: bertsky,kba
-License: BSD
+Maintainer: kba
+License: AGPL
 Description: pylsd
         =============
         
+        [![Build Wheels](https://github.com/kba/pylsd/actions/workflows/wheels.yml/badge.svg?branch=pypi-fork)](https://github.com/kba/pylsd/actions/workflows/wheels.yml)
+        [![PyPI Release](https://img.shields.io/pypi/v/ocrd-fork-pylsd.svg)](https://pypi.org/project/ocrd-fork-pylsd/)
+        
         ### 1. Introduction
         
         pylsd is the python bindings for [LSD - Line Segment Detector](http://www.ipol.im/pub/art/2012/gjmr-lsd/).
         
         ### 2. Install
         
         This package uses distutils, which is the default way of installing python modules. To install in your home directory, securely run the following:
         ```
         git clone https://github.com/primetang/pylsd.git
         cd pylsd
-        [sudo] python setup.py install
+        python setup.py install
         ```
         
         Or directly through `pip` to install it:
         ```
-        [sudo] pip install pylsd
+        pip install pylsd
         ```
         
         ### 3. Usage
         
         We can use the package by using `from pylsd.lsd import lsd`, and `lines = lsd(src)` is the call format for the `lsd` function, where `src` is a Grayscale Image (`H * W` numpy.array), and the return value `lines` is the Detected Line Segment, `lines` is an `N * 5` numpy.array, each row represents a straight line, the 5-dimensional vector is:
         
         `[point1.x, point1.y, point2.x, point2.y, width]`
```

### Comparing `ocrd-fork-pylsd-0.0.4/README.md` & `ocrd-fork-pylsd-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 pylsd
 =============
 
+[![Build Wheels](https://github.com/kba/pylsd/actions/workflows/wheels.yml/badge.svg?branch=pypi-fork)](https://github.com/kba/pylsd/actions/workflows/wheels.yml)
+[![PyPI Release](https://img.shields.io/pypi/v/ocrd-fork-pylsd.svg)](https://pypi.org/project/ocrd-fork-pylsd/)
+
 ### 1. Introduction
 
 pylsd is the python bindings for [LSD - Line Segment Detector](http://www.ipol.im/pub/art/2012/gjmr-lsd/).
 
 ### 2. Install
 
 This package uses distutils, which is the default way of installing python modules. To install in your home directory, securely run the following:
 ```
 git clone https://github.com/primetang/pylsd.git
 cd pylsd
-[sudo] python setup.py install
+python setup.py install
 ```
 
 Or directly through `pip` to install it:
 ```
-[sudo] pip install pylsd
+pip install pylsd
 ```
 
 ### 3. Usage
 
 We can use the package by using `from pylsd.lsd import lsd`, and `lines = lsd(src)` is the call format for the `lsd` function, where `src` is a Grayscale Image (`H * W` numpy.array), and the return value `lines` is the Detected Line Segment, `lines` is an `N * 5` numpy.array, each row represents a straight line, the 5-dimensional vector is:
 
 `[point1.x, point1.y, point2.x, point2.y, width]`
```

### Comparing `ocrd-fork-pylsd-0.0.4/ocrd_fork_pylsd.egg-info/PKG-INFO` & `ocrd-fork-pylsd-0.0.8/ocrd_fork_pylsd.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: ocrd-fork-pylsd
-Version: 0.0.4
+Version: 0.0.8
 Summary: pylsd is the python bindings for LSD - Line Segment Detector
-Home-page: https://github.com/kba/pylsd
+Home-page: https://github.com/OCR-D/pylsd
 Author: Gefu Tang
 Author-email: tanggefu@gmail.com
-Maintainer: bertsky,kba
-License: BSD
+Maintainer: kba
+License: AGPL
 Description: pylsd
         =============
         
+        [![Build Wheels](https://github.com/kba/pylsd/actions/workflows/wheels.yml/badge.svg?branch=pypi-fork)](https://github.com/kba/pylsd/actions/workflows/wheels.yml)
+        [![PyPI Release](https://img.shields.io/pypi/v/ocrd-fork-pylsd.svg)](https://pypi.org/project/ocrd-fork-pylsd/)
+        
         ### 1. Introduction
         
         pylsd is the python bindings for [LSD - Line Segment Detector](http://www.ipol.im/pub/art/2012/gjmr-lsd/).
         
         ### 2. Install
         
         This package uses distutils, which is the default way of installing python modules. To install in your home directory, securely run the following:
         ```
         git clone https://github.com/primetang/pylsd.git
         cd pylsd
-        [sudo] python setup.py install
+        python setup.py install
         ```
         
         Or directly through `pip` to install it:
         ```
-        [sudo] pip install pylsd
+        pip install pylsd
         ```
         
         ### 3. Usage
         
         We can use the package by using `from pylsd.lsd import lsd`, and `lines = lsd(src)` is the call format for the `lsd` function, where `src` is a Grayscale Image (`H * W` numpy.array), and the return value `lines` is the Detected Line Segment, `lines` is an `N * 5` numpy.array, each row represents a straight line, the 5-dimensional vector is:
         
         `[point1.x, point1.y, point2.x, point2.y, width]`
```

### Comparing `ocrd-fork-pylsd-0.0.4/pylsd/bindings/lsd_ctypes.py` & `ocrd-fork-pylsd-0.0.8/pylsd/bindings/lsd_ctypes.py`

 * *Files identical despite different names*

### Comparing `ocrd-fork-pylsd-0.0.4/pylsd/lsd.py` & `ocrd-fork-pylsd-0.0.8/pylsd/lsd.py`

 * *Files identical despite different names*

### Comparing `ocrd-fork-pylsd-0.0.4/setup.py` & `ocrd-fork-pylsd-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# @Date    : 2019-01-08 09:32:00
-# @Author  : Gefu Tang (tanggefu@gmail.com)
-# @Link    : https://github.com/primetang/pylsd
-# @Version : 0.0.3
 
 from setuptools import setup, Extension
 
 clib = Extension('pylsd.lib',
                  sources=['source/src/lsd.cpp'],
                  include_dirs=['source/include'],
                  depends=['source/include/lsd.h'],
                  language="c++")
 
 setup(
     name='ocrd-fork-pylsd',
-    version='0.0.4',
+    version='0.0.8',
     description='pylsd is the python bindings for LSD - Line Segment Detector',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Gefu Tang',
     author_email='tanggefu@gmail.com',
-    maintainer='bertsky,kba',
-    license='BSD',
+    maintainer='kba',
+    license='AGPL',
     keywords=["LSD", 'line segmentation'],
-    url='https://github.com/kba/pylsd',
+    url='https://github.com/OCR-D/pylsd',
     packages=['pylsd', 'pylsd.bindings'],
     install_requires=['numpy'],
     ext_modules=[clib],
 )
```

### Comparing `ocrd-fork-pylsd-0.0.4/source/src/lsd.cpp` & `ocrd-fork-pylsd-0.0.8/source/src/lsd.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1435,15 +1435,15 @@
     that gives:
 
       lambda1 = ( Ixx + Iyy + sqrt( (Ixx-Iyy)^2 + 4.0*Ixy*Ixy) ) / 2
 
       lambda2 = ( Ixx + Iyy - sqrt( (Ixx-Iyy)^2 + 4.0*Ixy*Ixy) ) / 2
 
     To get the line segment direction we want to get the angle the
-    eigenvector assotiated to the smaller eigenvalue. We have to solve
+    eigenvector associated to the smaller eigenvalue. We have to solve
     a,b in:
 
       a.Ixx + b.Ixy = a.lambda2
 
       a.Ixy + b.Iyy = b.lambda2
 
     We want the angle theta = atan(b/a). It can be computed with
```

