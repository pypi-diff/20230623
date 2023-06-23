# Comparing `tmp/merkly-0.6.0.tar.gz` & `tmp/merkly-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merkly-0.6.0.tar", max compression
+gzip compressed data, was "merkly-0.6.1.tar", max compression
```

## Comparing `merkly-0.6.0.tar` & `merkly-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-06-23 05:22:14.916906 merkly-0.6.0/LICENSE
--rw-r--r--   0        0        0     4707 2023-06-23 05:22:14.916906 merkly-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-06-23 05:22:14.916906 merkly-0.6.0/merkly/__init__.py
--rw-r--r--   0        0        0     4209 2023-06-23 05:22:14.916906 merkly-0.6.0/merkly/mtree.py
--rw-r--r--   0        0        0        0 2023-06-23 05:22:14.916906 merkly-0.6.0/merkly/utils/__init__.py
--rw-r--r--   0        0        0     1511 2023-06-23 05:22:14.916906 merkly-0.6.0/merkly/utils/crypto.py
--rw-r--r--   0        0        0      664 2023-06-23 05:22:14.916906 merkly-0.6.0/merkly/utils/math.py
--rw-r--r--   0        0        0      854 2023-06-23 05:22:14.916906 merkly-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5590 1970-01-01 00:00:00.000000 merkly-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-23 06:07:37.020355 merkly-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4756 2023-06-23 06:07:37.024355 merkly-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 06:07:37.024355 merkly-0.6.1/merkly/__init__.py
+-rw-r--r--   0        0        0     4209 2023-06-23 06:07:37.024355 merkly-0.6.1/merkly/mtree.py
+-rw-r--r--   0        0        0        0 2023-06-23 06:07:37.024355 merkly-0.6.1/merkly/utils/__init__.py
+-rw-r--r--   0        0        0     1511 2023-06-23 06:07:37.024355 merkly-0.6.1/merkly/utils/crypto.py
+-rw-r--r--   0        0        0      664 2023-06-23 06:07:37.024355 merkly-0.6.1/merkly/utils/math.py
+-rw-r--r--   0        0        0      878 2023-06-23 06:07:37.024355 merkly-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5680 1970-01-01 00:00:00.000000 merkly-0.6.1/PKG-INFO
```

### Comparing `merkly-0.6.0/LICENSE` & `merkly-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `merkly-0.6.0/README.md` & `merkly-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 <p align="center">
   <a href="https://pypi.org/project/merkly/">
-    <img alt="Merkly" src="./assets/merkly-banner.png" width="1000">
+    <img alt="Merkly" src="https://raw.githubusercontent.com/olivmath/merkly/main/assets/merkly-banner.png" width="1000">
   </a>
 </p>
 
 <p align="center">The simple and easy implementation of Python Merkle Tree.</p>
 
 ---
 
 <p align="center">
     <a href="https://pypi.org/project/merkly/">
         <img src="https://img.shields.io/pypi/v/merkly">
     </a>
-    <a href="https://github.com/olivmath/merkly/actions/workflows/test.yml">
-        <img src="https://github.com/olivmath/merkly/actions/workflows/test.yml/badge.svg?branch=main">
+    <a href="https://github.com/olivmath/merkly/actions/workflows/ci.yml">
+        <img src="https://github.com/olivmath/merkly/actions/workflows/ci.yml/badge.svg?branch=main">
     </a>
     <a href="https://pypi.org/project/merkly/">
         <img src="https://img.shields.io/pypi/pyversions/merkly">
     </a>
     <a href="https://pypi.org/project/merkly/">
         <img src="https://img.shields.io/pypi/dm/merkly">
     </a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
                                    [Merkly]
            The simple and easy implementation of Python Merkle Tree.
 ---
   [https://img.shields.io/pypi/v/merkly] [https://github.com/olivmath/merkly/
-actions/workflows/test.yml/badge.svg?branch=main] [https://img.shields.io/pypi/
+ actions/workflows/ci.yml/badge.svg?branch=main] [https://img.shields.io/pypi/
      pyversions/merkly] [https://img.shields.io/pypi/dm/merkly] [https://
       img.shields.io/github/commit-activity/m/olivmath/merkly] [https://
                          img.shields.io/pypi/l/merkly]
 --- ## Table of Contents - [Credits](#credits) - [How to install](#how-to-
 install) - [How it works](#how-it-works) - [How to use](#how-to-use) -
 [Roadmap](#roadmap) - [Contributing](#contributing) - [License](#license) ##
 Credits [![GitHub Contributors Image](https://contrib.rocks/
```

### Comparing `merkly-0.6.0/merkly/mtree.py` & `merkly-0.6.1/merkly/mtree.py`

 * *Files identical despite different names*

### Comparing `merkly-0.6.0/merkly/utils/crypto.py` & `merkly-0.6.1/merkly/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `merkly-0.6.0/merkly/utils/math.py` & `merkly-0.6.1/merkly/utils/math.py`

 * *Files identical despite different names*

### Comparing `merkly-0.6.0/pyproject.toml` & `merkly-0.6.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merkly"
-version = "0.6.0"
+version = "0.6.1"
 description = "🌳 The simple and easy implementation of Merkle Tree"
 authors = ["Lucas Oliveira <olivmath@protonmail.com>"]
 repository = "https://github.com/olivmath/merkly.git"
 documentation = "https://pypi.org/project/merkly/"
 readme = "README.md"
 license = "MIT"
 keywords = [
@@ -15,14 +15,15 @@
     "blockchain",
 ]
 
 [tool.poetry.dependencies]
     python = "^3.8"
     pysha3 = "^1.0.2"
     pydantic = "^1.10.2"
+    coverage = "^7.2.7"
 
 [tool.poetry.dev-dependencies]
     conventional-pre-commit = "^2.1.1"
     pre-commit = "^3.0.3"
     pyclean = "^2.2.0"
     pytest = "^7.2.1"
     black = "^23.1.0"
```

### Comparing `merkly-0.6.0/PKG-INFO` & `merkly-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 Metadata-Version: 2.1
 Name: merkly
-Version: 0.6.0
+Version: 0.6.1
 Summary: 🌳 The simple and easy implementation of Merkle Tree
 Home-page: https://github.com/olivmath/merkly.git
 License: MIT
 Keywords: merkle-tree,merkle-proof,merkle-root,keccak256,blockchain
 Author: Lucas Oliveira
 Author-email: olivmath@protonmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: coverage (>=7.2.7,<8.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pysha3 (>=1.0.2,<2.0.0)
 Project-URL: Documentation, https://pypi.org/project/merkly/
 Project-URL: Repository, https://github.com/olivmath/merkly.git
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://pypi.org/project/merkly/">
-    <img alt="Merkly" src="./assets/merkly-banner.png" width="1000">
+    <img alt="Merkly" src="https://raw.githubusercontent.com/olivmath/merkly/main/assets/merkly-banner.png" width="1000">
   </a>
 </p>
 
 <p align="center">The simple and easy implementation of Python Merkle Tree.</p>
 
 ---
 
 <p align="center">
     <a href="https://pypi.org/project/merkly/">
         <img src="https://img.shields.io/pypi/v/merkly">
     </a>
-    <a href="https://github.com/olivmath/merkly/actions/workflows/test.yml">
-        <img src="https://github.com/olivmath/merkly/actions/workflows/test.yml/badge.svg?branch=main">
+    <a href="https://github.com/olivmath/merkly/actions/workflows/ci.yml">
+        <img src="https://github.com/olivmath/merkly/actions/workflows/ci.yml/badge.svg?branch=main">
     </a>
     <a href="https://pypi.org/project/merkly/">
         <img src="https://img.shields.io/pypi/pyversions/merkly">
     </a>
     <a href="https://pypi.org/project/merkly/">
         <img src="https://img.shields.io/pypi/dm/merkly">
     </a>
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: merkly Version: 0.6.0 Summary: ð³ The simple and
+Metadata-Version: 2.1 Name: merkly Version: 0.6.1 Summary: ð³ The simple and
 easy implementation of Merkle Tree Home-page: https://github.com/olivmath/
 merkly.git License: MIT Keywords: merkle-tree,merkle-proof,merkle-
 root,keccak256,blockchain Author: Lucas Oliveira Author-email:
 olivmath@protonmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: pydantic
-(>=1.10.2,<2.0.0) Requires-Dist: pysha3 (>=1.0.2,<2.0.0) Project-URL:
-Documentation, https://pypi.org/project/merkly/ Project-URL: Repository, https:
-//github.com/olivmath/merkly.git Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: coverage
+(>=7.2.7,<8.0.0) Requires-Dist: pydantic (>=1.10.2,<2.0.0) Requires-Dist:
+pysha3 (>=1.0.2,<2.0.0) Project-URL: Documentation, https://pypi.org/project/
+merkly/ Project-URL: Repository, https://github.com/olivmath/merkly.git
+Description-Content-Type: text/markdown
                                    [Merkly]
            The simple and easy implementation of Python Merkle Tree.
 ---
   [https://img.shields.io/pypi/v/merkly] [https://github.com/olivmath/merkly/
-actions/workflows/test.yml/badge.svg?branch=main] [https://img.shields.io/pypi/
+ actions/workflows/ci.yml/badge.svg?branch=main] [https://img.shields.io/pypi/
      pyversions/merkly] [https://img.shields.io/pypi/dm/merkly] [https://
       img.shields.io/github/commit-activity/m/olivmath/merkly] [https://
                          img.shields.io/pypi/l/merkly]
 --- ## Table of Contents - [Credits](#credits) - [How to install](#how-to-
 install) - [How it works](#how-it-works) - [How to use](#how-to-use) -
 [Roadmap](#roadmap) - [Contributing](#contributing) - [License](#license) ##
 Credits [![GitHub Contributors Image](https://contrib.rocks/
```

