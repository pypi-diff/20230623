# Comparing `tmp/Airvue-gn-0.0.1.tar.gz` & `tmp/Airvue-gn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Airvue-gn-0.0.1.tar", last modified: Fri Jun 23 07:05:15 2023, max compression
+gzip compressed data, was "Airvue-gn-0.0.2.tar", last modified: Fri Jun 23 07:16:05 2023, max compression
```

## Comparing `Airvue-gn-0.0.1.tar` & `Airvue-gn-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-06-23 07:05:15.622942 Airvue-gn-0.0.1/
-drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-06-23 07:05:15.622089 Airvue-gn-0.0.1/Airvue_gn.egg-info/
--rw-r--r--   0 hamsa      (501) staff       (20)      223 2023-06-23 07:05:15.000000 Airvue-gn-0.0.1/Airvue_gn.egg-info/PKG-INFO
--rw-r--r--   0 hamsa      (501) staff       (20)      285 2023-06-23 07:05:15.000000 Airvue-gn-0.0.1/Airvue_gn.egg-info/SOURCES.txt
--rw-r--r--   0 hamsa      (501) staff       (20)        1 2023-06-23 07:05:15.000000 Airvue-gn-0.0.1/Airvue_gn.egg-info/dependency_links.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      124 2023-06-23 07:05:15.000000 Airvue-gn-0.0.1/Airvue_gn.egg-info/requires.txt
--rw-r--r--   0 hamsa      (501) staff       (20)        6 2023-06-23 07:05:15.000000 Airvue-gn-0.0.1/Airvue_gn.egg-info/top_level.txt
--rw-r--r--   0 hamsa      (501) staff       (20)      223 2023-06-23 07:05:15.622805 Airvue-gn-0.0.1/PKG-INFO
--rw-rw-r--   0 hamsa      (501) staff       (20)        1 2023-06-23 06:53:28.000000 Airvue-gn-0.0.1/README.md
-drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-06-23 07:05:15.622305 Airvue-gn-0.0.1/gnews/
--rw-rw-r--   0 hamsa      (501) staff       (20)       61 2023-02-10 09:24:12.000000 Airvue-gn-0.0.1/gnews/__init__.py
--rw-rw-r--   0 hamsa      (501) staff       (20)    12718 2023-02-10 09:24:12.000000 Airvue-gn-0.0.1/gnews/gnews.py
-drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-06-23 07:05:15.622653 Airvue-gn-0.0.1/gnews/utils/
--rw-rw-r--   0 hamsa      (501) staff       (20)        0 2023-02-10 09:24:12.000000 Airvue-gn-0.0.1/gnews/utils/__init__.py
--rw-rw-r--   0 hamsa      (501) staff       (20)    24441 2023-02-10 09:24:12.000000 Airvue-gn-0.0.1/gnews/utils/constants.py
--rw-rw-r--   0 hamsa      (501) staff       (20)     2040 2023-02-10 09:24:12.000000 Airvue-gn-0.0.1/gnews/utils/utils.py
--rw-r--r--   0 hamsa      (501) staff       (20)       38 2023-06-23 07:05:15.622979 Airvue-gn-0.0.1/setup.cfg
--rw-rw-r--   0 hamsa      (501) staff       (20)      535 2023-06-23 06:58:45.000000 Airvue-gn-0.0.1/setup.py
+drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-06-23 07:16:05.102419 Airvue-gn-0.0.2/
+drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-06-23 07:16:05.101029 Airvue-gn-0.0.2/Airvue_gn.egg-info/
+-rw-r--r--   0 hamsa      (501) staff       (20)      223 2023-06-23 07:16:05.000000 Airvue-gn-0.0.2/Airvue_gn.egg-info/PKG-INFO
+-rw-r--r--   0 hamsa      (501) staff       (20)      285 2023-06-23 07:16:05.000000 Airvue-gn-0.0.2/Airvue_gn.egg-info/SOURCES.txt
+-rw-r--r--   0 hamsa      (501) staff       (20)        1 2023-06-23 07:16:05.000000 Airvue-gn-0.0.2/Airvue_gn.egg-info/dependency_links.txt
+-rw-r--r--   0 hamsa      (501) staff       (20)      124 2023-06-23 07:16:05.000000 Airvue-gn-0.0.2/Airvue_gn.egg-info/requires.txt
+-rw-r--r--   0 hamsa      (501) staff       (20)        6 2023-06-23 07:16:05.000000 Airvue-gn-0.0.2/Airvue_gn.egg-info/top_level.txt
+-rw-r--r--   0 hamsa      (501) staff       (20)      223 2023-06-23 07:16:05.102260 Airvue-gn-0.0.2/PKG-INFO
+-rw-rw-r--   0 hamsa      (501) staff       (20)        1 2023-06-23 06:53:28.000000 Airvue-gn-0.0.2/README.md
+drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-06-23 07:16:05.101432 Airvue-gn-0.0.2/gnews/
+-rw-rw-r--   0 hamsa      (501) staff       (20)       61 2023-02-10 09:24:12.000000 Airvue-gn-0.0.2/gnews/__init__.py
+-rw-rw-r--   0 hamsa      (501) staff       (20)    12718 2023-02-10 09:24:12.000000 Airvue-gn-0.0.2/gnews/gnews.py
+drwxr-xr-x   0 hamsa      (501) staff       (20)        0 2023-06-23 07:16:05.102010 Airvue-gn-0.0.2/gnews/utils/
+-rw-rw-r--   0 hamsa      (501) staff       (20)        0 2023-02-10 09:24:12.000000 Airvue-gn-0.0.2/gnews/utils/__init__.py
+-rw-rw-r--   0 hamsa      (501) staff       (20)    24441 2023-02-10 09:24:12.000000 Airvue-gn-0.0.2/gnews/utils/constants.py
+-rw-rw-r--   0 hamsa      (501) staff       (20)     2040 2023-02-10 09:24:12.000000 Airvue-gn-0.0.2/gnews/utils/utils.py
+-rw-r--r--   0 hamsa      (501) staff       (20)       38 2023-06-23 07:16:05.102463 Airvue-gn-0.0.2/setup.cfg
+-rw-rw-r--   0 hamsa      (501) staff       (20)      535 2023-06-23 07:15:57.000000 Airvue-gn-0.0.2/setup.py
```

### Comparing `Airvue-gn-0.0.1/gnews/gnews.py` & `Airvue-gn-0.0.2/gnews/gnews.py`

 * *Files identical despite different names*

### Comparing `Airvue-gn-0.0.1/gnews/utils/constants.py` & `Airvue-gn-0.0.2/gnews/utils/constants.py`

 * *Files identical despite different names*

### Comparing `Airvue-gn-0.0.1/gnews/utils/utils.py` & `Airvue-gn-0.0.2/gnews/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Airvue-gn-0.0.1/setup.py` & `Airvue-gn-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='Airvue-gn',
-    version='0.0.1',
+    version='0.0.2',
     author="AirvueTech",
     author_email="dev@airvue.news",
     description='Airvue-gn',
     long_description="Airvue-gn",
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=requirements,
```

