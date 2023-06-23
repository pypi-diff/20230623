# Comparing `tmp/Boombers-0.2.tar.gz` & `tmp/Boombers-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Boombers-0.2.tar", last modified: Fri Jun 23 13:15:35 2023, max compression
+gzip compressed data, was "Boombers-0.3.tar", last modified: Fri Jun 23 13:32:16 2023, max compression
```

## Comparing `Boombers-0.2.tar` & `Boombers-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-23 13:15:35.050359 Boombers-0.2/
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-23 13:15:35.050359 Boombers-0.2/Boombers/
--rw-r--r--   0 themamad  (1000) themamad  (1000)       17 2023-06-20 12:46:43.000000 Boombers-0.2/Boombers/__init__.py
--rwxr-----   0 themamad  (1000) themamad  (1000)      513 2023-06-23 12:28:00.000000 Boombers-0.2/Boombers/config.py
--rwxr-----   0 themamad  (1000) themamad  (1000)     3079 2023-06-22 21:16:41.000000 Boombers-0.2/Boombers/main.py
-drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-23 13:15:35.050359 Boombers-0.2/Boombers.egg-info/
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1026 2023-06-23 13:15:35.000000 Boombers-0.2/Boombers.egg-info/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      211 2023-06-23 13:15:35.000000 Boombers-0.2/Boombers.egg-info/SOURCES.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-23 13:15:35.000000 Boombers-0.2/Boombers.egg-info/dependency_links.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)        9 2023-06-23 13:15:35.000000 Boombers-0.2/Boombers.egg-info/top_level.txt
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 Boombers-0.2/LICENSE
--rw-r--r--   0 themamad  (1000) themamad  (1000)     1026 2023-06-23 13:15:35.050359 Boombers-0.2/PKG-INFO
--rw-r--r--   0 themamad  (1000) themamad  (1000)      337 2023-06-23 12:52:56.000000 Boombers-0.2/README.md
--rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-23 13:15:35.050359 Boombers-0.2/setup.cfg
--rw-r--r--   0 themamad  (1000) themamad  (1000)      923 2023-06-23 13:15:15.000000 Boombers-0.2/setup.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-23 13:32:16.770694 Boombers-0.3/
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-23 13:32:16.770694 Boombers-0.3/Boombers/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)       17 2023-06-20 12:46:43.000000 Boombers-0.3/Boombers/__init__.py
+-rwxr-----   0 themamad  (1000) themamad  (1000)      513 2023-06-23 12:28:00.000000 Boombers-0.3/Boombers/config.py
+-rwxr-----   0 themamad  (1000) themamad  (1000)     3081 2023-06-23 13:26:54.000000 Boombers-0.3/Boombers/main.py
+drwxr-xr-x   0 themamad  (1000) themamad  (1000)        0 2023-06-23 13:32:16.770694 Boombers-0.3/Boombers.egg-info/
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1026 2023-06-23 13:32:16.000000 Boombers-0.3/Boombers.egg-info/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      211 2023-06-23 13:32:16.000000 Boombers-0.3/Boombers.egg-info/SOURCES.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        1 2023-06-23 13:32:16.000000 Boombers-0.3/Boombers.egg-info/dependency_links.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)        9 2023-06-23 13:32:16.000000 Boombers-0.3/Boombers.egg-info/top_level.txt
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1077 2023-06-20 12:51:32.000000 Boombers-0.3/LICENSE
+-rw-r--r--   0 themamad  (1000) themamad  (1000)     1026 2023-06-23 13:32:16.770694 Boombers-0.3/PKG-INFO
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      337 2023-06-23 12:52:56.000000 Boombers-0.3/README.md
+-rw-r--r--   0 themamad  (1000) themamad  (1000)       38 2023-06-23 13:32:16.770694 Boombers-0.3/setup.cfg
+-rw-r--r--   0 themamad  (1000) themamad  (1000)      923 2023-06-23 13:31:26.000000 Boombers-0.3/setup.py
```

### Comparing `Boombers-0.2/Boombers/config.py` & `Boombers-0.3/Boombers/config.py`

 * *Files identical despite different names*

### Comparing `Boombers-0.2/Boombers/main.py` & `Boombers-0.3/Boombers/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from config import __copyright__ , __version__ , __license__ , welcome
 from colorama import Fore as f
 
 
 welcome(f"boomber library virsion {__version__}{__copyright__}")
 
 
-class Boombers:
+class send_sms:
     
     def __init__(self , phonenumber:str , TimeForOnSMS:float , SMS:int):
         self.phonenumber = phonenumber
         self.timeforonsms = TimeForOnSMS
         self.sms = SMS
         tim = self.timeforonsms * self.sms
         print(f"Time For Send SMS: {tim}")
@@ -82,8 +82,9 @@
                 time += 0.25
                 print(f"{f.CYAN}{time}{f.RESET}")
 
             re.post(url=url , data=phone)
             code += 1
             print(f"{f.RED}Send Code {f.RESET}: {f.GREEN}{code}{f.RESET}")
             time -= self.timeforonsms
-        print(f"{f.MAGENTA}\n<github.com/OnlyRad>\n{f.RESET}")
+        print(f"{f.MAGENTA}\n<github.com/OnlyRad>\n{f.RESET}")
+
```

### Comparing `Boombers-0.2/Boombers.egg-info/PKG-INFO` & `Boombers-0.3/Boombers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Boombers
-Version: 0.2
+Version: 0.3
 Summary: Boombers Library Python
 Home-page: https://github.com/OnlyRad/Boombers
 Author: Mohammad and Amir
 Author-email: mohammadmehrabi175@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Boombers-0.2/LICENSE` & `Boombers-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Boombers-0.2/PKG-INFO` & `Boombers-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Boombers
-Version: 0.2
+Version: 0.3
 Summary: Boombers Library Python
 Home-page: https://github.com/OnlyRad/Boombers
 Author: Mohammad and Amir
 Author-email: mohammadmehrabi175@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `Boombers-0.2/setup.py` & `Boombers-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'Boombers',
-    version = '0.2',
+    version = '0.3',
     author='Mohammad and Amir',
     author_email = 'mohammadmehrabi175@gmail.com',
     description = 'Boombers Library Python',
     keywords = [''],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
```

