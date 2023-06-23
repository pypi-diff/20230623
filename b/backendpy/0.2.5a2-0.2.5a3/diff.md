# Comparing `tmp/backendpy-0.2.5a2.tar.gz` & `tmp/backendpy-0.2.5a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backendpy-0.2.5a2.tar", last modified: Sat May 13 10:57:36 2023, max compression
+gzip compressed data, was "backendpy-0.2.5a3.tar", last modified: Fri Jun 23 15:21:12 2023, max compression
```

## Comparing `backendpy-0.2.5a2.tar` & `backendpy-0.2.5a3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-13 10:57:36.810663 backendpy-0.2.5a2/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1517 2022-01-24 11:39:51.000000 backendpy-0.2.5a2/LICENSE
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-05-13 10:57:36.814663 backendpy-0.2.5a2/PKG-INFO
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2543 2022-12-24 20:09:28.000000 backendpy-0.2.5a2/README.md
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-13 10:57:36.662669 backendpy-0.2.5a2/backendpy/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       27 2022-02-20 19:27:36.000000 backendpy-0.2.5a2/backendpy/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1965 2022-08-26 21:11:09.000000 backendpy-0.2.5a2/backendpy/app.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    10027 2023-01-02 18:54:04.000000 backendpy-0.2.5a2/backendpy/asgi.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-13 10:57:36.678668 backendpy-0.2.5a2/backendpy/cli/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-06-05 08:33:23.000000 backendpy-0.2.5a2/backendpy/cli/__init__.py
--rwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)    15657 2022-12-27 08:15:36.000000 backendpy-0.2.5a2/backendpy/cli/admin.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2601 2022-12-10 12:10:57.000000 backendpy-0.2.5a2/backendpy/config.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-13 10:57:36.714667 backendpy-0.2.5a2/backendpy/data_handler/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-08-27 14:31:27.000000 backendpy-0.2.5a2/backendpy/data_handler/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3476 2023-01-04 01:03:30.000000 backendpy-0.2.5a2/backendpy/data_handler/data.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5370 2023-01-03 19:42:13.000000 backendpy-0.2.5a2/backendpy/data_handler/fields.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4609 2023-01-12 22:24:35.000000 backendpy-0.2.5a2/backendpy/data_handler/filters.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    21377 2023-04-02 12:48:01.000000 backendpy-0.2.5a2/backendpy/data_handler/validators.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4099 2022-12-10 12:07:53.000000 backendpy-0.2.5a2/backendpy/db.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5125 2023-01-03 03:06:50.000000 backendpy-0.2.5a2/backendpy/error.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5129 2023-01-03 03:06:50.000000 backendpy-0.2.5a2/backendpy/exception.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3090 2022-02-27 14:42:53.000000 backendpy-0.2.5a2/backendpy/hook.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1453 2022-08-26 21:56:05.000000 backendpy-0.2.5a2/backendpy/initializer.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1598 2022-05-20 16:53:26.000000 backendpy-0.2.5a2/backendpy/logging.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-13 10:57:36.738666 backendpy-0.2.5a2/backendpy/middleware/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       35 2022-12-27 07:51:13.000000 backendpy-0.2.5a2/backendpy/middleware/__init__.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-13 10:57:36.754665 backendpy-0.2.5a2/backendpy/middleware/defaults/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2022-12-27 07:51:11.000000 backendpy-0.2.5a2/backendpy/middleware/defaults/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5825 2022-12-27 08:01:32.000000 backendpy-0.2.5a2/backendpy/middleware/defaults/cors.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3973 2022-12-27 08:01:32.000000 backendpy-0.2.5a2/backendpy/middleware/middleware.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     9319 2023-01-04 01:13:10.000000 backendpy-0.2.5a2/backendpy/request.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    17355 2023-05-11 10:44:24.000000 backendpy-0.2.5a2/backendpy/response.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    13275 2023-03-20 19:22:31.000000 backendpy-0.2.5a2/backendpy/router.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2918 2022-06-04 13:28:58.000000 backendpy-0.2.5a2/backendpy/templating.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      908 2022-05-20 16:53:26.000000 backendpy-0.2.5a2/backendpy/unittest.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-13 10:57:36.798663 backendpy-0.2.5a2/backendpy/utils/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2019-10-11 09:00:54.000000 backendpy-0.2.5a2/backendpy/utils/__init__.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      258 2022-01-23 06:37:37.000000 backendpy-0.2.5a2/backendpy/utils/bytes.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    13121 2023-05-13 10:40:37.000000 backendpy-0.2.5a2/backendpy/utils/file.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4630 2023-01-29 02:21:14.000000 backendpy-0.2.5a2/backendpy/utils/http.py
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      477 2022-02-27 20:01:42.000000 backendpy-0.2.5a2/backendpy/utils/json.py
-drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-05-13 10:57:36.678668 backendpy-0.2.5a2/backendpy.egg-info/
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-05-13 10:57:36.000000 backendpy-0.2.5a2/backendpy.egg-info/PKG-INFO
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1042 2023-05-13 10:57:36.000000 backendpy-0.2.5a2/backendpy.egg-info/SOURCES.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        1 2023-05-13 10:57:36.000000 backendpy-0.2.5a2/backendpy.egg-info/dependency_links.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       55 2023-05-13 10:57:36.000000 backendpy-0.2.5a2/backendpy.egg-info/entry_points.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      100 2023-05-13 10:57:36.000000 backendpy-0.2.5a2/backendpy.egg-info/requires.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       10 2023-05-13 10:57:36.000000 backendpy-0.2.5a2/backendpy.egg-info/top_level.txt
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      105 2021-09-12 18:23:47.000000 backendpy-0.2.5a2/pyproject.toml
--rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1426 2023-05-13 10:57:36.818663 backendpy-0.2.5a2/setup.cfg
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-06-23 15:21:12.979828 backendpy-0.2.5a3/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1517 2022-01-24 11:39:51.000000 backendpy-0.2.5a3/LICENSE
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-06-23 15:21:12.979828 backendpy-0.2.5a3/PKG-INFO
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2543 2022-12-24 20:09:28.000000 backendpy-0.2.5a3/README.md
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-06-23 15:21:12.799834 backendpy-0.2.5a3/backendpy/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       27 2022-02-20 19:27:36.000000 backendpy-0.2.5a3/backendpy/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1965 2022-08-26 21:11:09.000000 backendpy-0.2.5a3/backendpy/app.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    10027 2023-01-02 18:54:04.000000 backendpy-0.2.5a3/backendpy/asgi.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-06-23 15:21:12.819833 backendpy-0.2.5a3/backendpy/cli/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-06-05 08:33:23.000000 backendpy-0.2.5a3/backendpy/cli/__init__.py
+-rwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)    15657 2022-12-27 08:15:36.000000 backendpy-0.2.5a3/backendpy/cli/admin.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2601 2022-12-10 12:10:57.000000 backendpy-0.2.5a3/backendpy/config.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-06-23 15:21:12.875831 backendpy-0.2.5a3/backendpy/data_handler/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2020-08-27 14:31:27.000000 backendpy-0.2.5a3/backendpy/data_handler/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3476 2023-01-04 01:03:30.000000 backendpy-0.2.5a3/backendpy/data_handler/data.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5370 2023-01-03 19:42:13.000000 backendpy-0.2.5a3/backendpy/data_handler/fields.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4609 2023-01-12 22:24:35.000000 backendpy-0.2.5a3/backendpy/data_handler/filters.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    21377 2023-04-02 12:48:01.000000 backendpy-0.2.5a3/backendpy/data_handler/validators.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4099 2022-12-10 12:07:53.000000 backendpy-0.2.5a3/backendpy/db.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5125 2023-01-03 03:06:50.000000 backendpy-0.2.5a3/backendpy/error.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5129 2023-01-03 03:06:50.000000 backendpy-0.2.5a3/backendpy/exception.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3090 2022-02-27 14:42:53.000000 backendpy-0.2.5a3/backendpy/hook.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1453 2022-08-26 21:56:05.000000 backendpy-0.2.5a3/backendpy/initializer.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1598 2022-05-20 16:53:26.000000 backendpy-0.2.5a3/backendpy/logging.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-06-23 15:21:12.907830 backendpy-0.2.5a3/backendpy/middleware/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       35 2022-12-27 07:51:13.000000 backendpy-0.2.5a3/backendpy/middleware/__init__.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-06-23 15:21:12.919830 backendpy-0.2.5a3/backendpy/middleware/defaults/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2022-12-27 07:51:11.000000 backendpy-0.2.5a3/backendpy/middleware/defaults/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     5825 2022-12-27 08:01:32.000000 backendpy-0.2.5a3/backendpy/middleware/defaults/cors.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3973 2022-12-27 08:01:32.000000 backendpy-0.2.5a3/backendpy/middleware/middleware.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     9342 2023-06-23 15:18:12.000000 backendpy-0.2.5a3/backendpy/request.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    17355 2023-05-11 10:44:24.000000 backendpy-0.2.5a3/backendpy/response.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    13275 2023-03-20 19:22:31.000000 backendpy-0.2.5a3/backendpy/router.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     2918 2022-06-04 13:28:58.000000 backendpy-0.2.5a3/backendpy/templating.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      908 2022-05-20 16:53:26.000000 backendpy-0.2.5a3/backendpy/unittest.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-06-23 15:21:12.967828 backendpy-0.2.5a3/backendpy/utils/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        0 2019-10-11 09:00:54.000000 backendpy-0.2.5a3/backendpy/utils/__init__.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      258 2022-01-23 06:37:37.000000 backendpy-0.2.5a3/backendpy/utils/bytes.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)    13118 2023-06-19 16:28:04.000000 backendpy-0.2.5a3/backendpy/utils/file.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     4630 2023-01-29 02:21:14.000000 backendpy-0.2.5a3/backendpy/utils/http.py
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      477 2022-02-27 20:01:42.000000 backendpy-0.2.5a3/backendpy/utils/json.py
+drwxrwxr-x   0 hamdollahi  (1000) hamdollahi  (1000)        0 2023-06-23 15:21:12.815833 backendpy-0.2.5a3/backendpy.egg-info/
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     3810 2023-06-23 15:21:12.000000 backendpy-0.2.5a3/backendpy.egg-info/PKG-INFO
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1042 2023-06-23 15:21:12.000000 backendpy-0.2.5a3/backendpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)        1 2023-06-23 15:21:12.000000 backendpy-0.2.5a3/backendpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       55 2023-06-23 15:21:12.000000 backendpy-0.2.5a3/backendpy.egg-info/entry_points.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      100 2023-06-23 15:21:12.000000 backendpy-0.2.5a3/backendpy.egg-info/requires.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)       10 2023-06-23 15:21:12.000000 backendpy-0.2.5a3/backendpy.egg-info/top_level.txt
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)      105 2021-09-12 18:23:47.000000 backendpy-0.2.5a3/pyproject.toml
+-rw-rw-r--   0 hamdollahi  (1000) hamdollahi  (1000)     1426 2023-06-23 15:21:12.983828 backendpy-0.2.5a3/setup.cfg
```

### Comparing `backendpy-0.2.5a2/LICENSE` & `backendpy-0.2.5a3/LICENSE`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/PKG-INFO` & `backendpy-0.2.5a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backendpy
-Version: 0.2.5a2
+Version: 0.2.5a3
 Summary: Async (ASGI) Python web framework
 Home-page: https://github.com/savangco/backendpy
 Author: Savang Co.
 Author-email: backendpy@savang.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/savangco/backendpy/issues
 Project-URL: Documentation, https://backendpy.readthedocs.io
```

### Comparing `backendpy-0.2.5a2/README.md` & `backendpy-0.2.5a3/README.md`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/app.py` & `backendpy-0.2.5a3/backendpy/app.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/asgi.py` & `backendpy-0.2.5a3/backendpy/asgi.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/cli/admin.py` & `backendpy-0.2.5a3/backendpy/cli/admin.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/config.py` & `backendpy-0.2.5a3/backendpy/config.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/data_handler/data.py` & `backendpy-0.2.5a3/backendpy/data_handler/data.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/data_handler/fields.py` & `backendpy-0.2.5a3/backendpy/data_handler/fields.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/data_handler/filters.py` & `backendpy-0.2.5a3/backendpy/data_handler/filters.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/data_handler/validators.py` & `backendpy-0.2.5a3/backendpy/data_handler/validators.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/db.py` & `backendpy-0.2.5a3/backendpy/db.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/error.py` & `backendpy-0.2.5a3/backendpy/error.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/exception.py` & `backendpy-0.2.5a3/backendpy/exception.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/hook.py` & `backendpy-0.2.5a3/backendpy/hook.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/initializer.py` & `backendpy-0.2.5a3/backendpy/initializer.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/logging.py` & `backendpy-0.2.5a3/backendpy/logging.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/middleware/defaults/cors.py` & `backendpy-0.2.5a3/backendpy/middleware/defaults/cors.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/middleware/middleware.py` & `backendpy-0.2.5a3/backendpy/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/request.py` & `backendpy-0.2.5a3/backendpy/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         """Parse and set the received request body"""
         if body:
             if self._content_type == 'application/json':
                 self.json = from_json(body)
             elif self._content_type == 'application/x-www-form-urlencoded':
                 self.form = {k: (v[0] if len(v) == 1 else v)
                              for k, v in parse_qs(body.decode('utf8')).items()}
-            elif self._content_type.startswith('multipart/form-data'):
+            elif self._content_type and self._content_type.startswith('multipart/form-data'):
                 self.form = dict()
                 self.files = dict()
                 body = str.encode(f'content-type: {self._content_type}\n') + body
                 for part in parser.BytesParser().parsebytes(body).get_payload():
                     if part.get_param(param='filename', header='content-disposition'):
                         self.files[part.get_param(param='name', header='content-disposition')] = \
                             {'content': part.get_payload(decode=True),
```

### Comparing `backendpy-0.2.5a2/backendpy/response.py` & `backendpy-0.2.5a3/backendpy/response.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/router.py` & `backendpy-0.2.5a3/backendpy/router.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/templating.py` & `backendpy-0.2.5a3/backendpy/templating.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/unittest.py` & `backendpy-0.2.5a3/backendpy/unittest.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy/utils/file.py` & `backendpy-0.2.5a3/backendpy/utils/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,18 +109,18 @@
             await aiofiles.os.remove(path)
         except:
             pass
         return not os.path.exists(path)
     return False
 
 
-async def remove_file(path):
-    if os.path.isfile(path):
+async def remove_dir(path):
+    if os.path.isdir(path):
         try:
-            await aiofiles.os.remove(path)
+            await aiofiles.os.rmdir(path)
         except:
             pass
         return not os.path.exists(path)
     return False
 
 
 async def get_checksum(data=b'', path=None, chunk_size=32768):
```

### Comparing `backendpy-0.2.5a2/backendpy/utils/http.py` & `backendpy-0.2.5a3/backendpy/utils/http.py`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/backendpy.egg-info/PKG-INFO` & `backendpy-0.2.5a3/backendpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backendpy
-Version: 0.2.5a2
+Version: 0.2.5a3
 Summary: Async (ASGI) Python web framework
 Home-page: https://github.com/savangco/backendpy
 Author: Savang Co.
 Author-email: backendpy@savang.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/savangco/backendpy/issues
 Project-URL: Documentation, https://backendpy.readthedocs.io
```

### Comparing `backendpy-0.2.5a2/backendpy.egg-info/SOURCES.txt` & `backendpy-0.2.5a3/backendpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backendpy-0.2.5a2/setup.cfg` & `backendpy-0.2.5a3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = backendpy
-version = v0.2.5-alpha.2
+version = v0.2.5-alpha.3
 author = Savang Co.
 author_email = backendpy@savang.com
 description = Async (ASGI) Python web framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Backendpy, Web, Framework, Python, Async, ASGI
 license = BSD 3-Clause License
```

