# Comparing `tmp/tuic-tunnel-0.1.4.tar.gz` & `tmp/tuic-tunnel-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuic-tunnel-0.1.4.tar", last modified: Fri Mar  3 18:06:53 2023, max compression
+gzip compressed data, was "tuic-tunnel-0.1.5.tar", last modified: Fri Jun 23 10:25:09 2023, max compression
```

## Comparing `tuic-tunnel-0.1.4.tar` & `tuic-tunnel-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:06:53.890519 tuic-tunnel-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-03 18:06:44.000000 tuic-tunnel-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-03 18:06:44.000000 tuic-tunnel-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-03 18:06:53.890519 tuic-tunnel-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-03 18:06:44.000000 tuic-tunnel-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-03 18:06:44.000000 tuic-tunnel-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 18:06:53.890519 tuic-tunnel-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-03 18:06:44.000000 tuic-tunnel-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:06:53.890519 tuic-tunnel-0.1.4/tuic_tunnel/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-03 18:06:44.000000 tuic-tunnel-0.1.4/tuic_tunnel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-03-03 18:06:45.000000 tuic-tunnel-0.1.4/tuic_tunnel/tuic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 18:06:53.890519 tuic-tunnel-0.1.4/tuic_tunnel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-03 18:06:53.000000 tuic-tunnel-0.1.4/tuic_tunnel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-03 18:06:53.000000 tuic-tunnel-0.1.4/tuic_tunnel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 18:06:53.000000 tuic-tunnel-0.1.4/tuic_tunnel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-03 18:06:53.000000 tuic-tunnel-0.1.4/tuic_tunnel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-03 18:06:53.000000 tuic-tunnel-0.1.4/tuic_tunnel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:25:09.864206 tuic-tunnel-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-23 10:24:56.000000 tuic-tunnel-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 10:24:56.000000 tuic-tunnel-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-23 10:25:09.864206 tuic-tunnel-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-23 10:24:56.000000 tuic-tunnel-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 10:24:56.000000 tuic-tunnel-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:25:09.864206 tuic-tunnel-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-23 10:24:56.000000 tuic-tunnel-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:25:09.852206 tuic-tunnel-0.1.5/tuic_tunnel/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 10:24:56.000000 tuic-tunnel-0.1.5/tuic_tunnel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:25:09.852206 tuic-tunnel-0.1.5/tuic_tunnel/bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:25:09.856206 tuic-tunnel-0.1.5/tuic_tunnel/bin/darwin/
+-rw-r--r--   0 runner    (1001) docker     (123)  2112904 2023-06-23 10:24:56.000000 tuic-tunnel-0.1.5/tuic_tunnel/bin/darwin/tuic-client-x86_64
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:25:09.860206 tuic-tunnel-0.1.5/tuic_tunnel/bin/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1812560 2023-06-23 10:24:56.000000 tuic-tunnel-0.1.5/tuic_tunnel/bin/linux/tuic-client-aarch64
+-rw-r--r--   0 runner    (1001) docker     (123)  2284232 2023-06-23 10:24:56.000000 tuic-tunnel-0.1.5/tuic_tunnel/bin/linux/tuic-client-x86_64
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:25:09.860206 tuic-tunnel-0.1.5/tuic_tunnel/bin/win32/
+-rw-r--r--   0 runner    (1001) docker     (123)  2111488 2023-06-23 10:24:56.000000 tuic-tunnel-0.1.5/tuic_tunnel/bin/win32/tuic-client-amd64.exe
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-23 10:24:56.000000 tuic-tunnel-0.1.5/tuic_tunnel/tuic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:25:09.856206 tuic-tunnel-0.1.5/tuic_tunnel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-23 10:25:09.000000 tuic-tunnel-0.1.5/tuic_tunnel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-23 10:25:09.000000 tuic-tunnel-0.1.5/tuic_tunnel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:25:09.000000 tuic-tunnel-0.1.5/tuic_tunnel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 10:25:09.000000 tuic-tunnel-0.1.5/tuic_tunnel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 10:25:09.000000 tuic-tunnel-0.1.5/tuic_tunnel.egg-info/top_level.txt
```

### Comparing `tuic-tunnel-0.1.4/LICENSE` & `tuic-tunnel-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tuic-tunnel-0.1.4/PKG-INFO` & `tuic-tunnel-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuic-tunnel
-Version: 0.1.4
+Version: 0.1.5
 Summary: TUIC tunnel plugin for turbo-tunnel.
 Home-page: https://github.com/turbo-tunnel/tuic-tunnel
 Author: drunkdream
 Author-email: drunkdream@qq.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuic-tunnel-0.1.4/README.md` & `tuic-tunnel-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tuic-tunnel-0.1.4/setup.py` & `tuic-tunnel-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `tuic-tunnel-0.1.4/tuic_tunnel/tuic.py` & `tuic-tunnel-0.1.5/tuic_tunnel/tuic.py`

 * *Files identical despite different names*

### Comparing `tuic-tunnel-0.1.4/tuic_tunnel.egg-info/PKG-INFO` & `tuic-tunnel-0.1.5/tuic_tunnel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuic-tunnel
-Version: 0.1.4
+Version: 0.1.5
 Summary: TUIC tunnel plugin for turbo-tunnel.
 Home-page: https://github.com/turbo-tunnel/tuic-tunnel
 Author: drunkdream
 Author-email: drunkdream@qq.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

