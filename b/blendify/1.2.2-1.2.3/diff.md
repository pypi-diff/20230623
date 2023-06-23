# Comparing `tmp/blendify-1.2.2.tar.gz` & `tmp/blendify-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/blendify-1.2.2.tar", last modified: Sat May 13 14:03:22 2023, max compression
+gzip compressed data, was "dist/blendify-1.2.3.tar", last modified: Fri Jun 23 16:40:42 2023, max compression
```

## Comparing `blendify-1.2.2.tar` & `blendify-1.2.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-05-13 14:03:22.000000 blendify-1.2.2/
--rw-r--r--   0 vguzov     (502) staff       (20)     5888 2023-05-13 14:03:22.000000 blendify-1.2.2/PKG-INFO
--rw-r--r--   0 vguzov     (502) staff       (20)     5528 2023-05-13 13:57:46.000000 blendify-1.2.2/README.md
-drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-05-13 14:03:22.000000 blendify-1.2.2/blendify/
--rw-r--r--   0 vguzov     (502) staff       (20)      302 2023-05-13 13:59:05.000000 blendify-1.2.2/blendify/__init__.py
-drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-05-13 14:03:22.000000 blendify-1.2.2/blendify/cameras/
--rw-r--r--   0 vguzov     (502) staff       (20)       58 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/cameras/__init__.py
--rw-r--r--   0 vguzov     (502) staff       (20)     3071 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/cameras/base.py
--rw-r--r--   0 vguzov     (502) staff       (20)     5470 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/cameras/common.py
-drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-05-13 14:03:22.000000 blendify-1.2.2/blendify/colors/
--rw-r--r--   0 vguzov     (502) staff       (20)      121 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/colors/__init__.py
--rw-r--r--   0 vguzov     (502) staff       (20)      718 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/colors/base.py
--rw-r--r--   0 vguzov     (502) staff       (20)     2604 2023-05-03 18:18:43.000000 blendify-1.2.2/blendify/colors/common.py
--rw-r--r--   0 vguzov     (502) staff       (20)     3838 2023-04-24 18:05:40.000000 blendify-1.2.2/blendify/colors/texture.py
-drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-05-13 14:03:22.000000 blendify-1.2.2/blendify/internal/
--rw-r--r--   0 vguzov     (502) staff       (20)       32 2021-12-06 17:55:11.000000 blendify-1.2.2/blendify/internal/__init__.py
--rw-r--r--   0 vguzov     (502) staff       (20)     1886 2023-05-01 16:57:41.000000 blendify-1.2.2/blendify/internal/io.py
--rw-r--r--   0 vguzov     (502) staff       (20)     3925 2023-04-24 18:05:40.000000 blendify-1.2.2/blendify/internal/parser.py
--rw-r--r--   0 vguzov     (502) staff       (20)     3068 2023-05-01 15:22:56.000000 blendify-1.2.2/blendify/internal/positionable.py
--rw-r--r--   0 vguzov     (502) staff       (20)      575 2022-03-31 07:59:42.000000 blendify-1.2.2/blendify/internal/singleton.py
--rw-r--r--   0 vguzov     (502) staff       (20)     2434 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/internal/texture.py
--rw-r--r--   0 vguzov     (502) staff       (20)      395 2022-03-28 15:22:56.000000 blendify-1.2.2/blendify/internal/types.py
-drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-05-13 14:03:22.000000 blendify-1.2.2/blendify/lights/
--rw-r--r--   0 vguzov     (502) staff       (20)      190 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/lights/__init__.py
--rw-r--r--   0 vguzov     (502) staff       (20)     6083 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/lights/area.py
--rw-r--r--   0 vguzov     (502) staff       (20)     2112 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/lights/base.py
--rw-r--r--   0 vguzov     (502) staff       (20)    10174 2023-05-01 19:24:08.000000 blendify-1.2.2/blendify/lights/collection.py
--rw-r--r--   0 vguzov     (502) staff       (20)     5412 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/lights/common.py
-drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-05-13 14:03:22.000000 blendify-1.2.2/blendify/materials/
--rw-r--r--   0 vguzov     (502) staff       (20)       87 2023-05-13 14:00:45.000000 blendify-1.2.2/blendify/materials/__init__.py
--rw-r--r--   0 vguzov     (502) staff       (20)      665 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/materials/base.py
--rw-r--r--   0 vguzov     (502) staff       (20)     4938 2023-05-13 13:57:58.000000 blendify-1.2.2/blendify/materials/common.py
-drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-05-13 14:03:22.000000 blendify-1.2.2/blendify/renderables/
--rw-r--r--   0 vguzov     (502) staff       (20)      249 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/renderables/__init__.py
--rw-r--r--   0 vguzov     (502) staff       (20)     9851 2023-05-03 16:18:59.000000 blendify-1.2.2/blendify/renderables/base.py
--rw-r--r--   0 vguzov     (502) staff       (20)    14942 2023-05-03 15:27:36.000000 blendify-1.2.2/blendify/renderables/collection.py
--rw-r--r--   0 vguzov     (502) staff       (20)     5355 2023-05-03 18:18:39.000000 blendify-1.2.2/blendify/renderables/mesh.py
--rw-r--r--   0 vguzov     (502) staff       (20)    24366 2023-05-01 16:03:16.000000 blendify-1.2.2/blendify/renderables/pointcloud.py
--rw-r--r--   0 vguzov     (502) staff       (20)    14788 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/renderables/primitives.py
--rw-r--r--   0 vguzov     (502) staff       (20)    21860 2023-05-10 11:14:58.000000 blendify-1.2.2/blendify/scene.py
-drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-05-13 14:03:22.000000 blendify-1.2.2/blendify/utils/
--rw-r--r--   0 vguzov     (502) staff       (20)        0 2021-12-06 13:26:58.000000 blendify-1.2.2/blendify/utils/__init__.py
--rw-r--r--   0 vguzov     (502) staff       (20)     4899 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/utils/camera_trajectory.py
--rw-r--r--   0 vguzov     (502) staff       (20)      870 2022-03-31 07:59:42.000000 blendify-1.2.2/blendify/utils/image.py
--rw-r--r--   0 vguzov     (502) staff       (20)     4767 2023-04-24 17:47:43.000000 blendify-1.2.2/blendify/utils/pointcloud.py
--rw-r--r--   0 vguzov     (502) staff       (20)     1127 2023-04-24 18:05:40.000000 blendify-1.2.2/blendify/utils/shadow_catcher.py
--rw-r--r--   0 vguzov     (502) staff       (20)     2543 2023-04-24 18:05:40.000000 blendify-1.2.2/blendify/utils/smpl_wrapper.py
-drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-05-13 14:03:22.000000 blendify-1.2.2/blendify.egg-info/
--rw-r--r--   0 vguzov     (502) staff       (20)     5888 2023-05-13 14:03:21.000000 blendify-1.2.2/blendify.egg-info/PKG-INFO
--rw-r--r--   0 vguzov     (502) staff       (20)     1200 2023-05-13 14:03:21.000000 blendify-1.2.2/blendify.egg-info/SOURCES.txt
--rw-r--r--   0 vguzov     (502) staff       (20)        1 2023-05-13 14:03:21.000000 blendify-1.2.2/blendify.egg-info/dependency_links.txt
--rw-r--r--   0 vguzov     (502) staff       (20)      273 2023-05-13 14:03:21.000000 blendify-1.2.2/blendify.egg-info/requires.txt
--rw-r--r--   0 vguzov     (502) staff       (20)        9 2023-05-13 14:03:21.000000 blendify-1.2.2/blendify.egg-info/top_level.txt
--rw-r--r--   0 vguzov     (502) staff       (20)       38 2023-05-13 14:03:22.000000 blendify-1.2.2/setup.cfg
--rw-r--r--   0 vguzov     (502) staff       (20)     2214 2023-05-13 13:58:44.000000 blendify-1.2.2/setup.py
+drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-06-23 16:40:42.000000 blendify-1.2.3/
+-rw-r--r--   0 vguzov     (502) staff       (20)     5888 2023-06-23 16:40:42.000000 blendify-1.2.3/PKG-INFO
+-rw-r--r--   0 vguzov     (502) staff       (20)     5528 2023-05-13 13:57:46.000000 blendify-1.2.3/README.md
+drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify/
+-rw-r--r--   0 vguzov     (502) staff       (20)      302 2023-06-23 16:27:21.000000 blendify-1.2.3/blendify/__init__.py
+drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify/cameras/
+-rw-r--r--   0 vguzov     (502) staff       (20)       58 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/cameras/__init__.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     3071 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/cameras/base.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     5470 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/cameras/common.py
+drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify/colors/
+-rw-r--r--   0 vguzov     (502) staff       (20)      121 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/colors/__init__.py
+-rw-r--r--   0 vguzov     (502) staff       (20)      718 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/colors/base.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     2604 2023-05-03 18:18:43.000000 blendify-1.2.3/blendify/colors/common.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     3838 2023-04-24 18:05:40.000000 blendify-1.2.3/blendify/colors/texture.py
+drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify/internal/
+-rw-r--r--   0 vguzov     (502) staff       (20)       32 2021-12-06 17:55:11.000000 blendify-1.2.3/blendify/internal/__init__.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     2115 2023-06-23 16:16:52.000000 blendify-1.2.3/blendify/internal/io.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     3925 2023-04-24 18:05:40.000000 blendify-1.2.3/blendify/internal/parser.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     3068 2023-05-01 15:22:56.000000 blendify-1.2.3/blendify/internal/positionable.py
+-rw-r--r--   0 vguzov     (502) staff       (20)      575 2022-03-31 07:59:42.000000 blendify-1.2.3/blendify/internal/singleton.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     2434 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/internal/texture.py
+-rw-r--r--   0 vguzov     (502) staff       (20)      395 2022-03-28 15:22:56.000000 blendify-1.2.3/blendify/internal/types.py
+drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify/lights/
+-rw-r--r--   0 vguzov     (502) staff       (20)      190 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/lights/__init__.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     6083 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/lights/area.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     2112 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/lights/base.py
+-rw-r--r--   0 vguzov     (502) staff       (20)    10174 2023-05-01 19:24:08.000000 blendify-1.2.3/blendify/lights/collection.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     5412 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/lights/common.py
+drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify/materials/
+-rw-r--r--   0 vguzov     (502) staff       (20)       87 2023-05-13 14:00:45.000000 blendify-1.2.3/blendify/materials/__init__.py
+-rw-r--r--   0 vguzov     (502) staff       (20)      665 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/materials/base.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     4938 2023-05-13 13:57:58.000000 blendify-1.2.3/blendify/materials/common.py
+drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify/renderables/
+-rw-r--r--   0 vguzov     (502) staff       (20)      249 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/renderables/__init__.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     9851 2023-05-03 16:18:59.000000 blendify-1.2.3/blendify/renderables/base.py
+-rw-r--r--   0 vguzov     (502) staff       (20)    14942 2023-05-03 15:27:36.000000 blendify-1.2.3/blendify/renderables/collection.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     5355 2023-05-03 18:18:39.000000 blendify-1.2.3/blendify/renderables/mesh.py
+-rw-r--r--   0 vguzov     (502) staff       (20)    24366 2023-05-01 16:03:16.000000 blendify-1.2.3/blendify/renderables/pointcloud.py
+-rw-r--r--   0 vguzov     (502) staff       (20)    14788 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/renderables/primitives.py
+-rw-r--r--   0 vguzov     (502) staff       (20)    21860 2023-06-23 16:12:00.000000 blendify-1.2.3/blendify/scene.py
+drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify/utils/
+-rw-r--r--   0 vguzov     (502) staff       (20)        0 2021-12-06 13:26:58.000000 blendify-1.2.3/blendify/utils/__init__.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     4899 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/utils/camera_trajectory.py
+-rw-r--r--   0 vguzov     (502) staff       (20)      870 2022-03-31 07:59:42.000000 blendify-1.2.3/blendify/utils/image.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     4767 2023-04-24 17:47:43.000000 blendify-1.2.3/blendify/utils/pointcloud.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     1127 2023-04-24 18:05:40.000000 blendify-1.2.3/blendify/utils/shadow_catcher.py
+-rw-r--r--   0 vguzov     (502) staff       (20)     2543 2023-04-24 18:05:40.000000 blendify-1.2.3/blendify/utils/smpl_wrapper.py
+drwxr-xr-x   0 vguzov     (502) staff       (20)        0 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify.egg-info/
+-rw-r--r--   0 vguzov     (502) staff       (20)     5888 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify.egg-info/PKG-INFO
+-rw-r--r--   0 vguzov     (502) staff       (20)     1200 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify.egg-info/SOURCES.txt
+-rw-r--r--   0 vguzov     (502) staff       (20)        1 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify.egg-info/dependency_links.txt
+-rw-r--r--   0 vguzov     (502) staff       (20)      273 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify.egg-info/requires.txt
+-rw-r--r--   0 vguzov     (502) staff       (20)        9 2023-06-23 16:40:42.000000 blendify-1.2.3/blendify.egg-info/top_level.txt
+-rw-r--r--   0 vguzov     (502) staff       (20)       38 2023-06-23 16:40:42.000000 blendify-1.2.3/setup.cfg
+-rw-r--r--   0 vguzov     (502) staff       (20)     2214 2023-06-23 16:27:21.000000 blendify-1.2.3/setup.py
```

### Comparing `blendify-1.2.2/PKG-INFO` & `blendify-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendify
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python rendering framework for Blender
 Home-page: https://github.com/ptrvilya/blendify
 Author: Vladimir Guzov, Ilya Petrov
 Author-email: vguzov@mpi-inf.mpg.de, i.petrov@uni-tuebingen.de
 License: UNKNOWN
 Description: ![blendify Logo](https://github.com/ptrvilya/blendify/blob/main/.github/blendify_logo_light_bg.png?raw=true)
```

### Comparing `blendify-1.2.2/README.md` & `blendify-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/cameras/base.py` & `blendify-1.2.3/blendify/cameras/base.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/cameras/common.py` & `blendify-1.2.3/blendify/cameras/common.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/colors/base.py` & `blendify-1.2.3/blendify/colors/base.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/colors/common.py` & `blendify-1.2.3/blendify/colors/common.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/colors/texture.py` & `blendify-1.2.3/blendify/colors/texture.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/internal/io.py` & `blendify-1.2.3/blendify/internal/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 import os
 import sys
-from io import open
+from io import open, UnsupportedOperation
+
 
 class catch_stdout:
     """Stdout hook to ignore or reroute the blender output
     """
 
     def __init__(self, skip=False, logfile=None):
         """Creates a stdout hook object
         Args:
             skip: whether to skip the hook and pass the output to stdout
             logfile: filename to pass the output to (None to ignore the output completely)
         """
-        self.skip = skip
+        self.skip = skip or not self._check_if_hook_possible()
         self.logfile_path = logfile if logfile is not None else os.devnull
 
+    def _check_if_hook_possible(self):
+        try:
+            sys.stdout.fileno()
+        except UnsupportedOperation:
+            return False
+        return True
+
     def set_hook(self):
         if self.skip:
             return
         self.logfile = open(self.logfile_path, 'w')
         self.logfile_fd = self.logfile.fileno()
         self.stdout_fd = sys.stdout.fileno()
         self.saved_stdout_fd = os.dup(self.stdout_fd)
@@ -44,9 +52,10 @@
             os.close(self.internal_stdout_fd)
             os.dup2(self.saved_internal_stdout_fd, self.internal_stdout_fd)
             os.close(self.saved_internal_stdout_fd)
         self.logfile.close()
 
     def __enter__(self):
         self.set_hook()
+
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.release_hook()
```

### Comparing `blendify-1.2.2/blendify/internal/parser.py` & `blendify-1.2.3/blendify/internal/parser.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/internal/positionable.py` & `blendify-1.2.3/blendify/internal/positionable.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/internal/singleton.py` & `blendify-1.2.3/blendify/internal/singleton.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/internal/texture.py` & `blendify-1.2.3/blendify/internal/texture.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/lights/area.py` & `blendify-1.2.3/blendify/lights/area.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/lights/base.py` & `blendify-1.2.3/blendify/lights/base.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/lights/collection.py` & `blendify-1.2.3/blendify/lights/collection.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/lights/common.py` & `blendify-1.2.3/blendify/lights/common.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/materials/base.py` & `blendify-1.2.3/blendify/materials/base.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/materials/common.py` & `blendify-1.2.3/blendify/materials/common.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/renderables/base.py` & `blendify-1.2.3/blendify/renderables/base.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/renderables/collection.py` & `blendify-1.2.3/blendify/renderables/collection.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/renderables/mesh.py` & `blendify-1.2.3/blendify/renderables/mesh.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/renderables/pointcloud.py` & `blendify-1.2.3/blendify/renderables/pointcloud.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/renderables/primitives.py` & `blendify-1.2.3/blendify/renderables/primitives.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/scene.py` & `blendify-1.2.3/blendify/scene.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/utils/camera_trajectory.py` & `blendify-1.2.3/blendify/utils/camera_trajectory.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/utils/image.py` & `blendify-1.2.3/blendify/utils/image.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/utils/pointcloud.py` & `blendify-1.2.3/blendify/utils/pointcloud.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/utils/shadow_catcher.py` & `blendify-1.2.3/blendify/utils/shadow_catcher.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify/utils/smpl_wrapper.py` & `blendify-1.2.3/blendify/utils/smpl_wrapper.py`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/blendify.egg-info/PKG-INFO` & `blendify-1.2.3/blendify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blendify
-Version: 1.2.2
+Version: 1.2.3
 Summary: Python rendering framework for Blender
 Home-page: https://github.com/ptrvilya/blendify
 Author: Vladimir Guzov, Ilya Petrov
 Author-email: vguzov@mpi-inf.mpg.de, i.petrov@uni-tuebingen.de
 License: UNKNOWN
 Description: ![blendify Logo](https://github.com/ptrvilya/blendify/blob/main/.github/blendify_logo_light_bg.png?raw=true)
```

### Comparing `blendify-1.2.2/blendify.egg-info/SOURCES.txt` & `blendify-1.2.3/blendify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blendify-1.2.2/setup.py` & `blendify-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pkg_resources import DistributionNotFound, get_distribution
 from setuptools import setup, find_packages
-version = '1.2.2'
+version = '1.2.3'
 
 with open("docs/pip_readme.md", "r") as fi:
     long_description = fi.read()
 
 keywords = ["rendering", "pointcloud", "blender", "mesh"]
 
 classifiers = [
```

