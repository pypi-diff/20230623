# Comparing `tmp/xfss-0.8.5.tar.gz` & `tmp/xfss-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfss-0.8.5.tar", last modified: Mon Oct 17 06:37:27 2022, max compression
+gzip compressed data, was "xfss-0.9.0.tar", last modified: Fri Jun 23 05:07:29 2023, max compression
```

## Comparing `xfss-0.8.5.tar` & `xfss-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 06:37:27.177766 xfss-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-17 06:37:15.000000 xfss-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-10-17 06:37:27.177766 xfss-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-17 06:37:27.177766 xfss-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-10-17 06:37:15.000000 xfss-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 06:37:27.173766 xfss-0.8.5/xfss/
--rw-r--r--   0 runner    (1001) docker     (121)     4723 2022-10-17 06:37:15.000000 xfss-0.8.5/xfss/Auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-10-17 06:37:15.000000 xfss-0.8.5/xfss/HTTPStatus.py
--rw-r--r--   0 runner    (1001) docker     (121)     8647 2022-10-17 06:37:15.000000 xfss-0.8.5/xfss/RemoteSession.py
--rw-r--r--   0 runner    (1001) docker     (121)     9913 2022-10-17 06:37:15.000000 xfss-0.8.5/xfss/StatefulSession.py
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-10-17 06:37:15.000000 xfss-0.8.5/xfss/TelegramBot.py
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-10-17 06:37:15.000000 xfss-0.8.5/xfss/Util.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-10-17 06:37:15.000000 xfss-0.8.5/xfss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 06:37:27.177766 xfss-0.8.5/xfss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-10-17 06:37:27.000000 xfss-0.8.5/xfss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-10-17 06:37:27.000000 xfss-0.8.5/xfss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 06:37:27.000000 xfss-0.8.5/xfss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-17 06:37:27.000000 xfss-0.8.5/xfss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-17 06:37:27.000000 xfss-0.8.5/xfss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:07:29.246663 xfss-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-23 05:07:17.000000 xfss-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-23 05:07:29.246663 xfss-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 05:07:29.246663 xfss-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-23 05:07:17.000000 xfss-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:07:29.246663 xfss-0.9.0/xfss/
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-23 05:07:17.000000 xfss-0.9.0/xfss/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-23 05:07:17.000000 xfss-0.9.0/xfss/HTTPStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-06-23 05:07:17.000000 xfss-0.9.0/xfss/RemoteSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-23 05:07:17.000000 xfss-0.9.0/xfss/StatefulSession.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-23 05:07:17.000000 xfss-0.9.0/xfss/TelegramBot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-23 05:07:17.000000 xfss-0.9.0/xfss/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-23 05:07:17.000000 xfss-0.9.0/xfss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:07:29.246663 xfss-0.9.0/xfss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-23 05:07:29.000000 xfss-0.9.0/xfss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-23 05:07:29.000000 xfss-0.9.0/xfss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 05:07:29.000000 xfss-0.9.0/xfss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-23 05:07:29.000000 xfss-0.9.0/xfss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 05:07:29.000000 xfss-0.9.0/xfss.egg-info/top_level.txt
```

### Comparing `xfss-0.8.5/LICENSE` & `xfss-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xfss-0.8.5/PKG-INFO` & `xfss-0.9.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfss
-Version: 0.8.5
+Version: 0.9.0
 Summary: A package to handle auth on flask. Made by Xatal
 Home-page: https://github.com/Masakuata/xatal_flask_auth
 Author: Edson Manuel Carballo Vera
 Author-email: edsonmanuelcarballovera@gmail.com
 License: MIT License
 Download-URL: https://pypi.org/project/xf-auth/
 Platform: UNKNOWN
```

### Comparing `xfss-0.8.5/setup.py` & `xfss-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
 	name='xfss',
-	version='0.8.5',
+	version='0.9.0',
 	description='A package to handle auth on flask. Made by Xatal',
 	url='https://github.com/Masakuata/xatal_flask_auth',
 	download_url="https://pypi.org/project/xf-auth/",
 	author='Edson Manuel Carballo Vera',
 	author_email='edsonmanuelcarballovera@gmail.com',
 	license='MIT License',
 	packages=['xfss'],
 	install_requires=[
-		'cryptography==3.1.1',
+		'cryptography==41.0.1',
 		"Flask~=2.2.2",
 		"Werkzeug~=2.2.2",
 		"requests~=2.28.1",
 		"setuptools~=60.2.0",
 		"validators==0.20.0"
 	],
```

### Comparing `xfss-0.8.5/xfss/Auth.py` & `xfss-0.9.0/xfss/Auth.py`

 * *Files identical despite different names*

### Comparing `xfss-0.8.5/xfss/HTTPStatus.py` & `xfss-0.9.0/xfss/HTTPStatus.py`

 * *Files identical despite different names*

### Comparing `xfss-0.8.5/xfss/RemoteSession.py` & `xfss-0.9.0/xfss/RemoteSession.py`

 * *Files identical despite different names*

### Comparing `xfss-0.8.5/xfss/StatefulSession.py` & `xfss-0.9.0/xfss/StatefulSession.py`

 * *Files identical despite different names*

### Comparing `xfss-0.8.5/xfss/TelegramBot.py` & `xfss-0.9.0/xfss/TelegramBot.py`

 * *Files identical despite different names*

### Comparing `xfss-0.8.5/xfss/Util.py` & `xfss-0.9.0/xfss/Util.py`

 * *Files identical despite different names*

### Comparing `xfss-0.8.5/xfss.egg-info/PKG-INFO` & `xfss-0.9.0/xfss.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfss
-Version: 0.8.5
+Version: 0.9.0
 Summary: A package to handle auth on flask. Made by Xatal
 Home-page: https://github.com/Masakuata/xatal_flask_auth
 Author: Edson Manuel Carballo Vera
 Author-email: edsonmanuelcarballovera@gmail.com
 License: MIT License
 Download-URL: https://pypi.org/project/xf-auth/
 Platform: UNKNOWN
```

