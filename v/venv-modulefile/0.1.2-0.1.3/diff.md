# Comparing `tmp/venv-modulefile-0.1.2.tar.gz` & `tmp/venv-modulefile-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmpwc0d4fos/venv-modulefile-0.1.2.tar", last modified: Wed May 31 15:21:01 2023, max compression
+gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/venv-modulefile/dist/tmpynp_so4b/venv-modulefile-0.1.3.tar", last modified: Fri Jun 23 13:15:55 2023, max compression
```

## Comparing `venv-modulefile-0.1.2.tar` & `venv-modulefile-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-05-24 12:42:33.000000 venv-modulefile-0.1.2/pyproject.toml
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/setup.cfg
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-04-19 16:42:18.000000 venv-modulefile-0.1.2/MANIFEST.in
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-05-22 14:55:50.000000 venv-modulefile-0.1.2/README.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9606 2023-05-24 11:56:17.000000 venv-modulefile-0.1.2/setup.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venvmod/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-05-31 15:18:02.000000 venv-modulefile-0.1.2/src/venvmod/VERSION
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2023-05-23 10:47:49.000000 venv-modulefile-0.1.2/src/venvmod/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1624 2023-05-24 15:09:55.000000 venv-modulefile-0.1.2/src/venvmod/tools.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venvmod/commands/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1715 2023-05-24 14:50:10.000000 venv-modulefile-0.1.2/src/venvmod/commands/test_imports.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3825 2023-05-24 16:12:10.000000 venv-modulefile-0.1.2/src/venvmod/commands/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     5049 2023-05-24 16:11:24.000000 venv-modulefile-0.1.2/src/venvmod/commands/create_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    11077 2023-05-24 16:13:07.000000 venv-modulefile-0.1.2/src/venvmod/commands/append_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10550 2023-05-24 17:54:10.000000 venv-modulefile-0.1.2/src/venvmod/modulefile.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2899 2023-05-24 11:55:46.000000 venv-modulefile-0.1.2/src/README.md
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      807 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/entry_points.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/top_level.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/SOURCES.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/dependency_links.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2023-05-31 15:21:01.000000 venv-modulefile-0.1.2/src/venv_modulefile.egg-info/requires.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-05-04 08:19:39.000000 venv-modulefile-0.1.2/LICENSE.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/pyproject.toml
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/setup.cfg
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/MANIFEST.in
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      959 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/README.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9606 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/setup.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/src/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/src/venvmod/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-06-23 13:11:32.000000 venv-modulefile-0.1.3/src/venvmod/VERSION
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      247 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/src/venvmod/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1624 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/src/venvmod/tools.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/src/venvmod/commands/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1715 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/src/venvmod/commands/test_imports.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3825 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/src/venvmod/commands/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     5049 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/src/venvmod/commands/create_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    11077 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/src/venvmod/commands/append_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10655 2023-06-23 13:10:38.000000 venv-modulefile-0.1.3/src/venvmod/modulefile.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2899 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/src/README.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/src/venv_modulefile.egg-info/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      807 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/src/venv_modulefile.egg-info/entry_points.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/src/venv_modulefile.egg-info/top_level.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/src/venv_modulefile.egg-info/SOURCES.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4043 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/src/venv_modulefile.egg-info/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/src/venv_modulefile.egg-info/dependency_links.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      241 2023-06-23 13:15:55.000000 venv-modulefile-0.1.3/src/venv_modulefile.egg-info/requires.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-06-23 13:08:24.000000 venv-modulefile-0.1.3/LICENSE.md
```

### Comparing `venv-modulefile-0.1.2/PKG-INFO` & `venv-modulefile-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/roland-lenain/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/roland-lenain/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
```

### Comparing `venv-modulefile-0.1.2/README.md` & `venv-modulefile-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.2/setup.py` & `venv-modulefile-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.2/src/venvmod/tools.py` & `venv-modulefile-0.1.3/src/venvmod/tools.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.2/src/venvmod/commands/test_imports.py` & `venv-modulefile-0.1.3/src/venvmod/commands/test_imports.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.2/src/venvmod/commands/__init__.py` & `venv-modulefile-0.1.3/src/venvmod/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.2/src/venvmod/commands/create_module.py` & `venv-modulefile-0.1.3/src/venvmod/commands/create_module.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.2/src/venvmod/commands/append_module.py` & `venv-modulefile-0.1.3/src/venvmod/commands/append_module.py`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.2/src/venvmod/modulefile.py` & `venv-modulefile-0.1.3/src/venvmod/modulefile.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,24 +51,27 @@
     """Gets modulefile version
 
     Returns
     -------
     str
         version as 'x.y.z', '0.0.0' if not found
     """
-    result = subprocess.run([get_shell_command(), '-c', "module --version"],
-                            stderr=subprocess.PIPE, stdout=subprocess.PIPE, check=False)
+    try:
+        result = subprocess.run([get_shell_command(), '-c', "module --version"],
+                                stderr=subprocess.PIPE, stdout=subprocess.PIPE, check=False)
 
-    logger.debug("get_version: %s\n%s\n%s", result, result.stderr.decode(), result.stdout.decode())
-    if result.returncode == 0:
-        if 'VERSION=' in result.stderr.decode().split()[0]:  # version < 4.0
-            return result.stderr.decode().split()[0].split("=")[1]
-        if 'Modules' == result.stderr.decode().split()[0]:
-            return result.stderr.decode().split()[2]
-    return "0.0.0"
+        logger.debug(
+            "get_version: %s\n%s\n%s", result, result.stderr.decode(), result.stdout.decode())
+        if result.returncode == 0:
+            if 'VERSION=' in result.stderr.decode().split()[0]:  # version < 4.0
+                return result.stderr.decode().split()[0].split("=")[1]
+            if 'Modules' == result.stderr.decode().split()[0]:
+                return result.stderr.decode().split()[2]
+    finally:
+        return "0.0.0"  # pylint: disable=lost-exception
 
 
 class ModuleInstaller:  # pylint: disable=too-few-public-methods
     """Class to install Environment Module.
     """
 
     def __init__(self,
```

### Comparing `venv-modulefile-0.1.2/src/README.md` & `venv-modulefile-0.1.3/src/README.md`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.2/src/venv_modulefile.egg-info/entry_points.txt` & `venv-modulefile-0.1.3/src/venv_modulefile.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.2/src/venv_modulefile.egg-info/SOURCES.txt` & `venv-modulefile-0.1.3/src/venv_modulefile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.1.2/src/venv_modulefile.egg-info/PKG-INFO` & `venv-modulefile-0.1.3/src/venv_modulefile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venv-modulefile
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python venv extension using Modulefile
 Home-page: https://github.com/roland-lenain/venv-modulefile
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/roland-lenain/venv-modulefile/issues
 Project-URL: Doc, https://venv-modulefile.readthedocs.io/en/latest/index.html
```

### Comparing `venv-modulefile-0.1.2/LICENSE.md` & `venv-modulefile-0.1.3/LICENSE.md`

 * *Files identical despite different names*

