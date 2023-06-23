# Comparing `tmp/cribbage_scorer-0.2.3.tar.gz` & `tmp/cribbage_scorer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cribbage_scorer-0.2.3.tar", last modified: Fri Apr 14 19:29:11 2023, max compression
+gzip compressed data, was "cribbage_scorer-0.2.4.tar", last modified: Fri Jun 23 18:18:41 2023, max compression
```

## Comparing `cribbage_scorer-0.2.3.tar` & `cribbage_scorer-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:29:11.683847 cribbage_scorer-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-14 19:29:11.683847 cribbage_scorer-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-14 19:29:01.000000 cribbage_scorer-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:29:11.683847 cribbage_scorer-0.2.3/cribbage_scorer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:29:01.000000 cribbage_scorer-0.2.3/cribbage_scorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-04-14 19:29:01.000000 cribbage_scorer-0.2.3/cribbage_scorer/cribbage_scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:29:11.683847 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-14 19:29:11.000000 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 19:29:11.000000 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:29:11.000000 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 19:29:11.000000 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 19:29:11.000000 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 19:29:11.683847 cribbage_scorer-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 19:29:01.000000 cribbage_scorer-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:18:41.626497 cribbage_scorer-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-23 18:18:41.626497 cribbage_scorer-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-23 18:18:31.000000 cribbage_scorer-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:18:41.622497 cribbage_scorer-0.2.4/cribbage_scorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 18:18:31.000000 cribbage_scorer-0.2.4/cribbage_scorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-06-23 18:18:31.000000 cribbage_scorer-0.2.4/cribbage_scorer/cribbage_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:18:41.626497 cribbage_scorer-0.2.4/cribbage_scorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-23 18:18:41.000000 cribbage_scorer-0.2.4/cribbage_scorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-23 18:18:41.000000 cribbage_scorer-0.2.4/cribbage_scorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:18:41.000000 cribbage_scorer-0.2.4/cribbage_scorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 18:18:41.000000 cribbage_scorer-0.2.4/cribbage_scorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 18:18:41.000000 cribbage_scorer-0.2.4/cribbage_scorer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:18:41.626497 cribbage_scorer-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-23 18:18:31.000000 cribbage_scorer-0.2.4/setup.py
```

### Comparing `cribbage_scorer-0.2.3/PKG-INFO` & `cribbage_scorer-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cribbage_scorer
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Cribbage scoring tool
 Home-page: https://github.com/phoughton/cribbage_scorer
 Author: Peter Houghton
 Author-email: pete@investigatingsoftware.co.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cribbage_scorer-0.2.3/README.md` & `cribbage_scorer-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cribbage_scorer-0.2.3/cribbage_scorer/cribbage_scorer.py` & `cribbage_scorer-0.2.4/cribbage_scorer/cribbage_scorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,18 +300,21 @@
     running_score = []
     running_msg = []
     card_set = sorted(set(card_nums))
     for group in more_itertools.consecutive_groups(list(card_set)):
         group_list = list(group)
         group_length = len(group_list)
         if group_length >= 3:
-            multiples_length = len(count_multiples(card_nums))
-            if multiples_length > 0:
-                running_msg.append(f"Multi-run: {card_nameify(card_nums)} ({group_length * multiples_length}pts)")
-                running_score.append((group_length * multiples_length))
+            the_multiples = count_multiples(card_nums)
+
+            multiples_in_run = sum([1 for card_num in the_multiples if card_num in group_list])
+
+            if multiples_in_run > 0:
+                running_msg.append(f"Multi-run: {card_nameify(card_nums)} ({group_length * multiples_in_run}pts)")
+                running_score.append((group_length * multiples_in_run))
             else:
                 running_score.append(group_length)
                 running_msg.append(f"Run of {group_length} cards ({group_length}pts)")
 
     return sum(running_score), "|".join(running_msg)
```

### Comparing `cribbage_scorer-0.2.3/cribbage_scorer.egg-info/PKG-INFO` & `cribbage_scorer-0.2.4/cribbage_scorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cribbage-scorer
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Cribbage scoring tool
 Home-page: https://github.com/phoughton/cribbage_scorer
 Author: Peter Houghton
 Author-email: pete@investigatingsoftware.co.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cribbage_scorer-0.2.3/setup.py` & `cribbage_scorer-0.2.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cribbage_scorer",
-    version="0.2.3",
+    version="0.2.4",
     author="Peter Houghton",
     author_email="pete@investigatingsoftware.co.uk",
     description="A Cribbage scoring tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phoughton/cribbage_scorer",
     packages=setuptools.find_packages(),
```

