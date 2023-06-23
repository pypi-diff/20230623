# Comparing `tmp/screen_cls-1.0.4.tar.gz` & `tmp/screen_cls-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screen_cls-1.0.4.tar", last modified: Thu Jun 22 19:37:19 2023, max compression
+gzip compressed data, was "screen_cls-1.0.5.tar", last modified: Fri Jun 23 06:27:37 2023, max compression
```

## Comparing `screen_cls-1.0.4.tar` & `screen_cls-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 19:37:19.441943 screen_cls-1.0.4/
--rw-rw-rw-   0        0        0     1101 2023-06-22 11:49:23.000000 screen_cls-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      914 2023-06-22 19:37:19.442943 screen_cls-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-06-22 19:22:26.000000 screen_cls-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 19:37:19.400946 screen_cls-1.0.4/screen_cls/
--rw-rw-rw-   0        0        0        0 2023-06-22 12:24:08.000000 screen_cls-1.0.4/screen_cls/_init_.py
--rw-rw-rw-   0        0        0       99 2023-06-22 12:51:35.000000 screen_cls-1.0.4/screen_cls/example.py
--rw-rw-rw-   0        0        0      147 2023-06-22 19:37:05.000000 screen_cls-1.0.4/screen_cls/main.py
-drwxrwxrwx   0        0        0        0 2023-06-22 19:37:19.437946 screen_cls-1.0.4/screen_cls.egg-info/
--rw-rw-rw-   0        0        0      914 2023-06-22 19:37:19.000000 screen_cls-1.0.4/screen_cls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-06-22 19:37:19.000000 screen_cls-1.0.4/screen_cls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 19:37:19.000000 screen_cls-1.0.4/screen_cls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 19:37:19.000000 screen_cls-1.0.4/screen_cls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 19:37:19.445945 screen_cls-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      787 2023-06-22 19:37:14.000000 screen_cls-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 06:27:37.553499 screen_cls-1.0.5/
+-rw-rw-rw-   0        0        0     1100 2023-06-23 06:27:04.000000 screen_cls-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      914 2023-06-23 06:27:37.553499 screen_cls-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-06-22 19:22:26.000000 screen_cls-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 06:27:37.508501 screen_cls-1.0.5/screen_cls/
+-rw-rw-rw-   0        0        0       52 2023-06-23 06:03:20.000000 screen_cls-1.0.5/screen_cls/__init__.py
+-rw-rw-rw-   0        0        0      194 2023-06-23 06:00:52.000000 screen_cls-1.0.5/screen_cls/main.py
+drwxrwxrwx   0        0        0        0 2023-06-23 06:27:37.551500 screen_cls-1.0.5/screen_cls.egg-info/
+-rw-rw-rw-   0        0        0      914 2023-06-23 06:27:37.000000 screen_cls-1.0.5/screen_cls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-06-23 06:27:37.000000 screen_cls-1.0.5/screen_cls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 06:27:37.000000 screen_cls-1.0.5/screen_cls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 06:27:37.000000 screen_cls-1.0.5/screen_cls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 06:27:37.566504 screen_cls-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-06-23 06:27:00.000000 screen_cls-1.0.5/setup.py
```

### Comparing `screen_cls-1.0.4/LICENSE` & `screen_cls-1.0.5/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MIT License 
+MIT License
 
 Copyright (c) 2023 Igor V. Chaban (IgorMan)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `screen_cls-1.0.4/PKG-INFO` & `screen_cls-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen_cls
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python script for clearing screen for any OS's: Windows, MAC, Linux
 Home-page: https://github.com/IgorMan2005/screen_cls
 Author: IgorMan (IgorMan2005)
 Author-email: igorman2005@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://best-itpro.ru/news/screen_cls/
 Keywords: python screen cls
```

### Comparing `screen_cls-1.0.4/screen_cls.egg-info/PKG-INFO` & `screen_cls-1.0.5/screen_cls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screen-cls
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python script for clearing screen for any OS's: Windows, MAC, Linux
 Home-page: https://github.com/IgorMan2005/screen_cls
 Author: IgorMan (IgorMan2005)
 Author-email: igorman2005@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://best-itpro.ru/news/screen_cls/
 Keywords: python screen cls
```

### Comparing `screen_cls-1.0.4/setup.py` & `screen_cls-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='screen_cls',
-  version='1.0.4',
+  version='1.0.5',
   author='IgorMan (IgorMan2005)',
   author_email='igorman2005@gmail.com',
   description='Python script for clearing screen for any OS\'s: Windows, MAC, Linux',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/IgorMan2005/screen_cls',
   packages=['screen_cls'],
```

