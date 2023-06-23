# Comparing `tmp/merkly-0.6.1.tar.gz` & `tmp/merkly-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merkly-0.6.1.tar", max compression
+gzip compressed data, was "merkly-0.7.0.tar", max compression
```

## Comparing `merkly-0.6.1.tar` & `merkly-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-06-23 06:07:37.020355 merkly-0.6.1/LICENSE
--rw-r--r--   0        0        0     4756 2023-06-23 06:07:37.024355 merkly-0.6.1/README.md
--rw-r--r--   0        0        0        0 2023-06-23 06:07:37.024355 merkly-0.6.1/merkly/__init__.py
--rw-r--r--   0        0        0     4209 2023-06-23 06:07:37.024355 merkly-0.6.1/merkly/mtree.py
--rw-r--r--   0        0        0        0 2023-06-23 06:07:37.024355 merkly-0.6.1/merkly/utils/__init__.py
--rw-r--r--   0        0        0     1511 2023-06-23 06:07:37.024355 merkly-0.6.1/merkly/utils/crypto.py
--rw-r--r--   0        0        0      664 2023-06-23 06:07:37.024355 merkly-0.6.1/merkly/utils/math.py
--rw-r--r--   0        0        0      878 2023-06-23 06:07:37.024355 merkly-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5680 1970-01-01 00:00:00.000000 merkly-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-23 18:27:46.463000 merkly-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4756 2023-06-23 18:27:46.463000 merkly-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 18:27:46.467000 merkly-0.7.0/merkly/__init__.py
+-rw-r--r--   0        0        0     4488 2023-06-23 18:27:46.467000 merkly-0.7.0/merkly/mtree.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:27:46.467000 merkly-0.7.0/merkly/utils/__init__.py
+-rw-r--r--   0        0        0     1511 2023-06-23 18:27:46.467000 merkly-0.7.0/merkly/utils/crypto.py
+-rw-r--r--   0        0        0      664 2023-06-23 18:27:46.467000 merkly-0.7.0/merkly/utils/math.py
+-rw-r--r--   0        0        0      878 2023-06-23 18:27:46.467000 merkly-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5680 1970-01-01 00:00:00.000000 merkly-0.7.0/PKG-INFO
```

### Comparing `merkly-0.6.1/LICENSE` & `merkly-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merkly-0.6.1/README.md` & `merkly-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -142,17 +142,17 @@
 ## Roadmap
 
 | Feature                                                                                                   | Status | Priority |
 | --------------------------------------------------------------------------------------------------------- | ------ | -------- |
 | Create Root                                                                                               | ✅     | 🔥       |
 | Create Proof                                                                                              | ✅     | 🔥       |
 | Verify Proof                                                                                              | ✅     | 🔥       |
+| Use any Hash function                                                                                     | ✅     | 🧐       |
 | Support **[OpenZeppelin](https://docs.openzeppelin.com/contracts/4.x/utilities#verifying_merkle_proofs)** | ⏰     | 🔥       |
 | Compatible with **[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)**                            | ⏰     | 🔥       |
-| Use any Hash function                                                                                     | ⏰     | 🧐       |
 | Leafs of any size                                                                                         | ⏰     | 🧐       |
 
 ## Contributing
 
 - Before read a code of conduct: **[CODE_OF_CONDUCT](CODE_OF_CONDUCT.md)**
 - Follow the guide of development: **[CONTRIBUTING](CONTRIBUTING.md)**
```

#### html2text {}

```diff
@@ -34,14 +34,14 @@
 'b555...'), Node(right: '6467...') ] ``` **Verify Proof of a leaf** ```python
 from merkly.mtree import MerkleTree # create a Merkle Tree mtree = MerkleTree(
 ['a', 'b', 'c', 'd']) # get proof of a raw leaf p = mtree.proof('b') # verify
 your proof of raw leaf assert mtree.verify(p, 'b') == True ``` ## Roadmap |
 Feature | Status | Priority | | -----------------------------------------------
 ---------------------------------------------------------- | ------ | -------
 - | | Create Root | â | ð¥ | | Create Proof | â | ð¥ | | Verify Proof |
-â | ð¥ | | Support **[OpenZeppelin](https://docs.openzeppelin.com/
-contracts/4.x/utilities#verifying_merkle_proofs)** | â° | ð¥ | | Compatible
-with **[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)** | â° |
-ð¥ | | Use any Hash function | â° | ð§ | | Leafs of any size | â° | ð§
-| ## Contributing - Before read a code of conduct: **[CODE_OF_CONDUCT]
-(CODE_OF_CONDUCT.md)** - Follow the guide of development: **[CONTRIBUTING]
-(CONTRIBUTING.md)** ## License [MIT](LICENSE)
+â | ð¥ | | Use any Hash function | â | ð§ | | Support **[OpenZeppelin]
+(https://docs.openzeppelin.com/contracts/4.x/
+utilities#verifying_merkle_proofs)** | â° | ð¥ | | Compatible with **
+[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)** | â° | ð¥ | |
+Leafs of any size | â° | ð§ | ## Contributing - Before read a code of
+conduct: **[CODE_OF_CONDUCT](CODE_OF_CONDUCT.md)** - Follow the guide of
+development: **[CONTRIBUTING](CONTRIBUTING.md)** ## License [MIT](LICENSE)
```

### Comparing `merkly-0.6.1/merkly/mtree.py` & `merkly-0.7.0/merkly/mtree.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """
-# Merkle Tree model
+Merkle Tree Model
 """
-from merkly.utils.crypto import keccak, half, slice_in_pairs
-from merkly.utils.math import is_power_2
-from typing import List, Optional
+
+from typing import Callable, List, Optional
 from pydantic import BaseModel
 from functools import reduce
 
+from merkly.utils.crypto import half, keccak, slice_in_pairs
+from merkly.utils.math import is_power_2
+
 
 class Node(BaseModel):
     """
-    # 🍃 Leaf of Tree
+    # 🍃 Leaf of Merkle Tree
+
+    ## Args:
+        - left (Optional[str]): Left child node hash.
+        - right (Optional[str]): Right child node hash.
     """
 
     left: Optional[str]
     right: Optional[str]
 
     def __repr__(self) -> str:
         if self.left is None:
@@ -23,114 +29,111 @@
             return f"Node(left: {self.left[:4]}...)"
         else:
             return ""
 
 
 class MerkleTree:
     """
-    # 🌳 Merkle Tree
-    - You can pass a list of raw data
-    - They will hashed by `keccak-256`
+    # 🌳 Merkle Tree implementation
+
+    ## Args:
+        - leafs: List of raw data
+        - concat_function (Callable[[str], str], optional): Function that hashes the data.
+            * Defaults to `keccak` if not provided. It must have the signature (data: str) -> str.
+
     """
 
-    def __init__(self, leafs: List[str]) -> None:
-        is_power_2(leafs.__len__())
+    def __init__(
+        self, leafs: List[str], concat_function: Callable[[str], str] = keccak
+    ) -> None:
+        is_power_2(len(leafs))
+        self.concat_function: Callable[[str], str] = concat_function
+        self.raw_leafs: List[str] = leafs
         self.leafs: List[str] = self.__hash_leafs(leafs)
-        self.raw_leafs = leafs
-        self.short_leafs = self.short(self.leafs)
+        self.short_leafs: List[str] = self.short(leafs)
 
     def __hash_leafs(self, leafs: List[str]) -> List[str]:
-        return list(map(keccak, leafs))
+        return list(map(self.concat_function, leafs))
 
     def __repr__(self) -> str:
-        return f"""MerkleTree(
-            raw_leafs: {self.raw_leafs}
-            leafs: {self.leafs}
-            short_leafs: {self.short(self.leafs)}
-        )"""
+        return f"""MerkleTree(\nraw_leafs: {self.raw_leafs}\nleafs: {self.leafs}\nshort_leafs: {self.short(self.leafs)})"""
 
     def short(self, data: List[str]) -> List[str]:
         return [f"{x[:4]}..." for x in data]
 
     @property
     def root(self) -> str:
-        return MerkleTree.merkle_root(self.leafs)[0]
+        return self.make_root(self.leafs)[0]
 
     def proof(self, raw_leaf: str) -> List[Node]:
-        proof = MerkleTree.merkle_proof(self.leafs, [], keccak(raw_leaf))
+        proof = self.make_proof(self.leafs, [], self.concat_function(raw_leaf))
         proof.reverse()
         return proof
 
     def verify(self, proof: List[str], raw_leaf: str) -> bool:
-        full_proof = [keccak(raw_leaf)]
+        full_proof = [self.concat_function(raw_leaf)]
         full_proof.extend(proof)
 
         def _f(_x: Node, _y: Node) -> Node:
-            """
-            # f(x,y) -> Node
-            """
             if not isinstance(_x, Node):
                 if _y.left is not None:
-                    return Node(left=keccak(_y.left + _x))
+                    return Node(left=self.concat_function(_y.left + _x))
                 else:
-                    return Node(left=keccak(_x + _y.right))
+                    return Node(left=self.concat_function(_x + _y.right))
             if _x.left is not None and _y.left is not None:
-                return Node(left=keccak(_y.left + _x.left))
+                return Node(left=self.concat_function(_y.left + _x.left))
             if _x.right is not None and _y.right is not None:
-                return Node(right=keccak(_x.right + _y.right))
+                return Node(right=self.concat_function(_x.right + _y.right))
 
             if _x.right is not None:
-                return Node(right=keccak(_y.left + _x.right))
+                return Node(right=self.concat_function(_y.left + _x.right))
             if _x.left is not None:
-                return Node(left=keccak(_x.left + _y.right))
+                return Node(left=self.concat_function(_x.left + _y.right))
 
         return reduce(_f, full_proof).left == self.root
 
-    @staticmethod
-    def merkle_root(leafs: list):
-        """
-        # Merkle Root of `x: list[str]` using keccak256
-        - params `x: list[str]`
-        - return `hexadecimal: list[str]`
-
-        ```python
-        >>> merkle_root(["a", "b", "c", "d"])
-        ["159b0d5005a27c97537ff0e6d1d0d619be408a5e3f2570816b02dc5a18b74f47"]
-
-        >>> merkle_root(["a", "b"])
-        ["414e3a845393ef6d68973ddbf5bd85ff524443cf0e06a361624f3d51b879ec1c"]
-        ```
-        """
+    def make_root(self, leafs: List[str]) -> List[str]:
         if len(leafs) == 1:
             return leafs
 
-        return MerkleTree.merkle_root([keccak(i + j) for i, j in slice_in_pairs(leafs)])
+        return self.make_root(
+            [self.concat_function(i + j) for i, j in slice_in_pairs(leafs)]
+        )
 
-    @staticmethod
-    def merkle_proof(leafs: List[str], proof: List[str], leaf: str) -> list:
+    def make_proof(self, leafs: List[str], proof: List[Node], leaf: str) -> List[Node]:
         """
         # Make a proof
-        - if the `leaf` index is less than half the size of the `leafs`
+
+        ## Dev:
+            - if the `leaf` index is less than half the size of the `leafs`
         list then the right side must reach root and vice versa
+
+        ## Args:
+            - leafs: List of leafs
+            - proof: Accumulated proof
+            - leaf: Leaf for which to create the proof
+
+        ## Returns:
+            - List of Nodes representing the proof
         """
 
         try:
             index = leafs.index(leaf)
         except ValueError as err:
-            msg = f"leaf: {leaf} does not exist in the tree: {leafs}"
+            msg = f"Leaf: {leaf} does not exist in the tree: {leafs}"
             raise ValueError(msg) from err
 
         if len(leafs) == 2:
             if index == 1:
                 proof.append(Node(left=leafs[0]))
             else:
                 proof.append(Node(right=leafs[1]))
             return proof
 
         left, right = half(leafs)
 
         if index < len(leafs) / 2:
-            proof.append(Node(right=MerkleTree.merkle_root(right)[0]))
-            return MerkleTree.merkle_proof(left, proof, leaf)
+            proof.append(Node(right=self.make_root(right)[0]))
+            return self.make_proof(left, proof, leaf)
         else:
-            proof.append(Node(left=MerkleTree.merkle_root(left)[0]))
-            return MerkleTree.merkle_proof(right, proof, leaf)
+            proof.append(Node(left=self.make_root(left)[0]))
+            return self.make_proof(right, proof, leaf)
```

### Comparing `merkly-0.6.1/merkly/utils/crypto.py` & `merkly-0.7.0/merkly/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `merkly-0.6.1/merkly/utils/math.py` & `merkly-0.7.0/merkly/utils/math.py`

 * *Files identical despite different names*

### Comparing `merkly-0.6.1/pyproject.toml` & `merkly-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merkly"
-version = "0.6.1"
+version = "0.7.0"
 description = "🌳 The simple and easy implementation of Merkle Tree"
 authors = ["Lucas Oliveira <olivmath@protonmail.com>"]
 repository = "https://github.com/olivmath/merkly.git"
 documentation = "https://pypi.org/project/merkly/"
 readme = "README.md"
 license = "MIT"
 keywords = [
```

### Comparing `merkly-0.6.1/PKG-INFO` & `merkly-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merkly
-Version: 0.6.1
+Version: 0.7.0
 Summary: 🌳 The simple and easy implementation of Merkle Tree
 Home-page: https://github.com/olivmath/merkly.git
 License: MIT
 Keywords: merkle-tree,merkle-proof,merkle-root,keccak256,blockchain
 Author: Lucas Oliveira
 Author-email: olivmath@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -165,17 +165,17 @@
 ## Roadmap
 
 | Feature                                                                                                   | Status | Priority |
 | --------------------------------------------------------------------------------------------------------- | ------ | -------- |
 | Create Root                                                                                               | ✅     | 🔥       |
 | Create Proof                                                                                              | ✅     | 🔥       |
 | Verify Proof                                                                                              | ✅     | 🔥       |
+| Use any Hash function                                                                                     | ✅     | 🧐       |
 | Support **[OpenZeppelin](https://docs.openzeppelin.com/contracts/4.x/utilities#verifying_merkle_proofs)** | ⏰     | 🔥       |
 | Compatible with **[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)**                            | ⏰     | 🔥       |
-| Use any Hash function                                                                                     | ⏰     | 🧐       |
 | Leafs of any size                                                                                         | ⏰     | 🧐       |
 
 ## Contributing
 
 - Before read a code of conduct: **[CODE_OF_CONDUCT](CODE_OF_CONDUCT.md)**
 - Follow the guide of development: **[CONTRIBUTING](CONTRIBUTING.md)**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: merkly Version: 0.6.1 Summary: ð³ The simple and
+Metadata-Version: 2.1 Name: merkly Version: 0.7.0 Summary: ð³ The simple and
 easy implementation of Merkle Tree Home-page: https://github.com/olivmath/
 merkly.git License: MIT Keywords: merkle-tree,merkle-proof,merkle-
 root,keccak256,blockchain Author: Lucas Oliveira Author-email:
 olivmath@protonmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -47,14 +47,14 @@
 'b555...'), Node(right: '6467...') ] ``` **Verify Proof of a leaf** ```python
 from merkly.mtree import MerkleTree # create a Merkle Tree mtree = MerkleTree(
 ['a', 'b', 'c', 'd']) # get proof of a raw leaf p = mtree.proof('b') # verify
 your proof of raw leaf assert mtree.verify(p, 'b') == True ``` ## Roadmap |
 Feature | Status | Priority | | -----------------------------------------------
 ---------------------------------------------------------- | ------ | -------
 - | | Create Root | â | ð¥ | | Create Proof | â | ð¥ | | Verify Proof |
-â | ð¥ | | Support **[OpenZeppelin](https://docs.openzeppelin.com/
-contracts/4.x/utilities#verifying_merkle_proofs)** | â° | ð¥ | | Compatible
-with **[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)** | â° |
-ð¥ | | Use any Hash function | â° | ð§ | | Leafs of any size | â° | ð§
-| ## Contributing - Before read a code of conduct: **[CODE_OF_CONDUCT]
-(CODE_OF_CONDUCT.md)** - Follow the guide of development: **[CONTRIBUTING]
-(CONTRIBUTING.md)** ## License [MIT](LICENSE)
+â | ð¥ | | Use any Hash function | â | ð§ | | Support **[OpenZeppelin]
+(https://docs.openzeppelin.com/contracts/4.x/
+utilities#verifying_merkle_proofs)** | â° | ð¥ | | Compatible with **
+[MerkleTreeJs](https://github.com/miguelmota/merkletreejs)** | â° | ð¥ | |
+Leafs of any size | â° | ð§ | ## Contributing - Before read a code of
+conduct: **[CODE_OF_CONDUCT](CODE_OF_CONDUCT.md)** - Follow the guide of
+development: **[CONTRIBUTING](CONTRIBUTING.md)** ## License [MIT](LICENSE)
```

