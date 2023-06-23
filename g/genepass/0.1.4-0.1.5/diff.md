# Comparing `tmp/genepass-0.1.4.tar.gz` & `tmp/genepass-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepass-0.1.4.tar", last modified: Thu Jun 22 14:10:57 2023, max compression
+gzip compressed data, was "genepass-0.1.5.tar", last modified: Fri Jun 23 14:11:19 2023, max compression
```

## Comparing `genepass-0.1.4.tar` & `genepass-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:10:57.586479 genepass-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 14:10:46.000000 genepass-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-22 14:10:57.586479 genepass-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-22 14:10:46.000000 genepass-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:10:57.582479 genepass-0.1.4/genepass/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 14:10:46.000000 genepass-0.1.4/genepass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-22 14:10:46.000000 genepass-0.1.4/genepass/genepass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:10:57.586479 genepass-0.1.4/genepass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-22 14:10:57.000000 genepass-0.1.4/genepass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-22 14:10:57.000000 genepass-0.1.4/genepass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:10:57.000000 genepass-0.1.4/genepass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 14:10:57.000000 genepass-0.1.4/genepass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:10:57.586479 genepass-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-22 14:10:46.000000 genepass-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:11:19.874393 genepass-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 14:11:08.000000 genepass-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-23 14:11:19.874393 genepass-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-23 14:11:08.000000 genepass-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:11:19.874393 genepass-0.1.5/genepass/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 14:11:08.000000 genepass-0.1.5/genepass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-23 14:11:08.000000 genepass-0.1.5/genepass/genepass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:11:19.874393 genepass-0.1.5/genepass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-23 14:11:19.000000 genepass-0.1.5/genepass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-23 14:11:19.000000 genepass-0.1.5/genepass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:11:19.000000 genepass-0.1.5/genepass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 14:11:19.000000 genepass-0.1.5/genepass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:11:19.874393 genepass-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-23 14:11:08.000000 genepass-0.1.5/setup.py
```

### Comparing `genepass-0.1.4/LICENSE` & `genepass-0.1.5/LICENSE`

 * *Files identical despite different names*

