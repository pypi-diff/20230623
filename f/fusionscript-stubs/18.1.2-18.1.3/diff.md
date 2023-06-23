# Comparing `tmp/fusionscript-stubs-18.1.2.tar.gz` & `tmp/fusionscript-stubs-18.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Workspace\DaVinci\Fusionscript\dist\.tmp-c2fge47p\fusionscript-stubs-18.1.2.tar", last modified: Fri Jun 23 08:53:46 2023, max compression
+gzip compressed data, was "fusionscript-stubs-18.1.3.tar", last modified: Fri Jun 23 15:06:28 2023, max compression
```

## Comparing `fusionscript-stubs-18.1.2.tar` & `fusionscript-stubs-18.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 08:53:46.000000 fusionscript-stubs-18.1.2/
--rw-rw-rw-   0        0        0     1079 2023-06-18 12:26:33.000000 fusionscript-stubs-18.1.2/LICENSE.md
--rw-rw-rw-   0        0        0      212 2023-06-23 08:53:46.000000 fusionscript-stubs-18.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1170 2023-06-20 07:23:38.000000 fusionscript-stubs-18.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 08:53:46.000000 fusionscript-stubs-18.1.2/fusionscript-stubs/
--rw-rw-rw-   0        0        0     5259 2023-06-23 08:48:38.000000 fusionscript-stubs-18.1.2/fusionscript-stubs/__init__.pyi
--rw-rw-rw-   0        0        0    77962 2023-06-21 17:29:31.000000 fusionscript-stubs-18.1.2/fusionscript-stubs/fusionscript.pyi
-drwxrwxrwx   0        0        0        0 2023-06-23 08:53:46.000000 fusionscript-stubs-18.1.2/fusionscript_stubs.egg-info/
--rw-rw-rw-   0        0        0      212 2023-06-23 08:53:46.000000 fusionscript-stubs-18.1.2/fusionscript_stubs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-06-23 08:53:46.000000 fusionscript-stubs-18.1.2/fusionscript_stubs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 08:53:46.000000 fusionscript-stubs-18.1.2/fusionscript_stubs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-23 08:53:46.000000 fusionscript-stubs-18.1.2/fusionscript_stubs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 08:53:46.000000 fusionscript-stubs-18.1.2/setup.cfg
--rw-rw-rw-   0        0        0      353 2023-06-23 08:52:58.000000 fusionscript-stubs-18.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 15:06:28.784717 fusionscript-stubs-18.1.3/
+-rw-rw-rw-   0        0        0     1079 2023-06-18 12:26:33.000000 fusionscript-stubs-18.1.3/LICENSE.md
+-rw-rw-rw-   0        0        0     1468 2023-06-23 15:06:28.782716 fusionscript-stubs-18.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1170 2023-06-20 07:23:38.000000 fusionscript-stubs-18.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 15:06:28.763716 fusionscript-stubs-18.1.3/fusionscript-stubs/
+-rw-rw-rw-   0        0        0     5259 2023-06-23 08:48:38.000000 fusionscript-stubs-18.1.3/fusionscript-stubs/__init__.pyi
+-rw-rw-rw-   0        0        0    77962 2023-06-21 17:29:31.000000 fusionscript-stubs-18.1.3/fusionscript-stubs/fusionscript.pyi
+drwxrwxrwx   0        0        0        0 2023-06-23 15:06:28.777717 fusionscript-stubs-18.1.3/fusionscript_stubs.egg-info/
+-rw-rw-rw-   0        0        0     1468 2023-06-23 15:06:28.000000 fusionscript-stubs-18.1.3/fusionscript_stubs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-23 15:06:28.000000 fusionscript-stubs-18.1.3/fusionscript_stubs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 15:06:28.000000 fusionscript-stubs-18.1.3/fusionscript_stubs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-23 15:06:28.000000 fusionscript-stubs-18.1.3/fusionscript_stubs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 15:06:28.784717 fusionscript-stubs-18.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-06-23 15:05:31.000000 fusionscript-stubs-18.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fusionscript-stubs-18.1.2/LICENSE.md` & `fusionscript-stubs-18.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fusionscript-stubs-18.1.2/README.md` & `fusionscript-stubs-18.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fusionscript-stubs-18.1.2/fusionscript-stubs/__init__.pyi` & `fusionscript-stubs-18.1.3/fusionscript-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `fusionscript-stubs-18.1.2/fusionscript-stubs/fusionscript.pyi` & `fusionscript-stubs-18.1.3/fusionscript-stubs/fusionscript.pyi`

 * *Files identical despite different names*

