# Comparing `tmp/cardamom_ai-0.0.3.tar.gz` & `tmp/cardamom_ai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardamom_ai-0.0.3.tar", last modified: Tue May 23 00:24:09 2023, max compression
+gzip compressed data, was "cardamom_ai-0.0.4.tar", last modified: Fri Jun 23 13:08:17 2023, max compression
```

## Comparing `cardamom_ai-0.0.3.tar` & `cardamom_ai-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 nmh        (501) staff       (20)        0 2023-05-23 00:24:09.908830 cardamom_ai-0.0.3/
--rw-r--r--   0 nmh        (501) staff       (20)    34523 2023-05-21 21:37:45.000000 cardamom_ai-0.0.3/LICENSE
--rw-r--r--   0 nmh        (501) staff       (20)      279 2023-05-23 00:24:09.908872 cardamom_ai-0.0.3/PKG-INFO
--rw-r--r--   0 nmh        (501) staff       (20)        0 2023-05-22 22:37:46.000000 cardamom_ai-0.0.3/README.md
-drwxr-xr-x   0 nmh        (501) staff       (20)        0 2023-05-23 00:24:09.908728 cardamom_ai-0.0.3/cardamom_ai.egg-info/
--rw-r--r--   0 nmh        (501) staff       (20)      279 2023-05-23 00:24:09.000000 cardamom_ai-0.0.3/cardamom_ai.egg-info/PKG-INFO
--rw-r--r--   0 nmh        (501) staff       (20)      216 2023-05-23 00:24:09.000000 cardamom_ai-0.0.3/cardamom_ai.egg-info/SOURCES.txt
--rw-r--r--   0 nmh        (501) staff       (20)        1 2023-05-23 00:24:09.000000 cardamom_ai-0.0.3/cardamom_ai.egg-info/dependency_links.txt
--rw-r--r--   0 nmh        (501) staff       (20)       52 2023-05-23 00:24:09.000000 cardamom_ai-0.0.3/cardamom_ai.egg-info/requires.txt
--rw-r--r--   0 nmh        (501) staff       (20)        1 2023-05-23 00:24:09.000000 cardamom_ai-0.0.3/cardamom_ai.egg-info/top_level.txt
--rw-r--r--   0 nmh        (501) staff       (20)      122 2023-05-22 23:42:19.000000 cardamom_ai-0.0.3/pyproject.toml
--rw-r--r--   0 nmh        (501) staff       (20)      524 2023-05-23 00:24:09.909103 cardamom_ai-0.0.3/setup.cfg
+drwxr-xr-x   0 nmh        (501) staff       (20)        0 2023-06-23 13:08:17.433880 cardamom_ai-0.0.4/
+-rw-r--r--   0 nmh        (501) staff       (20)    34523 2023-05-21 21:37:45.000000 cardamom_ai-0.0.4/LICENSE
+-rw-r--r--   0 nmh        (501) staff       (20)      279 2023-06-23 13:08:17.433924 cardamom_ai-0.0.4/PKG-INFO
+-rw-r--r--   0 nmh        (501) staff       (20)        0 2023-05-22 22:37:46.000000 cardamom_ai-0.0.4/README.md
+drwxr-xr-x   0 nmh        (501) staff       (20)        0 2023-06-23 13:08:17.433778 cardamom_ai-0.0.4/cardamom_ai.egg-info/
+-rw-r--r--   0 nmh        (501) staff       (20)      279 2023-06-23 13:08:17.000000 cardamom_ai-0.0.4/cardamom_ai.egg-info/PKG-INFO
+-rw-r--r--   0 nmh        (501) staff       (20)      216 2023-06-23 13:08:17.000000 cardamom_ai-0.0.4/cardamom_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 nmh        (501) staff       (20)        1 2023-06-23 13:08:17.000000 cardamom_ai-0.0.4/cardamom_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 nmh        (501) staff       (20)       52 2023-06-23 13:08:17.000000 cardamom_ai-0.0.4/cardamom_ai.egg-info/requires.txt
+-rw-r--r--   0 nmh        (501) staff       (20)        1 2023-06-23 13:08:17.000000 cardamom_ai-0.0.4/cardamom_ai.egg-info/top_level.txt
+-rw-r--r--   0 nmh        (501) staff       (20)      122 2023-05-22 23:42:19.000000 cardamom_ai-0.0.4/pyproject.toml
+-rw-r--r--   0 nmh        (501) staff       (20)      524 2023-06-23 13:08:17.434137 cardamom_ai-0.0.4/setup.cfg
```

### Comparing `cardamom_ai-0.0.3/LICENSE` & `cardamom_ai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cardamom_ai-0.0.3/setup.cfg` & `cardamom_ai-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardamom_ai
-version = 0.0.3
+version = 0.0.4
 author = Cardamom AI
 author_email = sales@cardamom.ai
 long_description = Deploy ML with Cardamom
 url = https://cardamom.ai
 keywords = cardamom, ml, deployment
 description_file = README.md
 license_files = LICENSE
```

