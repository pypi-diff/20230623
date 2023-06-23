# Comparing `tmp/Candataloader-1.1.5.tar.gz` & `tmp/Candataloader-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Candataloader-1.1.5.tar", last modified: Tue May 30 13:09:12 2023, max compression
+gzip compressed data, was "dist/Candataloader-1.1.6.tar", last modified: Fri Jun 23 09:07:36 2023, max compression
```

## Comparing `Candataloader-1.1.5.tar` & `Candataloader-1.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-30 13:09:12.000000 Candataloader-1.1.5/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1729 2023-05-25 12:52:06.000000 Candataloader-1.1.5/README.md
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:31:46.000000 Candataloader-1.1.5/Candataloader/__init__.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1441 2023-05-30 13:08:02.000000 Candataloader-1.1.5/Candataloader/download.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       38 2023-05-30 13:09:12.000000 Candataloader-1.1.5/setup.cfg
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader.egg-info/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        1 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader.egg-info/dependency_links.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      218 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader.egg-info/SOURCES.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       23 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader.egg-info/top_level.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader.egg-info/PKG-INFO
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      299 2023-05-30 13:08:09.000000 Candataloader-1.1.5/setup.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-05-30 13:09:12.000000 Candataloader-1.1.5/PKG-INFO
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-06-23 09:07:36.000000 Candataloader-1.1.6/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1729 2023-05-25 12:52:06.000000 Candataloader-1.1.6/README.md
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:31:46.000000 Candataloader-1.1.6/Candataloader/__init__.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     2007 2023-06-23 09:02:35.000000 Candataloader-1.1.6/Candataloader/download.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       38 2023-06-23 09:07:36.000000 Candataloader-1.1.6/setup.cfg
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader.egg-info/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        1 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader.egg-info/dependency_links.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      218 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader.egg-info/SOURCES.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       23 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader.egg-info/top_level.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-06-23 09:07:36.000000 Candataloader-1.1.6/Candataloader.egg-info/PKG-INFO
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      299 2023-06-23 09:07:10.000000 Candataloader-1.1.6/setup.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-06-23 09:07:36.000000 Candataloader-1.1.6/PKG-INFO
```

### Comparing `Candataloader-1.1.5/README.md` & `Candataloader-1.1.6/README.md`

 * *Files identical despite different names*

