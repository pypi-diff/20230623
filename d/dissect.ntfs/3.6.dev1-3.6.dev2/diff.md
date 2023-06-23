# Comparing `tmp/dissect.ntfs-3.6.dev1.tar.gz` & `tmp/dissect.ntfs-3.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ntfs-3.6.dev1.tar", last modified: Fri Jun 16 12:50:15 2023, max compression
+gzip compressed data, was "dissect.ntfs-3.6.dev2.tar", last modified: Fri Jun 23 15:01:23 2023, max compression
```

## Comparing `dissect.ntfs-3.6.dev1.tar` & `dissect.ntfs-3.6.dev2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.440333 dissect.ntfs-3.6.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.440333 dissect.ntfs-3.6.dev1/dissect/ntfs/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/c_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    16517 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/mft.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/secure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/dissect/ntfs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.440333 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-16 12:50:15.000000 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-16 12:50:15.000000 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 12:50:15.000000 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 12:50:15.000000 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 12:50:15.000000 dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-16 12:50:06.000000 dissect.ntfs-3.6.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/data/boot_2m.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/data/mft.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)   908628 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/data/ntfs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/data/ntfs_fragmented_mft.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/data/sds.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 12:50:15.444333 dissect.ntfs-3.6.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_mft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_secure.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 12:50:02.000000 dissect.ntfs-3.6.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.508539 dissect.ntfs-3.6.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-23 15:01:23.508539 dissect.ntfs-3.6.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.496539 dissect.ntfs-3.6.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.500539 dissect.ntfs-3.6.dev2/dissect/ntfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/c_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/mft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/dissect/ntfs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.496539 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-23 15:01:23.000000 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-23 15:01:23.000000 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:01:23.000000 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 15:01:23.000000 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 15:01:23.000000 dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-23 15:01:13.000000 dissect.ntfs-3.6.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:01:23.508539 dissect.ntfs-3.6.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.504539 dissect.ntfs-3.6.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.508539 dissect.ntfs-3.6.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/data/boot_2m.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/data/mft.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   908628 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/data/ntfs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/data/ntfs_fragmented_mft.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/data/sds.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:01:23.508539 dissect.ntfs-3.6.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_mft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-23 15:01:07.000000 dissect.ntfs-3.6.dev2/tox.ini
```

### Comparing `dissect.ntfs-3.6.dev1/LICENSE` & `dissect.ntfs-3.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/PKG-INFO` & `dissect.ntfs-3.6.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ntfs
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
 Project-URL: repository, https://github.com/fox-it/dissect.ntfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ntfs-3.6.dev1/README.md` & `dissect.ntfs-3.6.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/dissect/ntfs/__init__.py` & `dissect.ntfs-3.6.dev2/dissect/ntfs/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/dissect/ntfs/attr.py` & `dissect.ntfs-3.6.dev2/dissect/ntfs/attr.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,21 +508,27 @@
         return f"<$FILE_NAME {self.print_name}>"
 
     @property
     def tag(self) -> IO_REPARSE_TAG:
         return self.attr.ReparseTag
 
     @property
-    def substitute_name(self) -> str:
+    def substitute_name(self) -> Optional[str]:
+        if not self.tag_header:
+            return None
+
         offset = self.tag_header.SubstituteNameOffset
         length = self.tag_header.SubstituteNameLength
         return self.buffer[offset : offset + length].decode("utf-16-le")
 
     @property
-    def print_name(self) -> str:
+    def print_name(self) -> Optional[str]:
+        if not self.tag_header:
+            return None
+
         offset = self.tag_header.PrintNameOffset
         length = self.tag_header.PrintNameLength
         return self.buffer[offset : offset + length].decode("utf-16-le")
 
     @property
     def absolute(self) -> bool:
         if self.tag != IO_REPARSE_TAG.SYMLINK:
```

### Comparing `dissect.ntfs-3.6.dev1/dissect/ntfs/c_ntfs.py` & `dissect.ntfs-3.6.dev2/dissect/ntfs/c_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/dissect/ntfs/index.py` & `dissect.ntfs-3.6.dev2/dissect/ntfs/index.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/dissect/ntfs/mft.py` & `dissect.ntfs-3.6.dev2/dissect/ntfs/mft.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from dissect.ntfs.c_ntfs import (
     ATTRIBUTE_TYPE_CODE,
     DEFAULT_RECORD_SIZE,
     FILE_FILE_NAME_INDEX_PRESENT,
     FILE_NAME_DOS,
     FILE_NUMBER_MFT,
     FILE_NUMBER_ROOT,
+    IO_REPARSE_TAG,
     c_ntfs,
     segment_reference,
 )
 from dissect.ntfs.exceptions import (
     BrokenMftError,
     Error,
     FileNotFoundError,
@@ -316,36 +317,46 @@
         """Return whether this record is a file."""
         return not self.is_dir()
 
     def is_reparse_point(self) -> bool:
         """Return whether this record is a reparse point."""
         return ATTRIBUTE_TYPE_CODE.REPARSE_POINT in self.attributes
 
+    def is_symlink(self) -> bool:
+        """Return whether this record is a symlink reparse point."""
+        attr = self.attributes[ATTRIBUTE_TYPE_CODE.REPARSE_POINT]
+        return bool(attr) and attr.tag == IO_REPARSE_TAG.SYMLINK
+
+    def is_mount_point(self) -> bool:
+        """Return whether this record is a mount point reparse point."""
+        attr = self.attributes[ATTRIBUTE_TYPE_CODE.REPARSE_POINT]
+        return bool(attr) and attr.tag == IO_REPARSE_TAG.MOUNT_POINT
+
     @cached_property
     def reparse_point_name(self) -> str:
         """Return the (printable) name of this reparse point."""
-        if not self.is_reparse_point:
+        if not self.is_reparse_point():
             raise NotAReparsePointError(f"{self!r} is not a reparse point")
         return self.attributes[ATTRIBUTE_TYPE_CODE.REPARSE_POINT].print_name
 
     @cached_property
     def reparse_point_substitute_name(self) -> str:
         """Return the substitute name of this reparse point."""
-        if not self.is_reparse_point:
+        if not self.is_reparse_point():
             raise NotAReparsePointError(f"{self!r} is not a reparse point")
         return self.attributes[ATTRIBUTE_TYPE_CODE.REPARSE_POINT].substitute_name
 
     @cached_property
     def reparse_point_record(self) -> MftRecord:
         """Resolve a reparse point and return the target record.
 
         Note: absolute links (such as directory junctions) will _always_ fail in the context of a single filesystem.
         Absolute links include the drive letter, of which we have no knowledge here.
         """
-        if not self.is_reparse_point:
+        if not self.is_reparse_point():
             raise NotAReparsePointError(f"{self!r} is not a reparse point")
 
         if not self.ntfs or not self.ntfs.mft:
             raise MftNotAvailableError()
 
         reparse_point = self.attributes[ATTRIBUTE_TYPE_CODE.REPARSE_POINT]
```

### Comparing `dissect.ntfs-3.6.dev1/dissect/ntfs/ntfs.py` & `dissect.ntfs-3.6.dev2/dissect/ntfs/ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/dissect/ntfs/secure.py` & `dissect.ntfs-3.6.dev2/dissect/ntfs/secure.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/dissect/ntfs/stream.py` & `dissect.ntfs-3.6.dev2/dissect/ntfs/stream.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/dissect/ntfs/usnjrnl.py` & `dissect.ntfs-3.6.dev2/dissect/ntfs/usnjrnl.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/dissect/ntfs/util.py` & `dissect.ntfs-3.6.dev2/dissect/ntfs/util.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/PKG-INFO` & `dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ntfs
-Version: 3.6.dev1
+Version: 3.6.dev2
 Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
 Project-URL: repository, https://github.com/fox-it/dissect.ntfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ntfs-3.6.dev1/dissect.ntfs.egg-info/SOURCES.txt` & `dissect.ntfs-3.6.dev2/dissect.ntfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/pyproject.toml` & `dissect.ntfs-3.6.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/conftest.py` & `dissect.ntfs-3.6.dev2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/data/boot_2m.bin.gz` & `dissect.ntfs-3.6.dev2/tests/data/boot_2m.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/data/mft.bin.gz` & `dissect.ntfs-3.6.dev2/tests/data/mft.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/data/ntfs.bin.gz` & `dissect.ntfs-3.6.dev2/tests/data/ntfs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/data/ntfs_fragmented_mft.csv.gz` & `dissect.ntfs-3.6.dev2/tests/data/ntfs_fragmented_mft.csv.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/data/sds.bin.gz` & `dissect.ntfs-3.6.dev2/tests/data/sds.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/docs/Makefile` & `dissect.ntfs-3.6.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/docs/conf.py` & `dissect.ntfs-3.6.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/test_attr.py` & `dissect.ntfs-3.6.dev2/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/test_index.py` & `dissect.ntfs-3.6.dev2/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/test_mft.py` & `dissect.ntfs-3.6.dev2/tests/test_mft.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/test_ntfs.py` & `dissect.ntfs-3.6.dev2/tests/test_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/test_secure.py` & `dissect.ntfs-3.6.dev2/tests/test_secure.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/test_usnjrnl.py` & `dissect.ntfs-3.6.dev2/tests/test_usnjrnl.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tests/test_util.py` & `dissect.ntfs-3.6.dev2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev1/tox.ini` & `dissect.ntfs-3.6.dev2/tox.ini`

 * *Files identical despite different names*

