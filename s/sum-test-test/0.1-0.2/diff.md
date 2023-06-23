# Comparing `tmp/sum_test_test-0.1.tar.gz` & `tmp/sum_test_test-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sum_test_test-0.1.tar", last modified: Fri Jun 23 15:18:38 2023, max compression
+gzip compressed data, was "sum_test_test-0.2.tar", last modified: Fri Jun 23 15:28:46 2023, max compression
```

## Comparing `sum_test_test-0.1.tar` & `sum_test_test-0.2.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 mohamedfadl   (501) staff       (20)        0 2023-06-23 15:18:38.839579 sum_test_test-0.1/
--rw-r--r--   0 mohamedfadl   (501) staff       (20)      166 2023-06-23 15:18:38.839438 sum_test_test-0.1/PKG-INFO
--rw-r--r--   0 mohamedfadl   (501) staff       (20)       14 2023-06-23 14:29:10.000000 sum_test_test-0.1/README.md
--rw-r--r--   0 mohamedfadl   (501) staff       (20)       38 2023-06-23 15:18:38.839620 sum_test_test-0.1/setup.cfg
--rw-r--r--   0 mohamedfadl   (501) staff       (20)      236 2023-06-23 15:16:44.000000 sum_test_test-0.1/setup.py
-drwxr-xr-x   0 mohamedfadl   (501) staff       (20)        0 2023-06-23 15:18:38.839248 sum_test_test-0.1/sum_test_test.egg-info/
--rw-r--r--   0 mohamedfadl   (501) staff       (20)      166 2023-06-23 15:18:38.000000 sum_test_test-0.1/sum_test_test.egg-info/PKG-INFO
--rw-r--r--   0 mohamedfadl   (501) staff       (20)      166 2023-06-23 15:18:38.000000 sum_test_test-0.1/sum_test_test.egg-info/SOURCES.txt
--rw-r--r--   0 mohamedfadl   (501) staff       (20)        1 2023-06-23 15:18:38.000000 sum_test_test-0.1/sum_test_test.egg-info/dependency_links.txt
--rw-r--r--   0 mohamedfadl   (501) staff       (20)        4 2023-06-23 15:18:38.000000 sum_test_test-0.1/sum_test_test.egg-info/top_level.txt
+drwxr-xr-x   0 mohamedfadl   (501) staff       (20)        0 2023-06-23 15:28:46.115182 sum_test_test-0.2/
+-rw-r--r--   0 mohamedfadl   (501) staff       (20)      166 2023-06-23 15:28:46.115015 sum_test_test-0.2/PKG-INFO
+-rw-r--r--   0 mohamedfadl   (501) staff       (20)       14 2023-06-23 14:29:10.000000 sum_test_test-0.2/README.md
+-rw-r--r--   0 mohamedfadl   (501) staff       (20)       38 2023-06-23 15:28:46.115235 sum_test_test-0.2/setup.cfg
+-rw-r--r--   0 mohamedfadl   (501) staff       (20)      234 2023-06-23 15:28:43.000000 sum_test_test-0.2/setup.py
+drwxr-xr-x   0 mohamedfadl   (501) staff       (20)        0 2023-06-23 15:28:46.113941 sum_test_test-0.2/sum/
+-rw-r--r--   0 mohamedfadl   (501) staff       (20)        0 2023-06-23 14:57:37.000000 sum_test_test-0.2/sum/__init__.py
+-rw-r--r--   0 mohamedfadl   (501) staff       (20)      230 2023-06-23 14:57:37.000000 sum_test_test-0.2/sum/summing.py
+drwxr-xr-x   0 mohamedfadl   (501) staff       (20)        0 2023-06-23 15:28:46.114751 sum_test_test-0.2/sum_test_test.egg-info/
+-rw-r--r--   0 mohamedfadl   (501) staff       (20)      166 2023-06-23 15:28:46.000000 sum_test_test-0.2/sum_test_test.egg-info/PKG-INFO
+-rw-r--r--   0 mohamedfadl   (501) staff       (20)      197 2023-06-23 15:28:46.000000 sum_test_test-0.2/sum_test_test.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamedfadl   (501) staff       (20)        1 2023-06-23 15:28:46.000000 sum_test_test-0.2/sum_test_test.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamedfadl   (501) staff       (20)        4 2023-06-23 15:28:46.000000 sum_test_test-0.2/sum_test_test.egg-info/top_level.txt
```

