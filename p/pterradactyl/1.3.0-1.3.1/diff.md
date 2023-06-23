# Comparing `tmp/pterradactyl-1.3.0.tar.gz` & `tmp/pterradactyl-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pterradactyl-1.3.0.tar", max compression
+gzip compressed data, was "pterradactyl-1.3.1.tar", max compression
```

## Comparing `pterradactyl-1.3.0.tar` & `pterradactyl-1.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    10346 2023-05-31 15:12:27.938916 pterradactyl-1.3.0/LICENSE.md
--rw-r--r--   0        0        0     8039 2023-05-31 15:12:27.938916 pterradactyl-1.3.0/README.md
--rw-r--r--   0        0        0       69 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/__init__.py
--rw-r--r--   0        0        0      188 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/__main__.py
--rw-r--r--   0        0        0     1082 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/cli.py
--rw-r--r--   0        0        0        0 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/__init__.py
--rw-r--r--   0        0        0      261 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/base.py
--rw-r--r--   0        0        0      814 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/dump.py
--rw-r--r--   0        0        0      129 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/env.py
--rw-r--r--   0        0        0     2307 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/lookup.py
--rw-r--r--   0        0        0     1407 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/manifest.py
--rw-r--r--   0        0        0      140 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/commands/state.py
--rw-r--r--   0        0        0     4292 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/config.py
--rw-r--r--   0        0        0      918 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/arguments.py
--rw-r--r--   0        0        0      151 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/base.py
--rw-r--r--   0        0        0      254 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/environment.py
--rw-r--r--   0        0        0      384 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/jinja.py
--rw-r--r--   0        0        0     1269 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/regex.py
--rw-r--r--   0        0        0     1225 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/shell.py
--rw-r--r--   0        0        0     2028 2023-05-31 15:12:27.942916 pterradactyl-1.3.0/pterradactyl/facter/woops/manifest_path.py
--rw-r--r--   0        0        0        0 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/terraform/__init__.py
--rw-r--r--   0        0        0     3406 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/terraform/config.py
--rw-r--r--   0        0        0     9344 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/terraform/terraform.py
--rw-r--r--   0        0        0      699 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/util/__init__.py
--rw-r--r--   0        0        0     2016 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/util/download.py
--rw-r--r--   0        0        0     2721 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/util/filesystem.py
--rw-r--r--   0        0        0      121 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/util/package.py
--rw-r--r--   0        0        0      794 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/validator/__init__.py
--rw-r--r--   0        0        0      169 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/validator/base.py
--rw-r--r--   0        0        0      764 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pterradactyl/validator/version.py
--rw-r--r--   0        0        0     2773 2023-05-31 15:12:27.946916 pterradactyl-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     9017 1970-01-01 00:00:00.000000 pterradactyl-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10346 2023-06-23 14:01:18.029620 pterradactyl-1.3.1/LICENSE.md
+-rw-r--r--   0        0        0     8039 2023-06-23 14:01:18.029620 pterradactyl-1.3.1/README.md
+-rw-r--r--   0        0        0       72 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/__init__.py
+-rw-r--r--   0        0        0      188 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/__main__.py
+-rw-r--r--   0        0        0     1082 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/cli.py
+-rw-r--r--   0        0        0        0 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/commands/__init__.py
+-rw-r--r--   0        0        0      261 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/commands/base.py
+-rw-r--r--   0        0        0      814 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/commands/dump.py
+-rw-r--r--   0        0        0      129 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/commands/env.py
+-rw-r--r--   0        0        0     2307 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/commands/lookup.py
+-rw-r--r--   0        0        0     1407 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/commands/manifest.py
+-rw-r--r--   0        0        0      140 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/commands/state.py
+-rw-r--r--   0        0        0     4292 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/config.py
+-rw-r--r--   0        0        0      918 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/facter/__init__.py
+-rw-r--r--   0        0        0     1738 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/facter/arguments.py
+-rw-r--r--   0        0        0      151 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/facter/base.py
+-rw-r--r--   0        0        0      254 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/facter/environment.py
+-rw-r--r--   0        0        0      384 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/facter/jinja.py
+-rw-r--r--   0        0        0     1269 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/facter/regex.py
+-rw-r--r--   0        0        0     1225 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/facter/shell.py
+-rw-r--r--   0        0        0     2028 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/facter/woops/manifest_path.py
+-rw-r--r--   0        0        0        0 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/terraform/__init__.py
+-rw-r--r--   0        0        0     3406 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/terraform/config.py
+-rw-r--r--   0        0        0     9344 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/terraform/terraform.py
+-rw-r--r--   0        0        0      699 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/util/__init__.py
+-rw-r--r--   0        0        0     2016 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/util/download.py
+-rw-r--r--   0        0        0     2721 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/util/filesystem.py
+-rw-r--r--   0        0        0      125 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/util/package.py
+-rw-r--r--   0        0        0      794 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/validator/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/validator/base.py
+-rw-r--r--   0        0        0      764 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pterradactyl/validator/version.py
+-rw-r--r--   0        0        0     2875 2023-06-23 14:01:18.037620 pterradactyl-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8932 1970-01-01 00:00:00.000000 pterradactyl-1.3.1/PKG-INFO
```

### Comparing `pterradactyl-1.3.0/LICENSE.md` & `pterradactyl-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/README.md` & `pterradactyl-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/cli.py` & `pterradactyl-1.3.1/pterradactyl/cli.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/commands/dump.py` & `pterradactyl-1.3.1/pterradactyl/commands/dump.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/commands/lookup.py` & `pterradactyl-1.3.1/pterradactyl/commands/lookup.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/commands/manifest.py` & `pterradactyl-1.3.1/pterradactyl/commands/manifest.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/config.py` & `pterradactyl-1.3.1/pterradactyl/config.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/facter/__init__.py` & `pterradactyl-1.3.1/pterradactyl/facter/__init__.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/facter/arguments.py` & `pterradactyl-1.3.1/pterradactyl/facter/arguments.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/facter/regex.py` & `pterradactyl-1.3.1/pterradactyl/facter/regex.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/facter/shell.py` & `pterradactyl-1.3.1/pterradactyl/facter/shell.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/facter/woops/manifest_path.py` & `pterradactyl-1.3.1/pterradactyl/facter/woops/manifest_path.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/terraform/config.py` & `pterradactyl-1.3.1/pterradactyl/terraform/config.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/terraform/terraform.py` & `pterradactyl-1.3.1/pterradactyl/terraform/terraform.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/util/__init__.py` & `pterradactyl-1.3.1/pterradactyl/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/util/download.py` & `pterradactyl-1.3.1/pterradactyl/util/download.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/util/filesystem.py` & `pterradactyl-1.3.1/pterradactyl/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/validator/__init__.py` & `pterradactyl-1.3.1/pterradactyl/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pterradactyl/validator/version.py` & `pterradactyl-1.3.1/pterradactyl/validator/version.py`

 * *Files identical despite different names*

### Comparing `pterradactyl-1.3.0/pyproject.toml` & `pterradactyl-1.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pterradactyl"
-version = "1.3.0"
+version = "1.3.1"
 description = "hiera-inspired terraform wrapper"
 authors = ["Rob King <rob.king@nike.com>",
            "Vincent Liu <vincent.liu@nike.com>"
 ]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
@@ -15,23 +15,27 @@
 packages = [
     { include = "pterradactyl" },
 ]
 repository = "https://github.com/Nike-Inc/pterradactyl"
 
 [tool.poetry.dependencies]
 python = "^3.10.10"
-python-interface = "^1.5.3"
-pyyaml = "^6.0.0"
-jinja2 = "^2.11.1"
-MarkupSafe = "2.0.1"
-appdirs = "^1.4.3"
-jsonpath-ng = "^1.5.1"
-semantic_version = "^2.8.4"
-phiera = "^2.1.0"
-requests = "^2.24.0"
+pyyaml = { version = "^6.0.0" }
+jinja2 = { version = "^3.1.2" }
+appdirs = { version = "^1.4.4" }
+jsonpath-ng = { version = "^1.5.3" }
+semantic_version = { version = "^2.10.0" }
+phiera = { version = "^2.1.0" }
+requests = { version = "^2.31.0" }
+
+[tool.poetry.group.dev.dependencies]
+pytest = { version = "^7.3.1" }
+pytest-cov = { version = "^4.1.0" }
+testfixtures = { version = "^7.1.0" }
+responses = { version = "^0.23.1" }
 
 [tool.poetry.scripts]
 pt = "pterradactyl.__main__:main"
 
 [tool.poetry.plugins."pterradactyl.registered_commands"]
 apply = "pterradactyl.commands.manifest:ManifestCommand"
 console = "pterradactyl.commands.manifest:ManifestCommand"
@@ -52,29 +56,20 @@
 validate = "pterradactyl.commands.manifest:ManifestCommand"
 workspace = "pterradactyl.commands.manifest:ManifestCommand"
 state = "pterradactyl.commands.state:StateCommand"
 root-module = "pterradactyl.commands.dump:DumpRootModuleCommand"
 facts = "pterradactyl.commands.dump:DumpFactsCommand"
 lookup = "pterradactyl.commands.lookup:LookupCommand"
 
-
 [tool.poetry.plugins."pterradactyl.facters"]
 arguments = "pterradactyl.facter.arguments:ArgumentsFacter"
 jinja = "pterradactyl.facter.jinja:JinjaFacter"
 shell = "pterradactyl.facter.shell:ShellFacter"
 environment = "pterradactyl.facter.environment:EnvironmentFacter"
 regex = "pterradactyl.facter.regex:RegexFacter"
 
-
 [tool.poetry.plugins."pterradactyl.validators"]
 version = "pterradactyl.validator.version:VersionValidator"
 
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
-pytest-cov = "^4.1.0"
-testfixtures = "^7.1.0"
-responses = "^0.23.1"
-
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.5.3"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pterradactyl-1.3.0/PKG-INFO` & `pterradactyl-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: pterradactyl
-Version: 1.3.0
+Version: 1.3.1
 Summary: hiera-inspired terraform wrapper
 Home-page: https://github.com/Nike-Inc/pterradactyl
 License: Apache-2.0
 Author: Rob King
 Author-email: rob.king@nike.com
 Maintainer: Mohamed Abdul Huq Ismail
 Maintainer-email: Abdul.Ismail@nike.com
 Requires-Python: >=3.10.10,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: MarkupSafe (==2.0.1)
-Requires-Dist: appdirs (>=1.4.3,<2.0.0)
-Requires-Dist: jinja2 (>=2.11.1,<3.0.0)
-Requires-Dist: jsonpath-ng (>=1.5.1,<2.0.0)
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
 Requires-Dist: phiera (>=2.1.0,<3.0.0)
-Requires-Dist: python-interface (>=1.5.3,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
-Requires-Dist: requests (>=2.24.0,<3.0.0)
-Requires-Dist: semantic_version (>=2.8.4,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: semantic_version (>=2.10.0,<3.0.0)
 Project-URL: Repository, https://github.com/Nike-Inc/pterradactyl
 Description-Content-Type: text/markdown
 
 Pterradactyl
 ---
 
 [![codecov](https://codecov.io/gh/Nike-Inc/pterradactyl/branch/master/graph/badge.svg?token=CvHYOh04mZ)](https://codecov.io/gh/Nike-Inc/pterradactyl)
```

