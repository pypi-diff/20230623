# Comparing `tmp/SmithWagnerCV-0.0.5.tar.gz` & `tmp/smithwagnercv-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmithWagnerCV-0.0.5.tar", last modified: Thu Nov 17 13:30:23 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `SmithWagnerCV-0.0.5.tar` & `smithwagnercv-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,11 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-11-17 13:30:23.411013 SmithWagnerCV-0.0.5/
--rw-r--r--   0 ben        (501) staff       (20)     1066 2019-12-06 17:49:09.000000 SmithWagnerCV-0.0.5/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)      807 2022-11-17 13:30:23.411145 SmithWagnerCV-0.0.5/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      963 2022-06-26 10:41:03.000000 SmithWagnerCV-0.0.5/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-11-17 13:30:23.408606 SmithWagnerCV-0.0.5/SmithWagnerCV/
--rw-r--r--   0 ben        (501) staff       (20)     6581 2022-11-17 12:54:50.000000 SmithWagnerCV-0.0.5/SmithWagnerCV/Methods.py
--rw-r--r--   0 ben        (501) staff       (20)       96 2022-11-17 13:02:32.000000 SmithWagnerCV-0.0.5/SmithWagnerCV/__init__.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2022-11-17 13:30:23.410750 SmithWagnerCV-0.0.5/SmithWagnerCV.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)      807 2022-11-17 13:30:23.000000 SmithWagnerCV-0.0.5/SmithWagnerCV.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      271 2022-11-17 13:30:23.000000 SmithWagnerCV-0.0.5/SmithWagnerCV.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2022-11-17 13:30:23.000000 SmithWagnerCV-0.0.5/SmithWagnerCV.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       18 2022-11-17 13:30:23.000000 SmithWagnerCV-0.0.5/SmithWagnerCV.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)       14 2022-11-17 13:30:23.000000 SmithWagnerCV-0.0.5/SmithWagnerCV.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       79 2022-11-17 13:30:23.411551 SmithWagnerCV-0.0.5/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)      982 2022-11-17 13:02:24.000000 SmithWagnerCV-0.0.5/setup.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/src/SmithWagnerCV/.DS_Store
+-rw-r--r--   0        0        0     6582 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/src/SmithWagnerCV/Methods.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/src/SmithWagnerCV/__init__.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/LICENSE
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/README.md
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 smithwagnercv-0.0.6/PKG-INFO
```

### Comparing `SmithWagnerCV-0.0.5/LICENSE` & `smithwagnercv-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SmithWagnerCV-0.0.5/README.md` & `smithwagnercv-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `SmithWagnerCV-0.0.5/SmithWagnerCV/Methods.py` & `smithwagnercv-0.0.6/src/SmithWagnerCV/Methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     muList : list
         List of mu values
     numoptions : int
         Number of options on the exam. Defaults to four.
     criticalValues : list
         List of critical values to extract from the learning distributions.  Defaults to [0.90,0.95].
     confInterval: : list
-        List of values to extact from the mu distribution.  Defaults to [0.025, 0.975].
+        List of values to extract from the mu distribution.  Defaults to [0.025, 0.975].
     R : int
         Number of iterations for each simulation.  Defaults to 10,000.
             
     Returns
     -------
         None
             Saves four CSV files.
```

