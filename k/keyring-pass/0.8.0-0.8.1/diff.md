# Comparing `tmp/keyring_pass-0.8.0.tar.gz` & `tmp/keyring_pass-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_pass-0.8.0.tar", max compression
+gzip compressed data, was "keyring_pass-0.8.1.tar", max compression
```

## Comparing `keyring_pass-0.8.0.tar` & `keyring_pass-0.8.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1077 2022-09-21 07:02:26.772102 keyring_pass-0.8.0/LICENSE
--rw-r--r--   0        0        0     1075 2022-10-20 13:22:58.861889 keyring_pass-0.8.0/README.md
--rw-r--r--   0        0        0     3154 2022-10-20 13:29:52.965947 keyring_pass-0.8.0/keyring_pass/__init__.py
--rw-r--r--   0        0        0      746 2022-10-20 13:00:14.839011 keyring_pass-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1978 1970-01-01 00:00:00.000000 keyring_pass-0.8.0/setup.py
--rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 keyring_pass-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-09-21 07:02:26.772102 keyring_pass-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1075 2022-10-20 13:22:58.861889 keyring_pass-0.8.1/README.md
+-rw-r--r--   0        0        0     3274 2023-06-23 07:46:03.306169 keyring_pass-0.8.1/keyring_pass/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-23 07:46:13.292339 keyring_pass-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 keyring_pass-0.8.1/PKG-INFO
```

### Comparing `keyring_pass-0.8.0/LICENSE` & `keyring_pass-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keyring_pass-0.8.0/README.md` & `keyring_pass-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `keyring_pass-0.8.0/keyring_pass/__init__.py` & `keyring_pass-0.8.1/keyring_pass/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,29 +7,35 @@
 import sys
 
 import keyring
 from jaraco.classes import properties
 from keyring import backend
 from keyring.util import platform_ as platform
 
+try:
+    from functools import cache
+except ImportError:
+    from functools import lru_cache
+    cache = lru_cache(maxsize=None)
+
 
 def command(cmd, **kwargs):
     kwargs.setdefault("stderr", sys.stderr)
     try:
         output = subprocess.check_output(cmd, **kwargs)
     except subprocess.CalledProcessError as exc:
         pattern = b"password store is empty"
         if pattern in exc.output:
             raise RuntimeError(exc.output)
         sys.stderr.write(exc.stdout.decode("utf8"))
         raise
     return codecs.decode(output, "utf8")
 
 
-@functools.cache
+@cache
 def _load_config(
     keyring_cfg=os.path.join(platform.config_root(), "keyringrc.cfg"),
 ):
     cfg = {}
     if not os.path.exists(keyring_cfg):
         return cfg
```

### Comparing `keyring_pass-0.8.0/pyproject.toml` & `keyring_pass-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keyring-pass"
-version = "0.8.0"
+version = "0.8.1"
 description = "https://www.passwordstore.org/ backend for https://pypi.org/project/keyring/"
 authors = ["Krzysztof Nazarewski <3494992+nazarewk@users.noreply.github.com>"]
 homepage = "https://github.com/nazarewk/keyring_pass"
 repository = "https://github.com/nazarewk/keyring_pass"
 license = "MIT"
 readme = "README.md"
 keywords = [
```

### Comparing `keyring_pass-0.8.0/PKG-INFO` & `keyring_pass-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyring-pass
-Version: 0.8.0
+Version: 0.8.1
 Summary: https://www.passwordstore.org/ backend for https://pypi.org/project/keyring/
 Home-page: https://github.com/nazarewk/keyring_pass
 License: MIT
 Keywords: keyring,pass
 Author: Krzysztof Nazarewski
 Author-email: 3494992+nazarewk@users.noreply.github.com
 Requires-Python: >=3.7
```

