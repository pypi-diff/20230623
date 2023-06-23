# Comparing `tmp/kyaah-0.1.8.tar.gz` & `tmp/kyaah-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kyaah-0.1.8.tar", last modified: Sat Apr  8 00:52:26 2023, max compression
+gzip compressed data, was "kyaah-0.1.9.tar", last modified: Sun Apr  9 14:45:56 2023, max compression
```

## Comparing `kyaah-0.1.8.tar` & `kyaah-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-08 00:52:25.738520 kyaah-0.1.8/
--rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-04-08 00:49:46.000000 kyaah-0.1.8/CHANGELOG
--rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-03-20 05:01:56.000000 kyaah-0.1.8/LICENSE
--rw-rw-r--   0 usman     (1000) usman     (1000)       54 2023-03-20 05:01:56.000000 kyaah-0.1.8/MANIFEST.in
--rw-rw-r--   0 usman     (1000) usman     (1000)     2720 2023-04-08 00:52:25.734520 kyaah-0.1.8/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     1344 2023-04-08 00:52:09.000000 kyaah-0.1.8/README.md
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-08 00:52:25.710519 kyaah-0.1.8/kyaah/
--rw-rw-r--   0 usman     (1000) usman     (1000)     1835 2023-04-08 00:42:35.000000 kyaah-0.1.8/kyaah/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     5711 2023-04-08 00:42:35.000000 kyaah-0.1.8/kyaah/api.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     8081 2023-04-08 00:42:35.000000 kyaah-0.1.8/kyaah/base.py
--rw-rw-r--   0 usman     (1000) usman     (1000)      490 2023-04-08 00:42:35.000000 kyaah-0.1.8/kyaah/server.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1468 2023-04-08 00:42:35.000000 kyaah-0.1.8/kyaah/utils.py
--rw-rw-r--   0 usman     (1000) usman     (1000)      712 2023-04-08 00:42:35.000000 kyaah-0.1.8/kyaah/vault.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-08 00:52:25.730520 kyaah-0.1.8/kyaah.egg-info/
--rw-rw-r--   0 usman     (1000) usman     (1000)     2720 2023-04-08 00:52:23.000000 kyaah-0.1.8/kyaah.egg-info/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)      283 2023-04-08 00:52:25.000000 kyaah-0.1.8/kyaah.egg-info/SOURCES.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-04-08 00:52:23.000000 kyaah-0.1.8/kyaah.egg-info/dependency_links.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       17 2023-04-08 00:52:23.000000 kyaah-0.1.8/kyaah.egg-info/requires.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        6 2023-04-08 00:52:23.000000 kyaah-0.1.8/kyaah.egg-info/top_level.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-04-08 00:52:25.738520 kyaah-0.1.8/setup.cfg
--rw-rw-r--   0 usman     (1000) usman     (1000)     1906 2023-04-08 00:42:35.000000 kyaah-0.1.8/setup.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-09 14:45:56.071633 kyaah-0.1.9/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      156 2023-04-09 14:44:03.000000 kyaah-0.1.9/CHANGELOG
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-03-20 05:01:56.000000 kyaah-0.1.9/LICENSE
+-rw-rw-r--   0 usman     (1000) usman     (1000)       54 2023-03-20 05:01:56.000000 kyaah-0.1.9/MANIFEST.in
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2873 2023-04-09 14:45:56.067633 kyaah-0.1.9/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1344 2023-04-09 14:44:31.000000 kyaah-0.1.9/README.md
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-09 14:45:56.055631 kyaah-0.1.9/kyaah/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1835 2023-04-09 14:44:03.000000 kyaah-0.1.9/kyaah/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     5711 2023-04-08 00:42:35.000000 kyaah-0.1.9/kyaah/api.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     8081 2023-04-08 00:42:35.000000 kyaah-0.1.9/kyaah/base.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)      490 2023-04-08 00:42:35.000000 kyaah-0.1.9/kyaah/server.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1468 2023-04-08 00:42:35.000000 kyaah-0.1.9/kyaah/utils.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)      712 2023-04-08 00:42:35.000000 kyaah-0.1.9/kyaah/vault.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-04-09 14:45:56.067633 kyaah-0.1.9/kyaah.egg-info/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2873 2023-04-09 14:45:54.000000 kyaah-0.1.9/kyaah.egg-info/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)      283 2023-04-09 14:45:56.000000 kyaah-0.1.9/kyaah.egg-info/SOURCES.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-04-09 14:45:54.000000 kyaah-0.1.9/kyaah.egg-info/dependency_links.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       17 2023-04-09 14:45:54.000000 kyaah-0.1.9/kyaah.egg-info/requires.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        6 2023-04-09 14:45:54.000000 kyaah-0.1.9/kyaah.egg-info/top_level.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-04-09 14:45:56.071633 kyaah-0.1.9/setup.cfg
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1900 2023-04-09 14:44:03.000000 kyaah-0.1.9/setup.py
```

### Comparing `kyaah-0.1.8/LICENSE` & `kyaah-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kyaah-0.1.8/PKG-INFO` & `kyaah-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kyaah
-Version: 0.1.8
+Version: 0.1.9
 Summary: Kyaah abstract away cognitive over-head of sending SMTP mail, together with other mailing operations things like, mail with file, tokens etc
 Home-page: https://kyaah.readthedocs.io
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
 License: UNKNOWN
 Description: 
         # Kyaah
@@ -51,25 +51,29 @@
         
         Pull requests are welcome
         
         
         Change Log
         ==========
         
-        0.1.8 (08/april/2023)
+        0.1.9 (09/april/2023)
         ---------------------
+        - 0.1.9 Release
+        
         - 0.1.8 Release
         
         This release mostly is for adding more documentations.
         
 Keywords: kyaah
-Platform: UNKNOWN
+Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kyaah Version: 0.1.8 Summary: Kyaah abstract away
+Metadata-Version: 2.1 Name: kyaah Version: 0.1.9 Summary: Kyaah abstract away
 cognitive over-head of sending SMTP mail, together with other mailing
 operations things like, mail with file, tokens etc Home-page: https://
 kyaah.readthedocs.io Author: Usman Musa Author-email: usmanmusa1920@gmail.com
 License: UNKNOWN Description: # Kyaah Kyaah abstract away cognitive over-head
 of sending SMTP mail, together with other mailing operations things like, mail
 with file, tokens etc. # Simple use of kyaah First we recommend creating a
 virtual environment `python3 -m venv venv` and then activate it `source venv/
@@ -15,16 +15,17 @@
 password server = "gmail" subj = f"Hellow world!" body = "Lorem ipsum dolor sit
 amet adipisicing elit, rerum voluptate ipsum volupt." kyaah.sendMail
 (from_usr=sender, to_usr=receiver, svr=server, subject=subj, body=body,
 mail_passwd=passwd) ``` save the file and navigate to where the file is located
 in terminal and your are ready to go (run the file) ``` python3 test.py ``` See
 more documentations here! ## Useful links - Documentation: https://
 kyaah.readthedocs.io - Repository: https://github.com/usmanmusa1920/kyaah Pull
-requests are welcome Change Log ========== 0.1.8 (08/april/2023) --------------
-------- - 0.1.8 Release This release mostly is for adding more documentations.
-Keywords: kyaah Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+requests are welcome Change Log ========== 0.1.9 (09/april/2023) --------------
+------- - 0.1.9 Release - 0.1.8 Release This release mostly is for adding more
+documentations. Keywords: kyaah Platform: any Classifier: Development Status ::
+5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Natural Language :: English Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.10 Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `kyaah-0.1.8/README.md` & `kyaah-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `kyaah-0.1.8/kyaah/__init__.py` & `kyaah-0.1.9/kyaah/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     >>> subj = f"Hellow world!"
     >>> body = "Lorem ipsum dolor sit amet adipisicing elit, rerum voluptate ipsum volupt."
 
     >>> kyaah.sendMail(from_usr=sender, to_usr=receiver, svr=server, subject=subj, body=body, mail_passwd=passwd)
 """
 
 __title__ = "kyaah"
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __author__ = "Usman Musa"
 __author_email__ = "usmanmusa1920@gmail.com"
 __author_website__ = "https://usmanmusa1920.github.io"
 __repository__ = "https://github.com/usmanmusa1920/kyaah"
 __website__ = "https://kyaah.readthedocs.io"
 __copyright__ = "Copyright (C) 2022 - 2023 Usman Musa"
```

### Comparing `kyaah-0.1.8/kyaah/api.py` & `kyaah-0.1.9/kyaah/api.py`

 * *Files identical despite different names*

### Comparing `kyaah-0.1.8/kyaah/base.py` & `kyaah-0.1.9/kyaah/base.py`

 * *Files identical despite different names*

### Comparing `kyaah-0.1.8/kyaah/utils.py` & `kyaah-0.1.9/kyaah/utils.py`

 * *Files identical despite different names*

### Comparing `kyaah-0.1.8/kyaah/vault.py` & `kyaah-0.1.9/kyaah/vault.py`

 * *Files identical despite different names*

### Comparing `kyaah-0.1.8/kyaah.egg-info/PKG-INFO` & `kyaah-0.1.9/kyaah.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kyaah
-Version: 0.1.8
+Version: 0.1.9
 Summary: Kyaah abstract away cognitive over-head of sending SMTP mail, together with other mailing operations things like, mail with file, tokens etc
 Home-page: https://kyaah.readthedocs.io
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
 License: UNKNOWN
 Description: 
         # Kyaah
@@ -51,25 +51,29 @@
         
         Pull requests are welcome
         
         
         Change Log
         ==========
         
-        0.1.8 (08/april/2023)
+        0.1.9 (09/april/2023)
         ---------------------
+        - 0.1.9 Release
+        
         - 0.1.8 Release
         
         This release mostly is for adding more documentations.
         
 Keywords: kyaah
-Platform: UNKNOWN
+Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kyaah Version: 0.1.8 Summary: Kyaah abstract away
+Metadata-Version: 2.1 Name: kyaah Version: 0.1.9 Summary: Kyaah abstract away
 cognitive over-head of sending SMTP mail, together with other mailing
 operations things like, mail with file, tokens etc Home-page: https://
 kyaah.readthedocs.io Author: Usman Musa Author-email: usmanmusa1920@gmail.com
 License: UNKNOWN Description: # Kyaah Kyaah abstract away cognitive over-head
 of sending SMTP mail, together with other mailing operations things like, mail
 with file, tokens etc. # Simple use of kyaah First we recommend creating a
 virtual environment `python3 -m venv venv` and then activate it `source venv/
@@ -15,16 +15,17 @@
 password server = "gmail" subj = f"Hellow world!" body = "Lorem ipsum dolor sit
 amet adipisicing elit, rerum voluptate ipsum volupt." kyaah.sendMail
 (from_usr=sender, to_usr=receiver, svr=server, subject=subj, body=body,
 mail_passwd=passwd) ``` save the file and navigate to where the file is located
 in terminal and your are ready to go (run the file) ``` python3 test.py ``` See
 more documentations here! ## Useful links - Documentation: https://
 kyaah.readthedocs.io - Repository: https://github.com/usmanmusa1920/kyaah Pull
-requests are welcome Change Log ========== 0.1.8 (08/april/2023) --------------
-------- - 0.1.8 Release This release mostly is for adding more documentations.
-Keywords: kyaah Platform: UNKNOWN Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+requests are welcome Change Log ========== 0.1.9 (09/april/2023) --------------
+------- - 0.1.9 Release - 0.1.8 Release This release mostly is for adding more
+documentations. Keywords: kyaah Platform: any Classifier: Development Status ::
+5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Natural Language :: English Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.10 Requires-Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `kyaah-0.1.8/setup.py` & `kyaah-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 from setuptools import find_packages
 
 
 setup(
   name = "kyaah", # name of the main package (base folder i.e kyaah)
-  version = "0.1.8",
+  version = "0.1.9",
   description = "Kyaah abstract away cognitive over-head of sending SMTP mail, together with other mailing operations things like, mail with file, tokens etc",
   long_description = open("README.md").read() + "\n\n" + open("CHANGELOG").read(),
   long_description_content_type="text/markdown",
   python_requires = ">=3.6",
-  # platforms="any",
+  platforms="any",
   
   url = "https://kyaah.readthedocs.io",
   repo = "https://github.com/usmanmusa1920/kyaah",
   author = "Usman Musa",
   author_email = "usmanmusa1920@gmail.com",
   License = "MIT",
   classifiers = [
     "Development Status :: 5 - Production/Stable",
     # "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Natural Language :: English",
-    "Operating System :: POSIX :: Linux",
-    # "Operating System :: OS Independent",
+    # "Operating System :: POSIX :: Linux",
+    "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
-    # "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Software Development :: Libraries :: Python Modules",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
-    # "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.10",
   ],
   
   # used when people are searching for a module, keywords separated with a space
   keywords = "kyaah",
   include_package_data = True, # include files listed in MANIFEST.in
   
   # The list of packages(directories) for your library
```

