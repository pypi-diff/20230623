# Comparing `tmp/napalm_nokia_olt-0.0.3.tar.gz` & `tmp/napalm_nokia_olt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nahanga/Desktop/NOKIA/napalm_nokia_olt/dist/.tmp-ld3l_zj6/napalm_nokia_olt-0.0.3.tar", last modified: Fri Jun 23 15:19:08 2023, max compression
+gzip compressed data, was "/Users/nahanga/Desktop/NOKIA/napalm_nokia_olt/dist/.tmp-7wcs4_cw/napalm_nokia_olt-0.0.4.tar", last modified: Fri Jun 23 15:21:55 2023, max compression
```

## Comparing `napalm_nokia_olt-0.0.3.tar` & `napalm_nokia_olt-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:19:08.119769 napalm_nokia_olt-0.0.3/
--rw-r--r--   0 nahanga    (501) staff       (20)    11324 2022-08-16 08:37:40.000000 napalm_nokia_olt-0.0.3/LICENSE.md
--rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-23 15:19:08.119945 napalm_nokia_olt-0.0.3/PKG-INFO
--rw-r--r--   0 nahanga    (501) staff       (20)      167 2023-02-10 17:17:02.000000 napalm_nokia_olt-0.0.3/README.md
-drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:19:08.096707 napalm_nokia_olt-0.0.3/napalm_nokia_olt/
--rw-r--r--   0 nahanga    (501) staff       (20)      115 2023-02-10 17:39:46.000000 napalm_nokia_olt-0.0.3/napalm_nokia_olt/__init__.py
--rw-r--r--   0 nahanga    (501) staff       (20)    10162 2023-06-23 15:13:18.000000 napalm_nokia_olt-0.0.3/napalm_nokia_olt/nokia_olt.py
-drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:19:08.119332 napalm_nokia_olt-0.0.3/napalm_nokia_olt.egg-info/
--rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-23 15:19:08.000000 napalm_nokia_olt-0.0.3/napalm_nokia_olt.egg-info/PKG-INFO
--rw-r--r--   0 nahanga    (501) staff       (20)      297 2023-06-23 15:19:08.000000 napalm_nokia_olt-0.0.3/napalm_nokia_olt.egg-info/SOURCES.txt
--rw-r--r--   0 nahanga    (501) staff       (20)        1 2023-06-23 15:19:08.000000 napalm_nokia_olt-0.0.3/napalm_nokia_olt.egg-info/dependency_links.txt
--rw-r--r--   0 nahanga    (501) staff       (20)       10 2023-06-23 15:19:08.000000 napalm_nokia_olt-0.0.3/napalm_nokia_olt.egg-info/requires.txt
--rw-r--r--   0 nahanga    (501) staff       (20)       17 2023-06-23 15:19:08.000000 napalm_nokia_olt-0.0.3/napalm_nokia_olt.egg-info/top_level.txt
--rw-r--r--   0 nahanga    (501) staff       (20)       38 2023-06-23 15:19:08.121081 napalm_nokia_olt-0.0.3/setup.cfg
--rw-r--r--   0 nahanga    (501) staff       (20)      927 2023-06-23 15:12:54.000000 napalm_nokia_olt-0.0.3/setup.py
+drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:21:55.158456 napalm_nokia_olt-0.0.4/
+-rw-r--r--   0 nahanga    (501) staff       (20)    11324 2022-08-16 08:37:40.000000 napalm_nokia_olt-0.0.4/LICENSE.md
+-rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-23 15:21:55.158620 napalm_nokia_olt-0.0.4/PKG-INFO
+-rw-r--r--   0 nahanga    (501) staff       (20)      167 2023-02-10 17:17:02.000000 napalm_nokia_olt-0.0.4/README.md
+drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:21:55.143758 napalm_nokia_olt-0.0.4/napalm_nokia_olt/
+-rw-r--r--   0 nahanga    (501) staff       (20)      115 2023-02-10 17:39:46.000000 napalm_nokia_olt-0.0.4/napalm_nokia_olt/__init__.py
+-rw-r--r--   0 nahanga    (501) staff       (20)    10141 2023-06-23 15:20:53.000000 napalm_nokia_olt-0.0.4/napalm_nokia_olt/nokia_olt.py
+drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:21:55.157856 napalm_nokia_olt-0.0.4/napalm_nokia_olt.egg-info/
+-rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-23 15:21:55.000000 napalm_nokia_olt-0.0.4/napalm_nokia_olt.egg-info/PKG-INFO
+-rw-r--r--   0 nahanga    (501) staff       (20)      297 2023-06-23 15:21:55.000000 napalm_nokia_olt-0.0.4/napalm_nokia_olt.egg-info/SOURCES.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)        1 2023-06-23 15:21:55.000000 napalm_nokia_olt-0.0.4/napalm_nokia_olt.egg-info/dependency_links.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)       10 2023-06-23 15:21:55.000000 napalm_nokia_olt-0.0.4/napalm_nokia_olt.egg-info/requires.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)       17 2023-06-23 15:21:55.000000 napalm_nokia_olt-0.0.4/napalm_nokia_olt.egg-info/top_level.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)       38 2023-06-23 15:21:55.159668 napalm_nokia_olt-0.0.4/setup.cfg
+-rw-r--r--   0 nahanga    (501) staff       (20)      927 2023-06-23 15:21:04.000000 napalm_nokia_olt-0.0.4/setup.py
```

### Comparing `napalm_nokia_olt-0.0.3/LICENSE.md` & `napalm_nokia_olt-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `napalm_nokia_olt-0.0.3/PKG-INFO` & `napalm_nokia_olt-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm_nokia_olt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Network Automation and Programmability Abstraction Layer driver for NOKIA OLT 
 Home-page: https://github.com/davama/napalm-nokia_olt
 Author: Dave Macias
 Author-email: davama@gmail.com
 Keywords: napalm driver
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napalm_nokia_olt Version: 0.0.3 Summary: Network
+Metadata-Version: 2.1 Name: napalm_nokia_olt Version: 0.0.4 Summary: Network
 Automation and Programmability Abstraction Layer driver for NOKIA OLT Home-
 page: https://github.com/davama/napalm-nokia_olt Author: Dave Macias Author-
 email: davama@gmail.com Keywords: napalm driver Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: BSD License Description-
 Content-Type: text/markdown License-File: LICENSE.md
 ***** napalm-nokia_olt *****
```

### Comparing `napalm_nokia_olt-0.0.3/napalm_nokia_olt/nokia_olt.py` & `napalm_nokia_olt-0.0.4/napalm_nokia_olt/nokia_olt.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         Send command to device with xml_format option
         """
         # if true; append xml to the end of the command
         if xml_format:
             command = command + ' ' + 'xml'
         #output = self.device.send_command(command, expect_string=r'#$')  ##This is the initial setup
         #>#
-        output = self.device.send_command(command, expect_string=r'>#')
+        output = self.device.send_command(command)
 
         return output
 
     def open(self):
         """Open a connection to the device."""
         device_type = "cisco_ios_ssh"
         if self.transport == "telnet":
```

### Comparing `napalm_nokia_olt-0.0.3/napalm_nokia_olt.egg-info/PKG-INFO` & `napalm_nokia_olt-0.0.4/napalm_nokia_olt.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-nokia-olt
-Version: 0.0.3
+Version: 0.0.4
 Summary: Network Automation and Programmability Abstraction Layer driver for NOKIA OLT 
 Home-page: https://github.com/davama/napalm-nokia_olt
 Author: Dave Macias
 Author-email: davama@gmail.com
 Keywords: napalm driver
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: napalm-nokia-olt Version: 0.0.3 Summary: Network
+Metadata-Version: 2.1 Name: napalm-nokia-olt Version: 0.0.4 Summary: Network
 Automation and Programmability Abstraction Layer driver for NOKIA OLT Home-
 page: https://github.com/davama/napalm-nokia_olt Author: Dave Macias Author-
 email: davama@gmail.com Keywords: napalm driver Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: BSD License Description-
 Content-Type: text/markdown License-File: LICENSE.md
 ***** napalm-nokia_olt *****
```

### Comparing `napalm_nokia_olt-0.0.3/setup.py` & `napalm_nokia_olt-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # read the contents of your README file
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="napalm_nokia_olt",
-    version="0.0.3",
+    version="0.0.4",
     author="Dave Macias",
     author_email = "davama@gmail.com",
     description=("Network Automation and Programmability Abstraction "
                  "Layer driver for NOKIA OLT "),
     keywords="napalm driver",
     url = "https://github.com/davama/napalm-nokia_olt",
     packages=find_packages(),
```

