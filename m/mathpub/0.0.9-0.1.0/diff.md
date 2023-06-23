# Comparing `tmp/mathpub-0.0.9.tar.gz` & `tmp/mathpub-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathpub-0.0.9.tar", last modified: Fri Jun 23 18:46:45 2023, max compression
+gzip compressed data, was "mathpub-0.1.0.tar", last modified: Fri Jun 23 19:09:15 2023, max compression
```

## Comparing `mathpub-0.0.9.tar` & `mathpub-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 18:46:45.321788 mathpub-0.0.9/
--rw-rw-rw-   0        0        0      159 2023-06-23 18:46:45.321788 mathpub-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-23 18:46:45.300789 mathpub-0.0.9/mathpub/
--rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.0.9/mathpub/__init__.py
--rw-rw-rw-   0        0        0     1855 2023-06-23 18:22:11.000000 mathpub-0.0.9/mathpub/page.py
--rw-rw-rw-   0        0        0     3321 2023-06-23 18:29:55.000000 mathpub-0.0.9/mathpub/text_processing.py
--rw-rw-rw-   0        0        0     1590 2023-06-22 23:10:58.000000 mathpub-0.0.9/mathpub/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:46:45.319788 mathpub-0.0.9/mathpub.egg-info/
--rw-rw-rw-   0        0        0      159 2023-06-23 18:46:44.000000 mathpub-0.0.9/mathpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-23 18:46:44.000000 mathpub-0.0.9/mathpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 18:46:44.000000 mathpub-0.0.9/mathpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 18:44:47.000000 mathpub-0.0.9/mathpub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-06-23 18:46:44.000000 mathpub-0.0.9/mathpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 18:46:45.323785 mathpub-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-06-23 18:40:19.000000 mathpub-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:09:15.143206 mathpub-0.1.0/
+-rw-rw-rw-   0        0        0      178 2023-06-23 19:09:15.144205 mathpub-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-23 19:09:14.975986 mathpub-0.1.0/mathpub/
+-rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.1.0/mathpub/__init__.py
+-rw-rw-rw-   0        0        0     1630 2023-06-23 19:00:06.000000 mathpub-0.1.0/mathpub/page.py
+-rw-rw-rw-   0        0        0     3321 2023-06-23 18:29:55.000000 mathpub-0.1.0/mathpub/text_processing.py
+-rw-rw-rw-   0        0        0     1590 2023-06-22 23:10:58.000000 mathpub-0.1.0/mathpub/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:09:15.141206 mathpub-0.1.0/mathpub.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-23 19:09:14.000000 mathpub-0.1.0/mathpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-23 19:09:14.000000 mathpub-0.1.0/mathpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 19:09:14.000000 mathpub-0.1.0/mathpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-23 18:44:47.000000 mathpub-0.1.0/mathpub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-23 19:09:14.000000 mathpub-0.1.0/mathpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 19:09:15.145212 mathpub-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      283 2023-06-23 19:00:06.000000 mathpub-0.1.0/setup.py
```

### Comparing `mathpub-0.0.9/mathpub/text_processing.py` & `mathpub-0.1.0/mathpub/text_processing.py`

 * *Files identical despite different names*

### Comparing `mathpub-0.0.9/mathpub/utils.py` & `mathpub-0.1.0/mathpub/utils.py`

 * *Files identical despite different names*

