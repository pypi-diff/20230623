# Comparing `tmp/mathpub-0.0.1.tar.gz` & `tmp/mathpub-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathpub-0.0.1.tar", last modified: Thu Jun 22 22:26:52 2023, max compression
+gzip compressed data, was "mathpub-0.0.2.tar", last modified: Thu Jun 22 22:41:14 2023, max compression
```

## Comparing `mathpub-0.0.1.tar` & `mathpub-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 22:26:52.238025 mathpub-0.0.1/
--rw-rw-rw-   0        0        0      159 2023-06-22 22:26:52.238310 mathpub-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 22:26:52.195242 mathpub-0.0.1/mathpub/
--rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.0.1/mathpub/__init__.py
--rw-rw-rw-   0        0        0     2208 2023-06-22 22:26:30.000000 mathpub-0.0.1/mathpub/page.py
--rw-rw-rw-   0        0        0     1583 2023-06-22 22:12:54.000000 mathpub-0.0.1/mathpub/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 22:26:52.235167 mathpub-0.0.1/mathpub.egg-info/
--rw-rw-rw-   0        0        0      159 2023-06-22 22:26:51.000000 mathpub-0.0.1/mathpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-22 22:26:51.000000 mathpub-0.0.1/mathpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 22:26:51.000000 mathpub-0.0.1/mathpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 22:22:34.000000 mathpub-0.0.1/mathpub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-06-22 22:26:51.000000 mathpub-0.0.1/mathpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 22:26:52.240174 mathpub-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-06-22 22:26:46.000000 mathpub-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 22:41:14.366747 mathpub-0.0.2/
+-rw-rw-rw-   0        0        0      159 2023-06-22 22:41:14.366747 mathpub-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 22:41:14.357367 mathpub-0.0.2/mathpub/
+-rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.0.2/mathpub/__init__.py
+-rw-rw-rw-   0        0        0     2208 2023-06-22 22:26:30.000000 mathpub-0.0.2/mathpub/page.py
+-rw-rw-rw-   0        0        0     1579 2023-06-22 22:40:53.000000 mathpub-0.0.2/mathpub/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-22 22:41:14.365721 mathpub-0.0.2/mathpub.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-06-22 22:41:14.000000 mathpub-0.0.2/mathpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-22 22:41:14.000000 mathpub-0.0.2/mathpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 22:41:14.000000 mathpub-0.0.2/mathpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 22:22:34.000000 mathpub-0.0.2/mathpub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-22 22:41:14.000000 mathpub-0.0.2/mathpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 22:41:14.368743 mathpub-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-06-22 22:41:10.000000 mathpub-0.0.2/setup.py
```

### Comparing `mathpub-0.0.1/mathpub/page.py` & `mathpub-0.0.2/mathpub/page.py`

 * *Files identical despite different names*

### Comparing `mathpub-0.0.1/mathpub/utils.py` & `mathpub-0.0.2/mathpub/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 def upper_ind(ind):
     return f"^{b(ind)}"
 
 
 def lr(ins, left, right):
     """Wraps \\left and \\right (with delimiters left and right respectively) around ins """
-    return f"\\left{b(left)} {ins} \\right{b(right)}"
+    return f"\\left {left} {ins} \\right {right}"
 
 
 def sqrt(ins):
     return f"\\sqrt{b(ins)}"
 
 
 class _Abc:
```

