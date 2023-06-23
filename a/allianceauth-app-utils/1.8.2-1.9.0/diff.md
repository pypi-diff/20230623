# Comparing `tmp/allianceauth-app-utils-1.8.2.tar.gz` & `tmp/allianceauth-app-utils-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/allianceauth-app-utils-1.8.2.tar", last modified: Fri Nov 12 10:42:00 2021, max compression
+gzip compressed data, was "dist/allianceauth-app-utils-1.9.0.tar", last modified: Wed Dec 22 16:49:17 2021, max compression
```

## Comparing `allianceauth-app-utils-1.8.2.tar` & `allianceauth-app-utils-1.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-12 10:42:00.000000 allianceauth-app-utils-1.8.2/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2021-02-08 23:03:19.000000 allianceauth-app-utils-1.8.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       67 2021-02-08 23:03:19.000000 allianceauth-app-utils-1.8.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2915 2021-11-12 10:42:00.000000 allianceauth-app-utils-1.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1868 2021-02-20 11:24:47.000000 allianceauth-app-utils-1.8.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-12 10:42:00.000000 allianceauth-app-utils-1.8.2/allianceauth_app_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2915 2021-11-12 10:42:00.000000 allianceauth-app-utils-1.8.2/allianceauth_app_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2021-11-12 10:42:00.000000 allianceauth-app-utils-1.8.2/allianceauth_app_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-12 10:42:00.000000 allianceauth-app-utils-1.8.2/allianceauth_app_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2021-11-12 10:42:00.000000 allianceauth-app-utils-1.8.2/allianceauth_app_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2021-11-12 10:42:00.000000 allianceauth-app-utils-1.8.2/allianceauth_app_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-12 10:42:00.000000 allianceauth-app-utils-1.8.2/app_utils/
--rw-rw-rw-   0 root         (0) root         (0)       59 2021-11-12 10:22:40.000000 allianceauth-app-utils-1.8.2/app_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      988 2021-07-02 12:37:13.000000 allianceauth-app-utils-1.8.2/app_utils/_app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3112 2021-07-14 13:19:04.000000 allianceauth-app-utils-1.8.2/app_utils/allianceauth.py
--rw-rw-rw-   0 root         (0) root         (0)     2521 2021-02-27 18:26:16.000000 allianceauth-app-utils-1.8.2/app_utils/caching.py
--rw-rw-rw-   0 root         (0) root         (0)     2425 2021-05-06 13:13:37.000000 allianceauth-app-utils-1.8.2/app_utils/datetime.py
--rw-rw-rw-   0 root         (0) root         (0)     5210 2021-11-03 14:55:13.000000 allianceauth-app-utils-1.8.2/app_utils/django.py
--rw-rw-rw-   0 root         (0) root         (0)     7100 2021-11-12 10:22:40.000000 allianceauth-app-utils-1.8.2/app_utils/esi.py
--rw-rw-rw-   0 root         (0) root         (0)     6926 2021-04-16 19:47:39.000000 allianceauth-app-utils-1.8.2/app_utils/esi_testing.py
--rw-rw-rw-   0 root         (0) root         (0)     2594 2021-07-01 17:51:15.000000 allianceauth-app-utils-1.8.2/app_utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2021-02-27 18:26:16.000000 allianceauth-app-utils-1.8.2/app_utils/json.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2021-02-27 18:26:16.000000 allianceauth-app-utils-1.8.2/app_utils/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1479 2021-06-29 14:09:35.000000 allianceauth-app-utils-1.8.2/app_utils/messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9787 2021-07-14 13:19:04.000000 allianceauth-app-utils-1.8.2/app_utils/testing.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2021-05-06 13:13:37.000000 allianceauth-app-utils-1.8.2/app_utils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     7159 2021-10-29 14:55:35.000000 allianceauth-app-utils-1.8.2/app_utils/views.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-11-12 10:42:00.000000 allianceauth-app-utils-1.8.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1798 2021-10-29 14:55:35.000000 allianceauth-app-utils-1.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 16:49:17.000000 allianceauth-app-utils-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2021-02-08 23:03:19.000000 allianceauth-app-utils-1.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       67 2021-02-08 23:03:19.000000 allianceauth-app-utils-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2915 2021-12-22 16:49:17.000000 allianceauth-app-utils-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2021-02-20 11:24:47.000000 allianceauth-app-utils-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 16:49:17.000000 allianceauth-app-utils-1.9.0/allianceauth_app_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2915 2021-12-22 16:49:17.000000 allianceauth-app-utils-1.9.0/allianceauth_app_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2021-12-22 16:49:17.000000 allianceauth-app-utils-1.9.0/allianceauth_app_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-22 16:49:17.000000 allianceauth-app-utils-1.9.0/allianceauth_app_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2021-12-22 16:49:17.000000 allianceauth-app-utils-1.9.0/allianceauth_app_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2021-12-22 16:49:17.000000 allianceauth-app-utils-1.9.0/allianceauth_app_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 16:49:17.000000 allianceauth-app-utils-1.9.0/app_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       59 2021-12-22 16:33:14.000000 allianceauth-app-utils-1.9.0/app_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      988 2021-07-02 12:37:13.000000 allianceauth-app-utils-1.9.0/app_utils/_app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2021-07-14 13:19:04.000000 allianceauth-app-utils-1.9.0/app_utils/allianceauth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2521 2021-02-27 18:26:16.000000 allianceauth-app-utils-1.9.0/app_utils/caching.py
+-rw-rw-rw-   0 root         (0) root         (0)     2425 2021-05-06 13:13:37.000000 allianceauth-app-utils-1.9.0/app_utils/datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)     5210 2021-11-03 14:55:13.000000 allianceauth-app-utils-1.9.0/app_utils/django.py
+-rw-rw-rw-   0 root         (0) root         (0)     7100 2021-11-12 10:22:40.000000 allianceauth-app-utils-1.9.0/app_utils/esi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6926 2021-04-16 19:47:39.000000 allianceauth-app-utils-1.9.0/app_utils/esi_testing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2021-12-22 16:33:14.000000 allianceauth-app-utils-1.9.0/app_utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2021-02-27 18:26:16.000000 allianceauth-app-utils-1.9.0/app_utils/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2021-02-27 18:26:16.000000 allianceauth-app-utils-1.9.0/app_utils/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1479 2021-06-29 14:09:35.000000 allianceauth-app-utils-1.9.0/app_utils/messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9787 2021-07-14 13:19:04.000000 allianceauth-app-utils-1.9.0/app_utils/testing.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2021-05-06 13:13:37.000000 allianceauth-app-utils-1.9.0/app_utils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     7159 2021-10-29 14:55:35.000000 allianceauth-app-utils-1.9.0/app_utils/views.py
+-rw-r--r--   0 root         (0) root         (0)       38 2021-12-22 16:49:17.000000 allianceauth-app-utils-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2021-10-29 14:55:35.000000 allianceauth-app-utils-1.9.0/setup.py
```

### Comparing `allianceauth-app-utils-1.8.2/LICENSE` & `allianceauth-app-utils-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/PKG-INFO` & `allianceauth-app-utils-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-app-utils
-Version: 1.8.2
+Version: 1.9.0
 Summary: Commonly used utility functions and classes for rapid development of Alliance Auth apps.
 Home-page: https://gitlab.com/ErikKalkoken/allianceauth-app-utils
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `allianceauth-app-utils-1.8.2/README.md` & `allianceauth-app-utils-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/allianceauth_app_utils.egg-info/PKG-INFO` & `allianceauth-app-utils-1.9.0/allianceauth_app_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-app-utils
-Version: 1.8.2
+Version: 1.9.0
 Summary: Commonly used utility functions and classes for rapid development of Alliance Auth apps.
 Home-page: https://gitlab.com/ErikKalkoken/allianceauth-app-utils
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `allianceauth-app-utils-1.8.2/allianceauth_app_utils.egg-info/SOURCES.txt` & `allianceauth-app-utils-1.9.0/allianceauth_app_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/_app_settings.py` & `allianceauth-app-utils-1.9.0/app_utils/_app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/allianceauth.py` & `allianceauth-app-utils-1.9.0/app_utils/allianceauth.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/caching.py` & `allianceauth-app-utils-1.9.0/app_utils/caching.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/datetime.py` & `allianceauth-app-utils-1.9.0/app_utils/datetime.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/django.py` & `allianceauth-app-utils-1.9.0/app_utils/django.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/esi.py` & `allianceauth-app-utils-1.9.0/app_utils/esi.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/esi_testing.py` & `allianceauth-app-utils-1.9.0/app_utils/esi_testing.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/helpers.py` & `allianceauth-app-utils-1.9.0/app_utils/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
 def chunks(lst, size):
     """Yield successive sized chunks from lst."""
     for i in range(0, len(lst), size):
         yield lst[i : i + size]
 
 
+def default_if_none(value, default):
+    """Return default if value is None."""
+    if value is None:
+        return default
+    return value
+
+
 # old: get_swagger_spec_path
 def swagger_spec_path() -> str:
     """returns the path to the current esi swagger spec file"""
     return os.path.join(os.path.dirname(os.path.abspath(__file__)), "swagger.json")
 
 
 def random_string(char_count: int) -> str:
```

### Comparing `allianceauth-app-utils-1.8.2/app_utils/json.py` & `allianceauth-app-utils-1.9.0/app_utils/json.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/logging.py` & `allianceauth-app-utils-1.9.0/app_utils/logging.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/messages.py` & `allianceauth-app-utils-1.9.0/app_utils/messages.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/testing.py` & `allianceauth-app-utils-1.9.0/app_utils/testing.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/urls.py` & `allianceauth-app-utils-1.9.0/app_utils/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/app_utils/views.py` & `allianceauth-app-utils-1.9.0/app_utils/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-app-utils-1.8.2/setup.py` & `allianceauth-app-utils-1.9.0/setup.py`

 * *Files identical despite different names*

