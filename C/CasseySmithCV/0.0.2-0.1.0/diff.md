# Comparing `tmp/CasseySmithCV-0.0.2.tar.gz` & `tmp/casseysmithcv-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CasseySmithCV-0.0.2.tar", last modified: Thu Nov 17 13:44:42 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `CasseySmithCV-0.0.2.tar` & `casseysmithcv-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,9 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-11-17 13:44:42.796321 CasseySmithCV-0.0.2/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-11-17 13:44:42.794424 CasseySmithCV-0.0.2/CasseySmithCV/
--rw-r--r--   0 ben        (501) staff       (20)     1384 2019-12-13 18:25:27.000000 CasseySmithCV-0.0.2/CasseySmithCV/ReadFiles.py
--rw-r--r--   0 ben        (501) staff       (20)     4778 2022-11-17 13:38:03.000000 CasseySmithCV-0.0.2/CasseySmithCV/Simulation.py
--rw-r--r--   0 ben        (501) staff       (20)      141 2022-11-17 13:38:53.000000 CasseySmithCV-0.0.2/CasseySmithCV/__init__.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-11-17 13:44:42.795915 CasseySmithCV-0.0.2/CasseySmithCV.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)      848 2022-11-17 13:44:42.000000 CasseySmithCV-0.0.2/CasseySmithCV.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      301 2022-11-17 13:44:42.000000 CasseySmithCV-0.0.2/CasseySmithCV.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2022-11-17 13:44:42.000000 CasseySmithCV-0.0.2/CasseySmithCV.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       18 2022-11-17 13:44:42.000000 CasseySmithCV-0.0.2/CasseySmithCV.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       14 2022-11-17 13:44:42.000000 CasseySmithCV-0.0.2/CasseySmithCV.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)     1066 2019-12-13 11:59:50.000000 CasseySmithCV-0.0.2/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)      848 2022-11-17 13:44:42.796513 CasseySmithCV-0.0.2/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     1134 2019-12-14 13:08:26.000000 CasseySmithCV-0.0.2/README.md
--rw-r--r--   0 ben        (501) staff       (20)       79 2022-11-17 13:44:42.797129 CasseySmithCV-0.0.2/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)     1023 2022-11-17 13:40:25.000000 CasseySmithCV-0.0.2/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 casseysmithcv-0.1.0/.gitattributes
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 casseysmithcv-0.1.0/src/CasseySmithCV/ReadFiles.py
+-rw-r--r--   0        0        0     4778 2020-02-02 00:00:00.000000 casseysmithcv-0.1.0/src/CasseySmithCV/Simulation.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 casseysmithcv-0.1.0/src/CasseySmithCV/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 casseysmithcv-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 casseysmithcv-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 casseysmithcv-0.1.0/README.md
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 casseysmithcv-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 casseysmithcv-0.1.0/PKG-INFO
```

### Comparing `CasseySmithCV-0.0.2/CasseySmithCV/ReadFiles.py` & `casseysmithcv-0.1.0/src/CasseySmithCV/ReadFiles.py`

 * *Files identical despite different names*

### Comparing `CasseySmithCV-0.0.2/CasseySmithCV/Simulation.py` & `casseysmithcv-0.1.0/src/CasseySmithCV/Simulation.py`

 * *Files identical despite different names*

### Comparing `CasseySmithCV-0.0.2/LICENSE` & `casseysmithcv-0.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Ben Smith
+Copyright (c) 2023 Ben Smith
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `CasseySmithCV-0.0.2/README.md` & `casseysmithcv-0.1.0/README.md`

 * *Files identical despite different names*

