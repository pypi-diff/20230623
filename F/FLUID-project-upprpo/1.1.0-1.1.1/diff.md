# Comparing `tmp/FLUID_project_upprpo-1.1.0.tar.gz` & `tmp/FLUID_project_upprpo-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLUID_project_upprpo-1.1.0.tar", last modified: Fri Jun 23 16:08:35 2023, max compression
+gzip compressed data, was "FLUID_project_upprpo-1.1.1.tar", last modified: Fri Jun 23 16:40:55 2023, max compression
```

## Comparing `FLUID_project_upprpo-1.1.0.tar` & `FLUID_project_upprpo-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-23 16:08:34.000000 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-23 16:08:34.000000 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:08:34.000000 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 16:08:34.000000 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 16:08:34.000000 FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/Interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/Properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:08:34.999646 FLUID_project_upprpo-1.1.0/src/Simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/Simulation/Calculations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/Simulation/FluidCube.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/Simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-23 16:07:56.000000 FLUID_project_upprpo-1.1.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:40:55.856069 FLUID_project_upprpo-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:40:55.856069 FLUID_project_upprpo-1.1.1/FLUID_project_upprpo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-23 16:40:55.000000 FLUID_project_upprpo-1.1.1/FLUID_project_upprpo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 16:40:55.000000 FLUID_project_upprpo-1.1.1/FLUID_project_upprpo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:40:55.000000 FLUID_project_upprpo-1.1.1/FLUID_project_upprpo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 16:40:55.000000 FLUID_project_upprpo-1.1.1/FLUID_project_upprpo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 16:40:55.000000 FLUID_project_upprpo-1.1.1/FLUID_project_upprpo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 16:40:24.000000 FLUID_project_upprpo-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-23 16:40:55.856069 FLUID_project_upprpo-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-23 16:40:24.000000 FLUID_project_upprpo-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:40:55.856069 FLUID_project_upprpo-1.1.1/fluid_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-23 16:40:24.000000 FLUID_project_upprpo-1.1.1/fluid_simulation/Interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-23 16:40:24.000000 FLUID_project_upprpo-1.1.1/fluid_simulation/Properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:40:55.856069 FLUID_project_upprpo-1.1.1/fluid_simulation/Simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-23 16:40:24.000000 FLUID_project_upprpo-1.1.1/fluid_simulation/Simulation/Calculations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-23 16:40:24.000000 FLUID_project_upprpo-1.1.1/fluid_simulation/Simulation/FluidCube.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 16:40:24.000000 FLUID_project_upprpo-1.1.1/fluid_simulation/Simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-23 16:40:24.000000 FLUID_project_upprpo-1.1.1/fluid_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:40:55.856069 FLUID_project_upprpo-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-23 16:40:24.000000 FLUID_project_upprpo-1.1.1/setup.py
```

### Comparing `FLUID_project_upprpo-1.1.0/FLUID_project_upprpo.egg-info/PKG-INFO` & `FLUID_project_upprpo-1.1.1/FLUID_project_upprpo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLUID-project-upprpo
-Version: 1.1.0
+Version: 1.1.1
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
-Metadata-Version: 2.1 Name: FLUID-project-upprpo Version: 1.1.0 Home-page:
+Metadata-Version: 2.1 Name: FLUID-project-upprpo Version: 1.1.1 Home-page:
 https://github.com/AxeVal/Fluid Author: VeLoR Author-email: Keywords:
 pypi,cicd,python Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: Microsoft :: Windows Description-Content-Type: text/
 markdown License-File: LICENSE \n
       [https://github.com/devicons/devicon/blob/master/icons/numpy/numpy-
  original.svg] [https://github.com/devicons/devicon/blob/master/icons/pycharm/
  pycharm-original.svg] [https://github.com/devicons/devicon/blob/master/icons/
```

### Comparing `FLUID_project_upprpo-1.1.0/LICENSE` & `FLUID_project_upprpo-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FLUID_project_upprpo-1.1.0/PKG-INFO` & `FLUID_project_upprpo-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLUID_project_upprpo
-Version: 1.1.0
+Version: 1.1.1
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
-Metadata-Version: 2.1 Name: FLUID_project_upprpo Version: 1.1.0 Home-page:
+Metadata-Version: 2.1 Name: FLUID_project_upprpo Version: 1.1.1 Home-page:
 https://github.com/AxeVal/Fluid Author: VeLoR Author-email: Keywords:
 pypi,cicd,python Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: Microsoft :: Windows Description-Content-Type: text/
 markdown License-File: LICENSE \n
       [https://github.com/devicons/devicon/blob/master/icons/numpy/numpy-
  original.svg] [https://github.com/devicons/devicon/blob/master/icons/pycharm/
  pycharm-original.svg] [https://github.com/devicons/devicon/blob/master/icons/
```

### Comparing `FLUID_project_upprpo-1.1.0/README.md` & `FLUID_project_upprpo-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `FLUID_project_upprpo-1.1.0/setup.py` & `FLUID_project_upprpo-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="FLUID_project_upprpo",
-    version='1.1.0',
+    version='1.1.1',
     author="VeLoR",
     author_email="",
     description="",
     url = "https://github.com/AxeVal/Fluid",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

### Comparing `FLUID_project_upprpo-1.1.0/src/Interface.py` & `FLUID_project_upprpo-1.1.1/fluid_simulation/Interface.py`

 * *Files identical despite different names*

### Comparing `FLUID_project_upprpo-1.1.0/src/Properties.py` & `FLUID_project_upprpo-1.1.1/fluid_simulation/Properties.py`

 * *Files identical despite different names*

### Comparing `FLUID_project_upprpo-1.1.0/src/Simulation/Calculations.py` & `FLUID_project_upprpo-1.1.1/fluid_simulation/Simulation/Calculations.py`

 * *Files identical despite different names*

### Comparing `FLUID_project_upprpo-1.1.0/src/Simulation/FluidCube.py` & `FLUID_project_upprpo-1.1.1/fluid_simulation/Simulation/FluidCube.py`

 * *Files identical despite different names*

