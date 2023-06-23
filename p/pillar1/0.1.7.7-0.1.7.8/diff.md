# Comparing `tmp/pillar1-0.1.7.7.tar.gz` & `tmp/pillar1-0.1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillar1-0.1.7.7.tar", last modified: Fri Jun 23 15:05:31 2023, max compression
+gzip compressed data, was "pillar1-0.1.7.8.tar", last modified: Fri Jun 23 15:42:56 2023, max compression
```

## Comparing `pillar1-0.1.7.7.tar` & `pillar1-0.1.7.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:05:31.853871 pillar1-0.1.7.7/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:05:31.853745 pillar1-0.1.7.7/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7.7/README.md
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:05:31.852995 pillar1-0.1.7.7/pillar1/
--rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7.7/pillar1/__init__.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     2855 2023-06-23 15:05:11.000000 pillar1-0.1.7.7/pillar1/constants.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7.7/pillar1/constants_original.py
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3683 2023-06-23 14:39:45.000000 pillar1-0.1.7.7/pillar1/pillar1.py
-drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:05:31.853572 pillar1-0.1.7.7/pillar1.egg-info/
--rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:05:31.000000 pillar1-0.1.7.7/pillar1.egg-info/PKG-INFO
--rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-23 15:05:31.000000 pillar1-0.1.7.7/pillar1.egg-info/SOURCES.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 15:05:31.000000 pillar1-0.1.7.7/pillar1.egg-info/dependency_links.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 15:05:31.000000 pillar1-0.1.7.7/pillar1.egg-info/top_level.txt
--rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 15:05:31.853915 pillar1-0.1.7.7/setup.cfg
--rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-23 15:05:25.000000 pillar1-0.1.7.7/setup.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:42:56.702218 pillar1-0.1.7.8/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:42:56.702101 pillar1-0.1.7.8/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2842 2023-06-19 22:34:12.000000 pillar1-0.1.7.8/README.md
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:42:56.701353 pillar1-0.1.7.8/pillar1/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       27 2023-06-19 22:42:24.000000 pillar1-0.1.7.8/pillar1/__init__.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     2855 2023-06-23 15:05:11.000000 pillar1-0.1.7.8/pillar1/constants.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     9993 2023-06-23 13:24:20.000000 pillar1-0.1.7.8/pillar1/constants_original.py
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     4150 2023-06-23 15:41:00.000000 pillar1-0.1.7.8/pillar1/pillar1.py
+drwxr-xr-x   0 aymanhajja   (501) staff       (20)        0 2023-06-23 15:42:56.701930 pillar1-0.1.7.8/pillar1.egg-info/
+-rw-r--r--   0 aymanhajja   (501) staff       (20)     3202 2023-06-23 15:42:56.000000 pillar1-0.1.7.8/pillar1.egg-info/PKG-INFO
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      232 2023-06-23 15:42:56.000000 pillar1-0.1.7.8/pillar1.egg-info/SOURCES.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        1 2023-06-23 15:42:56.000000 pillar1-0.1.7.8/pillar1.egg-info/dependency_links.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)        8 2023-06-23 15:42:56.000000 pillar1-0.1.7.8/pillar1.egg-info/top_level.txt
+-rw-r--r--   0 aymanhajja   (501) staff       (20)       38 2023-06-23 15:42:56.702255 pillar1-0.1.7.8/setup.cfg
+-rw-r--r--   0 aymanhajja   (501) staff       (20)      621 2023-06-23 15:42:54.000000 pillar1-0.1.7.8/setup.py
```

### Comparing `pillar1-0.1.7.7/PKG-INFO` & `pillar1-0.1.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7.7
+Version: 0.1.7.8
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7.7/README.md` & `pillar1-0.1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.7/pillar1/constants.py` & `pillar1-0.1.7.8/pillar1/constants.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.7/pillar1/constants_original.py` & `pillar1-0.1.7.8/pillar1/constants_original.py`

 * *Files identical despite different names*

### Comparing `pillar1-0.1.7.7/pillar1/pillar1.py` & `pillar1-0.1.7.8/pillar1/pillar1.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,16 @@
         'context': '',
         'stop_token': '<|endoftext|>'
     },
     'starcoder-beta': {
         'context': cn.STARCODER_BETA,
         'prepend': '<|user|>',
         'append': '(only return DataBricks-compatible SQL code)<|end|>',
-        'stop_token': '<|end|>'
+        'stop_token': '<|end|>',
+        'replaces': {'': '', }
     }
 }
 
 
 class Model:
     def __init__(self, user_name: str = '', password: str = '', end_point: str = '', max_new_tokens: int = 100, verbose: bool = False):
         self.end_point = end_point
@@ -38,14 +39,17 @@
 
     def code(self):
         self.cleaned_code = self.response.replace(self.prompt, '').strip()
         ELS_TO_REMOVE = ['<pre>', '<code>', '</code>', '</pre>']
         for curr_el_to_remove in ELS_TO_REMOVE:
             self.cleaned_code = self.cleaned_code.replace(curr_el_to_remove, '')
 
+        self.cleaned_code = self.cleaned_code.split('<|assistant|>')[1].split('<|end|>')[0].strip().replace(' claims;', ' uc_beesbridge.abacus.claims;').replace(' claims ',
+                                                                                                                                                                 ' uc_beesbridge.abacus.claims ').replace(
+            ' claims\n', ' uc_beesbridge.abacus.claims\n')
         self.cleaned_code = self.cleaned_code.strip()
         print(self.cleaned_code)
 
     def execute(self):
         spark = SparkSession.builder.getOrCreate()
         self.result = spark.sql(self.cleaned_code)
         self.result.show()
```

### Comparing `pillar1-0.1.7.7/pillar1.egg-info/PKG-INFO` & `pillar1-0.1.7.8/pillar1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillar1
-Version: 0.1.7.7
+Version: 0.1.7.8
 Summary: Official package for Pillar1 company
 Home-page: https://github.com/amhajja/pillar1
 Author: Ayman Hajja
 Author-email: amhajja@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `pillar1-0.1.7.7/setup.py` & `pillar1-0.1.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pillar1',
-    version='0.1.7.7',
+    version='0.1.7.8',
     packages=find_packages(),
     description='Official package for Pillar1 company',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayman Hajja',
     author_email='amhajja@gmail.com',
     url='https://github.com/amhajja/pillar1',
```

