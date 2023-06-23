# Comparing `tmp/polywrap_ethereum_provider-0.1.0a3.tar.gz` & `tmp/polywrap_ethereum_provider-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_ethereum_provider-0.1.0a3.tar", max compression
+gzip compressed data, was "polywrap_ethereum_provider-0.1.0a4.tar", max compression
```

## Comparing `polywrap_ethereum_provider-0.1.0a3.tar` & `polywrap_ethereum_provider-0.1.0a4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     6661 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/__init__.py
--rw-r--r--   0        0        0     1789 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/connection.py
--rw-r--r--   0        0        0     2759 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/connections.py
--rw-r--r--   0        0        0     1451 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/networks.py
--rw-r--r--   0        0        0        0 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/py.typed
--rw-r--r--   0        0        0      163 2023-06-23 18:33:04.379386 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/__init__.py
--rw-r--r--   0        0        0     2481 2023-06-23 18:33:04.379386 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/module.py
--rw-r--r--   0        0        0      816 2023-06-23 18:33:04.379386 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/types.py
--rw-r--r--   0        0        0     7359 2023-06-23 18:33:04.379386 polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/wrap_info.py
--rw-r--r--   0        0        0     1632 2023-06-23 18:32:47.091625 polywrap_ethereum_provider-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1646 2023-06-23 18:37:28.998852 polywrap_ethereum_provider-0.1.0a4/README.md
+-rw-r--r--   0        0        0     6661 2023-06-23 18:37:28.998852 polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/__init__.py
+-rw-r--r--   0        0        0     1789 2023-06-23 18:37:28.998852 polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/connection.py
+-rw-r--r--   0        0        0     2759 2023-06-23 18:37:28.998852 polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/connections.py
+-rw-r--r--   0        0        0     1451 2023-06-23 18:37:28.998852 polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/networks.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:37:28.998852 polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/py.typed
+-rw-r--r--   0        0        0      163 2023-06-23 18:37:46.398855 polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/wrap/__init__.py
+-rw-r--r--   0        0        0     2481 2023-06-23 18:37:46.398855 polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/wrap/module.py
+-rw-r--r--   0        0        0      816 2023-06-23 18:37:46.398855 polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/wrap/types.py
+-rw-r--r--   0        0        0     7359 2023-06-23 18:37:46.398855 polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/wrap/wrap_info.py
+-rw-r--r--   0        0        0     1706 2023-06-23 18:37:28.998852 polywrap_ethereum_provider-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0     2266 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0a4/PKG-INFO
```

### Comparing `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/__init__.py` & `polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/connection.py` & `polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/connection.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/connections.py` & `polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/connections.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/networks.py` & `polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/networks.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/module.py` & `polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/wrap/module.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/types.py` & `polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/wrap/types.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a3/polywrap_ethereum_provider/wrap/wrap_info.py` & `polywrap_ethereum_provider-0.1.0a4/polywrap_ethereum_provider/wrap/wrap_info.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a3/pyproject.toml` & `polywrap_ethereum_provider-0.1.0a4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-ethereum-provider"
-version = "0.1.0a3"
+version = "0.1.0a4"
 description = "Ethereum provider in python"
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
-
+readme = "README.md"
+packages = [{include = "polywrap_ethereum_provider"}]
 include = ["polywrap_ethereum_provider/wrap/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 web3 = "6.1.0"
 eth_account = "0.8.0"
 polywrap-plugin = "0.1.0a33"
```

