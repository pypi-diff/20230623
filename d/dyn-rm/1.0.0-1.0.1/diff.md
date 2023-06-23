# Comparing `tmp/dyn_rm-1.0.0.tar.gz` & `tmp/dyn_rm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyn_rm-1.0.0.tar", last modified: Thu Jun 22 06:24:48 2023, max compression
+gzip compressed data, was "dyn_rm-1.0.1.tar", last modified: Fri Jun 23 10:32:25 2023, max compression
```

## Comparing `dyn_rm-1.0.0.tar` & `dyn_rm-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-22 06:24:48.831955 dyn_rm-1.0.0/
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-06-22 06:24:48.831955 dyn_rm-1.0.0/PKG-INFO
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     1130 2023-04-26 12:59:17.000000 dyn_rm-1.0.0/README.md
-drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-22 06:24:48.831955 dyn_rm-1.0.0/dyn_rm/
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-21 14:15:38.000000 dyn_rm-1.0.0/dyn_rm/__init__.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    22366 2023-06-22 06:10:27.000000 dyn_rm-1.0.0/dyn_rm/dynamic_resource_manager.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    36301 2023-06-21 14:24:56.000000 dyn_rm-1.0.0/dyn_rm/hpc_system.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     5326 2023-06-21 14:25:06.000000 dyn_rm-1.0.0/dyn_rm/my_pmix.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     1440 2023-06-12 12:02:26.000000 dyn_rm-1.0.0/dyn_rm/my_pmix_constants.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     2935 2023-03-10 08:52:35.000000 dyn_rm-1.0.0/dyn_rm/plotter.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      391 2023-06-21 14:39:29.000000 dyn_rm-1.0.0/dyn_rm/setup.py
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       84 2023-03-02 07:52:20.000000 dyn_rm-1.0.0/dyn_rm/util.py
-drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-22 06:24:48.831955 dyn_rm-1.0.0/dyn_rm.egg-info/
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-06-22 06:24:48.000000 dyn_rm-1.0.0/dyn_rm.egg-info/PKG-INFO
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      370 2023-06-22 06:24:48.000000 dyn_rm-1.0.0/dyn_rm.egg-info/SOURCES.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        1 2023-06-22 06:24:48.000000 dyn_rm-1.0.0/dyn_rm.egg-info/dependency_links.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       65 2023-06-22 06:24:48.000000 dyn_rm-1.0.0/dyn_rm.egg-info/entry_points.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       15 2023-06-22 06:24:48.000000 dyn_rm-1.0.0/dyn_rm.egg-info/requires.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        7 2023-06-22 06:24:48.000000 dyn_rm-1.0.0/dyn_rm.egg-info/top_level.txt
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       38 2023-06-22 06:24:48.831955 dyn_rm-1.0.0/setup.cfg
--rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      569 2023-06-22 06:01:23.000000 dyn_rm-1.0.0/setup.py
+drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-23 10:32:25.688238 dyn_rm-1.0.1/
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-06-23 10:32:25.684238 dyn_rm-1.0.1/PKG-INFO
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     3391 2023-06-22 07:27:11.000000 dyn_rm-1.0.1/README.md
+drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-23 10:32:25.684238 dyn_rm-1.0.1/dyn_rm/
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-21 14:15:38.000000 dyn_rm-1.0.1/dyn_rm/__init__.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    22366 2023-06-22 07:23:15.000000 dyn_rm-1.0.1/dyn_rm/dynamic_resource_manager.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)    36301 2023-06-21 14:24:56.000000 dyn_rm-1.0.1/dyn_rm/hpc_system.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     5326 2023-06-21 14:25:06.000000 dyn_rm-1.0.1/dyn_rm/my_pmix.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     1440 2023-06-12 12:02:26.000000 dyn_rm-1.0.1/dyn_rm/my_pmix_constants.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)     2935 2023-03-10 08:52:35.000000 dyn_rm-1.0.1/dyn_rm/plotter.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      391 2023-06-21 14:39:29.000000 dyn_rm-1.0.1/dyn_rm/setup.py
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       84 2023-03-02 07:52:20.000000 dyn_rm-1.0.1/dyn_rm/util.py
+drwxrwxr-x   0 mpiuser   (1000) mpiuser   (1000)        0 2023-06-23 10:32:25.684238 dyn_rm-1.0.1/dyn_rm.egg-info/
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      292 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/PKG-INFO
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      370 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/SOURCES.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        1 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/dependency_links.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       65 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/entry_points.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        7 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/requires.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)        7 2023-06-23 10:32:25.000000 dyn_rm-1.0.1/dyn_rm.egg-info/top_level.txt
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)       38 2023-06-23 10:32:25.688238 dyn_rm-1.0.1/setup.cfg
+-rw-rw-r--   0 mpiuser   (1000) mpiuser   (1000)      551 2023-06-23 10:31:52.000000 dyn_rm-1.0.1/setup.py
```

### Comparing `dyn_rm-1.0.0/dyn_rm/dynamic_resource_manager.py` & `dyn_rm-1.0.1/dyn_rm/dynamic_resource_manager.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.0/dyn_rm/hpc_system.py` & `dyn_rm-1.0.1/dyn_rm/hpc_system.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.0/dyn_rm/my_pmix.py` & `dyn_rm-1.0.1/dyn_rm/my_pmix.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.0/dyn_rm/my_pmix_constants.py` & `dyn_rm-1.0.1/dyn_rm/my_pmix_constants.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.0/dyn_rm/plotter.py` & `dyn_rm-1.0.1/dyn_rm/plotter.py`

 * *Files identical despite different names*

### Comparing `dyn_rm-1.0.0/setup.py` & `dyn_rm-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='dyn_rm',
-    version='1.0.0',
+    version='1.0.1',
     description='A Dynamic Resource Manager for Dyn_PRRTE, Dyn_PMIx and Dyn_OMPI',
     author='Dominik Huber',
     author_email='domi.huber@tum.de',
     url='https://gitlab.inria.fr/dynres/dyn-procs/dyn_rm',
     packages=find_packages(),
     install_requires=[
         # List any dependencies your package requires
         'pypmix', 
-        'asyncio'
     ],
     entry_points={
     	'console_scripts': [
     		'dyn_rm = dyn_rm.dynamic_resource_manager:main',
     	],
     },
 )
```

