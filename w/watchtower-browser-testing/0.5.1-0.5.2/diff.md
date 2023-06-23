# Comparing `tmp/watchtower_browser_testing-0.5.1.tar.gz` & `tmp/watchtower_browser_testing-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.5.1.tar", last modified: Fri Jun 23 09:35:51 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.5.2.tar", last modified: Fri Jun 23 14:05:44 2023, max compression
```

## Comparing `watchtower_browser_testing-0.5.1.tar` & `watchtower_browser_testing-0.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 09:35:51.365560 watchtower_browser_testing-0.5.1/
--rw-rw-rw-   0        0        0      310 2023-06-23 09:35:51.365560 watchtower_browser_testing-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 09:35:51.365560 watchtower_browser_testing-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:35:51.358464 watchtower_browser_testing-0.5.1/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      241 2023-06-23 09:35:42.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      987 2023-06-13 13:37:35.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     3780 2023-06-23 09:08:00.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:35:51.365560 watchtower_browser_testing-0.5.1/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    18953 2023-06-13 13:52:56.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     9442 2023-06-23 09:08:00.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0      191 2023-05-20 15:42:04.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/utils.py
--rw-rw-rw-   0        0        0       21 2023-06-23 09:35:42.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:35:51.365560 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-06-23 09:35:51.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2023-06-23 09:35:51.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 09:35:51.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-23 09:35:51.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-06-23 09:35:51.000000 watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 14:05:44.195045 watchtower_browser_testing-0.5.2/
+-rw-rw-rw-   0        0        0      310 2023-06-23 14:05:44.195045 watchtower_browser_testing-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:05:44.195045 watchtower_browser_testing-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:05:44.180038 watchtower_browser_testing-0.5.2/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      241 2023-06-23 09:35:42.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      987 2023-06-13 13:37:35.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     4813 2023-06-23 14:01:53.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:05:44.195045 watchtower_browser_testing-0.5.2/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    18953 2023-06-13 13:52:56.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     9381 2023-06-23 13:59:03.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0      191 2023-05-20 15:42:04.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/utils.py
+-rw-rw-rw-   0        0        0       21 2023-06-23 14:05:31.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:05:44.195045 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-06-23 14:05:44.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2023-06-23 14:05:44.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 14:05:44.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-23 14:05:44.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-06-23 14:05:44.000000 watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.5.1/setup.py` & `watchtower_browser_testing-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.1/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.5.2/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.1/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.5.2/watchtower_browser_testing/helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import sys
 import json
 from marko.ext.gfm import gfm as markdown
 import collections
 from cerberus import Validator
 
+from watchtower_browser_testing import exceptions
+
 
 def trim(docstring):
     if not docstring:
         return ''
     # Convert tabs to spaces (following the normal Python rules)
     # and split into a list of lines:
     lines = docstring.expandtabs().splitlines()
@@ -106,33 +108,64 @@
     def errors(self):
         errors = super(WtValidator, self).errors
         if self.is_dict_list and self.rows_key in errors:
             return errors[self.rows_key]
         else:
             return errors
 
-class WtSelector(WtValidator):
+class CombinedSelector(object):
+
+    def __init__(self, selectors, operator='and'):
+
+        self.selectors = selectors
+        self.operator = operator
+
+    def __and__(self, other):
+
+        return CombinedSelector(selectors=[self, other], operator='and')
 
-    def select(self, *args, **kwargs):
+    def __or__(self, other):
+
+        return CombinedSelector(selectors=[self, other], operator='or')
+
+    def select(self, document):
+
+        if self.operator == 'and':
+            return all(s.select(document) for s in self.selectors)
+        elif self.operator == 'or':
+            return any(s.select(document) for s in self.selectors)
+        else:
+            raise exceptions.InvalidInputError(f'Unknown operator {self.operator}')
 
-        return super(WtSelector, self).validate(*args, **kwargs)
+class WtSelector(object):
 
-class ExactMatchSelector(object):
+
+    def __and__(self, other):
+        return CombinedSelector(selectors=[self, other], operator='and')
+
+    def __or__(self, other):
+        return CombinedSelector(selectors=[self, other], operator='or')
+
+class Selector(WtSelector, WtValidator):
+
+    def select(self, document):
+
+        return super(WtSelector, self).validate(document=document)
+
+class ExactMatchSelector(WtSelector):
 
     def __init__(self, value, inverse=False):
 
         self.value = value
         self.inverse = inverse
 
-    def select(self, doc):
+    def select(self, dcument):
 
         if self.inverse:
-            return not (doc is self.value)
+            return not (dcument is self.value)
 
-        return doc is self.value
+        return dcument is self.value
 
 class MissingSelector(ExactMatchSelector):
 
     def __init__(self, inverse=False):
-        super(ExactMatchSelector, self).__init__(value=None, inverse=inverse)
-
-
+        super(MissingSelector, self).__init__(value=None, inverse=inverse)
```

### Comparing `watchtower_browser_testing-0.5.1/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.5.2/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.1/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.5.2/watchtower_browser_testing/testsuite.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.5.1/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.5.2/watchtower_browser_testing/tracking_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 from http.cookies import SimpleCookie
 
 import playwright.sync_api
 
 from watchtower_browser_testing import config
 from watchtower_browser_testing import exceptions
 from watchtower_browser_testing.helpers import WtValidator as Validator
-from watchtower_browser_testing.helpers import WtSelector as Selector
-from watchtower_browser_testing.helpers import ExactMatchSelector, MissingSelector
+from watchtower_browser_testing.helpers import ExactMatchSelector, MissingSelector, Selector
 
 
 class ValidatorError(Exception): pass
 
 
 class RequestWrapper(object):
```

### Comparing `watchtower_browser_testing-0.5.1/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.5.2/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

