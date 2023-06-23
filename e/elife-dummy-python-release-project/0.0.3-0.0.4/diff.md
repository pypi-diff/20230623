# Comparing `tmp/elife-dummy-python-release-project-0.0.3.tar.gz` & `tmp/elife-dummy-python-release-project-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elife-dummy-python-release-project-0.0.3.tar", last modified: Fri May 14 04:40:36 2021, max compression
+gzip compressed data, was "elife-dummy-python-release-project-0.0.4.tar", last modified: Fri Jun 23 02:29:50 2023, max compression
```

## Comparing `elife-dummy-python-release-project-0.0.3.tar` & `elife-dummy-python-release-project-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-05-14 04:40:36.000000 elife-dummy-python-release-project-0.0.3/
--rw-r--r--   0 jenkins   (1002) jenkins    (999)       38 2021-05-14 04:40:36.000000 elife-dummy-python-release-project-0.0.3/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      906 2021-05-14 04:40:36.000000 elife-dummy-python-release-project-0.0.3/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      326 2021-05-14 04:39:39.000000 elife-dummy-python-release-project-0.0.3/README.md
--rw-r--r--   0 jenkins   (1002) jenkins    (999)    35147 2021-05-14 04:39:39.000000 elife-dummy-python-release-project-0.0.3/LICENCE
-drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-05-14 04:40:36.000000 elife-dummy-python-release-project-0.0.3/elife_dummy_python_release_project.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      906 2021-05-14 04:40:36.000000 elife-dummy-python-release-project-0.0.3/elife_dummy_python_release_project.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (999)        6 2021-05-14 04:40:36.000000 elife-dummy-python-release-project-0.0.3/elife_dummy_python_release_project.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (999)        1 2021-05-14 04:40:36.000000 elife-dummy-python-release-project-0.0.3/elife_dummy_python_release_project.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      276 2021-05-14 04:40:36.000000 elife-dummy-python-release-project-0.0.3/elife_dummy_python_release_project.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      772 2021-05-14 04:39:39.000000 elife-dummy-python-release-project-0.0.3/setup.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (999)        0 2021-05-14 04:40:36.000000 elife-dummy-python-release-project-0.0.3/dummy/
--rw-r--r--   0 jenkins   (1002) jenkins    (999)      150 2021-05-14 04:39:39.000000 elife-dummy-python-release-project-0.0.3/dummy/__init__.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-23 02:29:50.069399 elife-dummy-python-release-project-0.0.4/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    35147 2023-06-23 02:22:55.000000 elife-dummy-python-release-project-0.0.4/LICENCE
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1071 2023-06-23 02:29:50.069399 elife-dummy-python-release-project-0.0.4/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      573 2023-06-23 02:22:55.000000 elife-dummy-python-release-project-0.0.4/README.md
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-23 02:29:50.069399 elife-dummy-python-release-project-0.0.4/dummy/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      150 2023-06-23 02:22:55.000000 elife-dummy-python-release-project-0.0.4/dummy/__init__.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-06-23 02:29:50.069399 elife-dummy-python-release-project-0.0.4/elife_dummy_python_release_project.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1071 2023-06-23 02:29:50.000000 elife-dummy-python-release-project-0.0.4/elife_dummy_python_release_project.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      276 2023-06-23 02:29:50.000000 elife-dummy-python-release-project-0.0.4/elife_dummy_python_release_project.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-06-23 02:29:50.000000 elife-dummy-python-release-project-0.0.4/elife_dummy_python_release_project.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)        6 2023-06-23 02:29:50.000000 elife-dummy-python-release-project-0.0.4/elife_dummy_python_release_project.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-06-23 02:29:50.069399 elife-dummy-python-release-project-0.0.4/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      772 2023-06-23 02:22:55.000000 elife-dummy-python-release-project-0.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `elife-dummy-python-release-project-0.0.3/LICENCE` & `elife-dummy-python-release-project-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `elife-dummy-python-release-project-0.0.3/setup.py` & `elife-dummy-python-release-project-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="elife-dummy-python-release-project",
-    version="0.0.3",
+    version="0.0.4",
     author="Example Author",
     author_email="author@example.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elifesciences/dummy-python-release-project",
     packages=setuptools.find_packages(),
```

