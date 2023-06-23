# Comparing `tmp/hygiene_dm-0.0.1.tar.gz` & `tmp/hygiene_dm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hygiene_dm-0.0.1.tar", last modified: Mon Jun  5 16:01:29 2023, max compression
+gzip compressed data, was "hygiene_dm-0.0.5.tar", last modified: Fri Jun 23 12:27:26 2023, max compression
```

## Comparing `hygiene_dm-0.0.1.tar` & `hygiene_dm-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,39 @@
-drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-05 16:01:29.283366 hygiene_dm-0.0.1/
--rw-r--r--   0 dylanmoore   (501) staff       (20)     1062 2023-06-05 16:00:57.000000 hygiene_dm-0.0.1/LICENSE
--rw-r--r--   0 dylanmoore   (501) staff       (20)     5206 2023-06-05 16:01:29.283235 hygiene_dm-0.0.1/PKG-INFO
--rw-r--r--   0 dylanmoore   (501) staff       (20)     4881 2023-06-05 16:00:57.000000 hygiene_dm-0.0.1/README.md
-drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-05 16:01:29.282876 hygiene_dm-0.0.1/hygiene_dm.egg-info/
--rw-r--r--   0 dylanmoore   (501) staff       (20)     5206 2023-06-05 16:01:29.000000 hygiene_dm-0.0.1/hygiene_dm.egg-info/PKG-INFO
--rw-r--r--   0 dylanmoore   (501) staff       (20)      177 2023-06-05 16:01:29.000000 hygiene_dm-0.0.1/hygiene_dm.egg-info/SOURCES.txt
--rw-r--r--   0 dylanmoore   (501) staff       (20)        1 2023-06-05 16:01:29.000000 hygiene_dm-0.0.1/hygiene_dm.egg-info/dependency_links.txt
--rw-r--r--   0 dylanmoore   (501) staff       (20)        1 2023-06-05 16:01:29.000000 hygiene_dm-0.0.1/hygiene_dm.egg-info/top_level.txt
--rw-r--r--   0 dylanmoore   (501) staff       (20)      213 2023-06-05 16:00:57.000000 hygiene_dm-0.0.1/pyproject.toml
--rw-r--r--   0 dylanmoore   (501) staff       (20)       38 2023-06-05 16:01:29.283413 hygiene_dm-0.0.1/setup.cfg
--rw-r--r--   0 dylanmoore   (501) staff       (20)      257 2023-06-05 16:00:57.000000 hygiene_dm-0.0.1/setup.py
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.660894 hygiene_dm-0.0.5/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)     1062 2023-06-05 16:00:57.000000 hygiene_dm-0.0.5/LICENSE
+-rw-r--r--   0 dylanmoore   (501) staff       (20)     5248 2023-06-23 12:27:26.660772 hygiene_dm-0.0.5/PKG-INFO
+-rw-r--r--   0 dylanmoore   (501) staff       (20)     4923 2023-06-05 16:03:56.000000 hygiene_dm-0.0.5/README.md
+-rw-r--r--   0 dylanmoore   (501) staff       (20)      213 2023-06-23 12:27:17.000000 hygiene_dm-0.0.5/pyproject.toml
+-rw-r--r--   0 dylanmoore   (501) staff       (20)       38 2023-06-23 12:27:26.660936 hygiene_dm-0.0.5/setup.cfg
+-rw-r--r--   0 dylanmoore   (501) staff       (20)      257 2023-06-23 12:27:10.000000 hygiene_dm-0.0.5/setup.py
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.656847 hygiene_dm-0.0.5/src/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)       32 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/__init__.py
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.657511 hygiene_dm-0.0.5/src/hygiene_dm.egg-info/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)     5248 2023-06-23 12:27:26.000000 hygiene_dm-0.0.5/src/hygiene_dm.egg-info/PKG-INFO
+-rw-r--r--   0 dylanmoore   (501) staff       (20)      675 2023-06-23 12:27:26.000000 hygiene_dm-0.0.5/src/hygiene_dm.egg-info/SOURCES.txt
+-rw-r--r--   0 dylanmoore   (501) staff       (20)        1 2023-06-23 12:27:26.000000 hygiene_dm-0.0.5/src/hygiene_dm.egg-info/dependency_links.txt
+-rw-r--r--   0 dylanmoore   (501) staff       (20)       38 2023-06-23 12:27:26.000000 hygiene_dm-0.0.5/src/hygiene_dm.egg-info/top_level.txt
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.657627 hygiene_dm-0.0.5/src/payload/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)       26 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/payload/__init__.py
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.658018 hygiene_dm-0.0.5/src/payload/boxing/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)       27 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/payload/boxing/__init__.py
+-rw-r--r--   0 dylanmoore   (501) staff       (20)      918 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/payload/boxing/boxing.py
+-rw-r--r--   0 dylanmoore   (501) staff       (20)      103 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/singleton.py
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.658244 hygiene_dm-0.0.5/src/tests/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)     1607 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/tests/test.py
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.658447 hygiene_dm-0.0.5/src/util/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)       81 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/util/__init__.py
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.658897 hygiene_dm-0.0.5/src/util/builders/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)       20 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/util/builders/__init__.py
+-rw-r--r--   0 dylanmoore   (501) staff       (20)      820 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/util/builders/csv.py
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.659087 hygiene_dm-0.0.5/src/util/common/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)       25 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/util/common/__init__.py
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.659497 hygiene_dm-0.0.5/src/util/common/helpers/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)       19 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/util/common/helpers/__init__.py
+-rw-r--r--   0 dylanmoore   (501) staff       (20)      398 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/util/common/helpers/_csv.py
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.659666 hygiene_dm-0.0.5/src/util/formatters/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)       35 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/util/formatters/__init__.py
+drwxr-xr-x   0 dylanmoore   (501) staff       (20)        0 2023-06-23 12:27:26.660501 hygiene_dm-0.0.5/src/util/formatters/single/
+-rw-r--r--   0 dylanmoore   (501) staff       (20)       30 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/util/formatters/single/__init__.py
+-rw-r--r--   0 dylanmoore   (501) staff       (20)     2347 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/util/formatters/single/csv.py
+-rw-r--r--   0 dylanmoore   (501) staff       (20)     1652 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/util/formatters/single/json.py
+-rw-r--r--   0 dylanmoore   (501) staff       (20)     1728 2023-06-05 15:43:20.000000 hygiene_dm-0.0.5/src/util/formatters/single/yaml.py
```

### Comparing `hygiene_dm-0.0.1/LICENSE` & `hygiene_dm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hygiene_dm-0.0.1/PKG-INFO` & `hygiene_dm-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hygiene_dm
-Version: 0.0.1
+Version: 0.0.5
 Summary: hygiene (🪥) is a data preprocessing toolkit that makes it easy to create common LLM-related data structures; from training data to chain payloads!
 Home-page: https://github.com/DylanAlloy/hygiene
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hygiene 🪥
 
@@ -22,17 +22,23 @@
 
 3. Prompt-generated datasets<sup>[2] [3]</sup> in particular are unique but come with similar mundane routines as others.
 
 
 ## 💾 Installation
 
 ``` bash
+pip install hygiene-dm
+```
+or 
+``` bash
 python3 setup.py install
 ```
 
+
+
 ## 🤷 Usage
 
 ``` python
 Python 3.11.2 (main, Mar 24 2023, 00:16:47) [Clang 14.0.0 (clang-1400.0.29.202)] on darwin
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import hygiene
 >>> from hygiene import Singleton
```

### Comparing `hygiene_dm-0.0.1/README.md` & `hygiene_dm-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,23 @@
 
 3. Prompt-generated datasets<sup>[2] [3]</sup> in particular are unique but come with similar mundane routines as others.
 
 
 ## 💾 Installation
 
 ``` bash
+pip install hygiene-dm
+```
+or 
+``` bash
 python3 setup.py install
 ```
 
+
+
 ## 🤷 Usage
 
 ``` python
 Python 3.11.2 (main, Mar 24 2023, 00:16:47) [Clang 14.0.0 (clang-1400.0.29.202)] on darwin
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import hygiene
 >>> from hygiene import Singleton
```

### Comparing `hygiene_dm-0.0.1/hygiene_dm.egg-info/PKG-INFO` & `hygiene_dm-0.0.5/src/hygiene_dm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hygiene-dm
-Version: 0.0.1
+Version: 0.0.5
 Summary: hygiene (🪥) is a data preprocessing toolkit that makes it easy to create common LLM-related data structures; from training data to chain payloads!
 Home-page: https://github.com/DylanAlloy/hygiene
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hygiene 🪥
 
@@ -22,17 +22,23 @@
 
 3. Prompt-generated datasets<sup>[2] [3]</sup> in particular are unique but come with similar mundane routines as others.
 
 
 ## 💾 Installation
 
 ``` bash
+pip install hygiene-dm
+```
+or 
+``` bash
 python3 setup.py install
 ```
 
+
+
 ## 🤷 Usage
 
 ``` python
 Python 3.11.2 (main, Mar 24 2023, 00:16:47) [Clang 14.0.0 (clang-1400.0.29.202)] on darwin
 Type "help", "copyright", "credits" or "license" for more information.
 >>> import hygiene
 >>> from hygiene import Singleton
```

