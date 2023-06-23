# Comparing `tmp/biblioteca2080-1.0.1.tar.gz` & `tmp/biblioteca2080-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblioteca2080-1.0.1.tar", last modified: Thu Jun 22 06:27:53 2023, max compression
+gzip compressed data, was "biblioteca2080-1.0.2.tar", last modified: Fri Jun 23 19:05:33 2023, max compression
```

## Comparing `biblioteca2080-1.0.1.tar` & `biblioteca2080-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 06:27:53.104618 biblioteca2080-1.0.1/
--rw-rw-rw-   0        0        0      199 2023-06-22 06:27:53.104618 biblioteca2080-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-22 06:27:53.104618 biblioteca2080-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      422 2023-06-22 06:21:08.000000 biblioteca2080-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 06:27:53.088998 biblioteca2080-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 06:27:53.104618 biblioteca2080-1.0.1/src/biblioteca2080.egg-info/
--rw-rw-rw-   0        0        0      199 2023-06-22 06:27:52.000000 biblioteca2080-1.0.1/src/biblioteca2080.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-22 06:27:52.000000 biblioteca2080-1.0.1/src/biblioteca2080.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 06:27:52.000000 biblioteca2080-1.0.1/src/biblioteca2080.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-22 06:27:52.000000 biblioteca2080-1.0.1/src/biblioteca2080.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 19:05:33.899096 biblioteca2080-1.0.2/
+-rw-rw-rw-   0        0        0      199 2023-06-23 19:05:33.883470 biblioteca2080-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-23 19:05:33.899096 biblioteca2080-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      511 2023-06-23 18:58:13.000000 biblioteca2080-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:05:33.852235 biblioteca2080-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 19:05:33.883470 biblioteca2080-1.0.2/src/biblioteca2080.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-06-23 19:05:33.000000 biblioteca2080-1.0.2/src/biblioteca2080.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-23 19:05:33.000000 biblioteca2080-1.0.2/src/biblioteca2080.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 19:05:33.000000 biblioteca2080-1.0.2/src/biblioteca2080.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 19:05:33.000000 biblioteca2080-1.0.2/src/biblioteca2080.egg-info/top_level.txt
```

