# Comparing `tmp/PyDrive2-1.9.3.tar.gz` & `tmp/PyDrive2-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDrive2-1.9.3.tar", last modified: Wed Sep  8 18:59:14 2021, max compression
+gzip compressed data, was "PyDrive2-1.9.4.tar", last modified: Fri Sep 17 17:30:57 2021, max compression
```

## Comparing `PyDrive2-1.9.3.tar` & `PyDrive2-1.9.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:14.595425 PyDrive2-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/CHANGES
--rw-r--r--   0 runner    (1001) docker     (121)    10180 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4581 2021-09-08 18:59:14.595425 PyDrive2-1.9.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:14.587425 PyDrive2-1.9.3/PyDrive2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4581 2021-09-08 18:59:14.000000 PyDrive2-1.9.3/PyDrive2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-09-08 18:59:14.000000 PyDrive2-1.9.3/PyDrive2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-08 18:59:14.000000 PyDrive2-1.9.3/PyDrive2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      240 2021-09-08 18:59:14.000000 PyDrive2-1.9.3/PyDrive2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-09-08 18:59:14.000000 PyDrive2-1.9.3/PyDrive2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4017 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:14.591425 PyDrive2-1.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      793 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     9701 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1903 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/docs/filelist.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9611 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/docs/filemanagement.rst
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6668 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/docs/oauth.rst
--rw-r--r--   0 runner    (1001) docker     (121)      716 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/docs/pydrive2.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6083 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:14.591425 PyDrive2-1.9.3/pydrive2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5274 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/apiattr.py
--rw-r--r--   0 runner    (1001) docker     (121)    22569 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/drive.py
--rw-r--r--   0 runner    (1001) docker     (121)    29269 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/files.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:14.591425 PyDrive2-1.9.3/pydrive2/fs/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15386 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/fs/spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/fs/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5764 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:14.595425 PyDrive2-1.9.3/pydrive2/test/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      388 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/client_secrets.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:14.595425 PyDrive2-1.9.3/pydrive2/test/credentials/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/credentials/.keepme
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:14.595425 PyDrive2-1.9.3/pydrive2/test/settings/
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/settings/default.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:14.595425 PyDrive2-1.9.3/pydrive2/test/settings/local/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/settings/local/.keepme
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/settings/test_oauth_default.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/settings/test_oauth_test_01.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/settings/test_oauth_test_02.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/settings/test_oauth_test_03.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      220 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/settings/test_oauth_test_04.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       68 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/settings/test_oauth_test_05.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/settings/test_oauth_test_06.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      255 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/settings/test_oauth_test_07.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/test_apiattr.py
--rw-r--r--   0 runner    (1001) docker     (121)      789 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/test_drive.py
--rw-r--r--   0 runner    (1001) docker     (121)    31218 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/test_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     3862 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/test_filelist.py
--rw-r--r--   0 runner    (1001) docker     (121)     5757 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4006 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pydrive2/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-08 18:59:14.595425 PyDrive2-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2021-09-08 18:59:06.000000 PyDrive2-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:57.170957 PyDrive2-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (121)    10180 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4581 2021-09-17 17:30:57.170957 PyDrive2-1.9.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:57.166957 PyDrive2-1.9.4/PyDrive2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4581 2021-09-17 17:30:57.000000 PyDrive2-1.9.4/PyDrive2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2021-09-17 17:30:57.000000 PyDrive2-1.9.4/PyDrive2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-17 17:30:57.000000 PyDrive2-1.9.4/PyDrive2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2021-09-17 17:30:57.000000 PyDrive2-1.9.4/PyDrive2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-09-17 17:30:57.000000 PyDrive2-1.9.4/PyDrive2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4017 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:57.166957 PyDrive2-1.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     9701 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1903 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/docs/filelist.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9611 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/docs/filemanagement.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1315 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6668 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/docs/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/docs/pydrive2.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6083 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:57.166957 PyDrive2-1.9.4/pydrive2/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5274 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/apiattr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22569 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/drive.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29269 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/files.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:57.166957 PyDrive2-1.9.4/pydrive2/fs/
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15619 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/fs/spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1591 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/fs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5764 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:57.166957 PyDrive2-1.9.4/pydrive2/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     3232 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/client_secrets.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:57.166957 PyDrive2-1.9.4/pydrive2/test/credentials/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/credentials/.keepme
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:57.170957 PyDrive2-1.9.4/pydrive2/test/settings/
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/settings/default.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:57.170957 PyDrive2-1.9.4/pydrive2/test/settings/local/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/settings/local/.keepme
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/settings/test_oauth_default.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/settings/test_oauth_test_01.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/settings/test_oauth_test_02.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/settings/test_oauth_test_03.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/settings/test_oauth_test_04.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/settings/test_oauth_test_05.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/settings/test_oauth_test_06.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/settings/test_oauth_test_07.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/test_apiattr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/test_drive.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31218 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3862 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/test_filelist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6250 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4006 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2628 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pydrive2/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-17 17:30:57.170957 PyDrive2-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1275 2021-09-17 17:30:49.000000 PyDrive2-1.9.4/setup.py
```

### Comparing `PyDrive2-1.9.3/LICENSE` & `PyDrive2-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/PKG-INFO` & `PyDrive2-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDrive2
-Version: 1.9.3
+Version: 1.9.4
 Summary: Google Drive API made easy. Maintained fork of PyDrive.
 Home-page: https://github.com/iterative/PyDrive2
 Author: JunYoung Gwak
 Author-email: jgwak@dreamylab.com
 Maintainer: DVC team
 Maintainer-email: support@dvc.org
 License: Apache License 2.0
```

### Comparing `PyDrive2-1.9.3/PyDrive2.egg-info/PKG-INFO` & `PyDrive2-1.9.4/PyDrive2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDrive2
-Version: 1.9.3
+Version: 1.9.4
 Summary: Google Drive API made easy. Maintained fork of PyDrive.
 Home-page: https://github.com/iterative/PyDrive2
 Author: JunYoung Gwak
 Author-email: jgwak@dreamylab.com
 Maintainer: DVC team
 Maintainer-email: support@dvc.org
 License: Apache License 2.0
```

### Comparing `PyDrive2-1.9.3/PyDrive2.egg-info/SOURCES.txt` & `PyDrive2-1.9.4/PyDrive2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/README.rst` & `PyDrive2-1.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/docs/README.md` & `PyDrive2-1.9.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/docs/conf.py` & `PyDrive2-1.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/docs/filelist.rst` & `PyDrive2-1.9.4/docs/filelist.rst`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/docs/filemanagement.rst` & `PyDrive2-1.9.4/docs/filemanagement.rst`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/docs/index.rst` & `PyDrive2-1.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/docs/oauth.rst` & `PyDrive2-1.9.4/docs/oauth.rst`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/docs/pydrive2.rst` & `PyDrive2-1.9.4/docs/pydrive2.rst`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/docs/quickstart.rst` & `PyDrive2-1.9.4/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/apiattr.py` & `PyDrive2-1.9.4/pydrive2/apiattr.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/auth.py` & `PyDrive2-1.9.4/pydrive2/auth.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/drive.py` & `PyDrive2-1.9.4/pydrive2/drive.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/files.py` & `PyDrive2-1.9.4/pydrive2/files.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/fs/spec.py` & `PyDrive2-1.9.4/pydrive2/fs/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,29 +360,38 @@
         with self.open(lpath) as stream:
             # IterStream objects doesn't support full-length
             # seek() calls, so we have to wrap the data with
             # an external buffer.
             buffer = io.BytesIO(stream.read())
             self.upload_fobj(buffer, rpath)
 
-    def get_file(self, lpath, rpath, callback=None, **kwargs):
+    def get_file(self, lpath, rpath, callback=None, block_size=None, **kwargs):
         item_id = self._get_item_id(lpath)
-        return self.gdrive_get_file(item_id, rpath, callback)
+        return self.gdrive_get_file(
+            item_id, rpath, callback=callback, block_size=block_size
+        )
 
     @_gdrive_retry
-    def gdrive_get_file(self, item_id, rpath, callback):
+    def gdrive_get_file(self, item_id, rpath, callback=None, block_size=None):
         param = {"id": item_id}
         # it does not create a file on the remote
         gdrive_file = self.client.CreateFile(param)
 
         extra_args = {}
+        if block_size:
+            extra_args["chunksize"] = block_size
+
         if callback:
+
+            def cb(value, _):
+                callback.absolute_update(value)
+
             gdrive_file.FetchMetadata(fields="fileSize")
             callback.set_size(int(gdrive_file.get("fileSize")))
-            extra_args["callback"] = callback.update
+            extra_args["callback"] = cb
 
         gdrive_file.GetContentFile(rpath, **extra_args)
 
     def _open(self, path, mode, **kwargs):
         assert mode in {"rb", "wb"}
         if mode == "wb":
             return GDriveBufferedWriter(self, path)
```

### Comparing `PyDrive2-1.9.3/pydrive2/fs/utils.py` & `PyDrive2-1.9.4/pydrive2/fs/utils.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/settings.py` & `PyDrive2-1.9.4/pydrive2/settings.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/test/README.rst` & `PyDrive2-1.9.4/pydrive2/test/README.rst`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/test/test_apiattr.py` & `PyDrive2-1.9.4/pydrive2/test/test_apiattr.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/test/test_drive.py` & `PyDrive2-1.9.4/pydrive2/test/test_drive.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/test/test_file.py` & `PyDrive2-1.9.4/pydrive2/test/test_file.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/test/test_filelist.py` & `PyDrive2-1.9.4/pydrive2/test/test_filelist.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/test/test_fs.py` & `PyDrive2-1.9.4/pydrive2/test/test_fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import posixpath
 import secrets
 import uuid
 from concurrent import futures
 
 import pytest
-
+import fsspec
 from pydrive2.auth import GoogleAuth
 from pydrive2.fs import GDriveFileSystem
 from pydrive2.test.test_util import settings_file_path, setup_credentials
 
 TEST_GDRIVE_REPO_BUCKET = "root"
 
 
@@ -206,7 +206,25 @@
 
     with open(src_file, "wb") as file:
         file.write(b"data")
 
     fs.put_file(src_file, remote_dir + "/a.txt")
     fs.get_file(remote_dir + "/a.txt", dest_file)
     assert dest_file.read() == "data"
+
+
+def test_get_file_callback(fs, tmpdir, remote_dir):
+    src_file = tmpdir / "a.txt"
+    dest_file = tmpdir / "b.txt"
+
+    with open(src_file, "wb") as file:
+        file.write(b"data" * 10)
+
+    fs.put_file(src_file, remote_dir + "/a.txt")
+    callback = fsspec.Callback()
+    fs.get_file(
+        remote_dir + "/a.txt", dest_file, callback=callback, block_size=10
+    )
+    assert dest_file.read() == "data" * 10
+
+    assert callback.size == 40
+    assert callback.value == 40
```

### Comparing `PyDrive2-1.9.3/pydrive2/test/test_oauth.py` & `PyDrive2-1.9.4/pydrive2/test/test_oauth.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/pydrive2/test/test_util.py` & `PyDrive2-1.9.4/pydrive2/test/test_util.py`

 * *Files identical despite different names*

### Comparing `PyDrive2-1.9.3/setup.py` & `PyDrive2-1.9.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 
 if sys.version_info >= (3, 6):
     tests_requirements.append("black==19.10b0")
 
 setup(
     name="PyDrive2",
-    version="1.9.3",
+    version="1.9.4",
     author="JunYoung Gwak",
     author_email="jgwak@dreamylab.com",
     maintainer="DVC team",
     maintainer_email="support@dvc.org",
     packages=["pydrive2", "pydrive2.test", "pydrive2.fs"],
     url="https://github.com/iterative/PyDrive2",
     project_urls={
```

