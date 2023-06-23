# Comparing `tmp/lmt-cli-0.0.3.tar.gz` & `tmp/lmt-cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmt-cli-0.0.3.tar", last modified: Fri Jun 23 19:33:07 2023, max compression
+gzip compressed data, was "lmt-cli-0.0.4.tar", last modified: Fri Jun 23 19:36:50 2023, max compression
```

## Comparing `lmt-cli-0.0.3.tar` & `lmt-cli-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:33:07.714373 lmt-cli-0.0.3/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.3/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 19:33:07.714373 lmt-cli-0.0.3/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8412 2023-06-23 18:54:04.000000 lmt-cli-0.0.3/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:33:07.704373 lmt-cli-0.0.3/lmt/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.3/lmt/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7644 2023-06-23 19:17:15.000000 lmt-cli-0.0.3/lmt/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4828 2023-06-22 23:46:33.000000 lmt-cli-0.0.3/lmt/gpt_integration.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9224 2023-06-23 18:44:29.000000 lmt-cli-0.0.3/lmt/lib.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:33:07.714373 lmt-cli-0.0.3/lmt_cli.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 19:33:07.000000 lmt-cli-0.0.3/lmt_cli.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      275 2023-06-23 19:33:07.000000 lmt-cli-0.0.3/lmt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-23 19:33:07.000000 lmt-cli-0.0.3/lmt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       36 2023-06-23 19:33:07.000000 lmt-cli-0.0.3/lmt_cli.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-23 19:33:07.000000 lmt-cli-0.0.3/lmt_cli.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        4 2023-06-23 19:33:07.000000 lmt-cli-0.0.3/lmt_cli.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-23 19:33:07.714373 lmt-cli-0.0.3/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1170 2023-06-23 19:30:11.000000 lmt-cli-0.0.3/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:36:50.244373 lmt-cli-0.0.4/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.4/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 19:36:50.244373 lmt-cli-0.0.4/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     8412 2023-06-23 18:54:04.000000 lmt-cli-0.0.4/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:36:50.244373 lmt-cli-0.0.4/lmt/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.4/lmt/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7666 2023-06-23 19:35:04.000000 lmt-cli-0.0.4/lmt/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4828 2023-06-22 23:46:33.000000 lmt-cli-0.0.4/lmt/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9224 2023-06-23 18:44:29.000000 lmt-cli-0.0.4/lmt/lib.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-23 19:36:50.244373 lmt-cli-0.0.4/lmt_cli.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     9055 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      275 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       36 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        4 2023-06-23 19:36:50.000000 lmt-cli-0.0.4/lmt_cli.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-23 19:36:50.244373 lmt-cli-0.0.4/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1170 2023-06-23 19:36:19.000000 lmt-cli-0.0.4/setup.py
```

### Comparing `lmt-cli-0.0.3/LICENSE` & `lmt-cli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.3/PKG-INFO` & `lmt-cli-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmt-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
 Home-page: https://github.com/sderev/lmt
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/lmt
 Project-URL: Issues, http://github.com/sderev/lmt/issues
 Project-URL: Changelog, https://github.com/sderev/lmt/releases
```

### Comparing `lmt-cli-0.0.3/README.md` & `lmt-cli-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.3/lmt/cli.py` & `lmt-cli-0.0.4/lmt/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     if 0 <= value <= 2:
         return value
     else:
         raise click.BadParameter("Temperature must be between 0 and 2.")
 
 
 @click.group()
-@click.version_option()
+@click.version_option(package_name="lmt-cli")
 def lmt():
     """
     Talk to ChatGPT.
 
     Documentation: https://github.com/sderev/lmt
     """
     pass
```

### Comparing `lmt-cli-0.0.3/lmt/gpt_integration.py` & `lmt-cli-0.0.4/lmt/gpt_integration.py`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.3/lmt/lib.py` & `lmt-cli-0.0.4/lmt/lib.py`

 * *Files identical despite different names*

### Comparing `lmt-cli-0.0.3/lmt_cli.egg-info/PKG-INFO` & `lmt-cli-0.0.4/lmt_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmt-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: The main CLI tool within the LLM-Toolbox, designed to enable seamless communication with ChatGPT from your terminal. You can customize your experience by creating templates and using them to generate messages.
 Home-page: https://github.com/sderev/lmt
 Author: Sébastien De Revière
 License: Apache Licence, Version 2.0
 Project-URL: Documentation, https://github.com/sderev/lmt
 Project-URL: Issues, http://github.com/sderev/lmt/issues
 Project-URL: Changelog, https://github.com/sderev/lmt/releases
```

### Comparing `lmt-cli-0.0.3/setup.py` & `lmt-cli-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 
 def read_requirements():
     with open("requirements.txt") as file:
         return list(file)
```

