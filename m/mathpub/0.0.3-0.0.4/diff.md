# Comparing `tmp/mathpub-0.0.3.tar.gz` & `tmp/mathpub-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathpub-0.0.3.tar", last modified: Thu Jun 22 22:55:31 2023, max compression
+gzip compressed data, was "mathpub-0.0.4.tar", last modified: Thu Jun 22 23:00:27 2023, max compression
```

## Comparing `mathpub-0.0.3.tar` & `mathpub-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 22:55:31.911649 mathpub-0.0.3/
--rw-rw-rw-   0        0        0      159 2023-06-22 22:55:31.912646 mathpub-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 22:55:31.901647 mathpub-0.0.3/mathpub/
--rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.0.3/mathpub/__init__.py
--rw-rw-rw-   0        0        0     2242 2023-06-22 22:51:39.000000 mathpub-0.0.3/mathpub/page.py
--rw-rw-rw-   0        0        0     1579 2023-06-22 22:40:53.000000 mathpub-0.0.3/mathpub/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 22:55:31.910645 mathpub-0.0.3/mathpub.egg-info/
--rw-rw-rw-   0        0        0      159 2023-06-22 22:55:31.000000 mathpub-0.0.3/mathpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-22 22:55:31.000000 mathpub-0.0.3/mathpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 22:55:31.000000 mathpub-0.0.3/mathpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 22:55:31.000000 mathpub-0.0.3/mathpub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-06-22 22:55:31.000000 mathpub-0.0.3/mathpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 22:55:31.913648 mathpub-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-06-22 22:52:18.000000 mathpub-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:00:27.643624 mathpub-0.0.4/
+-rw-rw-rw-   0        0        0      159 2023-06-22 23:00:27.643624 mathpub-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 23:00:27.631622 mathpub-0.0.4/mathpub/
+-rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.0.4/mathpub/__init__.py
+-rw-rw-rw-   0        0        0     2000 2023-06-22 23:00:24.000000 mathpub-0.0.4/mathpub/page.py
+-rw-rw-rw-   0        0        0     1579 2023-06-22 22:40:53.000000 mathpub-0.0.4/mathpub/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:00:27.642629 mathpub-0.0.4/mathpub.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-06-22 23:00:27.000000 mathpub-0.0.4/mathpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-22 23:00:27.000000 mathpub-0.0.4/mathpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 23:00:27.000000 mathpub-0.0.4/mathpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 22:55:31.000000 mathpub-0.0.4/mathpub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-22 23:00:27.000000 mathpub-0.0.4/mathpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 23:00:27.645619 mathpub-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-06-22 23:00:24.000000 mathpub-0.0.4/setup.py
```

### Comparing `mathpub-0.0.3/mathpub/page.py` & `mathpub-0.0.4/mathpub/page.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,31 +43,21 @@
             self._page = page
 
         def _repr_latex_(self):
             return ''.join(x.latex() for x in self._page.lines)
 
         __str__ = _repr_latex_
 
-    class MarkupPrinter:
-        def __init__(self, page):
-            self._page = page
-
-        def __str__(self):
-            return ''.join(str(x) for x in self._page.lines)
-
-        def __repr__(self):
-            return repr(str(self))
-
     @property
     def display(self):
         return self.DisplayPrinter(self)
 
     @property
     def markup(self):
-        return self.MarkupPrinter(self)
+        return ''.join(str(x) for x in self.lines)
 
     def __init__(self):
         self.lines = []
 
     def _add_line(self, st: str):
         res = []
```

### Comparing `mathpub-0.0.3/mathpub/utils.py` & `mathpub-0.0.4/mathpub/utils.py`

 * *Files identical despite different names*

