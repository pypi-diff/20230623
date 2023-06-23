# Comparing `tmp/heygptcli-0.1.4.tar.gz` & `tmp/heygptcli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heygptcli-0.1.4.tar", max compression
+gzip compressed data, was "heygptcli-0.1.5.tar", max compression
```

## Comparing `heygptcli-0.1.4.tar` & `heygptcli-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       87 2023-06-21 13:32:50.445042 heygptcli-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/__init__.py
--rw-r--r--   0        0        0      774 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/api.py
--rwxr-xr-x   0        0        0     5292 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/cli.py
--rw-r--r--   0        0        0     2249 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/constant.py
--rw-r--r--   0        0        0     3519 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/core.py
--rw-r--r--   0        0        0     1984 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/serve.py
--rw-r--r--   0        0        0      153 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/serve_prompts.py
--rw-r--r--   0        0        0      849 2023-06-21 13:32:50.445042 heygptcli-0.1.4/heygpt/utils.py
--rw-r--r--   0        0        0      677 2023-06-21 13:32:50.445042 heygptcli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-23 09:09:49.068212 heygptcli-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/__init__.py
+-rw-r--r--   0        0        0      774 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/api.py
+-rwxr-xr-x   0        0        0     5292 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/cli.py
+-rw-r--r--   0        0        0     2249 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/constant.py
+-rw-r--r--   0        0        0     3515 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/core.py
+-rw-r--r--   0        0        0     1984 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/serve.py
+-rw-r--r--   0        0        0      153 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/serve_prompts.py
+-rw-r--r--   0        0        0      849 2023-06-23 09:09:49.068212 heygptcli-0.1.5/heygpt/utils.py
+-rw-r--r--   0        0        0      677 2023-06-23 09:09:49.068212 heygptcli-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 heygptcli-0.1.5/PKG-INFO
```

### Comparing `heygptcli-0.1.4/heygpt/api.py` & `heygptcli-0.1.5/heygpt/api.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.4/heygpt/cli.py` & `heygptcli-0.1.5/heygpt/cli.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.4/heygpt/constant.py` & `heygptcli-0.1.5/heygpt/constant.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.4/heygpt/core.py` & `heygptcli-0.1.5/heygpt/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     out = ""
     log.debug(f"model: {model}")
 
     if not text:
         raise Exception("No text found")
 
     if command != "":
-        _command = command + "\nTask: " + text
+        _command = command + "\n\n" + text
     else:
         _command = text
 
     if "gpt-3" in model:
         completion = openai.ChatCompletion.create(
             model=model,
             stream=True,
```

### Comparing `heygptcli-0.1.4/heygpt/serve.py` & `heygptcli-0.1.5/heygpt/serve.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.4/heygpt/utils.py` & `heygptcli-0.1.5/heygpt/utils.py`

 * *Files identical despite different names*

### Comparing `heygptcli-0.1.4/pyproject.toml` & `heygptcli-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heygptcli"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Rishang <rishang@localhost.com>"]
 readme = "README.md"
 packages = [
   { include = "heygpt" }
 ]
```

### Comparing `heygptcli-0.1.4/PKG-INFO` & `heygptcli-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heygptcli
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Rishang
 Author-email: rishang@localhost.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

