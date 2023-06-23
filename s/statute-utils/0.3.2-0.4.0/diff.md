# Comparing `tmp/statute_utils-0.3.2.tar.gz` & `tmp/statute_utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.3.2.tar", max compression
+gzip compressed data, was "statute_utils-0.4.0.tar", max compression
```

## Comparing `statute_utils-0.3.2.tar` & `statute_utils-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.3.2/LICENSE
--rw-r--r--   0        0        0      898 2023-06-21 15:08:07.622003 statute_utils-0.3.2/README.md
--rw-r--r--   0        0        0     1449 2023-06-22 07:34:05.596909 statute_utils-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      368 2023-06-22 07:34:05.597276 statute_utils-0.3.2/statute_utils/__init__.py
--rw-r--r--   0        0        0      319 2023-06-22 05:28:27.921068 statute_utils-0.3.2/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     9222 2023-06-22 07:34:05.597692 statute_utils-0.3.2/statute_utils/components/category.py
--rw-r--r--   0        0        0     3517 2023-06-22 07:34:05.598060 statute_utils-0.3.2/statute_utils/components/details.py
--rw-r--r--   0        0        0     4682 2023-06-22 07:34:05.598375 statute_utils-0.3.2/statute_utils/components/rule.py
--rw-r--r--   0        0        0     2015 2023-06-22 05:28:27.921653 statute_utils-0.3.2/statute_utils/components/short.py
--rw-r--r--   0        0        0     3326 2023-06-22 06:12:44.626570 statute_utils-0.3.2/statute_utils/components/utils.py
--rw-r--r--   0        0        0     4187 2023-06-22 07:34:05.598711 statute_utils-0.3.2/statute_utils/main.py
--rw-r--r--   0        0        0     5195 2023-06-22 06:12:44.627181 statute_utils-0.3.2/statute_utils/models.py
--rw-r--r--   0        0        0     4434 2023-06-22 06:12:44.627800 statute_utils-0.3.2/statute_utils/names.py
--rw-r--r--   0        0        0      249 2023-06-22 05:28:27.922206 statute_utils-0.3.2/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.3.2/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.3.2/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.3.2/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.3.2/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     6618 2023-06-22 06:11:13.995177 statute_utils-0.3.2/statute_utils/serials.py
--rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 statute_utils-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.4.0/LICENSE
+-rw-r--r--   0        0        0      898 2023-06-21 15:08:07.622003 statute_utils-0.4.0/README.md
+-rw-r--r--   0        0        0     1449 2023-06-23 10:42:11.417437 statute_utils-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      368 2023-06-22 07:34:05.597276 statute_utils-0.4.0/statute_utils/__init__.py
+-rw-r--r--   0        0        0      319 2023-06-22 05:28:27.921068 statute_utils-0.4.0/statute_utils/components/__init__.py
+-rw-r--r--   0        0        0     9198 2023-06-23 10:40:49.094740 statute_utils-0.4.0/statute_utils/components/category.py
+-rw-r--r--   0        0        0     3517 2023-06-22 07:34:05.598060 statute_utils-0.4.0/statute_utils/components/details.py
+-rw-r--r--   0        0        0     4679 2023-06-23 10:46:22.018647 statute_utils-0.4.0/statute_utils/components/rule.py
+-rw-r--r--   0        0        0     2015 2023-06-22 05:28:27.921653 statute_utils-0.4.0/statute_utils/components/short.py
+-rw-r--r--   0        0        0     3326 2023-06-22 06:12:44.626570 statute_utils-0.4.0/statute_utils/components/utils.py
+-rw-r--r--   0        0        0     4192 2023-06-23 10:44:32.008135 statute_utils-0.4.0/statute_utils/main.py
+-rw-r--r--   0        0        0     5170 2023-06-23 10:41:31.532335 statute_utils-0.4.0/statute_utils/models.py
+-rw-r--r--   0        0        0     4434 2023-06-22 06:12:44.627800 statute_utils-0.4.0/statute_utils/names.py
+-rw-r--r--   0        0        0      249 2023-06-22 05:28:27.922206 statute_utils-0.4.0/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.4.0/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.4.0/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.4.0/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.4.0/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     6618 2023-06-22 06:11:13.995177 statute_utils-0.4.0/statute_utils/serials.py
+-rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 statute_utils-0.4.0/PKG-INFO
```

### Comparing `statute_utils-0.3.2/LICENSE` & `statute_utils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.2/README.md` & `statute_utils-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.2/pyproject.toml` & `statute_utils-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.3.2"
+version = "0.4.0"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.3.2/statute_utils/components/category.py` & `statute_utils-0.4.0/statute_utils/components/category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import re
 from enum import StrEnum, auto
-from typing import Self
 
 from pydantic import BaseModel, ConfigDict
 
 
 class StatuteTitleCategory(StrEnum):
     """
     A [`Rule`][rule-model] in the Philippines involves various denominations.
```

### Comparing `statute_utils-0.3.2/statute_utils/components/details.py` & `statute_utils-0.4.0/statute_utils/components/details.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.2/statute_utils/components/rule.py` & `statute_utils-0.4.0/statute_utils/components/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     1. [`Named Patterns`][named-pattern] or
     2. [`Serial Patterns`][serial-pattern]
 
     Each rule implies:
 
     1. Previous validation via regex strings
-    2. Serial title generated by [`StatuteSerialCategory.serialize()`][statute_patterns.components.category.StatuteSerialCategory.serialize]
+    2. Serial title generated by [`StatuteSerialCategory.serialize()`][statute_utils.components.category.StatuteSerialCategory.serialize]
     """  # noqa: E501
 
     model_config = ConfigDict(use_enum_values=True)
     cat: StatuteSerialCategory = Field(
         ...,
         title="Statute Category",
         description="Classification under the limited StatuteSerialCategory taxonomy.",
```

### Comparing `statute_utils-0.3.2/statute_utils/components/short.py` & `statute_utils-0.4.0/statute_utils/components/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.2/statute_utils/components/utils.py` & `statute_utils-0.4.0/statute_utils/components/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.2/statute_utils/main.py` & `statute_utils-0.4.0/statute_utils/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             >>> str(results[0])
             'Republic Act No. 386'
             >>> repr(results[0])
             'ra 386: 2'
 
 
         Args:
-            texts (str): list of texts having `__repr__` format of a `CountedRule`
+            repr_texts (str): list of texts having `__repr__` format of a `CountedRule`
 
         Yields:
             Iterator[Self]: Instances of CountedRule
         """
         for text in repr_texts:
             counted_bits = text.split(":")
             if len(counted_bits) == 2:
```

### Comparing `statute_utils-0.3.2/statute_utils/models.py` & `statute_utils-0.4.0/statute_utils/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import re
 from collections.abc import Iterator
 from re import Pattern
 
 from pydantic import Field
 
-from .components import (
-    BaseCollection,
-    BasePattern,
-    Rule,
-    StatuteSerialCategory,
-    stx,
-)
+from .components import BaseCollection, BasePattern, Rule, StatuteSerialCategory, stx
 from .recipes import split_digits
 
 
 class NamedPattern(BasePattern):
     """A [`Rule`][rule-model] can be extracted from a `NamedPattern`"""
 
     name: str
```

### Comparing `statute_utils-0.3.2/statute_utils/names.py` & `statute_utils-0.4.0/statute_utils/names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.2/statute_utils/recipes/digits.py` & `statute_utils-0.4.0/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.2/statute_utils/recipes/spain.py` & `statute_utils-0.4.0/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.2/statute_utils/serials.py` & `statute_utils-0.4.0/statute_utils/serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.3.2/PKG-INFO` & `statute_utils-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.3.2
+Version: 0.4.0
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
```

