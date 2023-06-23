# Comparing `tmp/commitizen-3.4.0.tar.gz` & `tmp/commitizen-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.4.0.tar", max compression
+gzip compressed data, was "commitizen-3.4.1.tar", max compression
```

## Comparing `commitizen-3.4.0.tar` & `commitizen-3.4.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-06-20 08:11:51.512833 commitizen-3.4.0/LICENSE
--rw-r--r--   0        0        0      609 2023-06-20 08:11:51.512833 commitizen-3.4.0/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-06-20 08:11:51.512833 commitizen-3.4.0/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-06-20 08:11:51.512833 commitizen-3.4.0/commitizen/__version__.py
--rw-r--r--   0        0        0     4609 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/bump.py
--rw-r--r--   0        0        0    11712 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/changelog.py
--rw-r--r--   0        0        0     3455 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    17490 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    13971 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7142 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5075 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/check.py
--rw-r--r--   0        0        0     3435 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/info.py
--rw-r--r--   0        0        0    12966 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/commands/version.py
--rw-r--r--   0        0        0     1235 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/config/__init__.py
--rw-r--r--   0        0        0      898 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1568 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1746 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1431 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1213 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2983 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7070 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      287 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3176 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/defaults.py
--rw-r--r--   0        0        0     4706 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/factory.py
--rw-r--r--   0        0        0     6900 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/out.py
--rw-r--r--   0        0        0     7109 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     9690 2023-06-20 08:11:51.516833 commitizen-3.4.0/commitizen/version_schemes.py
--rw-r--r--   0        0        0     5750 2023-06-20 08:11:51.516833 commitizen-3.4.0/docs/README.md
--rw-r--r--   0        0        0     4202 2023-06-20 08:11:51.528833 commitizen-3.4.0/pyproject.toml
--rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-23 09:22:51.472965 commitizen-3.4.1/LICENSE
+-rw-r--r--   0        0        0      609 2023-06-23 09:22:51.472965 commitizen-3.4.1/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-23 09:22:51.472965 commitizen-3.4.1/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-23 09:22:51.472965 commitizen-3.4.1/commitizen/__version__.py
+-rw-r--r--   0        0        0     4609 2023-06-23 09:22:51.472965 commitizen-3.4.1/commitizen/bump.py
+-rw-r--r--   0        0        0    11712 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/changelog.py
+-rw-r--r--   0        0        0     3455 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    17490 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    13971 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7142 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5075 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3435 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12966 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1235 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1568 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1746 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1431 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1213 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2983 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7070 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3121 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      287 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3176 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/defaults.py
+-rw-r--r--   0        0        0     4706 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/factory.py
+-rw-r--r--   0        0        0     6900 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/out.py
+-rw-r--r--   0        0        0     7109 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     9732 2023-06-23 09:22:51.476965 commitizen-3.4.1/commitizen/version_schemes.py
+-rw-r--r--   0        0        0     5750 2023-06-23 09:22:51.476965 commitizen-3.4.1/docs/README.md
+-rw-r--r--   0        0        0     4200 2023-06-23 09:22:51.488965 commitizen-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7283 1970-01-01 00:00:00.000000 commitizen-3.4.1/PKG-INFO
```

### Comparing `commitizen-3.4.0/LICENSE` & `commitizen-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/__init__.py` & `commitizen-3.4.1/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/bump.py` & `commitizen-3.4.1/commitizen/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/changelog.py` & `commitizen-3.4.1/commitizen/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/changelog_parser.py` & `commitizen-3.4.1/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/cli.py` & `commitizen-3.4.1/commitizen/cli.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/cmd.py` & `commitizen-3.4.1/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/commands/bump.py` & `commitizen-3.4.1/commitizen/commands/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/commands/changelog.py` & `commitizen-3.4.1/commitizen/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/commands/check.py` & `commitizen-3.4.1/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/commands/commit.py` & `commitizen-3.4.1/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/commands/init.py` & `commitizen-3.4.1/commitizen/commands/init.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/commands/version.py` & `commitizen-3.4.1/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/config/__init__.py` & `commitizen-3.4.1/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/config/base_config.py` & `commitizen-3.4.1/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/config/json_config.py` & `commitizen-3.4.1/commitizen/config/json_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/config/toml_config.py` & `commitizen-3.4.1/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/config/yaml_config.py` & `commitizen-3.4.1/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/cz/__init__.py` & `commitizen-3.4.1/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/cz/base.py` & `commitizen-3.4.1/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.4.1/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.4.1/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/cz/customize/customize.py` & `commitizen-3.4.1/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/cz/jira/jira.py` & `commitizen-3.4.1/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/cz/jira/jira_info.txt` & `commitizen-3.4.1/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/defaults.py` & `commitizen-3.4.1/commitizen/defaults.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/exceptions.py` & `commitizen-3.4.1/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/factory.py` & `commitizen-3.4.1/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/git.py` & `commitizen-3.4.1/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/hooks.py` & `commitizen-3.4.1/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/out.py` & `commitizen-3.4.1/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/providers.py` & `commitizen-3.4.1/commitizen/providers.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/commitizen/version_schemes.py` & `commitizen-3.4.1/commitizen/version_schemes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
-from itertools import zip_longest
 import re
 import sys
-
-from typing import TYPE_CHECKING, ClassVar, Type, cast
 import warnings
-from commitizen.config.base_config import BaseConfig
-from commitizen.exceptions import VersionSchemeUnknown
+from itertools import zip_longest
+from typing import TYPE_CHECKING, ClassVar, Type, cast
 
 import importlib_metadata as metadata
-from packaging.version import Version as _BaseVersion
 from packaging.version import InvalidVersion  # noqa: F401: Rexpose the common exception
+from packaging.version import Version as _BaseVersion
+
+from commitizen.config.base_config import BaseConfig
 from commitizen.defaults import MAJOR, MINOR, PATCH
+from commitizen.exceptions import VersionSchemeUnknown
 
 if sys.version_info >= (3, 8):
     from typing import Protocol, runtime_checkable
 else:
     from typing_extensions import Protocol, runtime_checkable
 
 if TYPE_CHECKING:
@@ -25,14 +25,16 @@
         from typing import TypeAlias
     else:
         from typing_extensions import TypeAlias
 
     # Self is Python 3.11+ but backported in typing-extensions
     if sys.version_info < (3, 11):
         from typing_extensions import Self
+    else:
+        from typing import Self
 
 
 DEFAULT_VERSION_PARSER = r"v?(?P<version>([0-9]+)\.([0-9]+)\.([0-9]+)(?:-([0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+[0-9A-Za-z-]+)?(\w+)?)"
 
 
 @runtime_checkable
 class VersionProtocol(Protocol):
@@ -99,15 +101,15 @@
     def bump(
         self,
         increment: str,
         prerelease: str | None = None,
         prerelease_offset: int = 0,
         devrelease: int | None = None,
         is_local_version: bool = False,
-    ) -> Self:  # type: ignore
+    ) -> Self:
         """
         Based on the given increment, generate the next bumped version according to the version scheme
         """
 
 
 # With PEP 440 and SemVer semantic, Scheme is the type, Version is an instance
 Version: TypeAlias = VersionProtocol
@@ -194,36 +196,36 @@
     def bump(
         self,
         increment: str,
         prerelease: str | None = None,
         prerelease_offset: int = 0,
         devrelease: int | None = None,
         is_local_version: bool = False,
-    ) -> Self:  # type: ignore
+    ) -> Self:
         """Based on the given increment a proper semver will be generated.
 
         For now the rules and versioning scheme is based on
         python's PEP 0440.
         More info: https://www.python.org/dev/peps/pep-0440/
 
         Example:
             PATCH 1.0.0 -> 1.0.1
             MINOR 1.0.0 -> 1.1.0
             MAJOR 1.0.0 -> 2.0.0
         """
 
         if self.local and is_local_version:
             local_version = self.scheme(self.local).bump(increment)
-            return self.scheme(f"{self.public}+{local_version}")
+            return self.scheme(f"{self.public}+{local_version}")  # type: ignore
         else:
             base = self.increment_base(increment)
             dev_version = self.generate_devrelease(devrelease)
             pre_version = self.generate_prerelease(prerelease, offset=prerelease_offset)
             # TODO: post version
-            return self.scheme(f"{base}{pre_version}{dev_version}")
+            return self.scheme(f"{base}{pre_version}{dev_version}")  # type: ignore
 
 
 class Pep440(BaseVersion):
     """
     PEP 440 Version Scheme
 
     See: https://peps.python.org/pep-0440/
```

### Comparing `commitizen-3.4.0/docs/README.md` & `commitizen-3.4.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.4.0/pyproject.toml` & `commitizen-3.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.4.0"
+version = "3.4.1"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.4.0"
+version = "3.4.1"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
@@ -39,15 +39,15 @@
 decli = "^0.6.0"
 colorama = "^0.4.1"
 termcolor = ">= 1.1, < 3"
 packaging = ">=19"
 tomlkit = ">=0.5.3,<1.0.0"
 jinja2 = ">=2.10.3"
 pyyaml = ">=3.08"
-argcomplete = ">=1.12.1,<3.1"
+argcomplete = ">=1.12.1,<3.2"
 typing-extensions = { version = "^4.0.1", python = "<3.8" }
 charset-normalizer = ">=2.1.0,<4"
 # Use the Python 3.11 and 3.12 compatible API: https://github.com/python/importlib_metadata#compatibility
 importlib_metadata = { version = ">=4.13,<7"}
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^7.34"
@@ -57,17 +57,17 @@
 pytest-mock = "^3.10"
 pytest-regressions = "^2.4.0"
 pytest-freezer = "^0.4.6"
 pytest-xdist = "^3.1.0"
 # code formatter
 black = "^22.10"
 # linter
-ruff = "^0.0.262"
+ruff = "^0.0.275"
 pre-commit = "^2.18.0"
-mypy = "^0.931"
+mypy = "^1.4"
 types-PyYAML = "^5.4.3"
 types-termcolor = "^0.1.1"
 # documentation
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.6"
```

### Comparing `commitizen-3.4.0/PKG-INFO` & `commitizen-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.4.0
+Version: 3.4.1
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Dist: argcomplete (>=1.12.1,<3.1)
+Requires-Dist: argcomplete (>=1.12.1,<3.2)
 Requires-Dist: charset-normalizer (>=2.1.0,<4)
 Requires-Dist: colorama (>=0.4.1,<0.5.0)
 Requires-Dist: decli (>=0.6.0,<0.7.0)
 Requires-Dist: importlib_metadata (>=4.13,<7)
 Requires-Dist: jinja2 (>=2.10.3)
 Requires-Dist: packaging (>=19)
 Requires-Dist: pyyaml (>=3.08)
```

