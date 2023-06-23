# Comparing `tmp/napalm_nokia_olt-0.0.5.tar.gz` & `tmp/napalm_nokia_olt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nahanga/Desktop/NOKIA/napalm_nokia_olt/dist/.tmp-7itdtpns/napalm_nokia_olt-0.0.5.tar", last modified: Fri Jun 23 15:28:01 2023, max compression
+gzip compressed data, was "/Users/nahanga/Desktop/NOKIA/napalm_nokia_olt/dist/.tmp-q0z0nnst/napalm_nokia_olt-0.0.6.tar", last modified: Fri Jun 23 15:30:10 2023, max compression
```

## Comparing `napalm_nokia_olt-0.0.5.tar` & `napalm_nokia_olt-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:28:01.103097 napalm_nokia_olt-0.0.5/
--rw-r--r--   0 nahanga    (501) staff       (20)    11324 2022-08-16 08:37:40.000000 napalm_nokia_olt-0.0.5/LICENSE.md
--rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-23 15:28:01.103251 napalm_nokia_olt-0.0.5/PKG-INFO
--rw-r--r--   0 nahanga    (501) staff       (20)      167 2023-02-10 17:17:02.000000 napalm_nokia_olt-0.0.5/README.md
-drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:28:01.089132 napalm_nokia_olt-0.0.5/napalm_nokia_olt/
--rw-r--r--   0 nahanga    (501) staff       (20)      115 2023-02-10 17:39:46.000000 napalm_nokia_olt-0.0.5/napalm_nokia_olt/__init__.py
--rw-r--r--   0 nahanga    (501) staff       (20)    10230 2023-06-23 15:26:43.000000 napalm_nokia_olt-0.0.5/napalm_nokia_olt/nokia_olt.py
-drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:28:01.102715 napalm_nokia_olt-0.0.5/napalm_nokia_olt.egg-info/
--rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-23 15:28:01.000000 napalm_nokia_olt-0.0.5/napalm_nokia_olt.egg-info/PKG-INFO
--rw-r--r--   0 nahanga    (501) staff       (20)      297 2023-06-23 15:28:01.000000 napalm_nokia_olt-0.0.5/napalm_nokia_olt.egg-info/SOURCES.txt
--rw-r--r--   0 nahanga    (501) staff       (20)        1 2023-06-23 15:28:01.000000 napalm_nokia_olt-0.0.5/napalm_nokia_olt.egg-info/dependency_links.txt
--rw-r--r--   0 nahanga    (501) staff       (20)       10 2023-06-23 15:28:01.000000 napalm_nokia_olt-0.0.5/napalm_nokia_olt.egg-info/requires.txt
--rw-r--r--   0 nahanga    (501) staff       (20)       17 2023-06-23 15:28:01.000000 napalm_nokia_olt-0.0.5/napalm_nokia_olt.egg-info/top_level.txt
--rw-r--r--   0 nahanga    (501) staff       (20)       38 2023-06-23 15:28:01.104050 napalm_nokia_olt-0.0.5/setup.cfg
--rw-r--r--   0 nahanga    (501) staff       (20)      927 2023-06-23 15:27:48.000000 napalm_nokia_olt-0.0.5/setup.py
+drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:30:10.564096 napalm_nokia_olt-0.0.6/
+-rw-r--r--   0 nahanga    (501) staff       (20)    11324 2022-08-16 08:37:40.000000 napalm_nokia_olt-0.0.6/LICENSE.md
+-rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-23 15:30:10.564242 napalm_nokia_olt-0.0.6/PKG-INFO
+-rw-r--r--   0 nahanga    (501) staff       (20)      167 2023-02-10 17:17:02.000000 napalm_nokia_olt-0.0.6/README.md
+drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:30:10.550621 napalm_nokia_olt-0.0.6/napalm_nokia_olt/
+-rw-r--r--   0 nahanga    (501) staff       (20)      115 2023-02-10 17:39:46.000000 napalm_nokia_olt-0.0.6/napalm_nokia_olt/__init__.py
+-rw-r--r--   0 nahanga    (501) staff       (20)    10231 2023-06-23 15:29:46.000000 napalm_nokia_olt-0.0.6/napalm_nokia_olt/nokia_olt.py
+drwxr-xr-x   0 nahanga    (501) staff       (20)        0 2023-06-23 15:30:10.563706 napalm_nokia_olt-0.0.6/napalm_nokia_olt.egg-info/
+-rw-r--r--   0 nahanga    (501) staff       (20)      687 2023-06-23 15:30:10.000000 napalm_nokia_olt-0.0.6/napalm_nokia_olt.egg-info/PKG-INFO
+-rw-r--r--   0 nahanga    (501) staff       (20)      297 2023-06-23 15:30:10.000000 napalm_nokia_olt-0.0.6/napalm_nokia_olt.egg-info/SOURCES.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)        1 2023-06-23 15:30:10.000000 napalm_nokia_olt-0.0.6/napalm_nokia_olt.egg-info/dependency_links.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)       10 2023-06-23 15:30:10.000000 napalm_nokia_olt-0.0.6/napalm_nokia_olt.egg-info/requires.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)       17 2023-06-23 15:30:10.000000 napalm_nokia_olt-0.0.6/napalm_nokia_olt.egg-info/top_level.txt
+-rw-r--r--   0 nahanga    (501) staff       (20)       38 2023-06-23 15:30:10.565522 napalm_nokia_olt-0.0.6/setup.cfg
+-rw-r--r--   0 nahanga    (501) staff       (20)      927 2023-06-23 15:29:17.000000 napalm_nokia_olt-0.0.6/setup.py
```

### Comparing `napalm_nokia_olt-0.0.5/LICENSE.md` & `napalm_nokia_olt-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `napalm_nokia_olt-0.0.5/PKG-INFO` & `napalm_nokia_olt-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm_nokia_olt
-Version: 0.0.5
+Version: 0.0.6
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
-Metadata-Version: 2.1 Name: napalm_nokia_olt Version: 0.0.5 Summary: Network
+Metadata-Version: 2.1 Name: napalm_nokia_olt Version: 0.0.6 Summary: Network
 Automation and Programmability Abstraction Layer driver for NOKIA OLT Home-
 page: https://github.com/davama/napalm-nokia_olt Author: Dave Macias Author-
 email: davama@gmail.com Keywords: napalm driver Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: BSD License Description-
 Content-Type: text/markdown License-File: LICENSE.md
 ***** napalm-nokia_olt *****
```

### Comparing `napalm_nokia_olt-0.0.5/napalm_nokia_olt/nokia_olt.py` & `napalm_nokia_olt-0.0.6/napalm_nokia_olt/nokia_olt.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     def _send_command(self, command, xml_format=False):
         """
         Send command to device with xml_format option
         """
         # if true; append xml to the end of the command
         if xml_format:
             command = command + ' ' + 'xml'
-        #output = self.device.send_command(command, expect_string=r'#$')  ##This is the initial setup
+        output = self.device.send_command(command, expect_string=r'#$')  ##This is the initial setup
         #>#
-        output = self.device.send_command(command)
+        ##output = self.device.send_command(command)
 
         return output
 
     def open(self):
         """Open a connection to the device."""
         device_type = "cisco_ios_ssh"
         if self.transport == "telnet":
```

### Comparing `napalm_nokia_olt-0.0.5/napalm_nokia_olt.egg-info/PKG-INFO` & `napalm_nokia_olt-0.0.6/napalm_nokia_olt.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-nokia-olt
-Version: 0.0.5
+Version: 0.0.6
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
-Metadata-Version: 2.1 Name: napalm-nokia-olt Version: 0.0.5 Summary: Network
+Metadata-Version: 2.1 Name: napalm-nokia-olt Version: 0.0.6 Summary: Network
 Automation and Programmability Abstraction Layer driver for NOKIA OLT Home-
 page: https://github.com/davama/napalm-nokia_olt Author: Dave Macias Author-
 email: davama@gmail.com Keywords: napalm driver Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: BSD License Description-
 Content-Type: text/markdown License-File: LICENSE.md
 ***** napalm-nokia_olt *****
```

### Comparing `napalm_nokia_olt-0.0.5/setup.py` & `napalm_nokia_olt-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # read the contents of your README file
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="napalm_nokia_olt",
-    version="0.0.5",
+    version="0.0.6",
     author="Dave Macias",
     author_email = "davama@gmail.com",
     description=("Network Automation and Programmability Abstraction "
                  "Layer driver for NOKIA OLT "),
     keywords="napalm driver",
     url = "https://github.com/davama/napalm-nokia_olt",
     packages=find_packages(),
```

