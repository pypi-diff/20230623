# Comparing `tmp/mathpub-0.0.0.tar.gz` & `tmp/mathpub-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathpub-0.0.0.tar", last modified: Thu Jun 22 22:22:35 2023, max compression
+gzip compressed data, was "mathpub-0.0.1.tar", last modified: Thu Jun 22 22:26:52 2023, max compression
```

## Comparing `mathpub-0.0.0.tar` & `mathpub-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 22:22:34.976184 mathpub-0.0.0/
--rw-rw-rw-   0        0        0      159 2023-06-22 22:22:34.976184 mathpub-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 22:22:34.963194 mathpub-0.0.0/mathpub/
--rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.0.0/mathpub/__init__.py
--rw-rw-rw-   0        0        0     2208 2023-06-22 22:15:21.000000 mathpub-0.0.0/mathpub/page.py
--rw-rw-rw-   0        0        0     1583 2023-06-22 22:12:54.000000 mathpub-0.0.0/mathpub/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 22:22:34.974187 mathpub-0.0.0/mathpub.egg-info/
--rw-rw-rw-   0        0        0      159 2023-06-22 22:22:34.000000 mathpub-0.0.0/mathpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-22 22:22:34.000000 mathpub-0.0.0/mathpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 22:22:34.000000 mathpub-0.0.0/mathpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 22:22:34.000000 mathpub-0.0.0/mathpub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-06-22 22:22:34.000000 mathpub-0.0.0/mathpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 22:22:34.978184 mathpub-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      232 2023-06-22 22:21:03.000000 mathpub-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 22:26:52.238025 mathpub-0.0.1/
+-rw-rw-rw-   0        0        0      159 2023-06-22 22:26:52.238310 mathpub-0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 22:26:52.195242 mathpub-0.0.1/mathpub/
+-rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.0.1/mathpub/__init__.py
+-rw-rw-rw-   0        0        0     2208 2023-06-22 22:26:30.000000 mathpub-0.0.1/mathpub/page.py
+-rw-rw-rw-   0        0        0     1583 2023-06-22 22:12:54.000000 mathpub-0.0.1/mathpub/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-22 22:26:52.235167 mathpub-0.0.1/mathpub.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-06-22 22:26:51.000000 mathpub-0.0.1/mathpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-22 22:26:51.000000 mathpub-0.0.1/mathpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 22:26:51.000000 mathpub-0.0.1/mathpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 22:22:34.000000 mathpub-0.0.1/mathpub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-22 22:26:51.000000 mathpub-0.0.1/mathpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 22:26:52.240174 mathpub-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-06-22 22:26:46.000000 mathpub-0.0.1/setup.py
```

### Comparing `mathpub-0.0.0/mathpub/page.py` & `mathpub-0.0.1/mathpub/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 class Page:
     class DisplayPrinter:
         def __init__(self, page):
             self._page = page
 
-        def _latex_repr_(self):
+        def _repr_latex_(self):
             return ''.join(x.latex() for x in self._page.lines)
 
     class MarkupPrinter:
         def __init__(self, page):
             self._page = page
 
         def __str__(self):
```

### Comparing `mathpub-0.0.0/mathpub/utils.py` & `mathpub-0.0.1/mathpub/utils.py`

 * *Files identical despite different names*

