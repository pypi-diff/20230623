# Comparing `tmp/etm-dgraham-5.1.6.tar.gz` & `tmp/etm-dgraham-5.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.1.6.tar", last modified: Wed Jun 21 18:34:01 2023, max compression
+gzip compressed data, was "etm-dgraham-5.1.7.tar", last modified: Fri Jun 23 00:25:30 2023, max compression
```

## Comparing `etm-dgraham-5.1.6.tar` & `etm-dgraham-5.1.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 18:34:01.802148 etm-dgraham-5.1.6/
--rw-r--r--   0 dag        (501) staff       (20)     2480 2023-06-21 18:33:47.000000 etm-dgraham-5.1.6/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.6/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   132192 2023-06-21 18:34:01.801995 etm-dgraham-5.1.6/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   131280 2023-06-21 13:13:42.000000 etm-dgraham-5.1.6/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.6/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.6/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 18:34:01.794608 etm-dgraham-5.1.6/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.6/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.6/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.6/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 18:34:01.797877 etm-dgraham-5.1.6/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.6/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.6/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-21 18:33:47.000000 etm-dgraham-5.1.6/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.6/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.6/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.6/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   286973 2023-06-21 18:33:47.000000 etm-dgraham-5.1.6/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.6/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.6/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   100663 2023-06-21 18:33:47.000000 etm-dgraham-5.1.6/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 18:34:01.800187 etm-dgraham-5.1.6/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   132192 2023-06-21 18:34:01.000000 etm-dgraham-5.1.6/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.6/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.6/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-21 18:34:01.000000 etm-dgraham-5.1.6/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-21 18:34:01.000000 etm-dgraham-5.1.6/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-21 18:34:01.000000 etm-dgraham-5.1.6/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.6/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-21 18:34:01.000000 etm-dgraham-5.1.6/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.6/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-21 18:34:01.000000 etm-dgraham-5.1.6/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.6/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.6/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.6/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.6/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.6/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.6/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-21 18:34:01.802183 etm-dgraham-5.1.6/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.6/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 18:34:01.800286 etm-dgraham-5.1.6/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.6/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-21 18:34:01.801508 etm-dgraham-5.1.6/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.6/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.6/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.6/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.6/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.105715 etm-dgraham-5.1.7/
+-rw-r--r--   0 dag        (501) staff       (20)     2411 2023-06-23 00:25:16.000000 etm-dgraham-5.1.7/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.1.7/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   132192 2023-06-23 00:25:30.105573 etm-dgraham-5.1.7/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   131280 2023-06-21 13:13:42.000000 etm-dgraham-5.1.7/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.1.7/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.1.7/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.097038 etm-dgraham-5.1.7/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.1.7/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.1.7/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.1.7/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.101449 etm-dgraham-5.1.7/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.1.7/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.1.7/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-23 00:25:16.000000 etm-dgraham-5.1.7/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.1.7/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.1.7/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.1.7/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   287838 2023-06-23 00:25:16.000000 etm-dgraham-5.1.7/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37916 2023-06-18 11:28:27.000000 etm-dgraham-5.1.7/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.1.7/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   100599 2023-06-23 00:25:16.000000 etm-dgraham-5.1.7/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.103942 etm-dgraham-5.1.7/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   132192 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-23 00:25:30.000000 etm-dgraham-5.1.7/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.1.7/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.1.7/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.1.7/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.1.7/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.1.7/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.1.7/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-23 00:25:30.105751 etm-dgraham-5.1.7/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.1.7/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.104038 etm-dgraham-5.1.7/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.1.7/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-23 00:25:30.105106 etm-dgraham-5.1.7/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.1.7/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.1.7/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.1.7/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.1.7/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.1.6/CHANGES.txt` & `etm-dgraham-5.1.7/CHANGES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,82 @@
-Recent tagged changes as of 2023-06-21T14:33:46.525074-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.1.6) Daniel Graham
+Recent tagged changes as of 2023-06-22T20:25:12.409983-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.1.7) Daniel Graham
+    fe31c71 2023-06-22 20:25:12 -0400
+    Tagged version 5.1.7.
+
+- 30 hours ago (tag: 5.1.6) Daniel Graham
     9c70c17 2023-06-21 14:33:46 -0400
     Tagged version 5.1.6.
 
-- 5 hours ago (tag: 5.1.5) Daniel Graham
+- 35 hours ago (tag: 5.1.5) Daniel Graham
     17d91e2 2023-06-21 09:13:39 -0400
     Tagged version 5.1.5.
 
-- 2 days ago (tag: 5.1.4) Daniel Graham
+- 3 days ago (tag: 5.1.4) Daniel Graham
     84421ec 2023-06-19 13:40:16 -0400
     Tagged version 5.1.4.
 
-- 2 days ago (tag: 5.1.3) Daniel Graham
+- 3 days ago (tag: 5.1.3) Daniel Graham
     c776097 2023-06-19 11:40:16 -0400
     Tagged version 5.1.3.
 
-- 2 days ago (tag: 5.1.2) Daniel Graham
+- 4 days ago (tag: 5.1.2) Daniel Graham
     3483b69 2023-06-19 05:51:42 -0400
     Tagged version 5.1.2.
 
-- 3 days ago (tag: 5.1.1) Daniel Graham
+- 5 days ago (tag: 5.1.1) Daniel Graham
     d0c733f 2023-06-18 08:29:16 -0400
     Tagged version 5.1.1.
 
-- 3 days ago (tag: 5.1.0) Daniel Graham
+- 5 days ago (tag: 5.1.0) Daniel Graham
     ece86e8 2023-06-18 07:28:25 -0400
     Tagged version 5.1.0. Added ability to display completion history
     for tasks including skipped instead of finished instances.
 
-- 4 days ago (tag: 5.0.12) Daniel Graham
+- 5 days ago (tag: 5.0.12) Daniel Graham
     c42576c 2023-06-17 08:57:03 -0400
     Tagged version 5.0.12.
 
-- 4 days ago (tag: 5.0.11) Daniel Graham
+- 6 days ago (tag: 5.0.11) Daniel Graham
     e9228d2 2023-06-17 05:19:31 -0400
     Tagged version 5.0.11.
 
-- 4 days ago (tag: 5.0.10) Daniel Graham
+- 6 days ago (tag: 5.0.10) Daniel Graham
     2e1f579 2023-06-17 05:05:32 -0400
     Tagged version 5.0.10.
 
-- 6 days ago (tag: 5.0.9) Daniel Graham
+- 7 days ago (tag: 5.0.9) Daniel Graham
     7f30e8b 2023-06-15 10:14:19 -0400
     Tagged version 5.0.9.
 
-- 8 days ago (tag: 5.0.8) Daniel Graham
+- 9 days ago (tag: 5.0.8) Daniel Graham
     1f587d1 2023-06-13 20:17:48 -0400
     Tagged version 5.0.8. Only display and allow completion of jthe
     jobs of the oldest unfinished instance of a repeating task.
 
-- 13 days ago (tag: 5.0.7) Daniel Graham
+- 2 weeks ago (tag: 5.0.7) Daniel Graham
     b9eccc6 2023-06-08 08:38:27 -0400
     Tagged version 5.0.7.
 
 - 2 weeks ago (tag: 5.0.6) Daniel Graham
     345ca4e 2023-06-05 12:41:31 -0400
     Tagged version 5.0.6.
 
-- 2 weeks ago (tag: 5.0.5) Daniel Graham
+- 3 weeks ago (tag: 5.0.5) Daniel Graham
     9273685 2023-06-05 06:28:25 -0400
     Tagged version 5.0.5.
 
-- 2 weeks ago (tag: 5.0.4) Daniel Graham
+- 3 weeks ago (tag: 5.0.4) Daniel Graham
     ea199ac 2023-06-05 06:02:56 -0400
     Tagged version 5.0.4.
 
-- 2 weeks ago (tag: 5.0.3) Daniel Graham
+- 3 weeks ago (tag: 5.0.3) Daniel Graham
     e0a0d9e 2023-06-04 16:44:49 -0400
     Tagged version 5.0.3.
 
-- 2 weeks ago (tag: 5.0.2) Daniel Graham
+- 3 weeks ago (tag: 5.0.2) Daniel Graham
     4c5d4bb 2023-06-04 13:26:17 -0400
     Tagged version 5.0.2.
 
-- 2 weeks ago (tag: 5.0.1) Daniel Graham
+- 3 weeks ago (tag: 5.0.1) Daniel Graham
     b30f0ed 2023-06-04 12:47:15 -0400
     Tagged version 5.0.1.
-
-- 3 weeks ago (tag: 5.0.0) Daniel Graham
-    7bc8090 2023-06-03 07:21:38 -0400
-    Tagged version 5.0.0. Use pendulum periods for f and elements of h
-    instead of datetimes.
```

### Comparing `etm-dgraham-5.1.6/PKG-INFO` & `etm-dgraham-5.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.6
+Version: 5.1.7
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.6/README.md` & `etm-dgraham-5.1.7/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/bump.py` & `etm-dgraham-5.1.7/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/docs/index_konnections.md` & `etm-dgraham-5.1.7/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/docs/index_usedtime.md` & `etm-dgraham-5.1.7/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/docs/multiple_timers.md` & `etm-dgraham-5.1.7/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/etm/__main__.py` & `etm-dgraham-5.1.7/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/etm/data.py` & `etm-dgraham-5.1.7/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/etm/ical.py` & `etm-dgraham-5.1.7/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/etm/make_examples.py` & `etm-dgraham-5.1.7/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/etm/model.py` & `etm-dgraham-5.1.7/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/env python
 
+# standard sort order: ['!', '#', '$', '%', '&', '(', ')', '*', '+',
+# ',', '-', '.', ':', ';', '<', '=', '>', '?', '@', 'A', 'B', 'Y', 'Z',
+# '^', '_', 'a', 'b', 'y', 'z', '~']
+
 from pprint import pprint
 import datetime # for type testing in rrule
 import pendulum
 from pendulum import parse as pendulum_parse
 from pendulum.datetime import Timezone
 from pendulum import __version__ as pendulum_version
 import locale
@@ -37,15 +41,19 @@
         dt = dt.replace(tzinfo=tz)
     return dt
 
 import sys
 import re
 
 from tinydb import __version__ as tinydb_version
-from tinydb.table import Document
+from packaging.version import parse as parse_version
+if parse_version(tinydb_version) >= parse_version("4.0.0"):
+    from tinydb.table import Document
+else:
+    from tinydb.database import Document
 
 from jinja2 import Template
 from jinja2 import __version__ as jinja2_version
 
 import textwrap
 import os
 import platform
@@ -1942,15 +1950,18 @@
 
 def fmt_period(obj):
     if not isinstance(obj, pendulum.Period):
         return None
     start = obj.start
     end = obj.end
     neg = start > end
-    diff = end - start
+    if neg:
+        diff = start - end
+    else:
+        diff = end - start
     until = []
     days = diff.remaining_days
     hours = diff.hours
     minutes = diff.minutes
     if neg:
         until.append("-")
     else:
@@ -2339,20 +2350,22 @@
         self.settings = settings
         # if 'keep_current' in self.settings and self.settings['keep_current']:
         if 'keep_current' in self.settings and self.settings['keep_current'][0]:
             # weeks is not zero
             self.mk_current = True
             self.currfile = os.path.normpath(os.path.join(etmdir, 'current.txt'))
         else:
-            self.currfile = None
             self.mk_current = False
+            self.currfile = None
         if 'keep_next' in self.settings and self.settings['keep_next']:
             # keep_next is true
+            self.mk_next = True
             self.nextfile = os.path.normpath(os.path.join(etmdir, 'next.txt'))
         else:
+            self.mk_next = False
             self.nextfile = None
 
         if 'locale' in self.settings:
             locale_str = settings['locale']
             # locale_str should have the format "en_US"
             if locale_str:
                 try:
@@ -2747,15 +2760,15 @@
         if self.active_view == 'timers':
             self.timers_view, self.row2id = show_timers(self.db, self.pinned_list, self.link_list, self.konnected, self.timers, self.active_timer)
             return self.timers_view
         if self.active_view == 'forthcoming':
             self.forthcoming_view, self.row2id = show_forthcoming(self.db, self.id2relevant, self.pinned_list, self.link_list, self.konnected, self.timers)
             return self.forthcoming_view
         if self.active_view == 'do next':
-            self.next_view, self.row2id = show_next(self.db, self.pinned_list, self.link_list, self.konnected, self.timers)
+            self.next_view, self.row2id, self.next_txt = show_next(self.db, self.pinned_list, self.link_list, self.konnected, self.timers)
             return self.next_view
         if self.active_view == 'journal':
             self.journal_view, self.row2id = show_journal(self.db, self.id2relevant, self.pinned_list, self.link_list, self.konnected, self.timers)
             return self.journal_view
         if self.active_view == 'tags':
             self.tag_view, self.row2id = show_tags(self.db, self.id2relevant, self.pinned_list, self.link_list, self.konnected, self.timers)
             return self.tag_view
@@ -2890,19 +2903,21 @@
             if curr_lines:
                 with open(self.currfile, 'w', encoding='utf-8') as fo:
                     fo.write("\n\n".join([x.strip() for x in curr_lines]))
                 logger.info(f"saved {len(curr_lines)} weeks from current schedule to {self.currfile}")
             else:
                 logger.info("current schedule empty - did not save")
 
-        if self.nextfile is not None:
-            next_view, row2id = show_next(self.db, self.pinned_list, self.link_list, self.konnected, self.timers)
-            with open(self.nextfile, 'w', encoding='utf-8') as fo:
-                fo.write(re.sub(' {3,}', ' ', next_view))
-            logger.info(f"saved do next to {self.nextfile}")
+        if self.mk_next:
+            next_view, row2id, next_txt = show_next(self.db, self.pinned_list, self.link_list, self.konnected, self.timers)
+            next_view = current_hsh['next'] if 'next' in current_hsh else None
+            if next_txt:
+                with open(self.nextfile, 'w', encoding='utf-8') as fo:
+                    fo.write(re.sub(LINEDOT, '   ', next_txt))
+                logger.info(f"saved do next to {self.nextfile}")
 
 
     def show_query(self):
         self.is_showing_query = True
 
     def hide_query(self):
         self.is_showing_query = False
@@ -6316,14 +6331,19 @@
     return tree, row2id
 
 
 def show_next(db, pinned_list=[], link_list=[], konnect_list=[], timers={}):
     """
     Unfinished, undated tasks and jobs
     """
+    # width = settings['keep_current'][1]
+    global current_hsh
+    mk_next = settings['keep_next']
+    next_width = settings['keep_current'][1] - 1
+
     width = shutil.get_terminal_size()[0] - 3
     rows = []
     locations = set([])
     group_names = []
     groups = settings.get('locations', {})
     using_groups = True if groups else False
     if using_groups:
@@ -6406,16 +6426,34 @@
                 path = f"{group}/{row['location']}"
                 values = row['columns']
                 rdict.add(path, values)
         else:
             path = row['location']
             values = row['columns']
             rdict.add(path, values)
+
     tree, row2id = rdict.as_tree(rdict, level=0)
-    return tree, row2id
+
+    if mk_next:
+        cdict = NDict(compact=True, width=next_width)
+        for row in rows:
+            if using_groups:
+                groups = location2groups.get(row['location'], ['OTHER'])
+                for group in groups:
+                    path = f"{group}/{row['location']}"
+                    values = row['columns']
+                    cdict.add(path, values)
+            else:
+                path = row['location']
+                values = row['columns']
+                cdict.add(path, values)
+        ctree, crow2id = cdict.as_tree(cdict, level=0)
+        current_hsh['next'] = ctree
+
+    return tree, row2id, ctree
 
 
 def show_journal(db, id2relevant, pinned_list=[], link_list=[], konnect_list=[], timers={}):
     """
     journal grouped by index entry
     """
     width = shutil.get_terminal_size()[0] - 3
@@ -7367,22 +7405,14 @@
                 elif day_ == tomorrow:
                     day_ += " (Tomorrow)"
                 path = f"{wk_fmt}/{day_}"
                 values = row['columns']
                 # heading = f"Busy periods for {day_}"
                 if values[0] in ["*", "-"]:
                     values[1] = re.sub(' *\n+ *', ' ', values[1])
-                    # busyperiod = row.get('busyperiod', "")
-                    # if busyperiod:
-                    #     wrap = row.get('wrap', [])
-                    #     wrapped = row.get('wrapped', "")
-                    #     row = wkday2row(dayofweek)
-                    #     week2day2heading[week][row] = day_
-                    #     summary = values[1].ljust(current_summary_width-20, ' ')
-                    #     busy_row = f"{values[0]} {summary} {wrapped:^15}".rstrip()
                 cdict.add(path, values)
 
             ctree, crow2id = cdict.as_tree(cdict, level=0)
             current_hsh[week] = ctree
 
     busyday_details = {}
     for week in allday_details:
```

### Comparing `etm-dgraham-5.1.6/etm/options.py` & `etm-dgraham-5.1.7/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/etm/report.py` & `etm-dgraham-5.1.7/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/etm/view.py` & `etm-dgraham-5.1.7/etm/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1418,15 +1418,14 @@
             if now.second < 6:
                 # minutes = now.minute % interval if interval else now.minute % 5
                 minutes = now.minute
                 current_today = dataview.now.format("YYYYMMDD")
                 asyncio.ensure_future(maybe_alerts(now))
                 current_datetime = status_time(now)
                 today = now.format("YYYYMMDD")
-                logger.debug(f"now: {now}, minutes: {minutes}")
 
                 if updates_interval and minutes % updates_interval == 0:
                     loop = asyncio.get_event_loop()
                     asyncio.ensure_future(updates_loop(loop))
 
                 if minutes % 5 == 0:
                     loop = asyncio.get_event_loop()
```

### Comparing `etm-dgraham-5.1.6/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.1.7/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.1.6
+Version: 5.1.7
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.1.6/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.1.7/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.1.7/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/etmlogo.png` & `etm-dgraham-5.1.7/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/etmlogo_small.png` & `etm-dgraham-5.1.7/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/etmview_agenda.png` & `etm-dgraham-5.1.7/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/namedcolors.py` & `etm-dgraham-5.1.7/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/new.png` & `etm-dgraham-5.1.7/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/setup.py` & `etm-dgraham-5.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/test/test_parser.py` & `etm-dgraham-5.1.7/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/utilities/colons_to_slashes.py` & `etm-dgraham-5.1.7/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/utilities/etm_in` & `etm-dgraham-5.1.7/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/utilities/inbasket` & `etm-dgraham-5.1.7/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.1.6/utilities/open_in_mutt` & `etm-dgraham-5.1.7/utilities/open_in_mutt`

 * *Files identical despite different names*

