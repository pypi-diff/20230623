# Comparing `tmp/flict-1.0.8.tar.gz` & `tmp/flict-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flict-1.0.8.tar", last modified: Wed Nov 30 09:30:22 2022, max compression
+gzip compressed data, was "flict-1.0.9.tar", last modified: Mon Dec  5 08:30:34 2022, max compression
```

## Comparing `flict-1.0.8.tar` & `flict-1.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:30:22.789802 flict-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2022-11-30 09:30:02.000000 flict-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       88 2022-11-30 09:30:02.000000 flict-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7395 2022-11-30 09:30:22.789802 flict-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5084 2022-11-30 09:30:02.000000 flict-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:30:22.777801 flict-1.0.8/flict/
--rw-r--r--   0 runner    (1001) docker     (122)      248 2022-11-30 09:30:02.000000 flict-1.0.8/flict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11079 2022-11-30 09:30:02.000000 flict-1.0.8/flict/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:30:22.785802 flict-1.0.8/flict/flictlib/
--rw-r--r--   0 runner    (1001) docker     (122)      246 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1802 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/alias.py
--rw-r--r--   0 runner    (1001) docker     (122)     9517 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (122)    12191 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2022-11-30 09:30:22.000000 flict-1.0.8/flict/flictlib/flict_config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:30:22.789802 flict-1.0.8/flict/flictlib/format/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      752 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/format/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     4339 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/format/dot_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1206 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/format/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     2220 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/format/format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1775 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/format/json_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     6890 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/format/markdown_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     4581 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/format/text_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     8430 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/lic_comp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2741 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/license.py
--rw-r--r--   0 runner    (1001) docker     (122)     8470 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/license_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)      849 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:30:22.789802 flict-1.0.8/flict/flictlib/project/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9009 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/project/reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1719 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/return_codes.py
--rw-r--r--   0 runner    (1001) docker     (122)      535 2022-11-30 09:30:02.000000 flict-1.0.8/flict/flictlib/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4415 2022-11-30 09:30:02.000000 flict-1.0.8/flict/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:30:22.789802 flict-1.0.8/flict/var/
--rw-r--r--   0 runner    (1001) docker     (122)      295 2022-11-30 09:30:02.000000 flict-1.0.8/flict/var/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17319 2022-11-30 09:30:02.000000 flict-1.0.8/flict/var/alias.json
--rw-r--r--   0 runner    (1001) docker     (122)   457966 2022-11-30 09:30:02.000000 flict-1.0.8/flict/var/scancode-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 09:30:22.781802 flict-1.0.8/flict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7395 2022-11-30 09:30:22.000000 flict-1.0.8/flict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1044 2022-11-30 09:30:22.000000 flict-1.0.8/flict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 09:30:22.000000 flict-1.0.8/flict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       47 2022-11-30 09:30:22.000000 flict-1.0.8/flict.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      828 2022-11-30 09:30:22.000000 flict-1.0.8/flict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-11-30 09:30:22.000000 flict-1.0.8/flict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      828 2022-11-30 09:30:02.000000 flict-1.0.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       73 2022-11-30 09:30:02.000000 flict-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-30 09:30:22.789802 flict-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1949 2022-11-30 09:30:02.000000 flict-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.854724 flict-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2022-12-05 08:30:10.000000 flict-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-05 08:30:10.000000 flict-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2022-12-05 08:30:34.854724 flict-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2022-12-05 08:30:10.000000 flict-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.850724 flict-1.0.9/flict/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2022-12-05 08:30:10.000000 flict-1.0.9/flict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2022-12-05 08:30:10.000000 flict-1.0.9/flict/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.850724 flict-1.0.9/flict/flictlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2022-12-05 08:30:34.000000 flict-1.0.9/flict/flictlib/flict_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.854724 flict-1.0.9/flict/flictlib/format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/dot_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/json_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/markdown_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/format/text_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/lic_comp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/license_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.854724 flict-1.0.9/flict/flictlib/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/project/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/return_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-05 08:30:10.000000 flict-1.0.9/flict/flictlib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2022-12-05 08:30:10.000000 flict-1.0.9/flict/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.854724 flict-1.0.9/flict/var/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-05 08:30:10.000000 flict-1.0.9/flict/var/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2022-12-05 08:30:10.000000 flict-1.0.9/flict/var/alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)   457966 2022-12-05 08:30:10.000000 flict-1.0.9/flict/var/scancode-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-05 08:30:34.850724 flict-1.0.9/flict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-05 08:30:34.000000 flict-1.0.9/flict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2022-12-05 08:30:10.000000 flict-1.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2022-12-05 08:30:10.000000 flict-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-05 08:30:34.854724 flict-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2022-12-05 08:30:10.000000 flict-1.0.9/setup.py
```

### Comparing `flict-1.0.8/LICENSE` & `flict-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/README.md` & `flict-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/__main__.py` & `flict-1.0.9/flict/__main__.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/alias.py` & `flict-1.0.9/flict/flictlib/alias.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/arbiter.py` & `flict-1.0.9/flict/flictlib/arbiter.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/compatibility.py` & `flict-1.0.9/flict/flictlib/compatibility.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/flict_config.py` & `flict-1.0.9/flict/flictlib/flict_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         except Exception:  # noqa: S110 - it's okay ignore all errors here
             pass
     return {}
 
 
 _userconfig = read_user_config()
 
-flict_version = "1.0.8"
+flict_version = "1.0.9"
 
 SCRIPT_DIR = os.path.realpath(os.path.join(os.path.dirname(os.path.realpath(__file__)), "../"))
 
 VAR_DIR = os.path.join(SCRIPT_DIR, "var")
 
 BUILTIN_ALIAS_FILE = os.path.join(VAR_DIR, "alias.json")
 DEFAULT_FLICT_ALIAS_FILE = os.path.join(VAR_DIR, BUILTIN_ALIAS_FILE)
```

### Comparing `flict-1.0.8/flict/flictlib/format/common.py` & `flict-1.0.9/flict/flictlib/format/common.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/format/dot_format.py` & `flict-1.0.9/flict/flictlib/format/dot_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/format/factory.py` & `flict-1.0.9/flict/flictlib/format/factory.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/format/format.py` & `flict-1.0.9/flict/flictlib/format/format.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/format/json_format.py` & `flict-1.0.9/flict/flictlib/format/json_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/format/markdown_format.py` & `flict-1.0.9/flict/flictlib/format/markdown_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/format/text_format.py` & `flict-1.0.9/flict/flictlib/format/text_format.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/lic_comp.py` & `flict-1.0.9/flict/flictlib/lic_comp.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/license.py` & `flict-1.0.9/flict/flictlib/license.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/license_parser.py` & `flict-1.0.9/flict/flictlib/license_parser.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/logger.py` & `flict-1.0.9/flict/flictlib/logger.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/project/reader.py` & `flict-1.0.9/flict/flictlib/project/reader.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/return_codes.py` & `flict-1.0.9/flict/flictlib/return_codes.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/flictlib/utils.py` & `flict-1.0.9/flict/flictlib/utils.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/impl.py` & `flict-1.0.9/flict/impl.py`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/var/alias.json` & `flict-1.0.9/flict/var/alias.json`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict/var/scancode-licenses.json` & `flict-1.0.9/flict/var/scancode-licenses.json`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict.egg-info/SOURCES.txt` & `flict-1.0.9/flict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flict-1.0.8/flict.egg-info/requires.txt` & `flict-1.0.9/flict.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 license-expression~=30.0
-osadl-matrix==2022.11.29.161124
+osadl-matrix==2022.12.2.81206
 wheel~=0.38
 
 [dev]
 bump2version~=1.0
 dataclasses~=0.6
 dlint~=0.13
 flake8-2020~=1.7
@@ -30,14 +30,14 @@
 flake8-string-format~=0.3
 flake8-variables-names==0.0.5
 flake8~=5.0
 pytest-bandit~=0.6
 pytest-cov~=4.0
 pytest-forked~=1.4
 pytest-icdiff~=0.6
-pytest-random-order~=1.0
+pytest-random-order~=1.1
 pytest-socket~=0.5
 pytest-sugar~=0.9
 pytest-tldr~=0.2
 pytest~=7.2
-reuse~=1.0
+reuse~=1.1
 twine~=4.0
```

### Comparing `flict-1.0.8/requirements-dev.txt` & `flict-1.0.9/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 flake8-string-format ~= 0.3
 flake8-variables-names == 0.0.5
 pytest ~= 7.2
 pytest-bandit ~= 0.6
 pytest-cov ~= 4.0
 pytest-forked ~= 1.4
 pytest-icdiff ~= 0.6
-pytest-random-order ~= 1.0
+pytest-random-order ~= 1.1
 pytest-socket ~= 0.5
 pytest-sugar ~= 0.9
 pytest-tldr ~= 0.2
 twine ~= 4.0
-reuse ~= 1.0
+reuse ~= 1.1
```

### Comparing `flict-1.0.8/setup.py` & `flict-1.0.9/setup.py`

 * *Files identical despite different names*

