# Comparing `tmp/deemon-2.9.2.tar.gz` & `tmp/deemon-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deemon-2.9.2.tar", last modified: Thu Mar 24 22:40:50 2022, max compression
+gzip compressed data, was "deemon-2.9.3.tar", last modified: Mon Mar 28 13:15:34 2022, max compression
```

## Comparing `deemon-2.9.2.tar` & `deemon-2.9.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 22:40:50.170439 deemon-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-03-24 22:40:37.000000 deemon-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-03-24 22:40:37.000000 deemon-2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-03-24 22:40:50.170439 deemon-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3000 2022-03-24 22:40:37.000000 deemon-2.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 22:40:50.166439 deemon-2.9.2/deemon/
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 22:40:50.166439 deemon-2.9.2/deemon/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 22:40:50.166439 deemon-2.9.2/deemon/assets/images/
--rw-r--r--   0 runner    (1001) docker     (121)    62627 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/assets/images/deemon.png
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/assets/images/discord.png
--rw-r--r--   0 runner    (1001) docker     (121)     4939 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/assets/images/github.png
--rw-r--r--   0 runner    (1001) docker     (121)    12580 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/assets/images/logo-medium.png
--rw-r--r--   0 runner    (1001) docker     (121)     7991 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/assets/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     4659 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/assets/images/reddit.png
--rw-r--r--   0 runner    (1001) docker     (121)     4837 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/assets/index.html
--rw-r--r--   0 runner    (1001) docker     (121)    17847 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 22:40:50.170439 deemon-2.9.2/deemon/cmd/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3421 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/artistconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     5150 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/backup.py
--rw-r--r--   0 runner    (1001) docker     (121)    16608 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/extra.py
--rw-r--r--   0 runner    (1001) docker     (121)     5161 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/generate.py
--rw-r--r--   0 runner    (1001) docker     (121)    11062 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     7208 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)    15687 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/refresh.py
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/rollback.py
--rw-r--r--   0 runner    (1001) docker     (121)    18596 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/search.py
--rw-r--r--   0 runner    (1001) docker     (121)    10626 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/cmd/show.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 22:40:50.170439 deemon-2.9.2/deemon/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13137 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/core/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    18906 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/core/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    27572 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/core/db.py
--rw-r--r--   0 runner    (1001) docker     (121)     8259 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/core/dmi.py
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     7518 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/core/notifier.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 22:40:50.170439 deemon-2.9.2/deemon/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/utils/dataprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (121)      541 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/utils/startup.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/utils/ui.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-03-24 22:40:37.000000 deemon-2.9.2/deemon/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-24 22:40:50.166439 deemon-2.9.2/deemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-03-24 22:40:50.000000 deemon-2.9.2/deemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1123 2022-03-24 22:40:50.000000 deemon-2.9.2/deemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-24 22:40:50.000000 deemon-2.9.2/deemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-03-24 22:40:50.000000 deemon-2.9.2/deemon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-24 22:40:50.000000 deemon-2.9.2/deemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-24 22:40:50.000000 deemon-2.9.2/deemon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-24 22:40:37.000000 deemon-2.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-24 22:40:50.170439 deemon-2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-03-24 22:40:37.000000 deemon-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:15:34.939640 deemon-2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-03-28 13:15:25.000000 deemon-2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-03-28 13:15:25.000000 deemon-2.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-03-28 13:15:34.939640 deemon-2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3000 2022-03-28 13:15:25.000000 deemon-2.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:15:34.935640 deemon-2.9.3/deemon/
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:15:34.935640 deemon-2.9.3/deemon/assets/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:15:34.935640 deemon-2.9.3/deemon/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    62627 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/assets/images/deemon.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/assets/images/discord.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4939 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/assets/images/github.png
+-rw-r--r--   0 runner    (1001) docker     (121)    12580 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/assets/images/logo-medium.png
+-rw-r--r--   0 runner    (1001) docker     (121)     7991 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/assets/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4659 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/assets/images/reddit.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4837 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/assets/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)    17847 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:15:34.939640 deemon-2.9.3/deemon/cmd/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3421 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/artistconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5150 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/backup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16608 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/download.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/extra.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5161 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/generate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11062 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7208 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15674 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/rollback.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18596 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/search.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10626 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/cmd/show.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:15:34.939640 deemon-2.9.3/deemon/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13137 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18906 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27572 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/core/db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8259 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/core/dmi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7518 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/core/notifier.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:15:34.939640 deemon-2.9.3/deemon/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/utils/dataprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (121)      541 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2373 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/utils/startup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      697 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/utils/ui.py
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-03-28 13:15:25.000000 deemon-2.9.3/deemon/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 13:15:34.935640 deemon-2.9.3/deemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3513 2022-03-28 13:15:34.000000 deemon-2.9.3/deemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1123 2022-03-28 13:15:34.000000 deemon-2.9.3/deemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-28 13:15:34.000000 deemon-2.9.3/deemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-03-28 13:15:34.000000 deemon-2.9.3/deemon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-28 13:15:34.000000 deemon-2.9.3/deemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-03-28 13:15:34.000000 deemon-2.9.3/deemon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-28 13:15:25.000000 deemon-2.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-28 13:15:34.939640 deemon-2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-03-28 13:15:25.000000 deemon-2.9.3/setup.py
```

### Comparing `deemon-2.9.2/LICENSE` & `deemon-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/PKG-INFO` & `deemon-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deemon
-Version: 2.9.2
+Version: 2.9.3
 Summary: Monitor new releases by a specified list of artists and auto download using the deemix library
 Home-page: https://github.com/digitalec/deemon
 Author: digitalec
 License: GPL3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `deemon-2.9.2/README.md` & `deemon-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/assets/images/deemon.png` & `deemon-2.9.3/deemon/assets/images/deemon.png`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/assets/images/discord.png` & `deemon-2.9.3/deemon/assets/images/discord.png`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/assets/images/github.png` & `deemon-2.9.3/deemon/assets/images/github.png`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/assets/images/logo-medium.png` & `deemon-2.9.3/deemon/assets/images/logo-medium.png`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/assets/images/logo.png` & `deemon-2.9.3/deemon/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/assets/images/reddit.png` & `deemon-2.9.3/deemon/assets/images/reddit.png`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/assets/index.html` & `deemon-2.9.3/deemon/assets/index.html`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/cli.py` & `deemon-2.9.3/deemon/cli.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/cmd/artistconfig.py` & `deemon-2.9.3/deemon/cmd/artistconfig.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/cmd/backup.py` & `deemon-2.9.3/deemon/cmd/backup.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/cmd/download.py` & `deemon-2.9.3/deemon/cmd/download.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/cmd/extra.py` & `deemon-2.9.3/deemon/cmd/extra.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/cmd/generate.py` & `deemon-2.9.3/deemon/cmd/generate.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/cmd/monitor.py` & `deemon-2.9.3/deemon/cmd/monitor.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/cmd/profile.py` & `deemon-2.9.3/deemon/cmd/profile.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/cmd/refresh.py` & `deemon-2.9.3/deemon/cmd/refresh.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.queue_list = []
         self.skip_download = skip_download
         self.download_all = ignore_filters
         self.seen = None
 
         if self.time_machine:
             logger.info(f":: Time Machine active: {datetime.strftime(self.time_machine, '%b %d, %Y')}!")
-            config.set('by_release_date', False)
+            config._CONFIG['new_releases']['release_max_age'] = 0
             if not self.waiting_for_refresh():
                 self.db.remove_specific_releases({'tm_date': str(self.time_machine)})
                 self.db.commit()
 
     @staticmethod
     def debugger(message: str, payload = None):
         if config.debug_mode():
@@ -190,14 +190,24 @@
         if len(p):
             p['releases'] = self.remove_existing_releases(p, self.seen)
             self.filter_artist_releases(p)
         else:
             logger.debug("No payload provided")
 
     def run(self, artists: list = None, playlists: list = None):
+
+        if config.check_account_status():
+            if self.api.account_type == "free" and config.bitrate() != "128":
+                notification = notifier.Notify()
+                notification.expired_arl()
+                return logger.error("   [X] ARL expired? Deezer account only allows low"
+                                    " quality. If you wish to download "
+                                    "anyway, set `check_account_status` "
+                                    "to False in the config.")
+
         if artists:
             self.debugger("ManualRefresh", artists)
             monitored_artists = [x for x in (self.db.get_monitored_artist_by_name(a) for a in artists) if x]
             if not len(monitored_artists):
                 return logger.warning("Specified artist(s) were not found")
             api_result = self.get_release_data({'artists': monitored_artists})
         elif playlists:
@@ -237,22 +247,14 @@
 
         if self.skip_download:
             logger.info(f"   [!] You have opted to skip downloads, clearing {len(self.queue_list):,} item(s) from queue...")
             self.queue_list.clear()
             self.new_releases_alert.clear()
 
         if len(self.queue_list):
-            if config.check_account_status():
-                if self.api.account_type == "free" and config.bitrate() != "128":
-                    notification = notifier.Notify()
-                    notification.expired_arl()
-                    return logger.error("   [X] ARL expired? Deezer account only allows low"
-                                        " quality. If you wish to download "
-                                        "anyway, set `check_account_status` "
-                                        "to False in the config.")
             dl = Download()
             dl.download_queue(self.queue_list)
 
 
         if len(self.new_playlist_releases) or len(self.new_releases):
             if len(self.new_playlist_releases):
                 logger.debug("Updating playlist releases in database...")
```

### Comparing `deemon-2.9.2/deemon/cmd/rollback.py` & `deemon-2.9.3/deemon/cmd/rollback.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/cmd/search.py` & `deemon-2.9.3/deemon/cmd/search.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/cmd/show.py` & `deemon-2.9.3/deemon/cmd/show.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/core/api.py` & `deemon-2.9.3/deemon/core/api.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/core/config.py` & `deemon-2.9.3/deemon/core/config.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/core/db.py` & `deemon-2.9.3/deemon/core/db.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/core/dmi.py` & `deemon-2.9.3/deemon/core/dmi.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/core/logger.py` & `deemon-2.9.3/deemon/core/logger.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/core/notifier.py` & `deemon-2.9.3/deemon/core/notifier.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/utils/dataprocessor.py` & `deemon-2.9.3/deemon/utils/dataprocessor.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/utils/dates.py` & `deemon-2.9.3/deemon/utils/dates.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/utils/performance.py` & `deemon-2.9.3/deemon/utils/performance.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/utils/startup.py` & `deemon-2.9.3/deemon/utils/startup.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon/utils/ui.py` & `deemon-2.9.3/deemon/utils/ui.py`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/deemon.egg-info/PKG-INFO` & `deemon-2.9.3/deemon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deemon
-Version: 2.9.2
+Version: 2.9.3
 Summary: Monitor new releases by a specified list of artists and auto download using the deemix library
 Home-page: https://github.com/digitalec/deemon
 Author: digitalec
 License: GPL3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `deemon-2.9.2/deemon.egg-info/SOURCES.txt` & `deemon-2.9.3/deemon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deemon-2.9.2/setup.py` & `deemon-2.9.3/setup.py`

 * *Files identical despite different names*

