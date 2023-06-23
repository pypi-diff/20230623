# Comparing `tmp/smqtk_image_io-0.17.0.tar.gz` & `tmp/smqtk_image_io-0.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smqtk_image_io-0.17.0.tar", max compression
+gzip compressed data, was "smqtk_image_io-0.17.1.tar", max compression
```

## Comparing `smqtk_image_io-0.17.0.tar` & `smqtk_image_io-0.17.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1481 2023-06-16 19:06:09.250499 smqtk_image_io-0.17.0/LICENSE.txt
--rw-r--r--   0        0        0      652 2023-06-16 19:06:09.250499 smqtk_image_io-0.17.0/README.md
--rw-r--r--   0        0        0     2395 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/pyproject.toml
--rw-r--r--   0        0        0      118 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/__init__.py
--rw-r--r--   0        0        0     7911 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/bbox.py
--rw-r--r--   0        0        0        0 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/impls/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/impls/image_reader/__init__.py
--rw-r--r--   0        0        0    19898 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/impls/image_reader/gdal_io.py
--rw-r--r--   0        0        0     4912 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/impls/image_reader/pil_io.py
--rw-r--r--   0        0        0        0 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/interfaces/__init__.py
--rw-r--r--   0        0        0     6770 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/interfaces/image_reader.py
--rw-r--r--   0        0        0        0 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/py.typed
--rw-r--r--   0        0        0        0 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/utils/__init__.py
--rw-r--r--   0        0        0    10265 2023-06-16 19:06:09.254500 smqtk_image_io-0.17.0/smqtk_image_io/utils/image.py
--rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 smqtk_image_io-0.17.0/PKG-INFO
+-rw-r--r--   0        0        0     1481 2023-06-23 15:05:57.522333 smqtk_image_io-0.17.1/LICENSE.txt
+-rw-r--r--   0        0        0      652 2023-06-23 15:05:57.522333 smqtk_image_io-0.17.1/README.md
+-rw-r--r--   0        0        0     2393 2023-06-23 15:05:57.522333 smqtk_image_io-0.17.1/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-06-23 15:05:57.526334 smqtk_image_io-0.17.1/smqtk_image_io/__init__.py
+-rw-r--r--   0        0        0     7911 2023-06-23 15:05:57.526334 smqtk_image_io-0.17.1/smqtk_image_io/bbox.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:05:57.526334 smqtk_image_io-0.17.1/smqtk_image_io/impls/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:05:57.526334 smqtk_image_io-0.17.1/smqtk_image_io/impls/image_reader/__init__.py
+-rw-r--r--   0        0        0    19898 2023-06-23 15:05:57.526334 smqtk_image_io-0.17.1/smqtk_image_io/impls/image_reader/gdal_io.py
+-rw-r--r--   0        0        0     4912 2023-06-23 15:05:57.526334 smqtk_image_io-0.17.1/smqtk_image_io/impls/image_reader/pil_io.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:05:57.526334 smqtk_image_io-0.17.1/smqtk_image_io/interfaces/__init__.py
+-rw-r--r--   0        0        0     6770 2023-06-23 15:05:57.526334 smqtk_image_io-0.17.1/smqtk_image_io/interfaces/image_reader.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:05:57.526334 smqtk_image_io-0.17.1/smqtk_image_io/py.typed
+-rw-r--r--   0        0        0        0 2023-06-23 15:05:57.526334 smqtk_image_io-0.17.1/smqtk_image_io/utils/__init__.py
+-rw-r--r--   0        0        0    10265 2023-06-23 15:05:57.526334 smqtk_image_io-0.17.1/smqtk_image_io/utils/image.py
+-rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 smqtk_image_io-0.17.1/PKG-INFO
```

### Comparing `smqtk_image_io-0.17.0/LICENSE.txt` & `smqtk_image_io-0.17.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.17.0/README.md` & `smqtk_image_io-0.17.1/README.md`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.17.0/pyproject.toml` & `smqtk_image_io-0.17.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 ###############################################################################
 [tool.poetry]
 name = "smqtk_image_io"
-version = "0.17.0"
+version = "0.17.1"
 description = "SMQTK Image IO"
 authors = ["Kitware, Inc. <smqtk-developers@kitware.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
@@ -23,15 +23,15 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pillow = ">=8.2.0"
-numpy = ">=1.19.5"
+numpy = ">=1.21"
 smqtk-core = ">=0.19"
 smqtk-dataprovider = ">=0.16.0"
 
 
 [tool.poetry.dev-dependencies]
 # CI
 flake8 = ">=3.9.0"
```

### Comparing `smqtk_image_io-0.17.0/smqtk_image_io/bbox.py` & `smqtk_image_io-0.17.1/smqtk_image_io/bbox.py`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.17.0/smqtk_image_io/impls/image_reader/gdal_io.py` & `smqtk_image_io-0.17.1/smqtk_image_io/impls/image_reader/gdal_io.py`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.17.0/smqtk_image_io/impls/image_reader/pil_io.py` & `smqtk_image_io-0.17.1/smqtk_image_io/impls/image_reader/pil_io.py`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.17.0/smqtk_image_io/interfaces/image_reader.py` & `smqtk_image_io-0.17.1/smqtk_image_io/interfaces/image_reader.py`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.17.0/smqtk_image_io/utils/image.py` & `smqtk_image_io-0.17.1/smqtk_image_io/utils/image.py`

 * *Files identical despite different names*

### Comparing `smqtk_image_io-0.17.0/PKG-INFO` & `smqtk_image_io-0.17.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smqtk-image-io
-Version: 0.17.0
+Version: 0.17.1
 Summary: SMQTK Image IO
 License: BSD-3-Clause
 Author: Kitware, Inc.
 Author-email: smqtk-developers@kitware.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.19.5)
+Requires-Dist: numpy (>=1.21)
 Requires-Dist: pillow (>=8.2.0)
 Requires-Dist: smqtk-core (>=0.19)
 Requires-Dist: smqtk-dataprovider (>=0.16.0)
 Description-Content-Type: text/markdown
 
 # SMQTK - Image-IO
```

