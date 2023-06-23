# Comparing `tmp/thipstercli-0.4.3.tar.gz` & `tmp/thipstercli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipstercli-0.4.3.tar", last modified: Thu Jun 22 10:30:59 2023, max compression
+gzip compressed data, was "thipstercli-0.5.0.tar", last modified: Thu Jun 22 14:26:55 2023, max compression
```

## Comparing `thipstercli-0.4.3.tar` & `thipstercli-0.5.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:30:59.525079 thipstercli-0.4.3/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-22 10:30:54.000000 thipstercli-0.4.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-22 10:30:59.525079 thipstercli-0.4.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4516 2023-06-22 10:30:54.000000 thipstercli-0.4.3/README.md
--rw-r--r--   0 root         (0) root         (0)     1372 2023-06-22 10:30:54.000000 thipstercli-0.4.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 10:30:59.525079 thipstercli-0.4.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1823 2023-06-22 10:30:55.000000 thipstercli-0.4.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:30:59.521079 thipstercli-0.4.3/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     3847 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     3155 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/test_providers.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-22 10:30:54.000000 thipstercli-0.4.3/tests/test_repository.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:30:59.525079 thipstercli-0.4.3/thipstercli/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6309 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:30:59.525079 thipstercli-0.4.3/thipstercli/commands/
--rw-r--r--   0 root         (0) root         (0)      131 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8194 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/commands/info.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/commands/providers.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/commands/repository.py
--rw-r--r--   0 root         (0) root         (0)     1881 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/config.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/constants.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/display.py
--rw-r--r--   0 root         (0) root         (0)     2686 2023-06-22 10:30:54.000000 thipstercli-0.4.3/thipstercli/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:30:59.525079 thipstercli-0.4.3/thipstercli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5204 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      284 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-22 10:30:59.000000 thipstercli-0.4.3/thipstercli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:26:55.702053 thipstercli-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-22 14:26:51.000000 thipstercli-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-22 14:26:55.702053 thipstercli-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4516 2023-06-22 14:26:51.000000 thipstercli-0.5.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-22 14:26:51.000000 thipstercli-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 14:26:55.702053 thipstercli-0.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-22 14:26:52.000000 thipstercli-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:26:55.698053 thipstercli-0.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:26:51.000000 thipstercli-0.5.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-06-22 14:26:51.000000 thipstercli-0.5.0/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-06-22 14:26:51.000000 thipstercli-0.5.0/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-22 14:26:51.000000 thipstercli-0.5.0/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-06-22 14:26:51.000000 thipstercli-0.5.0/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     3155 2023-06-22 14:26:51.000000 thipstercli-0.5.0/tests/test_providers.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-22 14:26:51.000000 thipstercli-0.5.0/tests/test_repository.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:26:55.702053 thipstercli-0.5.0/thipstercli/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6309 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:26:55.702053 thipstercli-0.5.0/thipstercli/commands/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)     8194 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/commands/info.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/commands/providers.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/commands/repository.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/config.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/display.py
+-rw-r--r--   0 root         (0) root         (0)     2686 2023-06-22 14:26:51.000000 thipstercli-0.5.0/thipstercli/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:26:55.702053 thipstercli-0.5.0/thipstercli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5204 2023-06-22 14:26:55.000000 thipstercli-0.5.0/thipstercli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      718 2023-06-22 14:26:55.000000 thipstercli-0.5.0/thipstercli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:26:55.000000 thipstercli-0.5.0/thipstercli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-22 14:26:55.000000 thipstercli-0.5.0/thipstercli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-22 14:26:55.000000 thipstercli-0.5.0/thipstercli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-22 14:26:55.000000 thipstercli-0.5.0/thipstercli.egg-info/top_level.txt
```

### Comparing `thipstercli-0.4.3/LICENSE` & `thipstercli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/PKG-INFO` & `thipstercli-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.4.3
+Version: 0.5.0
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
-Metadata-Version: 2.1 Name: thipstercli Version: 0.4.3 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.5.0 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.4.3/README.md` & `thipstercli-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/pyproject.toml` & `thipstercli-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/setup.py` & `thipstercli-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     for req_file in Path('.').glob('requirements-*.txt'):
         extras_require[
             req_file.stem.removeprefix('requirements-')
         ] = req_file.read_text().splitlines()
     return extras_require
 
 
-__version__ = '0.4.3'
+__version__ = '0.5.0'
 
 with Path('requirements.txt').open() as f:
     required = f.read().splitlines()
 
 with Path('README.md').open() as f:
     long_description = f.read()
```

### Comparing `thipstercli-0.4.3/tests/conftest.py` & `thipstercli-0.5.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,29 +35,30 @@
 
 
 @pytest.fixture
 def config_file(
     create_config_file,
 ):
     """Create a user config file with default values."""
-    create_config_file.write_text("""{
+    conf_str = """{
         "app_name": "thipstercli",
         "auth_provider": "google",
         "input_dir": "test/input_directory",
         "local_models_repository_path": "models",
         "models_repository": "THipster/models",
         "models_repository_branch": "main",
-        "models_repository_provider": "local",
+        "repository_recovery_mode": "local",
         "output_dir": "test/output_directory",
         "verbose": true
-}""")
+}"""
+    create_config_file.write_text(conf_str)
 
     init_parameters()
 
-    yield
+    yield json.loads(conf_str)
 
 
 @pytest.fixture
 def empty_config_file(create_config_file):
     """Create an empty user config file."""
     create_config_file.write_text("""{}""")
     init_parameters()
```

### Comparing `thipstercli-0.4.3/tests/test_cli.py` & `thipstercli-0.5.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/tests/test_info.py` & `thipstercli-0.5.0/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/tests/test_providers.py` & `thipstercli-0.5.0/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/tests/test_repository.py` & `thipstercli-0.5.0/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/thipstercli/cli.py` & `thipstercli-0.5.0/thipstercli/cli.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/thipstercli/commands/info.py` & `thipstercli-0.5.0/thipstercli/commands/info.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/thipstercli/commands/providers.py` & `thipstercli-0.5.0/thipstercli/commands/providers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/thipstercli/commands/repository.py` & `thipstercli-0.5.0/thipstercli/commands/repository.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/thipstercli/config.py` & `thipstercli-0.5.0/thipstercli/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,7 +50,17 @@
         config: dict[str, object] = json.loads(config_file.read_text())
         config.update(parameters)
     else:
         config_file.parent.mkdir(parents=True, exist_ok=True)
         config = parameters
 
     config_file.write_text(json.dumps(config, sort_keys=True, indent=4))
+
+
+def set_config_file(new_config: dict[str, object]) -> None:
+    """Update the config file with the given parameters."""
+    if not config_file.is_file():
+        config_file.parent.mkdir(parents=True, exist_ok=True)
+
+    config = new_config
+
+    config_file.write_text(json.dumps(config, sort_keys=True, indent=4))
```

### Comparing `thipstercli-0.4.3/thipstercli/display.py` & `thipstercli-0.5.0/thipstercli/display.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/thipstercli/helpers.py` & `thipstercli-0.5.0/thipstercli/helpers.py`

 * *Files identical despite different names*

### Comparing `thipstercli-0.4.3/thipstercli.egg-info/PKG-INFO` & `thipstercli-0.5.0/thipstercli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipstercli
-Version: 0.4.3
+Version: 0.5.0
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
-Metadata-Version: 2.1 Name: thipstercli Version: 0.4.3 Summary: CLI interface
+Metadata-Version: 2.1 Name: thipstercli Version: 0.5.0 Summary: CLI interface
 build with typer, designed to use the thipster package Home-page: https://
 github.com/THipster/THipster-cli Download-URL: https://github.com/THipster/
 THipster-cli.git License: MIT Keywords: thipster,cli,generator,infrastructure
 as code,iac,terraform,typer Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console Classifier: Programming Language :: Python
 :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `thipstercli-0.4.3/thipstercli.egg-info/SOURCES.txt` & `thipstercli-0.5.0/thipstercli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
+tests/test_config.py
 tests/test_info.py
 tests/test_providers.py
 tests/test_repository.py
 thipstercli/__init__.py
 thipstercli/__main__.py
 thipstercli/cli.py
 thipstercli/config.py
@@ -18,10 +19,11 @@
 thipstercli.egg-info/PKG-INFO
 thipstercli.egg-info/SOURCES.txt
 thipstercli.egg-info/dependency_links.txt
 thipstercli.egg-info/entry_points.txt
 thipstercli.egg-info/requires.txt
 thipstercli.egg-info/top_level.txt
 thipstercli/commands/__init__.py
+thipstercli/commands/config.py
 thipstercli/commands/info.py
 thipstercli/commands/providers.py
 thipstercli/commands/repository.py
```

