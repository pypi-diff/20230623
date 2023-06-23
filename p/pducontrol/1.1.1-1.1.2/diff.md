# Comparing `tmp/pducontrol-1.1.1.tar.gz` & `tmp/pducontrol-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pducontrol-1.1.1.tar", last modified: Wed Jun 21 10:55:41 2023, max compression
+gzip compressed data, was "pducontrol-1.1.2.tar", last modified: Fri Jun 23 07:40:15 2023, max compression
```

## Comparing `pducontrol-1.1.1.tar` & `pducontrol-1.1.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-21 10:55:41.086434 pducontrol-1.1.1/
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       63 2023-05-16 08:14:10.000000 pducontrol-1.1.1/.flake8
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      825 2023-06-08 13:36:39.000000 pducontrol-1.1.1/.gitignore
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      217 2023-05-16 12:35:17.000000 pducontrol-1.1.1/AUTHORS
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)    35149 2023-05-16 12:35:17.000000 pducontrol-1.1.1/COPYING
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     7652 2023-05-16 12:35:17.000000 pducontrol-1.1.1/COPYING.LESSER
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      748 2023-06-21 09:36:00.000000 pducontrol-1.1.1/Makefile
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     2330 2023-06-21 10:55:41.086434 pducontrol-1.1.1/PKG-INFO
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     1532 2023-06-21 09:53:28.000000 pducontrol-1.1.1/README.md
-drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-21 10:55:41.082434 pducontrol-1.1.1/config/
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      221 2023-06-08 13:36:39.000000 pducontrol-1.1.1/config/pdu_settings.cfg
-drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-21 10:55:41.082434 pducontrol-1.1.1/debian/
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      862 2023-06-21 09:53:28.000000 pducontrol-1.1.1/debian/changelog
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      694 2023-06-08 15:02:49.000000 pducontrol-1.1.1/debian/control
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      815 2023-06-08 15:02:49.000000 pducontrol-1.1.1/debian/copyright
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       18 2023-06-08 15:02:49.000000 pducontrol-1.1.1/debian/docs
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       41 2023-06-08 15:02:49.000000 pducontrol-1.1.1/debian/install
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       26 2023-06-08 15:02:49.000000 pducontrol-1.1.1/debian/manpages
--rwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)       88 2023-06-08 15:02:49.000000 pducontrol-1.1.1/debian/rules
-drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-21 10:55:41.082434 pducontrol-1.1.1/debian/source/
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       13 2023-06-08 15:02:49.000000 pducontrol-1.1.1/debian/source/format
-drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-21 10:55:41.078434 pducontrol-1.1.1/docker/
-drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-21 10:55:41.082434 pducontrol-1.1.1/docker/linux/
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      539 2023-06-09 08:07:52.000000 pducontrol-1.1.1/docker/linux/Dockerfile
-drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-21 10:55:41.082434 pducontrol-1.1.1/pducontrol/
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)    10611 2023-06-21 09:36:00.000000 pducontrol-1.1.1/pducontrol/__cli.py
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      835 2023-06-21 09:46:31.000000 pducontrol-1.1.1/pducontrol/__init__.py
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     1236 2023-06-21 09:42:16.000000 pducontrol-1.1.1/pducontrol/__main__.py
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     1413 2023-06-21 09:46:31.000000 pducontrol-1.1.1/pducontrol/__pdu.py
--rwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)     8759 2023-06-21 09:36:00.000000 pducontrol-1.1.1/pducontrol/__pdu8100x.py
--rwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)     6448 2023-06-08 13:36:39.000000 pducontrol-1.1.1/pducontrol/__pdu_swh_1023j.py
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     6202 2023-06-21 09:36:00.000000 pducontrol-1.1.1/pducontrol/__snmp.py
--rwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)       63 2023-05-17 14:18:27.000000 pducontrol-1.1.1/pducontrol-completion.sh
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     1285 2023-06-21 09:43:19.000000 pducontrol-1.1.1/pducontrol.5.md
-drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-21 10:55:41.086434 pducontrol-1.1.1/pducontrol.egg-info/
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     2330 2023-06-21 10:55:40.000000 pducontrol-1.1.1/pducontrol.egg-info/PKG-INFO
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      720 2023-06-21 10:55:40.000000 pducontrol-1.1.1/pducontrol.egg-info/SOURCES.txt
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)        1 2023-06-21 10:55:40.000000 pducontrol-1.1.1/pducontrol.egg-info/dependency_links.txt
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       57 2023-06-21 10:55:40.000000 pducontrol-1.1.1/pducontrol.egg-info/entry_points.txt
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       40 2023-06-21 10:55:40.000000 pducontrol-1.1.1/pducontrol.egg-info/requires.txt
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       11 2023-06-21 10:55:40.000000 pducontrol-1.1.1/pducontrol.egg-info/top_level.txt
--rwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)      887 2023-06-08 13:36:39.000000 pducontrol-1.1.1/refresh_package.sh
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       38 2023-06-21 10:55:41.086434 pducontrol-1.1.1/setup.cfg
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     1839 2023-06-21 08:47:00.000000 pducontrol-1.1.1/setup.py
-drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-21 10:55:41.086434 pducontrol-1.1.1/tests/
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)        0 2023-05-16 15:31:19.000000 pducontrol-1.1.1/tests/__init__.py
--rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     4291 2023-06-21 09:46:31.000000 pducontrol-1.1.1/tests/test_pdu8100x.py
+drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-23 07:40:15.066068 pducontrol-1.1.2/
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       63 2023-05-16 08:14:10.000000 pducontrol-1.1.2/.flake8
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      825 2023-06-08 13:36:39.000000 pducontrol-1.1.2/.gitignore
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      217 2023-05-16 12:35:17.000000 pducontrol-1.1.2/AUTHORS
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)    35149 2023-05-16 12:35:17.000000 pducontrol-1.1.2/COPYING
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     7652 2023-05-16 12:35:17.000000 pducontrol-1.1.2/COPYING.LESSER
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      748 2023-06-21 09:36:00.000000 pducontrol-1.1.2/Makefile
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     2330 2023-06-23 07:40:15.066068 pducontrol-1.1.2/PKG-INFO
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     1532 2023-06-21 09:53:28.000000 pducontrol-1.1.2/README.md
+drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-23 07:40:15.062068 pducontrol-1.1.2/config/
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      221 2023-06-08 13:36:39.000000 pducontrol-1.1.2/config/pdu_settings.cfg
+drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-23 07:40:15.062068 pducontrol-1.1.2/debian/
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     1078 2023-06-22 13:01:51.000000 pducontrol-1.1.2/debian/changelog
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      694 2023-06-08 15:02:49.000000 pducontrol-1.1.2/debian/control
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      815 2023-06-08 15:02:49.000000 pducontrol-1.1.2/debian/copyright
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       18 2023-06-08 15:02:49.000000 pducontrol-1.1.2/debian/docs
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       41 2023-06-08 15:02:49.000000 pducontrol-1.1.2/debian/install
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       26 2023-06-08 15:02:49.000000 pducontrol-1.1.2/debian/manpages
+-rwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)       88 2023-06-08 15:02:49.000000 pducontrol-1.1.2/debian/rules
+drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-23 07:40:15.062068 pducontrol-1.1.2/debian/source/
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       13 2023-06-08 15:02:49.000000 pducontrol-1.1.2/debian/source/format
+drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-23 07:40:15.058068 pducontrol-1.1.2/docker/
+drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-23 07:40:15.062068 pducontrol-1.1.2/docker/linux/
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      539 2023-06-09 08:07:52.000000 pducontrol-1.1.2/docker/linux/Dockerfile
+drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-23 07:40:15.062068 pducontrol-1.1.2/pducontrol/
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)    10611 2023-06-21 09:36:00.000000 pducontrol-1.1.2/pducontrol/__cli.py
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      835 2023-06-21 09:46:31.000000 pducontrol-1.1.2/pducontrol/__init__.py
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     1236 2023-06-21 09:42:16.000000 pducontrol-1.1.2/pducontrol/__main__.py
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     1413 2023-06-21 09:46:31.000000 pducontrol-1.1.2/pducontrol/__pdu.py
+-rwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)     8759 2023-06-21 09:36:00.000000 pducontrol-1.1.2/pducontrol/__pdu8100x.py
+-rwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)     6448 2023-06-08 13:36:39.000000 pducontrol-1.1.2/pducontrol/__pdu_swh_1023j.py
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     6202 2023-06-21 09:36:00.000000 pducontrol-1.1.2/pducontrol/__snmp.py
+-rwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)      192 2023-06-22 13:01:51.000000 pducontrol-1.1.2/pducontrol-completion.sh
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     1285 2023-06-21 09:43:19.000000 pducontrol-1.1.2/pducontrol.5.md
+drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-23 07:40:15.062068 pducontrol-1.1.2/pducontrol.egg-info/
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     2330 2023-06-23 07:40:14.000000 pducontrol-1.1.2/pducontrol.egg-info/PKG-INFO
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)      739 2023-06-23 07:40:14.000000 pducontrol-1.1.2/pducontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)        1 2023-06-23 07:40:14.000000 pducontrol-1.1.2/pducontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       57 2023-06-23 07:40:14.000000 pducontrol-1.1.2/pducontrol.egg-info/entry_points.txt
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       40 2023-06-23 07:40:14.000000 pducontrol-1.1.2/pducontrol.egg-info/requires.txt
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       11 2023-06-23 07:40:14.000000 pducontrol-1.1.2/pducontrol.egg-info/top_level.txt
+-rwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)      887 2023-06-08 13:36:39.000000 pducontrol-1.1.2/refresh_package.sh
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)       38 2023-06-23 07:40:15.066068 pducontrol-1.1.2/setup.cfg
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     1839 2023-06-22 13:01:51.000000 pducontrol-1.1.2/setup.py
+drwxr-xr-x   0 ncarrier  (1000) ncarrier  (1000)        0 2023-06-23 07:40:15.062068 pducontrol-1.1.2/tests/
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)        0 2023-05-16 15:31:19.000000 pducontrol-1.1.2/tests/__init__.py
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     4291 2023-06-21 09:46:31.000000 pducontrol-1.1.2/tests/test_pdu8100x.py
+-rw-r--r--   0 ncarrier  (1000) ncarrier  (1000)     2386 2023-06-22 12:30:09.000000 pducontrol-1.1.2/tests/test_snmp.py
```

### Comparing `pducontrol-1.1.1/.gitignore` & `pducontrol-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/COPYING` & `pducontrol-1.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/COPYING.LESSER` & `pducontrol-1.1.2/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/Makefile` & `pducontrol-1.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/PKG-INFO` & `pducontrol-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pducontrol
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple package to control PDUs
 Home-page: https://bitbucket.org/spectracom/pdu-control/src/master/
 Author: Pol Bodet, Nicolas Carrier, Jeremy Connat, Jai Mehra
 Author-email: pol.bodet@orolia.com
 License: LGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pducontrol-1.1.1/README.md` & `pducontrol-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/debian/changelog` & `pducontrol-1.1.2/debian/changelog`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+pdu-control (1.1.2) UNRELEASED; urgency=medium
+
+  * adapt to register-python-argcomplete having different names
+
+ -- Safran Trusted 4D SAS <timingsupport@nav-timing.safrangroup.com>  Wed, 22 Jun 2023 14:31:28 +0200
+
 pdu-control (1.1.1) UNRELEASED; urgency=medium
 
   * fix pip packaging issues
   * make functions in __main__.py private
 
  -- Safran Trusted 4D SAS <timingsupport@nav-timing.safrangroup.com>  Wed, 21 Jun 2023 10:48:00 +0200
```

### Comparing `pducontrol-1.1.1/debian/control` & `pducontrol-1.1.2/debian/control`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/debian/copyright` & `pducontrol-1.1.2/debian/copyright`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/docker/linux/Dockerfile` & `pducontrol-1.1.2/docker/linux/Dockerfile`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/pducontrol/__cli.py` & `pducontrol-1.1.2/pducontrol/__cli.py`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/pducontrol/__init__.py` & `pducontrol-1.1.2/pducontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/pducontrol/__main__.py` & `pducontrol-1.1.2/pducontrol/__main__.py`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/pducontrol/__pdu.py` & `pducontrol-1.1.2/pducontrol/__pdu.py`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/pducontrol/__pdu8100x.py` & `pducontrol-1.1.2/pducontrol/__pdu8100x.py`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/pducontrol/__pdu_swh_1023j.py` & `pducontrol-1.1.2/pducontrol/__pdu_swh_1023j.py`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/pducontrol/__snmp.py` & `pducontrol-1.1.2/pducontrol/__snmp.py`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/pducontrol.5.md` & `pducontrol-1.1.2/pducontrol.5.md`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/pducontrol.egg-info/PKG-INFO` & `pducontrol-1.1.2/pducontrol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pducontrol
-Version: 1.1.1
+Version: 1.1.2
 Summary: A simple package to control PDUs
 Home-page: https://bitbucket.org/spectracom/pdu-control/src/master/
 Author: Pol Bodet, Nicolas Carrier, Jeremy Connat, Jai Mehra
 Author-email: pol.bodet@orolia.com
 License: LGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pducontrol-1.1.1/pducontrol.egg-info/SOURCES.txt` & `pducontrol-1.1.2/pducontrol.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 pducontrol.egg-info/PKG-INFO
 pducontrol.egg-info/SOURCES.txt
 pducontrol.egg-info/dependency_links.txt
 pducontrol.egg-info/entry_points.txt
 pducontrol.egg-info/requires.txt
 pducontrol.egg-info/top_level.txt
 tests/__init__.py
-tests/test_pdu8100x.py
+tests/test_pdu8100x.py
+tests/test_snmp.py
```

### Comparing `pducontrol-1.1.1/refresh_package.sh` & `pducontrol-1.1.2/refresh_package.sh`

 * *Files identical despite different names*

### Comparing `pducontrol-1.1.1/setup.py` & `pducontrol-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='pducontrol',
-    version='1.1.1',
+    version='1.1.2',
     packages=["pducontrol"],
     entry_points={
         'console_scripts': [
             'pducontrol=pducontrol.__main__:main'
         ]
     },
     install_requires=[
```

### Comparing `pducontrol-1.1.1/tests/test_pdu8100x.py` & `pducontrol-1.1.2/tests/test_pdu8100x.py`

 * *Files identical despite different names*

