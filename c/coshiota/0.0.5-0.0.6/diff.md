# Comparing `tmp/coshiota-0.0.5.tar.gz` & `tmp/coshiota-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coshiota-0.0.5.tar", max compression
+gzip compressed data, was "coshiota-0.0.6.tar", max compression
```

## Comparing `coshiota-0.0.5.tar` & `coshiota-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      263 2021-05-25 12:20:50.956729 coshiota-0.0.5/coshiota/__init__.py
--rw-r--r--   0        0        0     5337 2022-10-29 07:09:38.011711 coshiota-0.0.5/coshiota/certificate.py
--rw-r--r--   0        0        0    10070 2022-11-06 13:23:43.135302 coshiota-0.0.5/coshiota/cryptography_lowlevel.py
--rw-r--r--   0        0        0      578 2022-10-27 14:59:32.860897 coshiota-0.0.5/coshiota/csv_tools.py
--rw-r--r--   0        0        0      398 2022-10-27 14:41:21.277066 coshiota-0.0.5/coshiota/linux_kernel.py
--rw-r--r--   0        0        0     3158 2022-10-27 14:54:24.293978 coshiota-0.0.5/coshiota/serial_number.py
--rw-r--r--   0        0        0     3902 2022-10-27 14:41:38.044780 coshiota-0.0.5/coshiota/tools.py
--rw-r--r--   0        0        0     3623 2022-11-06 14:46:19.744955 coshiota-0.0.5/coshiota/trusty_payload_message.py
--rw-r--r--   0        0        0      623 2022-11-06 14:47:53.914986 coshiota-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      636 2022-11-06 19:12:11.948029 coshiota-0.0.5/setup.py
--rw-r--r--   0        0        0      527 2022-11-06 19:12:11.948241 coshiota-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      263 2021-05-25 12:20:50.956729 coshiota-0.0.6/coshiota/__init__.py
+-rw-r--r--   0        0        0     5337 2022-10-29 07:09:38.011711 coshiota-0.0.6/coshiota/certificate.py
+-rw-r--r--   0        0        0    10070 2023-06-23 14:48:48.485525 coshiota-0.0.6/coshiota/cryptography_lowlevel.py
+-rw-r--r--   0        0        0      578 2022-10-27 14:59:32.860897 coshiota-0.0.6/coshiota/csv_tools.py
+-rw-r--r--   0        0        0      398 2022-10-27 14:41:21.277066 coshiota-0.0.6/coshiota/linux_kernel.py
+-rw-r--r--   0        0        0     2561 2022-11-13 07:01:06.160958 coshiota-0.0.6/coshiota/naming.py
+-rw-r--r--   0        0        0     3158 2022-10-27 14:54:24.293978 coshiota-0.0.6/coshiota/serial_number.py
+-rw-r--r--   0        0        0     4188 2023-06-23 14:52:51.055973 coshiota-0.0.6/coshiota/tools.py
+-rw-r--r--   0        0        0     3623 2023-06-23 14:48:48.489525 coshiota-0.0.6/coshiota/trusty_payload_message.py
+-rw-r--r--   0        0        0      623 2023-06-23 14:58:16.658684 coshiota-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      636 2023-06-23 14:59:31.562485 coshiota-0.0.6/setup.py
+-rw-r--r--   0        0        0      527 2023-06-23 14:59:31.562714 coshiota-0.0.6/PKG-INFO
```

### Comparing `coshiota-0.0.5/coshiota/certificate.py` & `coshiota-0.0.6/coshiota/certificate.py`

 * *Files identical despite different names*

### Comparing `coshiota-0.0.5/coshiota/cryptography_lowlevel.py` & `coshiota-0.0.6/coshiota/cryptography_lowlevel.py`

 * *Files identical despite different names*

### Comparing `coshiota-0.0.5/coshiota/csv_tools.py` & `coshiota-0.0.6/coshiota/csv_tools.py`

 * *Files identical despite different names*

### Comparing `coshiota-0.0.5/coshiota/serial_number.py` & `coshiota-0.0.6/coshiota/serial_number.py`

 * *Files identical despite different names*

### Comparing `coshiota-0.0.5/coshiota/tools.py` & `coshiota-0.0.6/coshiota/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,28 @@
 
     for line in orjson.dumps(
         data,
         option=orjson.OPT_INDENT_2 | orjson.OPT_APPEND_NEWLINE,
     ).split(b"\n"):
         uselog.log(level, line.decode("utf-8"))
 
+def dump_json_to_stdout(data):
+    """
+    Dump ``data`` in JSON format to STDOUT
+
+    Args:
+        data: data
+
+    """
+    for line in orjson.dumps(
+        data,
+        option=orjson.OPT_INDENT_2 | orjson.OPT_APPEND_NEWLINE,
+    ).split(b"\n"):
+        print(line.decode("utf-8"))
+
 
 def load_json(path):
     """
     Load JSON encoded file and return its contents.
 
     Args:
         path(str): path
```

### Comparing `coshiota-0.0.5/coshiota/trusty_payload_message.py` & `coshiota-0.0.6/coshiota/trusty_payload_message.py`

 * *Files identical despite different names*

### Comparing `coshiota-0.0.5/pyproject.toml` & `coshiota-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     | \.?venv3?
   )/
 )
 '''
 
 [tool.poetry]
 name = "coshiota"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["doubleO8 <wb008@hdm-stuttgart.de>"]
 license = "GPL2"
 
 [tool.poetry.dependencies]
 python = "^3.7.3"
 pendulum = "^2.1.2"
```

### Comparing `coshiota-0.0.5/setup.py` & `coshiota-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['cryptography>=3.2', 'orjson>=3.7.12,<4.0.0', 'pendulum>=2.1.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'coshiota',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': '',
     'long_description': None,
     'author': 'doubleO8',
     'author_email': 'wb008@hdm-stuttgart.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `coshiota-0.0.5/PKG-INFO` & `coshiota-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coshiota
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 License: GPL2
 Author: doubleO8
 Author-email: wb008@hdm-stuttgart.de
 Requires-Python: >=3.7.3,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

