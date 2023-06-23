# Comparing `tmp/pop-8.2.tar.gz` & `tmp/pop-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pop-8.2.tar", last modified: Sat Feb 15 18:10:48 2020, max compression
+gzip compressed data, was "dist/pop-9.tar", last modified: Fri Mar  6 15:43:01 2020, max compression
```

## Comparing `pop-8.2.tar` & `pop-9.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-02-15 18:10:48.122299 pop-8.2/
--rw-r--r--   0 thatch    (1000) thatch    (1000)      516 2020-02-15 18:10:48.122299 pop-8.2/PKG-INFO
--rw-r--r--   0 thatch    (1000) thatch    (1000)     3335 2020-02-07 03:08:14.000000 pop-8.2/README.rst
-drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-02-15 18:10:48.122299 pop-8.2/pop/
--rw-r--r--   0 thatch    (1000) thatch    (1000)     2604 2020-02-15 16:57:32.000000 pop-8.2/pop/__init__.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     5523 2020-02-15 17:24:32.000000 pop-8.2/pop/contract.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     2217 2020-02-15 16:57:32.000000 pop-8.2/pop/dirs.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     1393 2020-02-15 16:57:32.000000 pop-8.2/pop/exc.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)    12987 2020-02-15 17:56:56.000000 pop-8.2/pop/hub.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     9493 2020-02-15 17:24:33.000000 pop-8.2/pop/loader.py
-drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-02-15 18:10:48.122299 pop-8.2/pop/mods/
-drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-02-15 18:10:48.122299 pop-8.2/pop/mods/conf/
--rw-r--r--   0 thatch    (1000) thatch    (1000)     8884 2020-02-15 17:24:33.000000 pop-8.2/pop/mods/conf/args.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     1771 2020-02-15 17:24:32.000000 pop-8.2/pop/mods/conf/dirs.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     3543 2020-02-15 17:24:32.000000 pop-8.2/pop/mods/conf/file_parser.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)      104 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/conf/init.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     4917 2020-02-15 17:24:32.000000 pop-8.2/pop/mods/conf/integrate.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)      532 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/conf/json_conf.py
-drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-02-15 18:10:48.122299 pop-8.2/pop/mods/conf/log/
--rw-r--r--   0 thatch    (1000) thatch    (1000)      646 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/conf/log/basic.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     1814 2020-02-15 17:24:32.000000 pop-8.2/pop/mods/conf/log/init.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)      962 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/conf/nix_os.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     3820 2020-02-15 17:24:32.000000 pop-8.2/pop/mods/conf/reader.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)      669 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/conf/toml_conf.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)      443 2020-02-15 17:24:32.000000 pop-8.2/pop/mods/conf/version.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)      678 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/conf/yaml_conf.py
-drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-02-15 18:10:48.122299 pop-8.2/pop/mods/pop/
--rw-r--r--   0 thatch    (1000) thatch    (1000)      408 2020-02-15 17:24:32.000000 pop-8.2/pop/mods/pop/conf.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     1662 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/pop/dicts.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     4846 2020-02-15 17:24:33.000000 pop-8.2/pop/mods/pop/input.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     3903 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/pop/loop.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     1088 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/pop/ref.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     9053 2020-02-15 18:03:49.000000 pop-8.2/pop/mods/pop/seed.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     4776 2020-02-15 17:24:33.000000 pop-8.2/pop/mods/pop/sub.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     7122 2020-02-15 17:24:33.000000 pop-8.2/pop/mods/pop/testing.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)      348 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/pop/verify.py
-drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-02-15 18:10:48.122299 pop-8.2/pop/mods/proc/
--rw-r--r--   0 thatch    (1000) thatch    (1000)     4059 2020-02-15 17:24:33.000000 pop-8.2/pop/mods/proc/init.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     6021 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/proc/run.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     4897 2020-02-15 16:57:32.000000 pop-8.2/pop/mods/proc/worker.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     1355 2020-02-15 16:57:32.000000 pop-8.2/pop/scanner.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)      770 2020-02-15 17:24:33.000000 pop-8.2/pop/scripts.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)     4340 2020-02-15 17:24:33.000000 pop-8.2/pop/verify.py
--rw-r--r--   0 thatch    (1000) thatch    (1000)       40 2020-02-15 18:05:36.000000 pop-8.2/pop/version.py
-drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-02-15 18:10:48.122299 pop-8.2/pop.egg-info/
--rw-r--r--   0 thatch    (1000) thatch    (1000)      516 2020-02-15 18:10:47.000000 pop-8.2/pop.egg-info/PKG-INFO
--rw-r--r--   0 thatch    (1000) thatch    (1000)      901 2020-02-15 18:10:47.000000 pop-8.2/pop.egg-info/SOURCES.txt
--rw-r--r--   0 thatch    (1000) thatch    (1000)        1 2020-02-15 18:10:47.000000 pop-8.2/pop.egg-info/dependency_links.txt
--rw-r--r--   0 thatch    (1000) thatch    (1000)       51 2020-02-15 18:10:47.000000 pop-8.2/pop.egg-info/entry_points.txt
--rw-r--r--   0 thatch    (1000) thatch    (1000)        4 2020-02-15 18:10:47.000000 pop-8.2/pop.egg-info/top_level.txt
--rw-r--r--   0 thatch    (1000) thatch    (1000)      220 2020-02-15 17:56:55.000000 pop-8.2/pyproject.toml
--rw-r--r--   0 thatch    (1000) thatch    (1000)       38 2020-02-15 18:10:48.122299 pop-8.2/setup.cfg
--rw-r--r--   0 thatch    (1000) thatch    (1000)     1848 2020-02-15 17:24:33.000000 pop-8.2/setup.py
+drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-03-06 15:43:01.334848 pop-9/
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      514 2020-03-06 15:43:01.334848 pop-9/PKG-INFO
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     3335 2020-02-10 22:38:24.000000 pop-9/README.rst
+drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-03-06 15:43:01.331515 pop-9/pop/
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     2604 2020-02-19 23:44:46.000000 pop-9/pop/__init__.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     8281 2020-03-05 18:55:02.000000 pop-9/pop/contract.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     3605 2020-03-05 22:41:30.000000 pop-9/pop/dicts.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     2923 2020-03-05 23:22:46.000000 pop-9/pop/dirs.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     1393 2020-02-19 23:44:46.000000 pop-9/pop/exc.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)    13276 2020-03-05 22:45:16.000000 pop-9/pop/hub.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     9523 2020-03-05 18:55:02.000000 pop-9/pop/loader.py
+drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-03-06 15:43:01.331515 pop-9/pop/mods/
+drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-03-06 15:43:01.334848 pop-9/pop/mods/conf/
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     8884 2020-02-19 23:44:46.000000 pop-9/pop/mods/conf/args.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     1752 2020-03-06 15:23:17.000000 pop-9/pop/mods/conf/dirs.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     3543 2020-02-19 23:44:46.000000 pop-9/pop/mods/conf/file_parser.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      104 2020-02-19 23:44:46.000000 pop-9/pop/mods/conf/init.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     4735 2020-03-06 15:23:17.000000 pop-9/pop/mods/conf/integrate.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      532 2020-02-19 23:44:46.000000 pop-9/pop/mods/conf/json_conf.py
+drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-03-06 15:43:01.334848 pop-9/pop/mods/conf/log/
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      646 2020-02-19 23:44:46.000000 pop-9/pop/mods/conf/log/basic.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     1814 2020-02-19 23:44:46.000000 pop-9/pop/mods/conf/log/init.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      962 2020-02-19 23:44:46.000000 pop-9/pop/mods/conf/nix_os.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     3820 2020-02-19 23:44:46.000000 pop-9/pop/mods/conf/reader.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      669 2020-02-19 23:44:46.000000 pop-9/pop/mods/conf/toml_conf.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      443 2020-02-19 23:44:46.000000 pop-9/pop/mods/conf/version.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      678 2020-02-19 23:44:46.000000 pop-9/pop/mods/conf/yaml_conf.py
+drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-03-06 15:43:01.334848 pop-9/pop/mods/pop/
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      408 2020-02-19 23:44:46.000000 pop-9/pop/mods/pop/conf.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)    10324 2020-03-06 15:23:17.000000 pop-9/pop/mods/pop/data.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     1428 2020-03-05 23:27:15.000000 pop-9/pop/mods/pop/dicts.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      305 2020-03-05 16:56:20.000000 pop-9/pop/mods/pop/dyne.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     4846 2020-02-19 23:44:46.000000 pop-9/pop/mods/pop/input.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     4432 2020-03-06 15:23:17.000000 pop-9/pop/mods/pop/loop.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     1088 2020-02-19 23:44:46.000000 pop-9/pop/mods/pop/ref.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     9078 2020-03-02 17:56:04.000000 pop-9/pop/mods/pop/seed.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     4916 2020-03-05 16:20:21.000000 pop-9/pop/mods/pop/sub.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     7122 2020-03-05 00:03:35.000000 pop-9/pop/mods/pop/testing.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      348 2020-02-19 23:44:46.000000 pop-9/pop/mods/pop/verify.py
+drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-03-06 15:43:01.334848 pop-9/pop/mods/proc/
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     4059 2020-02-19 23:44:46.000000 pop-9/pop/mods/proc/init.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     6021 2020-02-19 23:44:46.000000 pop-9/pop/mods/proc/run.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     5074 2020-03-02 21:22:00.000000 pop-9/pop/mods/proc/worker.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     1370 2020-02-26 17:24:45.000000 pop-9/pop/scanner.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      770 2020-02-19 23:44:46.000000 pop-9/pop/scripts.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     4340 2020-02-19 23:44:46.000000 pop-9/pop/verify.py
+-rw-r--r--   0 thatch    (1000) thatch    (1000)       38 2020-03-06 15:42:55.000000 pop-9/pop/version.py
+drwxr-xr-x   0 thatch    (1000) thatch    (1000)        0 2020-03-06 15:43:01.334848 pop-9/pop.egg-info/
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      514 2020-03-06 15:43:01.000000 pop-9/pop.egg-info/PKG-INFO
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      956 2020-03-06 15:43:01.000000 pop-9/pop.egg-info/SOURCES.txt
+-rw-r--r--   0 thatch    (1000) thatch    (1000)        1 2020-03-06 15:43:01.000000 pop-9/pop.egg-info/dependency_links.txt
+-rw-r--r--   0 thatch    (1000) thatch    (1000)       51 2020-03-06 15:43:01.000000 pop-9/pop.egg-info/entry_points.txt
+-rw-r--r--   0 thatch    (1000) thatch    (1000)        4 2020-03-06 15:43:01.000000 pop-9/pop.egg-info/top_level.txt
+-rw-r--r--   0 thatch    (1000) thatch    (1000)      255 2020-02-21 01:23:14.000000 pop-9/pyproject.toml
+-rw-r--r--   0 thatch    (1000) thatch    (1000)       38 2020-03-06 15:43:01.334848 pop-9/setup.cfg
+-rw-r--r--   0 thatch    (1000) thatch    (1000)     1854 2020-03-06 15:23:17.000000 pop-9/setup.py
```

### Comparing `pop-8.2/PKG-INFO` & `pop-9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pop
-Version: 8.2
+Version: 9
 Summary: The Plugin Oriented Programming System
 Home-page: https://saltstack.com
 Author: Thomas S Hatch
 Author-email: thatch@saltstack.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pop-8.2/README.rst` & `pop-9/README.rst`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/__init__.py` & `pop-9/pop/__init__.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/dirs.py` & `pop-9/pop/dirs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Find directories
 """
+# Import pop libs
+import pop.dicts
+
 # Import python libs
 import os
 import sys
 import importlib
 
 
 def dir_list(subname, p_name, pypath=None, static=None):
@@ -69,11 +72,25 @@
         if "DYNE" in context:
             if not isinstance(context["DYNE"], dict):
                 continue
             for name, paths in context["DYNE"].items():
                 if not isinstance(paths, list):
                     continue
                 if name not in ret:
-                    ret[name] = []
+                    ret[name] = {"paths": [], "CONFIG": {}, "CLI_CONFIG": {}}
+                if "CONFIG" in context:
+                    pop.dicts.update(ret[name]["CONFIG"], context["CONFIG"])
+                if "CLI_CONFIG" in context:
+                    pop.dicts.update(ret[name]["CLI_CONFIG"], context["CLI_CONFIG"])
                 for path in paths:
-                    ret[name].append(os.path.join(dir_, path.replace(".", os.sep)))
+                    ref = os.path.join(dir_, path.replace(".", os.sep))
+                    if dir_.endswith(name):
+                        ret[name]["paths"].insert(0, ref)
+                    else:
+                        ret[name]["paths"].append(ref)
+    for name in ret:
+        if not ret[name]:
+            continue
+        first = ret[name]["paths"].pop(0)
+        ret[name]["paths"] = sorted(ret[name]["paths"])
+        ret[name]["paths"].insert(0, first)
     return ret
```

### Comparing `pop-8.2/pop/exc.py` & `pop-9/pop/exc.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/hub.py` & `pop-9/pop/hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
     def _load_dyne(self):
         """
         Load up the dynamic dirs for this sub
         """
         if not self._hub._dscan:
             self._hub._scan_dynamic()
-        for path in self._hub._dynamic.get(self._dyne_name, []):
+        for path in self._hub._dynamic.get(self._dyne_name, {}).get("paths", []):
             self._dirs.append(path)
 
     def _load_name_root(self):
         """
         Generate the root of the name to be used to apply to the loaded modules
         """
         if self._pypath:
@@ -312,15 +312,15 @@
             log.warning(error)
         else:
             log.info(error)
         return True
 
     def _find_mod(self, item, match_only=False):
         """
-        find the module named item
+        Find the module named item
         """
         for iface in self._scan:
             for bname in self._scan[iface]:
                 if os.path.basename(bname) == item:
                     self._load_item(iface, bname)
             if item in self._loaded:
                 return self._loaded[item]
@@ -345,15 +345,19 @@
             raise pop.exc.PopLoadError(
                 "Bad call to load item, no iface {}".format(iface)
             )
         if bname not in self._scan[iface]:
             raise pop.exc.PopLoadError(
                 "Bad call to load item, no bname {} in iface {}".format(bname, iface)
             )
-        mname = "{}.{}".format(self._name_root, os.path.basename(bname))
+        # The mname is the name to give the module in python's sys.modules
+        # This name must be unique for every loaded module, so we use the full
+        # module path sans the file extention
+        mname = self._scan[iface][bname]["path"].replace(os.sep, ".")
+        mname = mname[mname.index(".") + 1 : mname.rindex(".")].strip(".")
         mod = pop.loader.load_mod(mname, iface, self._scan[iface][bname]["path"],)
         if self._process_load_error(mod):
             self._load_errors[os.path.basename(bname)] = mod
             return
         self._prep_mod(mod, iface, bname)
 
     def _prep_mod(self, mod, iface, bname):
@@ -387,15 +391,15 @@
         # Now that the module has been added to the sub, call mod_init
         pop.loader.mod_init(self._hub, mod)
 
     def _load_all(self):
         """
         Load all modules found during the scan.
 
-        .. attention:: This completely disables the lazy loader behavior or pop
+        .. attention:: This completely disables the lazy loader behavior of pop
         """
         if self._loaded_all is True:
             return
         for iface in self._scan:
             for bname in self._scan[iface]:
                 if self._scan[iface][bname].get("loaded"):
                     continue
```

### Comparing `pop-8.2/pop/loader.py` & `pop-9/pop/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,16 +211,15 @@
 
 
 def prep_loaded_mod(this_sub, mod, mod_name, contracts):
     """
     Read the attributes of a python module and create a LoadedMod, which resolves
     aliases and omits objects that should not be exposed.
     """
-    # pylint: disable=protected-access
-    lmod = LoadedMod(mod_name)
+    lmod = this_sub._loaded.get(mod_name, LoadedMod(mod_name))
     ref = f"{this_sub._subname}.{mod_name}"  # getattr(hub, ref) should resolve to this module
     for attr in getattr(mod, "__load__", dir(mod)):
         name = getattr(mod, "__func_alias__", {}).get(attr, attr)
         func = getattr(mod, attr)
         if not this_sub._omit_vars:
             if (
                 not inspect.isfunction(func)
@@ -235,15 +234,17 @@
         if attr.endswith(this_sub._omit_end):
             continue
         if (
             inspect.isfunction(func)
             or inspect.isbuiltin(func)
             or type(func).__name__ == "cython_function_or_method"
         ):
-            obj = pop.contract.Contracted(this_sub._hub, contracts, func, ref, name)
+            obj = pop.contract.create_contracted(
+                this_sub._hub, contracts, func, ref, name
+            )
             if not this_sub._omit_func:
                 if this_sub._pypath and not func.__module__.startswith(mod.__name__):
                     # We're only interested in functions defined in this module, not
                     # imported functions
                     continue
                 lmod._funcs[name] = obj
                 lmod._attrs[name] = obj
```

### Comparing `pop-8.2/pop/mods/conf/args.py` & `pop-9/pop/mods/conf/args.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/conf/dirs.py` & `pop-9/pop/mods/conf/dirs.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import os
 
 
 def roots(hub, default_root, f_opts, root_dir):
     """
     Detect the root dir data and apply it
     """
-    # TODO: Make this safe for Windows
-    os_root = "/"
+    os_root = os.path.abspath(os.sep)
     root = os_root
     change = False
     non_priv = False
     if hasattr(os, "geteuid"):
         if not os.geteuid() == 0:
             change = True
             non_priv = True
```

### Comparing `pop-8.2/pop/mods/conf/file_parser.py` & `pop-9/pop/mods/conf/file_parser.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/conf/integrate.py` & `pop-9/pop/mods/conf/integrate.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 # Take an *args list of modules to import and look for conf.py
 # Import conf.py if present
 # After gathering all dicts, modify them to merge CLI options
 #
 # Import python libs
 import importlib
 import copy
+import os
 
 
-def _ex_final(confs, final, override, key_to_ref, ops_to_ref, globe=False):
+def _ex_final(confs, final, override, key_to_ref, ops_to_ref):
     """
     Scan the configuration datasets, create the final config
     value, and detect collisions
     """
     for arg in confs:
         for key in confs[arg]:
-            ref = f"global.{key}" if globe else f"{arg}.{key}"
+            ref = f"{arg}.{key}"
             if ref in override:
                 s_key = override[ref]["key"]
                 s_opts = override[ref]["options"]
             else:
                 s_key = key
                 s_opts = confs[arg][key].get("options", [])
             s_opts.append(f"--{s_key}")
@@ -57,84 +58,84 @@
     way modifying the cli options dynamically.
     The args look for the named <package>.conf python module and then
     looks for dictionaries named after the following convention:
 
     override = {'<package>.key': 'key': 'new_key', 'options': ['--option1', '--option2']}
 
     CONFIG: The main configuration for this package - loads to hub.OPT['<import>']
-    GLOBAL: Global configs to be used by other packages - loads to hub.OPT['global]
     CLI_CONFIG: Loaded only if this is the only import or if specified in the cli option
     SUBS: Used to define the subcommands, only loaded if this is the cli config
     """
     if override is None:
         override = {}
     if isinstance(imports, str):
         if cli is None:
             cli = imports
         imports = [imports]
     primary = imports[0] if cli is None else cli
     confs = {}
-    globe = {}
     final = {}
     collides = []
     key_to_ref = {}
     ops_to_ref = {}
     subs = {}
     for imp in imports:
-        cmod = importlib.import_module(f"{imp}.conf")
+        try:
+            cmod = importlib.import_module(f"{imp}.conf")
+        except ImportError:
+            continue
         if hasattr(cmod, "CONFIG"):
             confs[imp] = copy.deepcopy(cmod.CONFIG)
         if cli == imp:
             if hasattr(cmod, "CLI_CONFIG"):
                 confs[imp].update(copy.deepcopy(cmod.CLI_CONFIG))
             if hasattr(cmod, "SUBS"):
                 subs = copy.deepcopy(cmod.SUBS)
-        if hasattr(cmod, "GLOBAL"):
-            globe[imp] = copy.deepcopy(cmod.GLOBAL)
     if logs:
         lconf = hub.conf.log.init.conf(primary)
         lconf.update(confs[primary])
         confs[primary] = lconf
     if version:
         vconf = hub.conf.version.CONFIG
         vconf.update(confs[primary])
         confs[primary] = vconf
     _ex_final(confs, final, override, key_to_ref, ops_to_ref)
-    _ex_final(globe, final, override, key_to_ref, ops_to_ref, True)
     for opt in ops_to_ref:
         g_count = 0
         if len(ops_to_ref[opt]) > 1:
             collides.append({opt: ops_to_ref[opt]})
     for key in key_to_ref:
         col = []
         for ref in key_to_ref[key]:
-            if not ref.startswith("global."):
-                col.append(ref)
+            col.append(ref)
         if len(col) > 1:
             collides.append({key: key_to_ref[key]})
     if collides:
         raise KeyError(collides)
     opts = hub.conf.reader.read(final, subs, loader=loader)
-    f_opts = {}  # I don't want this to be a defaultdict,
-    # if someone tries to add a key willy nilly it should fail
+    # This will be put into an immutable data type before it is passed on
+    f_opts = {}
     for key in opts:
         if key == "_subparser_":
             f_opts["_subparser_"] = opts["_subparser_"]
             continue
         for ref in key_to_ref[key]:
             imp = ref[: ref.rindex(".")]
+            local_key = ref[ref.rindex(".") + 1 :]
             if imp not in f_opts:
                 f_opts[imp] = {}
-            f_opts[imp][key] = opts[key]
+            f_opts[imp][local_key] = opts[key]
     if roots:
         root_dir = f_opts.get(cli, {}).get("root_dir")
         hub.conf.dirs.roots(
-            final.get("root_dir", {}).get("default", "/"), f_opts, root_dir
+            final.get("root_dir", {}).get("default", os.path.abspath(os.sep)),
+            f_opts,
+            root_dir,
         )
         for imp in f_opts:
             hub.conf.dirs.verify(f_opts[imp])
-    hub.OPT = f_opts
+    hub.OPT = hub.pop.data.imap(f_opts)
     if logs:
         log_plugin = hub.OPT[primary].get("log_plugin")
         getattr(hub, f"conf.log.{log_plugin}.setup")(hub.OPT[primary])
     if hub.OPT[primary].get("version"):
         hub.conf.version.run(primary)
```

### Comparing `pop-8.2/pop/mods/conf/json_conf.py` & `pop-9/pop/mods/conf/json_conf.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/conf/log/basic.py` & `pop-9/pop/mods/conf/log/basic.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/conf/log/init.py` & `pop-9/pop/mods/conf/log/init.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/conf/nix_os.py` & `pop-9/pop/mods/conf/nix_os.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/conf/reader.py` & `pop-9/pop/mods/conf/reader.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/conf/toml_conf.py` & `pop-9/pop/mods/conf/toml_conf.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/conf/yaml_conf.py` & `pop-9/pop/mods/conf/yaml_conf.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/pop/input.py` & `pop-9/pop/mods/pop/input.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/pop/loop.py` & `pop-9/pop/mods/pop/loop.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,25 @@
 
 def create(hub):
     """
     Create the loop at hub.pop.Loop
     """
     if not hub.pop.Loop:
         hub.pop.loop.FUT_QUE = asyncio.Queue()
-        hub.pop.Loop = asyncio.get_event_loop()
+        if os.name == "nt":
+            hub.pop.Loop = asyncio._get_running_loop()
+            if hub.pop.Loop is not None:
+                return
+            # The default event loop on Windows, "SelectorEventLoop" has certain limitations
+            # ProactorEventLoop makes use of Window's I/O Completion Ports:
+            #   https://docs.microsoft.com/en-ca/windows/win32/fileio/i-o-completion-ports
+            hub.pop.Loop = asyncio.ProactorEventLoop()
+            asyncio.set_event_loop(hub.pop.Loop)
+        else:
+            hub.pop.Loop = asyncio.get_event_loop()
 
 
 def call_soon(hub, ref, *args, **kwargs):
     """
     Schedule a coroutine to be called when the loop has time. This needs
     to be called after the creation fo the loop
     """
```

### Comparing `pop-8.2/pop/mods/pop/ref.py` & `pop-9/pop/mods/pop/ref.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/pop/seed.py` & `pop-9/pop/mods/pop/seed.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,33 +81,37 @@
     ],
     packages=discover_packages(),
     entry_points={"console_scripts": ["%%NAME%% = %%NAME%%.scripts:start",],},
     cmdclass={"clean": Clean},
 )
 """
 
-PYPROJ = """[tool.black]
+PYPROJ = r"""[tool.black]
 line-length = 88
 target-version = ['py36', 'py37', 'py38']
 include = '\.pyi?$'
 exclude = '''
-/(
-    \.eggs
-  | \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
+(
+  /(
+      \.eggs
+    | \.git
+    | \.hg
+    | \.mypy_cache
+    | \.tox
+    | \.venv
+    | _build
+    | buck-out
+    | build
+    | dist
+  )/
+)
+'''
 """
 
-PRECOM = """---
+PRECOM = r"""---
 minimum_pre_commit_version: 1.15.2
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v2.5.0
     hooks:
       - id: check-merge-conflict  # Check for files that contain merge conflict strings.
         language_version: python3
@@ -146,30 +150,29 @@
 def start():
     hub = pop.hub.Hub()
     hub.pop.sub.add(dyne_name="%%NAME%%")
     hub.%%NAME%%.init.cli()
 """
 
 INIT = """def __init__(hub):
-    # Remmeber not to start your app in the __init__ function
+    # Remember not to start your app in the __init__ function
     # This function should just be used to set up the plugin subsystem
     # Add another function to call from your run.py to start the app
     pass
 
 
 def cli(hub):
     hub.pop.conf.integrate(["%%NAME%%"], cli="%%NAME%%", roots=True, loader="yaml")
     print("%%NAME%% works!")
 """
 
 REQ = "pop\n"
 
 CONF = """CLI_CONFIG = {}
 CONFIG = {}
-GLOBAL = {}
 SUBS = {}
 DYNE = {
     "%%NAME%%": ["%%NAME%%"],
 %%DYNE%%}
 """
 
 VER = 'version = "1"\n'
@@ -314,15 +317,15 @@
 
 
 def mkproj(hub):
     """
     Create the pyproject.toml file
     """
     path = os.path.join(hub.PATH, "pyproject.toml")
-    with open(path, "w+") as fp:
+    with open(path, "a+") as fp:
         fp.write(PYPROJ)
 
 
 def mkprecom(hub):
     """
     Create the precommit file
     """
```

### Comparing `pop-8.2/pop/mods/pop/sub.py` & `pop-9/pop/mods/pop/sub.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     omit_end=(),
     omit_func=False,
     omit_class=True,
     omit_vars=False,
     mod_basename="pop.sub",
     stop_on_failures=False,
     init=True,
+    load_all=True,
 ):
     """
     Add a new subsystem to the hub
     """
     if pypath:
         pypath = pop.hub.ex_path(pypath)
         subname = subname if subname else pypath[0].split(".")[-1]
@@ -59,14 +60,16 @@
         omit_class,
         omit_vars,
         mod_basename,
         stop_on_failures,
     )
     root._subs[subname]._sub_init(init)
     root._iter_subs = sorted(root._subs.keys())
+    if load_all:
+        root._subs[subname]._load_all()
 
 
 def remove(hub, subname):
     """
     Remove a pop from the hub, run the shutdown if needed
     """
     if hasattr(hub, subname):
@@ -142,15 +145,16 @@
             omit_func=sub._omit_func,
             omit_class=sub._omit_class,
             omit_vars=sub._omit_vars,
             mod_basename=sub._mod_basename,
             stop_on_failures=sub._stop_on_failures,
         )
         if recurse:
-            hub.pop.sub.load_subdirs(getattr(sub, name), recurse)
+            if isinstance(getattr(sub, name), pop.hub.Sub):
+                hub.pop.sub.load_subdirs(getattr(sub, name), recurse)
 
 
 def reload(hub, subname):
     """
     Instruct the hub to reload the modules for the given sub. This does not call
     the init.new function or remove sub level variables. But it does re-read the
     directory list and re-initialize the loader causing all modules to be re-evaluated
```

### Comparing `pop-8.2/pop/mods/pop/testing.py` & `pop-9/pop/mods/pop/testing.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/proc/init.py` & `pop-9/pop/mods/proc/init.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/proc/run.py` & `pop-9/pop/mods/proc/run.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/mods/proc/worker.py` & `pop-9/pop/mods/proc/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,18 @@
 
 async def work(hub, reader, writer):
     """
     Process the incoming work
     """
     inbound = await reader.readuntil(hub.proc.DELIM)
     inbound = inbound[: -len(hub.proc.DELIM)]
-    payload = msgpack.loads(inbound, encoding="utf8")
+    if msgpack.version < (1, 0, 0):
+        payload = msgpack.loads(inbound, encoding="utf-8")
+    else:
+        payload = msgpack.loads(inbound)
     ret = b""
     if "fun" not in payload:
         ret = {"err": "Invalid format"}
     elif payload["fun"] == "sub":
         # Time to add a sub to the hub!
         try:
             hub.proc.worker.add_sub(payload)
@@ -154,8 +157,11 @@
     mp += hub.proc.DELIM
     reader, writer = await asyncio.open_unix_connection(path=hub.proc.RET_SOCK_PATH)
     writer.write(mp)
     await writer.drain()
     ret = await reader.readuntil(hub.proc.DELIM)
     ret = ret[: -len(hub.proc.DELIM)]
     writer.close()
-    return msgpack.loads(ret, encoding="utf8")
+    if msgpack.version < (1, 0, 0):
+        return msgpack.loads(ret, encoding="utf-8")
+    else:
+        return msgpack.loads(ret)
```

### Comparing `pop-8.2/pop/scanner.py` & `pop-9/pop/scanner.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         for fn_ in os.listdir(dir_):
             _apply_scan(ret, dir_, fn_)
     return ret
 
 
 def _apply_scan(ret, dir_, fn_):
     """
-    Convert the scan data into
+    Convert the scan data into paths and refs
     """
     if fn_.startswith("_"):
         return
     if os.path.basename(dir_) in SKIP_DIRNAMES:
         return
     full = os.path.join(dir_, fn_)
     if "." not in full:
```

### Comparing `pop-8.2/pop/scripts.py` & `pop-9/pop/scripts.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop/verify.py` & `pop-9/pop/verify.py`

 * *Files identical despite different names*

### Comparing `pop-8.2/pop.egg-info/PKG-INFO` & `pop-9/pop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pop
-Version: 8.2
+Version: 9
 Summary: The Plugin Oriented Programming System
 Home-page: https://saltstack.com
 Author: Thomas S Hatch
 Author-email: thatch@saltstack.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pop-8.2/pop.egg-info/SOURCES.txt` & `pop-9/pop.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.rst
 pyproject.toml
 setup.py
 pop/__init__.py
 pop/contract.py
+pop/dicts.py
 pop/dirs.py
 pop/exc.py
 pop/hub.py
 pop/loader.py
 pop/scanner.py
 pop/scripts.py
 pop/verify.py
@@ -26,15 +27,17 @@
 pop/mods/conf/reader.py
 pop/mods/conf/toml_conf.py
 pop/mods/conf/version.py
 pop/mods/conf/yaml_conf.py
 pop/mods/conf/log/basic.py
 pop/mods/conf/log/init.py
 pop/mods/pop/conf.py
+pop/mods/pop/data.py
 pop/mods/pop/dicts.py
+pop/mods/pop/dyne.py
 pop/mods/pop/input.py
 pop/mods/pop/loop.py
 pop/mods/pop/ref.py
 pop/mods/pop/seed.py
 pop/mods/pop/sub.py
 pop/mods/pop/testing.py
 pop/mods/pop/verify.py
```

### Comparing `pop-8.2/setup.py` & `pop-9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 # Import python libs
 import os
-import sys
 import shutil
 from setuptools import setup, Command
 
 NAME = "pop"
 DESC = "The Plugin Oriented Programming System"
 
 # Version info -- read without importing
 _locals = {}
-with open("pop/version.py") as fp:
+with open(os.path.join("pop", "version.py")) as fp:
     exec(fp.read(), None, _locals)
 VERSION = _locals["version"]
 SETUP_DIRNAME = os.path.dirname(__file__)
 if not SETUP_DIRNAME:
     SETUP_DIRNAME = os.getcwd()
```

