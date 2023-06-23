# Comparing `tmp/merkly-0.7.0.tar.gz` & `tmp/merkly-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merkly-0.7.0.tar", max compression
+gzip compressed data, was "merkly-0.7.1.tar", max compression
```

## Comparing `merkly-0.7.0.tar` & `merkly-0.7.1.tar`

### file list

```diff
@@ -1,9 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-06-23 18:27:46.463000 merkly-0.7.0/LICENSE
--rw-r--r--   0        0        0     4756 2023-06-23 18:27:46.463000 merkly-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-06-23 18:27:46.467000 merkly-0.7.0/merkly/__init__.py
--rw-r--r--   0        0        0     4488 2023-06-23 18:27:46.467000 merkly-0.7.0/merkly/mtree.py
--rw-r--r--   0        0        0        0 2023-06-23 18:27:46.467000 merkly-0.7.0/merkly/utils/__init__.py
--rw-r--r--   0        0        0     1511 2023-06-23 18:27:46.467000 merkly-0.7.0/merkly/utils/crypto.py
--rw-r--r--   0        0        0      664 2023-06-23 18:27:46.467000 merkly-0.7.0/merkly/utils/math.py
--rw-r--r--   0        0        0      878 2023-06-23 18:27:46.467000 merkly-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5680 1970-01-01 00:00:00.000000 merkly-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-23 19:07:33.847162 merkly-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5392 2023-06-23 19:07:33.847162 merkly-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 19:07:33.851163 merkly-0.7.1/merkly/__init__.py
+-rw-r--r--   0        0        0     4549 2023-06-23 19:07:33.851163 merkly-0.7.1/merkly/mtree.py
+-rw-r--r--   0        0        0     2769 2023-06-23 19:07:33.851163 merkly-0.7.1/merkly/utils.py
+-rw-r--r--   0        0        0      878 2023-06-23 19:07:33.851163 merkly-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 merkly-0.7.1/PKG-INFO
```

### Comparing `merkly-0.7.0/LICENSE` & `merkly-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `merkly-0.7.0/README.md` & `merkly-0.7.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -53,31 +53,53 @@
 
 ```
 pip install merkly
 ```
 
 ## How to works
 
-- _We use keccak-256 under-the-hood_
+- _We use keccak-256 under-the-hood if you dont pass your hash function_
 
 This library provides a clean and easy to use implementation of the Merkle Tree with the following features:
 
 - Create Leaf
 - Create Root
 - Create Proof
 - Verify Proof
 
 ## How to Use
 
 **Create a Merkle Tree**
 
 ```python
 from merkly.mtree import MerkleTree
+from typing import Callable
+
+# choose any hash function that is of type (str) -> str
+my_hash_function: Callable[[str], str] = lambda data: str(ord(data) * 1000)
 
 # create a Merkle Tree
+mtree = MerkleTree(['a', 'b', 'c', 'd'], my_hash_function)
+
+# show original input
+assert mtree.raw_leafs == ['a', 'b', 'c', 'd']
+
+# hashed leafs
+assert mtree.leafs == ['97000', '98000', '99000', '100000']
+
+# shorted hashed leafs
+assert mtree.short_leafs == ['9700...', '9800...', '9900...', '1000...']
+```
+
+**Create a Merkle Tree (Default: Keccak256)**
+
+```python
+from merkly.mtree import MerkleTree
+
+# create a Merkle Tree with keccak256
 mtree = MerkleTree(['a', 'b', 'c', 'd'])
 
 # show original input
 assert mtree.raw_leafs == ['a', 'b', 'c', 'd']
 
 # hashed leafs
 assert mtree.leafs == [
```

#### html2text {}

```diff
@@ -8,21 +8,29 @@
                          img.shields.io/pypi/l/merkly]
 --- ## Table of Contents - [Credits](#credits) - [How to install](#how-to-
 install) - [How it works](#how-it-works) - [How to use](#how-to-use) -
 [Roadmap](#roadmap) - [Contributing](#contributing) - [License](#license) ##
 Credits [![GitHub Contributors Image](https://contrib.rocks/
 image?repo=olivmath/merkly)](https://github.com/olivmath/merkly/graphs/
 contributors) ## How to install ``` poetry add merkly ``` ``` pip install
-merkly ``` ## How to works - _We use keccak-256 under-the-hood_ This library
-provides a clean and easy to use implementation of the Merkle Tree with the
-following features: - Create Leaf - Create Root - Create Proof - Verify Proof
-## How to Use **Create a Merkle Tree** ```python from merkly.mtree import
-MerkleTree # create a Merkle Tree mtree = MerkleTree(['a', 'b', 'c', 'd']) #
-show original input assert mtree.raw_leafs == ['a', 'b', 'c', 'd'] # hashed
-leafs assert mtree.leafs ==
+merkly ``` ## How to works - _We use keccak-256 under-the-hood if you dont pass
+your hash function_ This library provides a clean and easy to use
+implementation of the Merkle Tree with the following features: - Create Leaf -
+Create Root - Create Proof - Verify Proof ## How to Use **Create a Merkle
+Tree** ```python from merkly.mtree import MerkleTree from typing import
+Callable # choose any hash function that is of type (str) -> str
+my_hash_function: Callable[[str], str] = lambda data: str(ord(data) * 1000) #
+create a Merkle Tree mtree = MerkleTree(['a', 'b', 'c', 'd'], my_hash_function)
+# show original input assert mtree.raw_leafs == ['a', 'b', 'c', 'd'] # hashed
+leafs assert mtree.leafs == ['97000', '98000', '99000', '100000'] # shorted
+hashed leafs assert mtree.short_leafs == ['9700...', '9800...', '9900...',
+'1000...'] ``` **Create a Merkle Tree (Default: Keccak256)** ```python from
+merkly.mtree import MerkleTree # create a Merkle Tree with keccak256 mtree =
+MerkleTree(['a', 'b', 'c', 'd']) # show original input assert mtree.raw_leafs
+== ['a', 'b', 'c', 'd'] # hashed leafs assert mtree.leafs ==
 [ '3ac225168df54212a25c1c01fd35bebfea408fdac2e31ddd6f80a4bbf9a5f1cb',
 'b5553de315e0edf504d9150af82dafa5c4667fa618ed0a6f19c69b41166c5510',
 '0b42b6393c1f53060fe3ddbfcd7aadcca894465a5a438f69c87d790b2299b9b2',
 'f1918e8562236eb17adc8502332f4c9c82bc14e19bfc0aa10ab674ff75b3d2f3' ] # shorted
 hashed leafs assert mtree.short_leafs == [ '3ac2...', 'b555...', '0b42...',
 'f191...' ] ``` **Create a Root** ```python from merkly.mtree import MerkleTree
 # create a Merkle Tree mtree = MerkleTree(['a', 'b', 'c', 'd']) # get root of
```

### Comparing `merkly-0.7.0/merkly/mtree.py` & `merkly-0.7.1/merkly/mtree.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 Merkle Tree Model
 """
 
 from typing import Callable, List, Optional
 from pydantic import BaseModel
 from functools import reduce
 
-from merkly.utils.crypto import half, keccak, slice_in_pairs
-from merkly.utils.math import is_power_2
+from merkly.utils import is_power_2
+from merkly.utils import (
+    hash_function_type_checking,
+    slice_in_pairs,
+    keccak,
+    half,
+)
 
 
 class Node(BaseModel):
     """
     # 🍃 Leaf of Merkle Tree
 
     ## Args:
@@ -33,74 +38,75 @@
 
 class MerkleTree:
     """
     # 🌳 Merkle Tree implementation
 
     ## Args:
         - leafs: List of raw data
-        - concat_function (Callable[[str], str], optional): Function that hashes the data.
+        - hash_function (Callable[[str], str], optional): Function that hashes the data.
             * Defaults to `keccak` if not provided. It must have the signature (data: str) -> str.
 
     """
 
     def __init__(
-        self, leafs: List[str], concat_function: Callable[[str], str] = keccak
+        self, leafs: List[str], hash_function: Callable[[str], str] = keccak
     ) -> None:
         is_power_2(len(leafs))
-        self.concat_function: Callable[[str], str] = concat_function
+        hash_function_type_checking(hash_function)
+        self.hash_function: Callable[[str], str] = hash_function
         self.raw_leafs: List[str] = leafs
         self.leafs: List[str] = self.__hash_leafs(leafs)
         self.short_leafs: List[str] = self.short(leafs)
 
     def __hash_leafs(self, leafs: List[str]) -> List[str]:
-        return list(map(self.concat_function, leafs))
+        return list(map(self.hash_function, leafs))
 
     def __repr__(self) -> str:
         return f"""MerkleTree(\nraw_leafs: {self.raw_leafs}\nleafs: {self.leafs}\nshort_leafs: {self.short(self.leafs)})"""
 
     def short(self, data: List[str]) -> List[str]:
         return [f"{x[:4]}..." for x in data]
 
     @property
     def root(self) -> str:
         return self.make_root(self.leafs)[0]
 
     def proof(self, raw_leaf: str) -> List[Node]:
-        proof = self.make_proof(self.leafs, [], self.concat_function(raw_leaf))
+        proof = self.make_proof(self.leafs, [], self.hash_function(raw_leaf))
         proof.reverse()
         return proof
 
     def verify(self, proof: List[str], raw_leaf: str) -> bool:
-        full_proof = [self.concat_function(raw_leaf)]
+        full_proof = [self.hash_function(raw_leaf)]
         full_proof.extend(proof)
 
         def _f(_x: Node, _y: Node) -> Node:
             if not isinstance(_x, Node):
                 if _y.left is not None:
-                    return Node(left=self.concat_function(_y.left + _x))
+                    return Node(left=self.hash_function(_y.left + _x))
                 else:
-                    return Node(left=self.concat_function(_x + _y.right))
+                    return Node(left=self.hash_function(_x + _y.right))
             if _x.left is not None and _y.left is not None:
-                return Node(left=self.concat_function(_y.left + _x.left))
+                return Node(left=self.hash_function(_y.left + _x.left))
             if _x.right is not None and _y.right is not None:
-                return Node(right=self.concat_function(_x.right + _y.right))
+                return Node(right=self.hash_function(_x.right + _y.right))
 
             if _x.right is not None:
-                return Node(right=self.concat_function(_y.left + _x.right))
+                return Node(right=self.hash_function(_y.left + _x.right))
             if _x.left is not None:
-                return Node(left=self.concat_function(_x.left + _y.right))
+                return Node(left=self.hash_function(_x.left + _y.right))
 
         return reduce(_f, full_proof).left == self.root
 
     def make_root(self, leafs: List[str]) -> List[str]:
         if len(leafs) == 1:
             return leafs
 
         return self.make_root(
-            [self.concat_function(i + j) for i, j in slice_in_pairs(leafs)]
+            [self.hash_function(i + j) for i, j in slice_in_pairs(leafs)]
         )
 
     def make_proof(self, leafs: List[str], proof: List[Node], leaf: str) -> List[Node]:
         """
         # Make a proof
 
         ## Dev:
```

### Comparing `merkly-0.7.0/pyproject.toml` & `merkly-0.7.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merkly"
-version = "0.7.0"
+version = "0.7.1"
 description = "🌳 The simple and easy implementation of Merkle Tree"
 authors = ["Lucas Oliveira <olivmath@protonmail.com>"]
 repository = "https://github.com/olivmath/merkly.git"
 documentation = "https://pypi.org/project/merkly/"
 readme = "README.md"
 license = "MIT"
 keywords = [
```

### Comparing `merkly-0.7.0/PKG-INFO` & `merkly-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merkly
-Version: 0.7.0
+Version: 0.7.1
 Summary: 🌳 The simple and easy implementation of Merkle Tree
 Home-page: https://github.com/olivmath/merkly.git
 License: MIT
 Keywords: merkle-tree,merkle-proof,merkle-root,keccak256,blockchain
 Author: Lucas Oliveira
 Author-email: olivmath@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -76,31 +76,53 @@
 
 ```
 pip install merkly
 ```
 
 ## How to works
 
-- _We use keccak-256 under-the-hood_
+- _We use keccak-256 under-the-hood if you dont pass your hash function_
 
 This library provides a clean and easy to use implementation of the Merkle Tree with the following features:
 
 - Create Leaf
 - Create Root
 - Create Proof
 - Verify Proof
 
 ## How to Use
 
 **Create a Merkle Tree**
 
 ```python
 from merkly.mtree import MerkleTree
+from typing import Callable
+
+# choose any hash function that is of type (str) -> str
+my_hash_function: Callable[[str], str] = lambda data: str(ord(data) * 1000)
 
 # create a Merkle Tree
+mtree = MerkleTree(['a', 'b', 'c', 'd'], my_hash_function)
+
+# show original input
+assert mtree.raw_leafs == ['a', 'b', 'c', 'd']
+
+# hashed leafs
+assert mtree.leafs == ['97000', '98000', '99000', '100000']
+
+# shorted hashed leafs
+assert mtree.short_leafs == ['9700...', '9800...', '9900...', '1000...']
+```
+
+**Create a Merkle Tree (Default: Keccak256)**
+
+```python
+from merkly.mtree import MerkleTree
+
+# create a Merkle Tree with keccak256
 mtree = MerkleTree(['a', 'b', 'c', 'd'])
 
 # show original input
 assert mtree.raw_leafs == ['a', 'b', 'c', 'd']
 
 # hashed leafs
 assert mtree.leafs == [
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: merkly Version: 0.7.0 Summary: ð³ The simple and
+Metadata-Version: 2.1 Name: merkly Version: 0.7.1 Summary: ð³ The simple and
 easy implementation of Merkle Tree Home-page: https://github.com/olivmath/
 merkly.git License: MIT Keywords: merkle-tree,merkle-proof,merkle-
 root,keccak256,blockchain Author: Lucas Oliveira Author-email:
 olivmath@protonmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -21,21 +21,29 @@
                          img.shields.io/pypi/l/merkly]
 --- ## Table of Contents - [Credits](#credits) - [How to install](#how-to-
 install) - [How it works](#how-it-works) - [How to use](#how-to-use) -
 [Roadmap](#roadmap) - [Contributing](#contributing) - [License](#license) ##
 Credits [![GitHub Contributors Image](https://contrib.rocks/
 image?repo=olivmath/merkly)](https://github.com/olivmath/merkly/graphs/
 contributors) ## How to install ``` poetry add merkly ``` ``` pip install
-merkly ``` ## How to works - _We use keccak-256 under-the-hood_ This library
-provides a clean and easy to use implementation of the Merkle Tree with the
-following features: - Create Leaf - Create Root - Create Proof - Verify Proof
-## How to Use **Create a Merkle Tree** ```python from merkly.mtree import
-MerkleTree # create a Merkle Tree mtree = MerkleTree(['a', 'b', 'c', 'd']) #
-show original input assert mtree.raw_leafs == ['a', 'b', 'c', 'd'] # hashed
-leafs assert mtree.leafs ==
+merkly ``` ## How to works - _We use keccak-256 under-the-hood if you dont pass
+your hash function_ This library provides a clean and easy to use
+implementation of the Merkle Tree with the following features: - Create Leaf -
+Create Root - Create Proof - Verify Proof ## How to Use **Create a Merkle
+Tree** ```python from merkly.mtree import MerkleTree from typing import
+Callable # choose any hash function that is of type (str) -> str
+my_hash_function: Callable[[str], str] = lambda data: str(ord(data) * 1000) #
+create a Merkle Tree mtree = MerkleTree(['a', 'b', 'c', 'd'], my_hash_function)
+# show original input assert mtree.raw_leafs == ['a', 'b', 'c', 'd'] # hashed
+leafs assert mtree.leafs == ['97000', '98000', '99000', '100000'] # shorted
+hashed leafs assert mtree.short_leafs == ['9700...', '9800...', '9900...',
+'1000...'] ``` **Create a Merkle Tree (Default: Keccak256)** ```python from
+merkly.mtree import MerkleTree # create a Merkle Tree with keccak256 mtree =
+MerkleTree(['a', 'b', 'c', 'd']) # show original input assert mtree.raw_leafs
+== ['a', 'b', 'c', 'd'] # hashed leafs assert mtree.leafs ==
 [ '3ac225168df54212a25c1c01fd35bebfea408fdac2e31ddd6f80a4bbf9a5f1cb',
 'b5553de315e0edf504d9150af82dafa5c4667fa618ed0a6f19c69b41166c5510',
 '0b42b6393c1f53060fe3ddbfcd7aadcca894465a5a438f69c87d790b2299b9b2',
 'f1918e8562236eb17adc8502332f4c9c82bc14e19bfc0aa10ab674ff75b3d2f3' ] # shorted
 hashed leafs assert mtree.short_leafs == [ '3ac2...', 'b555...', '0b42...',
 'f191...' ] ``` **Create a Root** ```python from merkly.mtree import MerkleTree
 # create a Merkle Tree mtree = MerkleTree(['a', 'b', 'c', 'd']) # get root of
```

