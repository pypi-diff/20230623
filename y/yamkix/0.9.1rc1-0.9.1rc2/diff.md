# Comparing `tmp/yamkix-0.9.1rc1.tar.gz` & `tmp/yamkix-0.9.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamkix-0.9.1rc1.tar", last modified: Mon Dec 20 16:43:07 2021, max compression
+gzip compressed data, was "yamkix-0.9.1rc2.tar", last modified: Mon Dec 20 16:57:25 2021, max compression
```

## Comparing `yamkix-0.9.1rc1.tar` & `yamkix-0.9.1rc2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 16:43:07.853268 yamkix-0.9.1rc1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-20 16:42:48.000000 yamkix-0.9.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2021-12-20 16:43:07.853268 yamkix-0.9.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7041 2021-12-20 16:42:48.000000 yamkix-0.9.1rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      597 2021-12-20 16:43:07.853268 yamkix-0.9.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-12-20 16:42:48.000000 yamkix-0.9.1rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 16:43:07.853268 yamkix-0.9.1rc1/yamkix/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-12-20 16:42:48.000000 yamkix-0.9.1rc1/yamkix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-12-20 16:42:48.000000 yamkix-0.9.1rc1/yamkix/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4382 2021-12-20 16:42:48.000000 yamkix-0.9.1rc1/yamkix/args.py
--rw-r--r--   0 runner    (1001) docker     (121)     2818 2021-12-20 16:42:48.000000 yamkix-0.9.1rc1/yamkix/comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     6421 2021-12-20 16:42:48.000000 yamkix-0.9.1rc1/yamkix/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2021-12-20 16:42:48.000000 yamkix-0.9.1rc1/yamkix/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2021-12-20 16:42:48.000000 yamkix-0.9.1rc1/yamkix/yamkix.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-12-20 16:42:48.000000 yamkix-0.9.1rc1/yamkix/yaml_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 16:43:07.853268 yamkix-0.9.1rc1/yamkix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2021-12-20 16:43:07.000000 yamkix-0.9.1rc1/yamkix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      365 2021-12-20 16:43:07.000000 yamkix-0.9.1rc1/yamkix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-20 16:43:07.000000 yamkix-0.9.1rc1/yamkix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-12-20 16:43:07.000000 yamkix-0.9.1rc1/yamkix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-12-20 16:43:07.000000 yamkix-0.9.1rc1/yamkix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-12-20 16:43:07.000000 yamkix-0.9.1rc1/yamkix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 16:57:25.298792 yamkix-0.9.1rc2/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-20 16:57:02.000000 yamkix-0.9.1rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2021-12-20 16:57:25.298792 yamkix-0.9.1rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7041 2021-12-20 16:57:02.000000 yamkix-0.9.1rc2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2021-12-20 16:57:25.298792 yamkix-0.9.1rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-12-20 16:57:02.000000 yamkix-0.9.1rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 16:57:25.298792 yamkix-0.9.1rc2/yamkix/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2021-12-20 16:57:02.000000 yamkix-0.9.1rc2/yamkix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-12-20 16:57:02.000000 yamkix-0.9.1rc2/yamkix/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4382 2021-12-20 16:57:02.000000 yamkix-0.9.1rc2/yamkix/args.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2818 2021-12-20 16:57:02.000000 yamkix-0.9.1rc2/yamkix/comments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6421 2021-12-20 16:57:02.000000 yamkix-0.9.1rc2/yamkix/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2021-12-20 16:57:02.000000 yamkix-0.9.1rc2/yamkix/helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3036 2021-12-20 16:57:02.000000 yamkix-0.9.1rc2/yamkix/yamkix.py
+-rw-r--r--   0 runner    (1001) docker     (121)      810 2021-12-20 16:57:02.000000 yamkix-0.9.1rc2/yamkix/yaml_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 16:57:25.298792 yamkix-0.9.1rc2/yamkix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2021-12-20 16:57:24.000000 yamkix-0.9.1rc2/yamkix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      365 2021-12-20 16:57:24.000000 yamkix-0.9.1rc2/yamkix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-20 16:57:24.000000 yamkix-0.9.1rc2/yamkix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-12-20 16:57:24.000000 yamkix-0.9.1rc2/yamkix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-12-20 16:57:24.000000 yamkix-0.9.1rc2/yamkix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-12-20 16:57:24.000000 yamkix-0.9.1rc2/yamkix.egg-info/top_level.txt
```

### Comparing `yamkix-0.9.1rc1/LICENSE` & `yamkix-0.9.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `yamkix-0.9.1rc1/PKG-INFO` & `yamkix-0.9.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamkix
-Version: 0.9.1rc1
+Version: 0.9.1rc2
 Summary: An opinionated yaml formatter based on ruamel.yaml
 Home-page: https://github.com/looztra/yamkix
 Author: Christophe Furmaniak
 Author-email: christophe.furmaniak@gmail.com
 License: [Apache License 2.0](http: // www.apache.org / licenses /)
 Keywords: yaml format
 Platform: UNKNOWN
```

### Comparing `yamkix-0.9.1rc1/README.rst` & `yamkix-0.9.1rc2/README.rst`

 * *Files identical despite different names*

### Comparing `yamkix-0.9.1rc1/setup.cfg` & `yamkix-0.9.1rc2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.1rc1
+current_version = 0.9.1rc2
 parse = (?P<major>\d+)(\.(?P<minor>\d+))(\.(?P<patch>\d+))(rc(?P<rc>\d+))?
 serialize = 
 	{major}.{minor}.{patch}rc{rc}
 	{major}.{minor}.{patch}
 commit = False
 tag = False
```

### Comparing `yamkix-0.9.1rc1/setup.py` & `yamkix-0.9.1rc2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 SETUP_REQUIREMENTS = ["pytest-runner"]
 
 TEST_REQUIREMENTS = ["pytest"]
 
 setup(
     name="yamkix",
-    version="0.9.1rc1",
+    version="0.9.1rc2",
     author="Christophe Furmaniak",
     author_email="christophe.furmaniak@gmail.com",
     description="An opinionated yaml formatter based on ruamel.yaml",
     long_description=README,
     long_description_content_type="text/x-rst",
     url="https://github.com/looztra/yamkix",
     license="[Apache License 2.0](http: // www.apache.org / licenses /)",
```

### Comparing `yamkix-0.9.1rc1/yamkix/args.py` & `yamkix-0.9.1rc2/yamkix/args.py`

 * *Files identical despite different names*

### Comparing `yamkix-0.9.1rc1/yamkix/comments.py` & `yamkix-0.9.1rc2/yamkix/comments.py`

 * *Files identical despite different names*

### Comparing `yamkix-0.9.1rc1/yamkix/config.py` & `yamkix-0.9.1rc2/yamkix/config.py`

 * *Files identical despite different names*

### Comparing `yamkix-0.9.1rc1/yamkix/helpers.py` & `yamkix-0.9.1rc2/yamkix/helpers.py`

 * *Files identical despite different names*

### Comparing `yamkix-0.9.1rc1/yamkix/yamkix.py` & `yamkix-0.9.1rc2/yamkix/yamkix.py`

 * *Files identical despite different names*

### Comparing `yamkix-0.9.1rc1/yamkix/yaml_writer.py` & `yamkix-0.9.1rc2/yamkix/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `yamkix-0.9.1rc1/yamkix.egg-info/PKG-INFO` & `yamkix-0.9.1rc2/yamkix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamkix
-Version: 0.9.1rc1
+Version: 0.9.1rc2
 Summary: An opinionated yaml formatter based on ruamel.yaml
 Home-page: https://github.com/looztra/yamkix
 Author: Christophe Furmaniak
 Author-email: christophe.furmaniak@gmail.com
 License: [Apache License 2.0](http: // www.apache.org / licenses /)
 Keywords: yaml format
 Platform: UNKNOWN
```

