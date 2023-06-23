# Comparing `tmp/FLUID_project_upprpo-1.0.6.tar.gz` & `tmp/FLUID_project_upprpo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLUID_project_upprpo-1.0.6.tar", last modified: Fri Jun 23 16:04:43 2023, max compression
+gzip compressed data, was "FLUID_project_upprpo-1.1.0.tar", last modified: Fri Jun 23 16:08:35 2023, max compression
```

## Comparing `FLUID_project_upprpo-1.0.6.tar` & `FLUID_project_upprpo-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:43.211565 FLUID_project_upprpo-1.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:43.207565 FLUID_project_upprpo-1.0.6/FLUID_project_upprpo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-23 16:04:43.000000 FLUID_project_upprpo-1.0.6/FLUID_project_upprpo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-23 16:04:43.000000 FLUID_project_upprpo-1.0.6/FLUID_project_upprpo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:04:43.000000 FLUID_project_upprpo-1.0.6/FLUID_project_upprpo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 16:04:43.000000 FLUID_project_upprpo-1.0.6/FLUID_project_upprpo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 16:04:43.000000 FLUID_project_upprpo-1.0.6/FLUID_project_upprpo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 16:04:09.000000 FLUID_project_upprpo-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-23 16:04:43.211565 FLUID_project_upprpo-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-23 16:04:09.000000 FLUID_project_upprpo-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:04:43.211565 FLUID_project_upprpo-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-23 16:04:09.000000 FLUID_project_upprpo-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:43.207565 FLUID_project_upprpo-1.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-23 16:04:09.000000 FLUID_project_upprpo-1.0.6/src/Interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-23 16:04:09.000000 FLUID_project_upprpo-1.0.6/src/Properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:43.211565 FLUID_project_upprpo-1.0.6/src/Simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-06-23 16:04:09.000000 FLUID_project_upprpo-1.0.6/src/Simulation/Calculations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-23 16:04:09.000000 FLUID_project_upprpo-1.0.6/src/Simulation/FluidCube.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 16:04:09.000000 FLUID_project_upprpo-1.0.6/src/Simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-23 16:04:09.000000 FLUID_project_upprpo-1.0.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-23 16:04:09.000000 FLUID_project_upprpo-1.0.6/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-23 16:08:34.000000 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-23 16:08:34.000000 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:08:34.000000 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 16:08:34.000000 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 16:08:34.000000 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/Interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/Properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/src/Simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/Simulation/Calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/Simulation/FluidCube.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/Simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/__init__.py
```

### Comparing `FLUID_project_upprpo-1.0.6/FLUID_project_upprpo.egg-info/PKG-INFO` & `FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLUID-project-upprpo
-Version: 1.0.6
+Version: 1.1.0
 Home-page: https://github.com/AxeVal/Fluid
 Author: VeLoR
 Author-email: 
 Keywords: pypi,cicd,python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FLUID-project-upprpo Version: 1.0.6 Home-page:
+Metadata-Version: 2.1 Name: FLUID-project-upprpo Version: 1.1.0 Home-page:
 https://github.com/AxeVal/Fluid Author: VeLoR Author-email: Keywords:
 pypi,cicd,python Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: Microsoft :: Windows Description-Content-Type: text/
 markdown License-File: LICENSE \n
       [https://github.com/devicons/devicon/blob/master/icons/numpy/numpy-
  original.svg] [https://github.com/devicons/devicon/blob/master/icons/pycharm/
  pycharm-original.svg] [https://github.com/devicons/devicon/blob/master/icons/
```

### Comparing `FLUID_project_upprpo-1.0.6/LICENSE` & `FLUID_project_upprpo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FLUID_project_upprpo-1.0.6/PKG-INFO` & `FLUID_project_upprpo-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLUID_project_upprpo
-Version: 1.0.6
+Version: 1.1.0
 Home-page: https://github.com/AxeVal/Fluid
 Author: VeLoR
 Author-email: 
 Keywords: pypi,cicd,python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FLUID_project_upprpo Version: 1.0.6 Home-page:
+Metadata-Version: 2.1 Name: FLUID_project_upprpo Version: 1.1.0 Home-page:
 https://github.com/AxeVal/Fluid Author: VeLoR Author-email: Keywords:
 pypi,cicd,python Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: Microsoft :: Windows Description-Content-Type: text/
 markdown License-File: LICENSE \n
       [https://github.com/devicons/devicon/blob/master/icons/numpy/numpy-
  original.svg] [https://github.com/devicons/devicon/blob/master/icons/pycharm/
  pycharm-original.svg] [https://github.com/devicons/devicon/blob/master/icons/
```

### Comparing `FLUID_project_upprpo-1.0.6/README.md` & `FLUID_project_upprpo-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `FLUID_project_upprpo-1.0.6/setup.py` & `FLUID_project_upprpo-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="FLUID_project_upprpo",
-    version='1.0.6',
+    version='1.1.0',
     author="VeLoR",
     author_email="",
     description="",
     url = "https://github.com/AxeVal/Fluid",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

### Comparing `FLUID_project_upprpo-1.0.6/src/Interface.py` & `FLUID_project_upprpo-1.1.0/src/Interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 
 import pygame as pg
 import cv2
 
-from Simulation import FluidCube
-from Properties import *
+from .Simulation import FluidCube
+from .Properties import *
 
 
 def create_window():
     """
     Создает окно для визуализации симуляции жидкости.
 
     Примечания:
```

### Comparing `FLUID_project_upprpo-1.0.6/src/Properties.py` & `FLUID_project_upprpo-1.1.0/src/Properties.py`

 * *Files identical despite different names*

### Comparing `FLUID_project_upprpo-1.0.6/src/Simulation/Calculations.py` & `FLUID_project_upprpo-1.1.0/src/Simulation/Calculations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from numba import njit
 
-from Properties import *
+from ..Properties import *
 
 def IX(x: int, y: int, NN = N):
     return int(x + y * NN)
 
 @njit
 def set_bnd(b, x):
     """
```

### Comparing `FLUID_project_upprpo-1.0.6/src/Simulation/FluidCube.py` & `FLUID_project_upprpo-1.1.0/src/Simulation/FluidCube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 from .Calculations import diffuse, advect, project
-from Properties import *
+from ..Properties import *
 
 
 class FluidCube:
     def __init__(self, dt, diffusion, viscosity, NN = N):
         """
         Инициализирует объект FluidCube.
```

