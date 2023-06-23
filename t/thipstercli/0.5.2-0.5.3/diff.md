# Comparing `tmp/thipstercli-0.5.2.tar.gz` & `tmp/thipstercli-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.5.2.tar", last modified: Fri Jun 23 14:17:04 2023, max compression
+gzip compressed data, was "thipstercli-0.5.3.tar", last modified: Fri Jun 23 14:19:37 2023, max compression
```

## Comparing `thipstercli-0.5.2.tar` & `thipstercli-0.5.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:17:04.373800 thipstercli-0.5.2/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-23 14:17:00.000000 thipstercli-0.5.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-23 14:17:04.373800 thipstercli-0.5.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4516 2023-06-23 14:17:00.000000 thipstercli-0.5.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1372 2023-06-23 14:17:00.000000 thipstercli-0.5.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 14:17:04.373800 thipstercli-0.5.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1823 2023-06-23 14:17:00.000000 thipstercli-0.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:17:04.369800 thipstercli-0.5.2/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 14:17:00.000000 thipstercli-0.5.2/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-06-23 14:17:00.000000 thipstercli-0.5.2/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-06-23 14:17:00.000000 thipstercli-0.5.2/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-06-23 14:17:00.000000 thipstercli-0.5.2/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-06-23 14:17:00.000000 thipstercli-0.5.2/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-06-23 14:17:00.000000 thipstercli-0.5.2/tests/test_providers.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-23 14:17:00.000000 thipstercli-0.5.2/tests/test_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:17:04.373800 thipstercli-0.5.2/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6309 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:17:04.373800 thipstercli-0.5.2/thipstercli/commands/
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)     8194 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/commands/info.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/commands/providers.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/commands/repository.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/config.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/constants.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/display.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-06-23 14:17:00.000000 thipstercli-0.5.2/thipstercli/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:17:04.373800 thipstercli-0.5.2/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-23 14:17:04.000000 thipstercli-0.5.2/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      718 2023-06-23 14:17:04.000000 thipstercli-0.5.2/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 14:17:04.000000 thipstercli-0.5.2/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-23 14:17:04.000000 thipstercli-0.5.2/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      284 2023-06-23 14:17:04.000000 thipstercli-0.5.2/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-23 14:17:04.000000 thipstercli-0.5.2/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:19:37.480798 thipstercli-0.5.3/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-23 14:19:33.000000 thipstercli-0.5.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-23 14:19:37.480798 thipstercli-0.5.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-06-23 14:19:33.000000 thipstercli-0.5.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-23 14:19:33.000000 thipstercli-0.5.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 14:19:37.480798 thipstercli-0.5.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-23 14:19:34.000000 thipstercli-0.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:19:37.476798 thipstercli-0.5.3/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 14:19:33.000000 thipstercli-0.5.3/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-06-23 14:19:33.000000 thipstercli-0.5.3/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-06-23 14:19:33.000000 thipstercli-0.5.3/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-23 14:19:33.000000 thipstercli-0.5.3/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-06-23 14:19:33.000000 thipstercli-0.5.3/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-06-23 14:19:33.000000 thipstercli-0.5.3/tests/test_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-23 14:19:33.000000 thipstercli-0.5.3/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:19:37.480798 thipstercli-0.5.3/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6309 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:19:37.480798 thipstercli-0.5.3/thipstercli/commands/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)     8194 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/commands/info.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/commands/providers.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/commands/repository.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-06-23 14:19:33.000000 thipstercli-0.5.3/thipstercli/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:19:37.480798 thipstercli-0.5.3/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-23 14:19:37.000000 thipstercli-0.5.3/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      718 2023-06-23 14:19:37.000000 thipstercli-0.5.3/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 14:19:37.000000 thipstercli-0.5.3/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-23 14:19:37.000000 thipstercli-0.5.3/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-23 14:19:37.000000 thipstercli-0.5.3/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-23 14:19:37.000000 thipstercli-0.5.3/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.5.2/LICENSE` & `thipstercli-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/PKG-INFO` & `thipstercli-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.5.2
+Version: 0.5.3
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.5.2 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.5.3 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.5.2/README.md` & `thipstercli-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/pyproject.toml` & `thipstercli-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/setup.py` & `thipstercli-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('.').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.5.2'
+__version__ = '0.5.3'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as f:
     long_description = f.read()
```

### Comparing `thipstercli-0.5.2/tests/conftest.py` & `thipstercli-0.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/tests/test_cli.py` & `thipstercli-0.5.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/tests/test_config.py` & `thipstercli-0.5.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/tests/test_info.py` & `thipstercli-0.5.3/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/tests/test_providers.py` & `thipstercli-0.5.3/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/tests/test_repository.py` & `thipstercli-0.5.3/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/thipstercli/cli.py` & `thipstercli-0.5.3/thipstercli/cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/thipstercli/commands/config.py` & `thipstercli-0.5.3/thipstercli/commands/config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/thipstercli/commands/info.py` & `thipstercli-0.5.3/thipstercli/commands/info.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/thipstercli/commands/providers.py` & `thipstercli-0.5.3/thipstercli/commands/providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/thipstercli/commands/repository.py` & `thipstercli-0.5.3/thipstercli/commands/repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/thipstercli/config.py` & `thipstercli-0.5.3/thipstercli/config.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/thipstercli/display.py` & `thipstercli-0.5.3/thipstercli/display.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/thipstercli/helpers.py` & `thipstercli-0.5.3/thipstercli/helpers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.5.2/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.5.3/thipstercli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.5.2
+Version: 0.5.3
 Summary: CLI interface build with typer, designed to use the thipster package
 Home-page: https://github.com/THipster/THipster-cli
 Download-URL: https://github.com/THipster/THipster-cli.git
 License: MIT
 Keywords: thipster,cli,generator,infrastructure as code,iac,terraform,typer
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thipstercli Version: 0.5.2 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.5.3 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.5.2/thipstercli.egg-info/SOURCES.txt` & `thipstercli-0.5.3/thipstercli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

