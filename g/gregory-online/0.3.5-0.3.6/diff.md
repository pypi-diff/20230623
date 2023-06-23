# Comparing `tmp/gregory_online-0.3.5.tar.gz` & `tmp/gregory_online-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gregory_online-0.3.5.tar", last modified: Fri Jun 23 14:26:48 2023, max compression
+gzip compressed data, was "gregory_online-0.3.6.tar", last modified: Fri Jun 23 14:48:12 2023, max compression
```

## Comparing `gregory_online-0.3.5.tar` & `gregory_online-0.3.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:26:48.216715 gregory_online-0.3.5/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 14:26:48.216715 gregory_online-0.3.5/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-02 15:20:26.000000 gregory_online-0.3.5/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:26:48.212715 gregory_online-0.3.5/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    70902 2023-06-23 13:32:52.000000 gregory_online-0.3.5/bin/gregory_online
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:26:48.212715 gregory_online-0.3.5/gregory_online/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2023-03-15 09:15:19.000000 gregory_online-0.3.5/gregory_online/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    28897 2023-06-23 14:26:22.000000 gregory_online-0.3.5/gregory_online/ascgeneric.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7269 2023-06-23 07:56:33.000000 gregory_online-0.3.5/gregory_online/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:26:48.216715 gregory_online-0.3.5/gregory_online/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    56290 2023-03-15 09:15:19.000000 gregory_online-0.3.5/gregory_online/data/Am241.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   503044 2023-03-15 09:15:19.000000 gregory_online-0.3.5/gregory_online/data/Cm247.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    53304 2023-03-15 09:15:19.000000 gregory_online-0.3.5/gregory_online/data/Np237.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    79580 2023-03-15 09:15:19.000000 gregory_online-0.3.5/gregory_online/data/Pa231.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    93285 2023-03-15 09:15:19.000000 gregory_online-0.3.5/gregory_online/data/Pu239.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59999 2023-03-15 09:15:19.000000 gregory_online-0.3.5/gregory_online/data/Th232.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    78694 2023-03-15 09:15:19.000000 gregory_online-0.3.5/gregory_online/data/U235.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    97718 2023-03-15 09:15:19.000000 gregory_online-0.3.5/gregory_online/data/U238.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   123572 2023-06-12 07:00:49.000000 gregory_online-0.3.5/gregory_online/data/decay_lara.parquet
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1139 2023-03-15 09:15:19.000000 gregory_online-0.3.5/gregory_online/data/testrebin.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3758 2023-06-12 07:00:49.000000 gregory_online-0.3.5/gregory_online/decay_db.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    15128 2023-06-23 07:56:33.000000 gregory_online-0.3.5/gregory_online/dpp2jpg.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3631 2023-06-23 07:56:33.000000 gregory_online-0.3.5/gregory_online/erlang.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12625 2023-06-12 07:00:49.000000 gregory_online-0.3.5/gregory_online/fetchnp.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4741 2023-06-23 13:32:00.000000 gregory_online-0.3.5/gregory_online/histo_analyze.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4169 2023-06-23 07:56:33.000000 gregory_online-0.3.5/gregory_online/histo_displ.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-12 07:00:49.000000 gregory_online-0.3.5/gregory_online/histo_global_cont.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    19157 2023-06-23 14:23:01.000000 gregory_online-0.3.5/gregory_online/histo_io.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:33:05.000000 gregory_online-0.3.5/gregory_online/histo_np_ops.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-19 12:31:34.000000 gregory_online-0.3.5/gregory_online/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2594 2023-06-23 07:56:33.000000 gregory_online-0.3.5/gregory_online/topbar.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2023-03-15 09:15:19.000000 gregory_online-0.3.5/gregory_online/utilone.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3293 2023-06-12 07:00:49.000000 gregory_online-0.3.5/gregory_online/utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-23 14:26:47.000000 gregory_online-0.3.5/gregory_online/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:26:48.212715 gregory_online-0.3.5/gregory_online.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 14:26:48.000000 gregory_online-0.3.5/gregory_online.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1006 2023-06-23 14:26:48.000000 gregory_online-0.3.5/gregory_online.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-23 14:26:48.000000 gregory_online-0.3.5/gregory_online.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      123 2023-06-23 14:26:48.000000 gregory_online-0.3.5/gregory_online.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-23 14:26:48.000000 gregory_online-0.3.5/gregory_online.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-23 14:26:48.216715 gregory_online-0.3.5/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1268 2023-06-23 14:25:45.000000 gregory_online-0.3.5/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:48:12.619422 gregory_online-0.3.6/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 14:48:12.615422 gregory_online-0.3.6/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-02 15:20:26.000000 gregory_online-0.3.6/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:48:12.611422 gregory_online-0.3.6/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    70902 2023-06-23 13:32:52.000000 gregory_online-0.3.6/bin/gregory_online
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:48:12.615422 gregory_online-0.3.6/gregory_online/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    28897 2023-06-23 14:26:22.000000 gregory_online-0.3.6/gregory_online/ascgeneric.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7269 2023-06-23 07:56:33.000000 gregory_online-0.3.6/gregory_online/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:48:12.615422 gregory_online-0.3.6/gregory_online/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    56290 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Am241.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   503044 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Cm247.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    53304 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Np237.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    79580 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Pa231.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    93285 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Pu239.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59999 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Th232.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    78694 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/U235.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    97718 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/U238.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   123572 2023-06-12 07:00:49.000000 gregory_online-0.3.6/gregory_online/data/decay_lara.parquet
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1139 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/testrebin.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3758 2023-06-12 07:00:49.000000 gregory_online-0.3.6/gregory_online/decay_db.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    15128 2023-06-23 07:56:33.000000 gregory_online-0.3.6/gregory_online/dpp2jpg.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3631 2023-06-23 07:56:33.000000 gregory_online-0.3.6/gregory_online/erlang.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12625 2023-06-12 07:00:49.000000 gregory_online-0.3.6/gregory_online/fetchnp.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4741 2023-06-23 13:32:00.000000 gregory_online-0.3.6/gregory_online/histo_analyze.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4169 2023-06-23 07:56:33.000000 gregory_online-0.3.6/gregory_online/histo_displ.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-12 07:00:49.000000 gregory_online-0.3.6/gregory_online/histo_global_cont.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    19157 2023-06-23 14:23:01.000000 gregory_online-0.3.6/gregory_online/histo_io.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:33:05.000000 gregory_online-0.3.6/gregory_online/histo_np_ops.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-19 12:31:34.000000 gregory_online-0.3.6/gregory_online/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2594 2023-06-23 07:56:33.000000 gregory_online-0.3.6/gregory_online/topbar.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/utilone.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3293 2023-06-12 07:00:49.000000 gregory_online-0.3.6/gregory_online/utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:48:12.615422 gregory_online-0.3.6/gregory_online.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1006 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      127 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-23 14:48:12.619422 gregory_online-0.3.6/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1275 2023-06-23 14:29:08.000000 gregory_online-0.3.6/setup.py
```

### Comparing `gregory_online-0.3.5/PKG-INFO` & `gregory_online-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gregory_online
-Version: 0.3.5
+Version: 0.3.6
 Summary: Online watching HTTP server of ROOT on port 9009
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 
 Project gregory~online~
```

### Comparing `gregory_online-0.3.5/README.md` & `gregory_online-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/bin/gregory_online` & `gregory_online-0.3.6/bin/gregory_online`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/ascgeneric.py` & `gregory_online-0.3.6/gregory_online/ascgeneric.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/config.py` & `gregory_online-0.3.6/gregory_online/config.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/data/Am241.svg` & `gregory_online-0.3.6/gregory_online/data/Am241.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/data/Cm247.png` & `gregory_online-0.3.6/gregory_online/data/Cm247.png`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/data/Np237.svg` & `gregory_online-0.3.6/gregory_online/data/Np237.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/data/Pa231.svg` & `gregory_online-0.3.6/gregory_online/data/Pa231.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/data/Pu239.svg` & `gregory_online-0.3.6/gregory_online/data/Pu239.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/data/Th232.svg` & `gregory_online-0.3.6/gregory_online/data/Th232.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/data/U235.svg` & `gregory_online-0.3.6/gregory_online/data/U235.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/data/U238.svg` & `gregory_online-0.3.6/gregory_online/data/U238.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/data/decay_lara.parquet` & `gregory_online-0.3.6/gregory_online/data/decay_lara.parquet`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/data/testrebin.py` & `gregory_online-0.3.6/gregory_online/data/testrebin.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/decay_db.py` & `gregory_online-0.3.6/gregory_online/decay_db.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/dpp2jpg.py` & `gregory_online-0.3.6/gregory_online/dpp2jpg.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/erlang.py` & `gregory_online-0.3.6/gregory_online/erlang.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/fetchnp.py` & `gregory_online-0.3.6/gregory_online/fetchnp.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/histo_analyze.py` & `gregory_online-0.3.6/gregory_online/histo_analyze.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/histo_displ.py` & `gregory_online-0.3.6/gregory_online/histo_displ.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/histo_global_cont.py` & `gregory_online-0.3.6/gregory_online/histo_global_cont.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/histo_io.py` & `gregory_online-0.3.6/gregory_online/histo_io.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/histo_np_ops.py` & `gregory_online-0.3.6/gregory_online/histo_np_ops.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/key_enter.py` & `gregory_online-0.3.6/gregory_online/key_enter.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/topbar.py` & `gregory_online-0.3.6/gregory_online/topbar.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online/utils.py` & `gregory_online-0.3.6/gregory_online/utils.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/gregory_online.egg-info/PKG-INFO` & `gregory_online-0.3.6/gregory_online.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gregory-online
-Version: 0.3.5
+Version: 0.3.6
 Summary: Online watching HTTP server of ROOT on port 9009
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 
 Project gregory~online~
```

### Comparing `gregory_online-0.3.5/gregory_online.egg-info/SOURCES.txt` & `gregory_online-0.3.6/gregory_online.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.5/setup.py` & `gregory_online-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     license="GPL2",
     version=get_version("gregory_online/version.py"),
     packages=['gregory_online'],
     package_data={'gregory_online': ['data/*']},
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     scripts = ['bin/gregory_online'],
-    install_requires = ['fire','scipy','pyfromroot','pytermgui','readchar','fastnumbers','sshkeyboard','terminaltables','fastparquet','tables','simple_term_menu',"tdb_io"],
+    install_requires = ['fire','scipy','pyfromroot','pytermgui','readchar','fastnumbers','sshkeyboard','terminaltables','fastparquet','tables','simple_term_menu',"tdb_io", "bs4"],
 )
```

