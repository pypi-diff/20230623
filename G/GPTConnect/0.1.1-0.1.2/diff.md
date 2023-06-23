# Comparing `tmp/GPTConnect-0.1.1.tar.gz` & `tmp/GPTConnect-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTConnect-0.1.1.tar", last modified: Fri Jun 23 13:48:46 2023, max compression
+gzip compressed data, was "GPTConnect-0.1.2.tar", last modified: Fri Jun 23 13:49:56 2023, max compression
```

## Comparing `GPTConnect-0.1.1.tar` & `GPTConnect-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 13:48:46.169783 GPTConnect-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-23 13:48:46.159784 GPTConnect-0.1.1/GPTConnect.egg-info/
--rw-rw-rw-   0        0        0      100 2023-06-23 13:48:45.000000 GPTConnect-0.1.1/GPTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-23 13:48:46.000000 GPTConnect-0.1.1/GPTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 13:48:45.000000 GPTConnect-0.1.1/GPTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-23 13:48:45.000000 GPTConnect-0.1.1/GPTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      100 2023-06-23 13:48:46.168782 GPTConnect-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      626 2023-06-23 12:40:28.000000 GPTConnect-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 13:48:46.164785 GPTConnect-0.1.1/gptconnect/
--rw-rw-rw-   0        0        0       27 2023-06-23 13:36:18.000000 GPTConnect-0.1.1/gptconnect/__init__.py
--rw-rw-rw-   0        0        0     2591 2023-06-23 13:36:05.000000 GPTConnect-0.1.1/gptconnect/gptconnect.py
--rw-rw-rw-   0        0        0       42 2023-06-23 13:48:46.169783 GPTConnect-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-06-23 13:46:26.000000 GPTConnect-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 13:49:56.969889 GPTConnect-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-23 13:49:56.960889 GPTConnect-0.1.2/GPTConnect.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-06-23 13:49:56.000000 GPTConnect-0.1.2/GPTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-23 13:49:56.000000 GPTConnect-0.1.2/GPTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 13:49:56.000000 GPTConnect-0.1.2/GPTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 13:49:56.000000 GPTConnect-0.1.2/GPTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2023-06-23 13:49:56.968890 GPTConnect-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2023-06-23 12:40:28.000000 GPTConnect-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 13:49:56.965891 GPTConnect-0.1.2/gptconnect/
+-rw-rw-rw-   0        0        0       27 2023-06-23 13:36:18.000000 GPTConnect-0.1.2/gptconnect/__init__.py
+-rw-rw-rw-   0        0        0     2591 2023-06-23 13:36:05.000000 GPTConnect-0.1.2/gptconnect/gptconnect.py
+-rw-rw-rw-   0        0        0       42 2023-06-23 13:49:56.969889 GPTConnect-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      211 2023-06-23 13:49:52.000000 GPTConnect-0.1.2/setup.py
```

### Comparing `GPTConnect-0.1.1/README.md` & `GPTConnect-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `GPTConnect-0.1.1/gptconnect/gptconnect.py` & `GPTConnect-0.1.2/gptconnect/gptconnect.py`

 * *Files identical despite different names*

