# Comparing `tmp/mathpub-0.0.6.tar.gz` & `tmp/mathpub-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathpub-0.0.6.tar", last modified: Thu Jun 22 23:28:40 2023, max compression
+gzip compressed data, was "dist\mathpub-0.0.7.tar", last modified: Fri Jun 23 07:15:01 2023, max compression
```

## Comparing `mathpub-0.0.6.tar` & `mathpub-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 23:28:40.463527 mathpub-0.0.6/
--rw-rw-rw-   0        0        0      159 2023-06-22 23:28:40.463527 mathpub-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 23:28:40.451535 mathpub-0.0.6/mathpub/
--rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.0.6/mathpub/__init__.py
--rw-rw-rw-   0        0        0     2185 2023-06-22 23:26:29.000000 mathpub-0.0.6/mathpub/page.py
--rw-rw-rw-   0        0        0     1590 2023-06-22 23:10:58.000000 mathpub-0.0.6/mathpub/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 23:28:40.461541 mathpub-0.0.6/mathpub.egg-info/
--rw-rw-rw-   0        0        0      159 2023-06-22 23:28:40.000000 mathpub-0.0.6/mathpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-22 23:28:40.000000 mathpub-0.0.6/mathpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 23:28:40.000000 mathpub-0.0.6/mathpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 22:55:31.000000 mathpub-0.0.6/mathpub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-06-22 23:28:40.000000 mathpub-0.0.6/mathpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 23:28:40.465509 mathpub-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-06-22 23:28:37.000000 mathpub-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:15:01.104780 mathpub-0.0.7/
+-rw-rw-rw-   0        0        0      255 2023-06-23 07:15:01.105782 mathpub-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-23 07:15:01.069770 mathpub-0.0.7/mathpub/
+-rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.0.7/mathpub/__init__.py
+-rw-rw-rw-   0        0        0     2560 2023-06-23 07:14:12.000000 mathpub-0.0.7/mathpub/page.py
+-rw-rw-rw-   0        0        0     1590 2023-06-22 23:10:58.000000 mathpub-0.0.7/mathpub/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:15:01.102780 mathpub-0.0.7/mathpub.egg-info/
+-rw-rw-rw-   0        0        0      255 2023-06-23 07:14:59.000000 mathpub-0.0.7/mathpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-23 07:14:59.000000 mathpub-0.0.7/mathpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 07:14:59.000000 mathpub-0.0.7/mathpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 22:55:31.000000 mathpub-0.0.7/mathpub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-23 07:14:59.000000 mathpub-0.0.7/mathpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 07:15:01.106779 mathpub-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-06-23 07:14:12.000000 mathpub-0.0.7/setup.py
```

### Comparing `mathpub-0.0.6/mathpub/page.py` & `mathpub-0.0.7/mathpub/page.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,25 @@
     def display(self):
         return self.DisplayPrinter(self)
 
     @property
     def markup(self):
         return ''.join(str(x) for x in self.lines)
 
+    class DebugPrinter:
+        def __init__(self, page):
+            self._page = page
+
+        def __repr__(self):
+            return self._page.markup
+
+    @property
+    def debug(self):
+        return self.DebugPrinter(self)
+
     def __init__(self):
         self.lines = []
         self._last_length = 0
 
     def _add_line(self, st: str):
         res = []
 
@@ -96,7 +107,12 @@
         return self
 
     def checkpoint(self):
         self._last_length = len(self.lines)
 
     def rollback(self):
         self.lines = self.lines[:self._last_length]
+
+    def latest(self):
+        new_page = Page()
+        new_page.lines = self.lines[self._last_length:]
+        return new_page
```

### Comparing `mathpub-0.0.6/mathpub/utils.py` & `mathpub-0.0.7/mathpub/utils.py`

 * *Files identical despite different names*

