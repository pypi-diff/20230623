# Comparing `tmp/polywrap_fs_plugin-0.1.0a1.tar.gz` & `tmp/polywrap_fs_plugin-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_fs_plugin-0.1.0a1.tar", max compression
+gzip compressed data, was "polywrap_fs_plugin-0.1.0a2.tar", max compression
```

## Comparing `polywrap_fs_plugin-0.1.0a1.tar` & `polywrap_fs_plugin-0.1.0a2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1713 2023-05-01 17:23:05.150531 polywrap_fs_plugin-0.1.0a1/README.md
--rw-r--r--   0        0        0     4026 2023-05-01 17:23:05.150531 polywrap_fs_plugin-0.1.0a1/polywrap_fs_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 17:23:05.150531 polywrap_fs_plugin-0.1.0a1/polywrap_fs_plugin/py.typed
--rw-r--r--   0        0        0     1410 2023-05-01 17:23:05.154531 polywrap_fs_plugin-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     2292 1970-01-01 00:00:00.000000 polywrap_fs_plugin-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-06-23 18:09:39.330501 polywrap_fs_plugin-0.1.0a2/README.md
+-rw-r--r--   0        0        0     3816 2023-06-23 18:09:39.330501 polywrap_fs_plugin-0.1.0a2/polywrap_fs_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:09:39.330501 polywrap_fs_plugin-0.1.0a2/polywrap_fs_plugin/py.typed
+-rw-r--r--   0        0        0     1410 2023-06-23 18:09:39.330501 polywrap_fs_plugin-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 polywrap_fs_plugin-0.1.0a2/PKG-INFO
```

### Comparing `polywrap_fs_plugin-0.1.0a1/polywrap_fs_plugin/__init__.py` & `polywrap_fs_plugin-0.1.0a2/polywrap_fs_plugin/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """This package contains the Filesystem plugin."""
 import base64
 import os
 import shutil
 import stat
 from typing import Any
 
-from polywrap_core import InvokerClient, UriPackageOrWrapper
+from polywrap_core import InvokerClient
 from polywrap_plugin import PluginPackage
 
 from .wrap import *
 
 
 class FileSystemPlugin(Module[None]):
     """Defines the Filesystem plugin."""
 
-    async def read_file(
-        self, args: ArgsReadFile, client: InvokerClient[UriPackageOrWrapper], env: None
+    def read_file(
+        self, args: ArgsReadFile, client: InvokerClient, env: None
     ) -> bytes:
         """Read a file from the filesystem and return its contents as bytes. """
         with open(args["path"], "rb") as f:
             return f.read()
 
-    async def read_file_as_string(
+    def read_file_as_string(
         self,
         args: ArgsReadFileAsString,
-        client: InvokerClient[UriPackageOrWrapper],
+        client: InvokerClient,
         env: None,
     ) -> str:
         """Read a file from the filesystem, decode it using provided encoding\
             and return its contents as a string. """
         encoding = args.get("encoding", "utf-8")
         with open(args["path"], "rb") as f:
             content = f.read()
@@ -50,43 +50,43 @@
         if encoding == "BASE64URL":
             return base64.urlsafe_b64encode(content).decode("ascii").rstrip("=")
         if encoding == "HEX":
             return content.hex()
 
         raise ValueError(f"Unsupported encoding: {encoding}")
 
-    async def exists(
-        self, args: ArgsExists, client: InvokerClient[UriPackageOrWrapper], env: None
+    def exists(
+        self, args: ArgsExists, client: InvokerClient, env: None
     ) -> bool:
         """Check if a file or directory exists."""
         return os.path.exists(args["path"])
 
-    async def write_file(
-        self, args: ArgsWriteFile, client: InvokerClient[UriPackageOrWrapper], env: None
+    def write_file(
+        self, args: ArgsWriteFile, client: InvokerClient, env: None
     ) -> bool:
         """Write data to a file on the filesystem."""
         with open(args["path"], "wb") as f:
             f.write(args["data"])
         return True
 
 
-    async def mkdir(self, args: ArgsMkdir, client: InvokerClient[UriPackageOrWrapper], env: None):
+    def mkdir(self, args: ArgsMkdir, client: InvokerClient, env: None):
         """Create directories on the filesystem."""
         path = args["path"]
         if args.get("recursive", False):
             os.makedirs(path, exist_ok=True)
         else:
             parent_dir = os.path.dirname(path)
             if not os.path.exists(parent_dir):
                 raise FileNotFoundError(f"Parent directory does not exist: {parent_dir}")
             os.mkdir(path)
 
 
-    async def rm(
-        self, args: ArgsRm, client: InvokerClient[UriPackageOrWrapper], env: None
+    def rm(
+        self, args: ArgsRm, client: InvokerClient, env: None
     ) -> bool:
         """Remove a file or directory from the filesystem."""
         if os.path.isdir(args["path"]):
             if args.get("force", False) and args.get("recursive", False):
                 def force_remove(action: Any, name: str, exc: Exception) -> None:
                     os.chmod(name, stat.S_IWRITE)
                     os.remove(name)
@@ -96,16 +96,16 @@
                 shutil.rmtree(args["path"])
             else:
                 os.rmdir(args["path"])
         else:
             os.remove(args["path"])
         return True
 
-    async def rmdir(
-        self, args: ArgsRmdir, client: InvokerClient[UriPackageOrWrapper], env: None
+    def rmdir(
+        self, args: ArgsRmdir, client: InvokerClient, env: None
     ) -> bool:
         """Remove an empty directory from the filesystem."""
         os.rmdir(args["path"])
         return True
 
 
 def file_system_plugin() -> PluginPackage[None]:
```

### Comparing `polywrap_fs_plugin-0.1.0a1/pyproject.toml` & `polywrap_fs_plugin-0.1.0a2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-fs-plugin"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = ""
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 packages = [{include = "polywrap_fs_plugin"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-plugin = "0.1.0a29"
+polywrap-plugin = "0.1.0a33"
 httpx = "^0.23.3"
-polywrap-core = "^0.1.0a29"
-polywrap-msgpack = "^0.1.0a29"
-polywrap-manifest = "^0.1.0a29"
+polywrap-core = "^0.1.0a33"
+polywrap-msgpack = "^0.1.0a33"
+polywrap-manifest = "^0.1.0a33"
 
 [tool.poetry.group.dev.dependencies]
-polywrap-client = "0.1.0a29"
+polywrap-client = "0.1.0a33"
 black = "^23.1.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 isort = "^5.12.0"
 bandit = "^1.7.4"
 pyright = "^1.1.296"
 pylint = "^2.16.3"
-polywrap-uri-resolvers = "^0.1.0a29"
-polywrap-client-config-builder = "^0.1.0a29"
+polywrap-uri-resolvers = "^0.1.0a33"
+polywrap-client-config-builder = "^0.1.0a33"
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 pytest-mock = "^3.10.0"
 pydocstyle = "^6.3.0"
 
 [tool.bandit]
 exclude_dirs = ["tests"]
```

