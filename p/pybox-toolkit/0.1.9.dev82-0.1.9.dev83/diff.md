# Comparing `tmp/pybox-toolkit-0.1.9.dev82.tar.gz` & `tmp/pybox-toolkit-0.1.9.dev83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybox-toolkit-0.1.9.dev82.tar", last modified: Thu Jun 22 17:31:30 2023, max compression
+gzip compressed data, was "pybox-toolkit-0.1.9.dev83.tar", last modified: Fri Jun 23 11:53:44 2023, max compression
```

## Comparing `pybox-toolkit-0.1.9.dev82.tar` & `pybox-toolkit-0.1.9.dev83.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.533342 pybox-toolkit-0.1.9.dev82/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 17:31:30.533342 pybox-toolkit-0.1.9.dev82/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.525342 pybox-toolkit-0.1.9.dev82/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 17:31:30.000000 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      419 2023-06-22 17:31:30.000000 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 17:31:30.000000 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-22 17:31:30.000000 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 17:31:30.000000 pybox-toolkit-0.1.9.dev82/src/pybox_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/src/toolkit/
--rw-rw-rw-   0 root         (0) root         (0)    15423 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/src/toolkit/graphing/
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/graphing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/src/toolkit/test/
--rw-rw-rw-   0 root         (0) root         (0)     5113 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:31:30.529343 pybox-toolkit-0.1.9.dev82/src/toolkit/typing/
--rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/typing/si.py
--rw-rw-rw-   0 root         (0) root         (0)     8004 2023-06-22 17:30:54.000000 pybox-toolkit-0.1.9.dev82/src/toolkit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.221078 pybox-toolkit-0.1.9.dev83/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-23 11:53:44.221078 pybox-toolkit-0.1.9.dev83/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev83/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev83/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 11:53:44.221078 pybox-toolkit-0.1.9.dev83/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.213078 pybox-toolkit-0.1.9.dev83/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.217078 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-23 11:53:44.000000 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      419 2023-06-23 11:53:44.000000 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 11:53:44.000000 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-23 11:53:44.000000 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-23 11:53:44.000000 pybox-toolkit-0.1.9.dev83/src/pybox_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.217078 pybox-toolkit-0.1.9.dev83/src/toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)    15423 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.217078 pybox-toolkit-0.1.9.dev83/src/toolkit/graphing/
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/graphing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 11:53:07.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.221078 pybox-toolkit-0.1.9.dev83/src/toolkit/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:53:44.221078 pybox-toolkit-0.1.9.dev83/src/toolkit/typing/
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-22 07:36:20.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/typing/si.py
+-rw-rw-rw-   0 root         (0) root         (0)     8004 2023-06-23 09:39:43.000000 pybox-toolkit-0.1.9.dev83/src/toolkit/utils.py
```

### Comparing `pybox-toolkit-0.1.9.dev82/pyproject.toml` & `pybox-toolkit-0.1.9.dev83/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev82/src/toolkit/__init__.py` & `pybox-toolkit-0.1.9.dev83/src/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev82/src/toolkit/graphing/__init__.py` & `pybox-toolkit-0.1.9.dev83/src/toolkit/graphing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev82/src/toolkit/test/__init__.py` & `pybox-toolkit-0.1.9.dev83/src/toolkit/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev82/src/toolkit/typing/__init__.py` & `pybox-toolkit-0.1.9.dev83/src/toolkit/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev82/src/toolkit/typing/si.py` & `pybox-toolkit-0.1.9.dev83/src/toolkit/typing/si.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev82/src/toolkit/utils.py` & `pybox-toolkit-0.1.9.dev83/src/toolkit/utils.py`

 * *Files identical despite different names*

