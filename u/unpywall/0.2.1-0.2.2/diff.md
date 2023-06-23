# Comparing `tmp/unpywall-0.2.1.tar.gz` & `tmp/unpywall-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unpywall-0.2.1.tar", last modified: Fri Jun 23 09:19:23 2023, max compression
+gzip compressed data, was "unpywall-0.2.2.tar", last modified: Fri Jun 23 09:27:11 2023, max compression
```

## Comparing `unpywall-0.2.1.tar` & `unpywall-0.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:19:23.931768 unpywall-0.2.1/
--rw-r--r--   0 naustica   (501) staff       (20)     1092 2023-06-23 08:32:38.000000 unpywall-0.2.1/LICENSE.txt
--rw-r--r--   0 naustica   (501) staff       (20)       27 2023-06-23 08:24:23.000000 unpywall-0.2.1/MANIFEST.in
--rw-r--r--   0 naustica   (501) staff       (20)     6827 2023-06-23 09:19:23.931637 unpywall-0.2.1/PKG-INFO
--rw-r--r--   0 naustica   (501) staff       (20)     5953 2023-06-23 09:17:13.000000 unpywall-0.2.1/README.md
--rw-r--r--   0 naustica   (501) staff       (20)       67 2023-06-23 09:07:16.000000 unpywall-0.2.1/requirements.txt
--rw-r--r--   0 naustica   (501) staff       (20)       38 2023-06-23 09:19:23.931806 unpywall-0.2.1/setup.cfg
--rw-r--r--   0 naustica   (501) staff       (20)     1590 2023-06-23 09:08:49.000000 unpywall-0.2.1/setup.py
-drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:19:23.929871 unpywall-0.2.1/tests/
--rw-r--r--   0 naustica   (501) staff       (20)     3222 2023-06-23 08:24:23.000000 unpywall-0.2.1/tests/test_cache.py
--rw-r--r--   0 naustica   (501) staff       (20)     1566 2023-06-23 08:24:23.000000 unpywall-0.2.1/tests/test_cli.py
--rw-r--r--   0 naustica   (501) staff       (20)     5591 2023-06-23 08:24:23.000000 unpywall-0.2.1/tests/test_unpywall.py
--rw-r--r--   0 naustica   (501) staff       (20)     1464 2023-06-23 08:24:23.000000 unpywall-0.2.1/tests/test_utils.py
-drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:19:23.930366 unpywall-0.2.1/unpywall/
--rw-r--r--   0 naustica   (501) staff       (20)    15316 2023-06-23 09:12:54.000000 unpywall-0.2.1/unpywall/__init__.py
--rw-r--r--   0 naustica   (501) staff       (20)     7720 2023-06-23 08:24:23.000000 unpywall-0.2.1/unpywall/__main__.py
--rw-r--r--   0 naustica   (501) staff       (20)     5777 2023-06-23 08:24:23.000000 unpywall-0.2.1/unpywall/cache.py
--rw-r--r--   0 naustica   (501) staff       (20)     3151 2023-06-23 08:24:23.000000 unpywall-0.2.1/unpywall/utils.py
-drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:19:23.931420 unpywall-0.2.1/unpywall.egg-info/
--rw-r--r--   0 naustica   (501) staff       (20)     6827 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/PKG-INFO
--rw-r--r--   0 naustica   (501) staff       (20)      443 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/SOURCES.txt
--rw-r--r--   0 naustica   (501) staff       (20)        1 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/dependency_links.txt
--rw-r--r--   0 naustica   (501) staff       (20)       52 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/entry_points.txt
--rw-r--r--   0 naustica   (501) staff       (20)        1 2023-06-23 08:26:01.000000 unpywall-0.2.1/unpywall.egg-info/not-zip-safe
--rw-r--r--   0 naustica   (501) staff       (20)       72 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/requires.txt
--rw-r--r--   0 naustica   (501) staff       (20)        9 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/top_level.txt
+drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:27:11.183295 unpywall-0.2.2/
+-rw-r--r--   0 naustica   (501) staff       (20)     1092 2023-06-23 08:32:38.000000 unpywall-0.2.2/LICENSE.txt
+-rw-r--r--   0 naustica   (501) staff       (20)       27 2023-06-23 08:24:23.000000 unpywall-0.2.2/MANIFEST.in
+-rw-r--r--   0 naustica   (501) staff       (20)     6827 2023-06-23 09:27:11.183177 unpywall-0.2.2/PKG-INFO
+-rw-r--r--   0 naustica   (501) staff       (20)     5953 2023-06-23 09:17:13.000000 unpywall-0.2.2/README.md
+-rw-r--r--   0 naustica   (501) staff       (20)       60 2023-06-23 09:24:12.000000 unpywall-0.2.2/requirements.txt
+-rw-r--r--   0 naustica   (501) staff       (20)       38 2023-06-23 09:27:11.183336 unpywall-0.2.2/setup.cfg
+-rw-r--r--   0 naustica   (501) staff       (20)     1585 2023-06-23 09:25:46.000000 unpywall-0.2.2/setup.py
+drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:27:11.181457 unpywall-0.2.2/tests/
+-rw-r--r--   0 naustica   (501) staff       (20)     3222 2023-06-23 08:24:23.000000 unpywall-0.2.2/tests/test_cache.py
+-rw-r--r--   0 naustica   (501) staff       (20)     1566 2023-06-23 08:24:23.000000 unpywall-0.2.2/tests/test_cli.py
+-rw-r--r--   0 naustica   (501) staff       (20)     5591 2023-06-23 08:24:23.000000 unpywall-0.2.2/tests/test_unpywall.py
+-rw-r--r--   0 naustica   (501) staff       (20)     1464 2023-06-23 08:24:23.000000 unpywall-0.2.2/tests/test_utils.py
+drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:27:11.181908 unpywall-0.2.2/unpywall/
+-rw-r--r--   0 naustica   (501) staff       (20)    15316 2023-06-23 09:12:54.000000 unpywall-0.2.2/unpywall/__init__.py
+-rw-r--r--   0 naustica   (501) staff       (20)     7720 2023-06-23 08:24:23.000000 unpywall-0.2.2/unpywall/__main__.py
+-rw-r--r--   0 naustica   (501) staff       (20)     5777 2023-06-23 08:24:23.000000 unpywall-0.2.2/unpywall/cache.py
+-rw-r--r--   0 naustica   (501) staff       (20)     3151 2023-06-23 08:24:23.000000 unpywall-0.2.2/unpywall/utils.py
+drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:27:11.183008 unpywall-0.2.2/unpywall.egg-info/
+-rw-r--r--   0 naustica   (501) staff       (20)     6827 2023-06-23 09:27:11.000000 unpywall-0.2.2/unpywall.egg-info/PKG-INFO
+-rw-r--r--   0 naustica   (501) staff       (20)      443 2023-06-23 09:27:11.000000 unpywall-0.2.2/unpywall.egg-info/SOURCES.txt
+-rw-r--r--   0 naustica   (501) staff       (20)        1 2023-06-23 09:27:11.000000 unpywall-0.2.2/unpywall.egg-info/dependency_links.txt
+-rw-r--r--   0 naustica   (501) staff       (20)       52 2023-06-23 09:27:11.000000 unpywall-0.2.2/unpywall.egg-info/entry_points.txt
+-rw-r--r--   0 naustica   (501) staff       (20)        1 2023-06-23 08:26:01.000000 unpywall-0.2.2/unpywall.egg-info/not-zip-safe
+-rw-r--r--   0 naustica   (501) staff       (20)       67 2023-06-23 09:27:11.000000 unpywall-0.2.2/unpywall.egg-info/requires.txt
+-rw-r--r--   0 naustica   (501) staff       (20)        9 2023-06-23 09:27:11.000000 unpywall-0.2.2/unpywall.egg-info/top_level.txt
```

### Comparing `unpywall-0.2.1/LICENSE.txt` & `unpywall-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unpywall-0.2.1/PKG-INFO` & `unpywall-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unpywall
-Version: 0.2.1
+Version: 0.2.2
 Summary: Interfacing the Unpaywall Database with Python
 Home-page: https://github.com/unpywall/unpywall
 Author: Nick Haupka, bganglia
 Author-email: nick.haupka@gmail.com, bganglia892@gmail.com
 License: MIT
 Project-URL: Documentation, https://unpywall.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/unpywall/unpywall
```

### Comparing `unpywall-0.2.1/README.md` & `unpywall-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `unpywall-0.2.1/setup.py` & `unpywall-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 dir = path.abspath(path.dirname(__file__))
 with open(path.join(dir, 'README.md'), encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(name='unpywall',
-      version='0.2.1',
+      version='0.2.2',
       description='Interfacing the Unpaywall Database with Python',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/unpywall/unpywall',
       author='Nick Haupka, bganglia',
       author_email='nick.haupka@gmail.com, bganglia892@gmail.com',
       license='MIT',
@@ -19,15 +19,15 @@
       keywords=['Unpaywall', 'Open Access', 'full text'],
       project_urls={
         'Documentation': 'https://unpywall.readthedocs.io/en/latest/',
         'Source': 'https://github.com/unpywall/unpywall',
         'Tracker': 'https://github.com/unpywall/unpywall/issues'
       },
       install_requires=[
-        'pandas>=2.0',
+        'pandas',
         'requests'
       ],
       extras_require={
        'dev': [
            'pytest',
            'coverage',
            'pytest-cov',
```

### Comparing `unpywall-0.2.1/tests/test_cache.py` & `unpywall-0.2.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `unpywall-0.2.1/tests/test_cli.py` & `unpywall-0.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `unpywall-0.2.1/tests/test_unpywall.py` & `unpywall-0.2.2/tests/test_unpywall.py`

 * *Files identical despite different names*

### Comparing `unpywall-0.2.1/tests/test_utils.py` & `unpywall-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `unpywall-0.2.1/unpywall/__init__.py` & `unpywall-0.2.2/unpywall/__init__.py`

 * *Files identical despite different names*

### Comparing `unpywall-0.2.1/unpywall/__main__.py` & `unpywall-0.2.2/unpywall/__main__.py`

 * *Files identical despite different names*

### Comparing `unpywall-0.2.1/unpywall/cache.py` & `unpywall-0.2.2/unpywall/cache.py`

 * *Files identical despite different names*

### Comparing `unpywall-0.2.1/unpywall/utils.py` & `unpywall-0.2.2/unpywall/utils.py`

 * *Files identical despite different names*

### Comparing `unpywall-0.2.1/unpywall.egg-info/PKG-INFO` & `unpywall-0.2.2/unpywall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unpywall
-Version: 0.2.1
+Version: 0.2.2
 Summary: Interfacing the Unpaywall Database with Python
 Home-page: https://github.com/unpywall/unpywall
 Author: Nick Haupka, bganglia
 Author-email: nick.haupka@gmail.com, bganglia892@gmail.com
 License: MIT
 Project-URL: Documentation, https://unpywall.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/unpywall/unpywall
```

