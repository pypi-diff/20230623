# Comparing `tmp/watchtower_browser_testing-0.5.0.tar.gz` & `tmp/watchtower_browser_testing-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.5.0.tar", last modified: Fri Jun 23 09:33:44 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.5.1.tar", last modified: Fri Jun 23 09:35:51 2023, max compression
```

## Comparing `watchtower_browser_testing-0.5.0.tar` & `watchtower_browser_testing-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 09:33:44.945702 watchtower_browser_testing-0.5.0/
--rw-rw-rw-   0        0        0      310 2023-06-23 09:33:44.944957 watchtower_browser_testing-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 09:33:44.946643 watchtower_browser_testing-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:33:44.929399 watchtower_browser_testing-0.5.0/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      204 2023-06-23 08:52:43.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      987 2023-06-13 13:37:35.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     3780 2023-06-23 09:08:00.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:33:44.934942 watchtower_browser_testing-0.5.0/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    18953 2023-06-13 13:52:56.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     9442 2023-06-23 09:08:00.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0      191 2023-05-20 15:42:04.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing/utils.py
--rw-rw-rw-   0        0        0       21 2023-06-23 09:33:19.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:33:44.934942 watchtower_browser_testing-0.5.0/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-06-23 09:33:44.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-06-23 09:33:44.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 09:33:44.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-23 09:33:44.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-23 09:33:44.000000 watchtower_browser_testing-0.5.0/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 09:35:51.365560 watchtower_browser_testing-0.5.1/
+-rw-rw-rw-   0        0        0      310 2023-06-23 09:35:51.365560 watchtower_browser_testing-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 09:35:51.365560 watchtower_browser_testing-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:35:51.358464 watchtower_browser_testing-0.5.1/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      241 2023-06-23 09:35:42.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      987 2023-06-13 13:37:35.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     3780 2023-06-23 09:08:00.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:35:51.365560 watchtower_browser_testing-0.5.1/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    18953 2023-06-13 13:52:56.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     9442 2023-06-23 09:08:00.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0      191 2023-05-20 15:42:04.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/utils.py
+-rw-rw-rw-   0        0        0       21 2023-06-23 09:35:42.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:35:51.365560 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-06-23 09:35:51.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-06-23 09:35:51.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 09:35:51.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-23 09:35:51.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-23 09:35:51.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.5.0/setup.py` & `watchtower_browser_testing-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.0/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.5.1/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.0/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.5.1/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.0/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.5.1/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.0/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.5.1/watchtower_browser_testing/testsuite.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.0/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.5.1/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.0/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

