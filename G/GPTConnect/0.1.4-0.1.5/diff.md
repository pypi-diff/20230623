# Comparing `tmp/GPTConnect-0.1.4.tar.gz` & `tmp/GPTConnect-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTConnect-0.1.4.tar", last modified: Fri Jun 23 14:23:18 2023, max compression
+gzip compressed data, was "GPTConnect-0.1.5.tar", last modified: Fri Jun 23 14:30:51 2023, max compression
```

## Comparing `GPTConnect-0.1.4.tar` & `GPTConnect-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 14:23:18.439107 GPTConnect-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-06-23 14:23:18.433106 GPTConnect-0.1.4/GPTConnect.egg-info/
--rw-rw-rw-   0        0        0      799 2023-06-23 14:23:18.000000 GPTConnect-0.1.4/GPTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-23 14:23:18.000000 GPTConnect-0.1.4/GPTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 14:23:18.000000 GPTConnect-0.1.4/GPTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 14:23:18.000000 GPTConnect-0.1.4/GPTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-23 14:23:18.000000 GPTConnect-0.1.4/GPTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      799 2023-06-23 14:23:18.438104 GPTConnect-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      666 2023-06-23 14:20:28.000000 GPTConnect-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 14:23:18.436106 GPTConnect-0.1.4/gptconnect/
--rw-rw-rw-   0        0        0       27 2023-06-23 13:36:18.000000 GPTConnect-0.1.4/gptconnect/__init__.py
--rw-rw-rw-   0        0        0     2605 2023-06-23 14:19:13.000000 GPTConnect-0.1.4/gptconnect/gptconnect.py
--rw-rw-rw-   0        0        0       42 2023-06-23 14:23:18.439107 GPTConnect-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      353 2023-06-23 14:23:16.000000 GPTConnect-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:30:51.118877 GPTConnect-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-06-23 14:30:51.111906 GPTConnect-0.1.5/GPTConnect.egg-info/
+-rw-rw-rw-   0        0        0      852 2023-06-23 14:30:50.000000 GPTConnect-0.1.5/GPTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-23 14:30:51.000000 GPTConnect-0.1.5/GPTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 14:30:50.000000 GPTConnect-0.1.5/GPTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 14:30:50.000000 GPTConnect-0.1.5/GPTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 14:30:50.000000 GPTConnect-0.1.5/GPTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      852 2023-06-23 14:30:51.117877 GPTConnect-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2023-06-23 14:20:28.000000 GPTConnect-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 14:30:51.115879 GPTConnect-0.1.5/gptconnect/
+-rw-rw-rw-   0        0        0       27 2023-06-23 13:36:18.000000 GPTConnect-0.1.5/gptconnect/__init__.py
+-rw-rw-rw-   0        0        0     2605 2023-06-23 14:19:13.000000 GPTConnect-0.1.5/gptconnect/gptconnect.py
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:30:51.119878 GPTConnect-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      346 2023-06-23 14:30:44.000000 GPTConnect-0.1.5/setup.py
```

### Comparing `GPTConnect-0.1.4/GPTConnect.egg-info/PKG-INFO` & `GPTConnect-0.1.5/GPTConnect.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package to make GPT functions easy
+Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 
 # GPTConnect
 
 GPTConnect is a Python package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating, defining and interacting with GPT functions, making your development process smoother and more efficient.
 
 ## Features
```

### Comparing `GPTConnect-0.1.4/PKG-INFO` & `GPTConnect-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package to make GPT functions easy
+Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
 
 # GPTConnect
 
 GPTConnect is a Python package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating, defining and interacting with GPT functions, making your development process smoother and more efficient.
 
 ## Features
```

### Comparing `GPTConnect-0.1.4/README.md` & `GPTConnect-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `GPTConnect-0.1.4/gptconnect/gptconnect.py` & `GPTConnect-0.1.5/gptconnect/gptconnect.py`

 * *Files identical despite different names*

