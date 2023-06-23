# Comparing `tmp/merkly-0.5.2.tar.gz` & `tmp/merkly-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merkly-0.5.2.tar", max compression
+gzip compressed data, was "merkly-0.6.0.tar", max compression
```

## Comparing `merkly-0.5.2.tar` & `merkly-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1071 2022-10-16 19:08:29.494677 merkly-0.5.2/LICENSE
--rw-r--r--   0        0        0     3481 2022-10-16 19:08:29.494677 merkly-0.5.2/README.md
--rw-r--r--   0        0        0        0 2022-10-16 19:08:29.502677 merkly-0.5.2/merkly/__init__.py
--rw-r--r--   0        0        0     4843 2022-10-16 19:08:29.502677 merkly-0.5.2/merkly/mtree.py
--rw-r--r--   0        0        0        0 2022-10-16 19:08:29.502677 merkly-0.5.2/merkly/utils/__init__.py
--rw-r--r--   0        0        0     1546 2022-10-16 19:08:29.502677 merkly-0.5.2/merkly/utils/crypto.py
--rw-r--r--   0        0        0      427 2022-10-16 19:08:29.502677 merkly-0.5.2/merkly/utils/math.py
--rw-r--r--   0        0        0      846 2022-10-16 19:08:29.502677 merkly-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4597 1970-01-01 00:00:00.000000 merkly-0.5.2/setup.py
--rw-r--r--   0        0        0     4494 1970-01-01 00:00:00.000000 merkly-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-23 05:22:14.916906 merkly-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4707 2023-06-23 05:22:14.916906 merkly-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 05:22:14.916906 merkly-0.6.0/merkly/__init__.py
+-rw-r--r--   0        0        0     4209 2023-06-23 05:22:14.916906 merkly-0.6.0/merkly/mtree.py
+-rw-r--r--   0        0        0        0 2023-06-23 05:22:14.916906 merkly-0.6.0/merkly/utils/__init__.py
+-rw-r--r--   0        0        0     1511 2023-06-23 05:22:14.916906 merkly-0.6.0/merkly/utils/crypto.py
+-rw-r--r--   0        0        0      664 2023-06-23 05:22:14.916906 merkly-0.6.0/merkly/utils/math.py
+-rw-r--r--   0        0        0      854 2023-06-23 05:22:14.916906 merkly-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     5590 1970-01-01 00:00:00.000000 merkly-0.6.0/PKG-INFO
```

### Comparing `merkly-0.5.2/LICENSE` & `merkly-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merkly-0.5.2/merkly/mtree.py` & `merkly-0.6.0/merkly/mtree.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,177 +1,136 @@
 """
 # Merkle Tree model
 """
+from merkly.utils.crypto import keccak, half, slice_in_pairs
+from merkly.utils.math import is_power_2
 from typing import List, Optional
 from pydantic import BaseModel
+from functools import reduce
 
 
 class Node(BaseModel):
     """
     # 🍃 Leaf of Tree
     """
+
     left: Optional[str]
     right: Optional[str]
 
     def __repr__(self) -> str:
         if self.left is None:
-            return f"{self.right[:3]}"
+            return f"Node(right: {self.right[:4]}...)"
         elif self.right is None:
-            return f"{self.left[:3]}"
+            return f"Node(left: {self.left[:4]}...)"
         else:
             return ""
 
-class MerkleTree():
+
+class MerkleTree:
     """
     # 🌳 Merkle Tree
-    - You can passa raw data
+    - You can pass a list of raw data
     - They will hashed by `keccak-256`
     """
-    def __init__(self, leafs: List[str]) -> None:
-        """
-        # Constructor
-        - Needs a `list` of `str` with length power of 2
-        """
-        from merkly.utils.math import is_power_2
 
-        if not is_power_2(leafs.__len__()):
-            raise Exception(
-                "size of leafs should be power of 2\n" +
-                "like: 2, 4, 8, 16, 32, 64, 128..."
-            )
-        # todo: to lazy initialize
-        # todo: cache leafs
+    def __init__(self, leafs: List[str]) -> None:
+        is_power_2(leafs.__len__())
         self.leafs: List[str] = self.__hash_leafs(leafs)
         self.raw_leafs = leafs
+        self.short_leafs = self.short(self.leafs)
 
     def __hash_leafs(self, leafs: List[str]) -> List[str]:
-        """
-        # hash leafs
-        - hash each leaf
-        """
-        from merkly.utils.crypto import keccak
-
         return list(map(keccak, leafs))
 
     def __repr__(self) -> str:
-        """
-        # repr
-        """
-        return f"MerkleTree\n{self.raw_leafs}\n{self.short(self.leafs)}"
+        return f"""MerkleTree(
+            raw_leafs: {self.raw_leafs}
+            leafs: {self.leafs}
+            short_leafs: {self.short(self.leafs)}
+        )"""
 
     def short(self, data: List[str]) -> List[str]:
-        """
-        # short any list of hash
-        """
-        return [x[:3] for x in data]
+        return [f"{x[:4]}..." for x in data]
 
     @property
     def root(self) -> str:
-        """
-        # Get a root of merkle tree
-        """
-
         return MerkleTree.merkle_root(self.leafs)[0]
 
-
-    def proof(self, leaf: str) -> List[Node]:
-        """
-        # Get a proof of merkle tree
-        """
-        from merkly.utils.crypto import keccak
-
-        proof = MerkleTree.merkle_proof(self.leafs, [], keccak(leaf))
+    def proof(self, raw_leaf: str) -> List[Node]:
+        proof = MerkleTree.merkle_proof(self.leafs, [], keccak(raw_leaf))
         proof.reverse()
         return proof
 
-    def verify(self, proof: List[str]) -> bool:
-        """
-        # Verify the Merkle Proof
-        """
-        from merkly.utils.crypto import keccak
-        from functools import reduce
+    def verify(self, proof: List[str], raw_leaf: str) -> bool:
+        full_proof = [keccak(raw_leaf)]
+        full_proof.extend(proof)
 
         def _f(_x: Node, _y: Node) -> Node:
             """
             # f(x,y) -> Node
             """
+            if not isinstance(_x, Node):
+                if _y.left is not None:
+                    return Node(left=keccak(_y.left + _x))
+                else:
+                    return Node(left=keccak(_x + _y.right))
             if _x.left is not None and _y.left is not None:
                 return Node(left=keccak(_y.left + _x.left))
             if _x.right is not None and _y.right is not None:
                 return Node(right=keccak(_x.right + _y.right))
 
             if _x.right is not None:
                 return Node(right=keccak(_y.left + _x.right))
             if _x.left is not None:
                 return Node(left=keccak(_x.left + _y.right))
 
-        return reduce(_f, proof).left == self.root
+        return reduce(_f, full_proof).left == self.root
 
     @staticmethod
     def merkle_root(leafs: list):
         """
         # Merkle Root of `x: list[str]` using keccak256
-        - params `x: lsit[str]`
+        - params `x: list[str]`
         - return `hexadecimal: list[str]`
 
         ```python
         >>> merkle_root(["a", "b", "c", "d"])
         ["159b0d5005a27c97537ff0e6d1d0d619be408a5e3f2570816b02dc5a18b74f47"]
 
         >>> merkle_root(["a", "b"])
         ["414e3a845393ef6d68973ddbf5bd85ff524443cf0e06a361624f3d51b879ec1c"]
         ```
         """
-        from merkly.utils.math import is_power_2
-        from merkly.utils.crypto import keccak, slice_in_pairs
-
-        if not is_power_2(len(leafs)):
-            raise Exception(f"PARÔ, {len(leafs)}")
-
         if len(leafs) == 1:
             return leafs
 
-        return MerkleTree.merkle_root([
-            keccak(i + j) for i, j in slice_in_pairs(leafs)
-        ])
+        return MerkleTree.merkle_root([keccak(i + j) for i, j in slice_in_pairs(leafs)])
 
     @staticmethod
-    def merkle_proof(
-        leafs: List[str],
-        proof: List[str],
-        leaf: str
-    ) -> list:
+    def merkle_proof(leafs: List[str], proof: List[str], leaf: str) -> list:
         """
         # Make a proof
         - if the `leaf` index is less than half the size of the `leafs`
         list then the right side must reach root and vice versa
         """
-        from merkly.utils.crypto import half
-
-        if len(leafs) == 2:
-            proof.append(
-                Node(right=leafs[1])
-            )
-            proof.append(
-                Node(left=leafs[0])
-            )
-            return proof
 
         try:
             index = leafs.index(leaf)
         except ValueError as err:
-            raise ValueError(
-                f'leaf: {leaf} does not exist in the tree: {leafs}'
-            ) from err
+            msg = f"leaf: {leaf} does not exist in the tree: {leafs}"
+            raise ValueError(msg) from err
+
+        if len(leafs) == 2:
+            if index == 1:
+                proof.append(Node(left=leafs[0]))
+            else:
+                proof.append(Node(right=leafs[1]))
+            return proof
 
         left, right = half(leafs)
 
         if index < len(leafs) / 2:
-            proof.append(
-                Node(right=MerkleTree.merkle_root(right)[0])
-            )
+            proof.append(Node(right=MerkleTree.merkle_root(right)[0]))
             return MerkleTree.merkle_proof(left, proof, leaf)
         else:
-            proof.append(
-                Node(left=MerkleTree.merkle_root(left)[0])
-            )
+            proof.append(Node(left=MerkleTree.merkle_root(left)[0]))
             return MerkleTree.merkle_proof(right, proof, leaf)
```

### Comparing `merkly-0.5.2/merkly/utils/crypto.py` & `merkly-0.6.0/merkly/utils/crypto.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,17 +22,15 @@
     >>> keccak("bitcoin")
     "7dee6e1aa550de37364ec77e03e62ea56bf42037b8297280de9d844d88444e4d"
 
     >>> keccak("ethereum")
     "541111248b45b7a8dc3f5579f630e74cb01456ea6ac067d3f4d793245a255155"
     ```
     """
-    return keccak_256(
-        data.encode()
-    ).hexdigest()
+    return keccak_256(data.encode()).hexdigest()
 
 
 def half(list_item: List[int]) -> Tuple[int, int]:
     """
     # Slice a `x: list[int]` in a pairs
     - params `x: list[int]`
     - return `list: list[list[int]]
@@ -62,11 +60,8 @@
     [[1, 2], [3, 4]]
 
     >>> slicer([i for i in range(10)])
     [[0, 1], [2, 3], [4, 5], [6, 7], [8, 9]]
     ```
     """
 
-    return [
-        list_item[i: i + 2]
-        for i in range(0, len(list_item), 2)
-    ]
+    return [list_item[i : i + 2] for i in range(0, len(list_item), 2)]
```

### Comparing `merkly-0.5.2/PKG-INFO` & `merkly-0.6.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d65 726b  : 2.1.Name: merk
-00000020: 6c79 0a56 6572 7369 6f6e 3a20 302e 352e  ly.Version: 0.5.
-00000030: 320a 5375 6d6d 6172 793a 20f0 9f8c b320  2.Summary: .... 
+00000020: 6c79 0a56 6572 7369 6f6e 3a20 302e 362e  ly.Version: 0.6.
+00000030: 300a 5375 6d6d 6172 793a 20f0 9f8c b320  0.Summary: .... 
 00000040: 5468 6520 7369 6d70 6c65 2061 6e64 2065  The simple and e
 00000050: 6173 7920 696d 706c 656d 656e 7461 7469  asy implementati
 00000060: 6f6e 206f 6620 4d65 726b 6c65 2054 7265  on of Merkle Tre
 00000070: 650a 486f 6d65 2d70 6167 653a 2068 7474  e.Home-page: htt
 00000080: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000090: 6f6c 6976 6d61 7468 2f6d 6572 6b6c 792e  olivmath/merkly.
 000000a0: 6769 740a 4c69 6365 6e73 653a 204d 4954  git.License: MIT
@@ -14,268 +14,337 @@
 000000d0: 6f6f 662c 6d65 726b 6c65 2d72 6f6f 742c  oof,merkle-root,
 000000e0: 6b65 6363 616b 3235 362c 626c 6f63 6b63  keccak256,blockc
 000000f0: 6861 696e 0a41 7574 686f 723a 204c 7563  hain.Author: Luc
 00000100: 6173 204f 6c69 7665 6972 610a 4175 7468  as Oliveira.Auth
 00000110: 6f72 2d65 6d61 696c 3a20 6f6c 6976 6d61  or-email: olivma
 00000120: 7468 4070 726f 746f 6e6d 6169 6c2e 636f  th@protonmail.co
 00000130: 6d0a 5265 7175 6972 6573 2d50 7974 686f  m.Requires-Pytho
-00000140: 6e3a 203e 3d33 2e37 2e32 2c3c 342e 302e  n: >=3.7.2,<4.0.
-00000150: 300a 436c 6173 7369 6669 6572 3a20 4c69  0.Classifier: Li
-00000160: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-00000170: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-00000180: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
-00000190: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000001a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001b0: 3a3a 2033 0a43 6c61 7373 6966 6965 723a  :: 3.Classifier:
-000001c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000001d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001e0: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
-000001f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000200: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000210: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
-00000220: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000230: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000240: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
-00000250: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-00000260: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000270: 5079 7468 6f6e 203a 3a20 332e 3131 0a52  Python :: 3.11.R
-00000280: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-00000290: 6461 6e74 6963 2028 3e3d 312e 3130 2e32  dantic (>=1.10.2
-000002a0: 2c3c 322e 302e 3029 0a52 6571 7569 7265  ,<2.0.0).Require
-000002b0: 732d 4469 7374 3a20 7079 6c69 6e74 2028  s-Dist: pylint (
-000002c0: 3e3d 322e 3134 2e35 2c3c 332e 302e 3029  >=2.14.5,<3.0.0)
-000002d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000002e0: 7079 7368 6133 2028 3e3d 312e 302e 322c  pysha3 (>=1.0.2,
-000002f0: 3c32 2e30 2e30 290a 5265 7175 6972 6573  <2.0.0).Requires
-00000300: 2d44 6973 743a 2070 7974 6573 742d 7761  -Dist: pytest-wa
-00000310: 7463 6865 7220 283e 3d30 2e32 2e33 2c3c  tcher (>=0.2.3,<
-00000320: 302e 332e 3029 0a52 6571 7569 7265 732d  0.3.0).Requires-
-00000330: 4469 7374 3a20 7269 6368 2028 3e3d 3132  Dist: rich (>=12
-00000340: 2e36 2e30 2c3c 3133 2e30 2e30 290a 5072  .6.0,<13.0.0).Pr
-00000350: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
-00000360: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
-00000370: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00000380: 6374 2f6d 6572 6b6c 792f 0a50 726f 6a65  ct/merkly/.Proje
-00000390: 6374 2d55 524c 3a20 5265 706f 7369 746f  ct-URL: Reposito
-000003a0: 7279 2c20 6874 7470 733a 2f2f 6769 7468  ry, https://gith
-000003b0: 7562 2e63 6f6d 2f6f 6c69 766d 6174 682f  ub.com/olivmath/
-000003c0: 6d65 726b 6c79 2e67 6974 0a44 6573 6372  merkly.git.Descr
-000003d0: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-000003e0: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
-000003f0: 776e 0a0a 2320 f09f 8cb3 204d 6572 6b6c  wn..# .... Merkl
-00000400: 790a 0a54 6865 202a 2a73 696d 706c 6520  y..The **simple 
-00000410: 616e 6420 6561 7379 2a2a 2069 6d70 6c65  and easy** imple
-00000420: 6d65 6e74 6174 696f 6e20 6f66 202a 2a50  mentation of **P
-00000430: 7974 686f 6e20 4d65 726b 6c65 2054 7265  ython Merkle Tre
-00000440: 652a 2a0a 0a2d 2d2d 0a0a 5b21 5b43 6f64  e**..---..[![Cod
-00000450: 6551 4c5d 2868 7474 7073 3a2f 2f67 6974  eQL](https://git
-00000460: 6875 622e 636f 6d2f 6f6c 6976 6d61 7468  hub.com/olivmath
-00000470: 2f6d 6572 6b6c 792f 6163 7469 6f6e 732f  /merkly/actions/
-00000480: 776f 726b 666c 6f77 732f 636f 6465 716c  workflows/codeql
-00000490: 2d61 6e61 6c79 7369 732e 796d 6c2f 6261  -analysis.yml/ba
-000004a0: 6467 652e 7376 6729 5d28 6874 7470 733a  dge.svg)](https:
-000004b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 6c69  //github.com/oli
-000004c0: 766d 6174 682f 6d65 726b 6c79 2f61 6374  vmath/merkly/act
-000004d0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f63  ions/workflows/c
-000004e0: 6f64 6571 6c2d 616e 616c 7973 6973 2e79  odeql-analysis.y
-000004f0: 6d6c 290a 5b21 5b4c 696e 745d 2868 7474  ml).[![Lint](htt
-00000500: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000510: 6f6c 6976 6d61 7468 2f6d 6572 6b6c 792f  olivmath/merkly/
-00000520: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000530: 732f 6c69 6e74 2e79 6d6c 2f62 6164 6765  s/lint.yml/badge
-00000540: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000550: 6974 6875 622e 636f 6d2f 6f6c 6976 6d61  ithub.com/olivma
-00000560: 7468 2f6d 6572 6b6c 792f 6163 7469 6f6e  th/merkly/action
-00000570: 732f 776f 726b 666c 6f77 732f 6c69 6e74  s/workflows/lint
-00000580: 2e79 6d6c 290a 5b21 5b54 6573 745d 2868  .yml).[![Test](h
-00000590: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000005a0: 6d2f 6f6c 6976 6d61 7468 2f6d 6572 6b6c  m/olivmath/merkl
-000005b0: 792f 6163 7469 6f6e 732f 776f 726b 666c  y/actions/workfl
-000005c0: 6f77 732f 7465 7374 2e79 6d6c 2f62 6164  ows/test.yml/bad
-000005d0: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
-000005e0: 696e 295d 2868 7474 7073 3a2f 2f67 6974  in)](https://git
-000005f0: 6875 622e 636f 6d2f 6f6c 6976 6d61 7468  hub.com/olivmath
-00000600: 2f6d 6572 6b6c 792f 6163 7469 6f6e 732f  /merkly/actions/
-00000610: 776f 726b 666c 6f77 732f 7465 7374 2e79  workflows/test.y
-00000620: 6d6c 290a 5b21 5b50 7950 495d 2868 7474  ml).[![PyPI](htt
-00000630: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000640: 2e69 6f2f 7079 7069 2f76 2f6d 6572 6b6c  .io/pypi/v/merkl
-00000650: 7929 5d28 6874 7470 733a 2f2f 7079 7069  y)](https://pypi
-00000660: 2e6f 7267 2f70 726f 6a65 6374 2f6d 6572  .org/project/mer
-00000670: 6b6c 792f 290a 0a21 5b47 6974 4875 6220  kly/)..![GitHub 
-00000680: 6c61 7374 2063 6f6d 6d69 745d 2868 7474  last commit](htt
-00000690: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000006a0: 2e69 6f2f 6769 7468 7562 2f6c 6173 742d  .io/github/last-
-000006b0: 636f 6d6d 6974 2f6f 6c69 766d 6174 682f  commit/olivmath/
-000006c0: 6d65 726b 6c79 290a 215b 4769 7448 7562  merkly).![GitHub
-000006d0: 2063 6f6d 6d69 7420 6163 7469 7669 7479   commit activity
-000006e0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000140: 6e3a 203e 3d33 2e38 2c3c 342e 300a 436c  n: >=3.8,<4.0.Cl
+00000150: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+00000160: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000170: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+00000180: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+00000190: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001a0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001b0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000001c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001e0: 2e38 0a43 6c61 7373 6966 6965 723a 2050  .8.Classifier: P
+000001f0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000200: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000210: 2033 2e39 0a43 6c61 7373 6966 6965 723a   3.9.Classifier:
+00000220: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000230: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000240: 3a3a 2033 2e31 300a 436c 6173 7369 6669  :: 3.10.Classifi
+00000250: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000260: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000270: 6f6e 203a 3a20 332e 3131 0a52 6571 7569  on :: 3.11.Requi
+00000280: 7265 732d 4469 7374 3a20 7079 6461 6e74  res-Dist: pydant
+00000290: 6963 2028 3e3d 312e 3130 2e32 2c3c 322e  ic (>=1.10.2,<2.
+000002a0: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
+000002b0: 7374 3a20 7079 7368 6133 2028 3e3d 312e  st: pysha3 (>=1.
+000002c0: 302e 322c 3c32 2e30 2e30 290a 5072 6f6a  0.2,<2.0.0).Proj
+000002d0: 6563 742d 5552 4c3a 2044 6f63 756d 656e  ect-URL: Documen
+000002e0: 7461 7469 6f6e 2c20 6874 7470 733a 2f2f  tation, https://
+000002f0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000300: 2f6d 6572 6b6c 792f 0a50 726f 6a65 6374  /merkly/.Project
+00000310: 2d55 524c 3a20 5265 706f 7369 746f 7279  -URL: Repository
+00000320: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
+00000330: 2e63 6f6d 2f6f 6c69 766d 6174 682f 6d65  .com/olivmath/me
+00000340: 726b 6c79 2e67 6974 0a44 6573 6372 6970  rkly.git.Descrip
+00000350: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00000360: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00000370: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000380: 6572 223e 0a20 203c 6120 6872 6566 3d22  er">.  <a href="
+00000390: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+000003a0: 2f70 726f 6a65 6374 2f6d 6572 6b6c 792f  /project/merkly/
+000003b0: 223e 0a20 2020 203c 696d 6720 616c 743d  ">.    <img alt=
+000003c0: 224d 6572 6b6c 7922 2073 7263 3d22 2e2f  "Merkly" src="./
+000003d0: 6173 7365 7473 2f6d 6572 6b6c 792d 6261  assets/merkly-ba
+000003e0: 6e6e 6572 2e70 6e67 2220 7769 6474 683d  nner.png" width=
+000003f0: 2231 3030 3022 3e0a 2020 3c2f 613e 0a3c  "1000">.  </a>.<
+00000400: 2f70 3e0a 0a3c 7020 616c 6967 6e3d 2263  /p>..<p align="c
+00000410: 656e 7465 7222 3e54 6865 2073 696d 706c  enter">The simpl
+00000420: 6520 616e 6420 6561 7379 2069 6d70 6c65  e and easy imple
+00000430: 6d65 6e74 6174 696f 6e20 6f66 2050 7974  mentation of Pyt
+00000440: 686f 6e20 4d65 726b 6c65 2054 7265 652e  hon Merkle Tree.
+00000450: 3c2f 703e 0a0a 2d2d 2d0a 0a3c 7020 616c  </p>..---..<p al
+00000460: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000470: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000480: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000490: 6563 742f 6d65 726b 6c79 2f22 3e0a 2020  ect/merkly/">.  
+000004a0: 2020 2020 2020 3c69 6d67 2073 7263 3d22        <img src="
+000004b0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000004c0: 6c64 732e 696f 2f70 7970 692f 762f 6d65  lds.io/pypi/v/me
+000004d0: 726b 6c79 223e 0a20 2020 203c 2f61 3e0a  rkly">.    </a>.
+000004e0: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+000004f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000500: 6f6c 6976 6d61 7468 2f6d 6572 6b6c 792f  olivmath/merkly/
+00000510: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000520: 732f 7465 7374 2e79 6d6c 223e 0a20 2020  s/test.yml">.   
+00000530: 2020 2020 203c 696d 6720 7372 633d 2268       <img src="h
+00000540: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000550: 6d2f 6f6c 6976 6d61 7468 2f6d 6572 6b6c  m/olivmath/merkl
+00000560: 792f 6163 7469 6f6e 732f 776f 726b 666c  y/actions/workfl
+00000570: 6f77 732f 7465 7374 2e79 6d6c 2f62 6164  ows/test.yml/bad
+00000580: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
+00000590: 696e 223e 0a20 2020 203c 2f61 3e0a 2020  in">.    </a>.  
+000005a0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000005b0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+000005c0: 6563 742f 6d65 726b 6c79 2f22 3e0a 2020  ect/merkly/">.  
+000005d0: 2020 2020 2020 3c69 6d67 2073 7263 3d22        <img src="
+000005e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000005f0: 6c64 732e 696f 2f70 7970 692f 7079 7665  lds.io/pypi/pyve
+00000600: 7273 696f 6e73 2f6d 6572 6b6c 7922 3e0a  rsions/merkly">.
+00000610: 2020 2020 3c2f 613e 0a20 2020 203c 6120      </a>.    <a 
+00000620: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
+00000630: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6d  pi.org/project/m
+00000640: 6572 6b6c 792f 223e 0a20 2020 2020 2020  erkly/">.       
+00000650: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000660: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000670: 6f2f 7079 7069 2f64 6d2f 6d65 726b 6c79  o/pypi/dm/merkly
+00000680: 223e 0a20 2020 203c 2f61 3e0a 2020 2020  ">.    </a>.    
+00000690: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000006a0: 2f67 6974 6875 622e 636f 6d2f 6f6c 6976  /github.com/oliv
+000006b0: 6d61 7468 2f6d 6572 6b6c 792f 6772 6170  math/merkly/grap
+000006c0: 6873 2f63 6f64 652d 6672 6571 7565 6e63  hs/code-frequenc
+000006d0: 7922 3e0a 2020 2020 3c69 6d67 2073 7263  y">.    <img src
+000006e0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
 000006f0: 6965 6c64 732e 696f 2f67 6974 6875 622f  ields.io/github/
 00000700: 636f 6d6d 6974 2d61 6374 6976 6974 792f  commit-activity/
 00000710: 6d2f 6f6c 6976 6d61 7468 2f6d 6572 6b6c  m/olivmath/merkl
-00000720: 7929 0a5b 215b 5079 5049 202d 2050 7974  y).[![PyPI - Pyt
-00000730: 686f 6e20 5665 7273 696f 6e5d 2868 7474  hon Version](htt
-00000740: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000750: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
-00000760: 6f6e 732f 6d65 726b 6c79 295d 2868 7474  ons/merkly)](htt
-00000770: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00000780: 6f6a 6563 742f 6d65 726b 6c79 2f29 0a5b  oject/merkly/).[
-00000790: 215b 5079 5049 202d 2044 6f77 6e6c 6f61  ![PyPI - Downloa
-000007a0: 6473 5d28 6874 7470 733a 2f2f 696d 672e  ds](https://img.
-000007b0: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-000007c0: 646d 2f6d 6572 6b6c 7929 5d28 6874 7470  dm/merkly)](http
-000007d0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000007e0: 6a65 6374 2f6d 6572 6b6c 792f 290a 215b  ject/merkly/).![
-000007f0: 5079 5049 202d 204c 6963 656e 7365 5d28  PyPI - License](
-00000800: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000810: 6c64 732e 696f 2f70 7970 692f 6c2f 6d65  lds.io/pypi/l/me
-00000820: 726b 6c79 290a 0a23 2320 5461 626c 6520  rkly)..## Table 
-00000830: 6f66 2043 6f6e 7465 6e74 730a 0a2d 205b  of Contents..- [
-00000840: 4372 6564 6974 735d 2823 6372 6564 6974  Credits](#credit
-00000850: 7329 0a2d 205b 486f 7720 746f 2069 6e73  s).- [How to ins
-00000860: 7461 6c6c 5d28 2368 6f77 2d74 6f2d 696e  tall](#how-to-in
-00000870: 7374 616c 6c29 0a2d 205b 486f 7720 6974  stall).- [How it
-00000880: 2077 6f72 6b73 5d28 2368 6f77 2d69 742d   works](#how-it-
-00000890: 776f 726b 7329 0a2d 205b 486f 7720 746f  works).- [How to
-000008a0: 2075 7365 5d28 2368 6f77 2d74 6f2d 7573   use](#how-to-us
-000008b0: 6529 0a2d 205b 526f 6164 6d61 705d 2823  e).- [Roadmap](#
-000008c0: 726f 6164 6d61 7029 0a2d 205b 436f 6e74  roadmap).- [Cont
-000008d0: 7269 6275 7469 6e67 5d28 2363 6f6e 7472  ributing](#contr
-000008e0: 6962 7574 696e 6729 0a2d 205b 4c69 6365  ibuting).- [Lice
-000008f0: 6e73 655d 2823 6c69 6365 6e73 6529 0a0a  nse](#license)..
-00000900: 2323 2043 7265 6469 7473 0a0a 5b21 5b47  ## Credits..[![G
-00000910: 6974 4875 6220 436f 6e74 7269 6275 746f  itHub Contributo
-00000920: 7273 2049 6d61 6765 5d28 6874 7470 733a  rs Image](https:
-00000930: 2f2f 636f 6e74 7269 622e 726f 636b 732f  //contrib.rocks/
-00000940: 696d 6167 653f 7265 706f 3d6f 6c69 766d  image?repo=olivm
-00000950: 6174 682f 6d65 726b 6c79 295d 2868 7474  ath/merkly)](htt
-00000960: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000970: 6f6c 6976 6d61 7468 2f6d 6572 6b6c 792f  olivmath/merkly/
-00000980: 6772 6170 6873 2f63 6f6e 7472 6962 7574  graphs/contribut
-00000990: 6f72 7329 0a0a 2323 2048 6f77 2074 6f20  ors)..## How to 
-000009a0: 696e 7374 616c 6c0a 0a60 6060 0a70 6f65  install..```.poe
-000009b0: 7472 7920 6164 6420 6d65 726b 6c79 0a60  try add merkly.`
-000009c0: 6060 0a0a 6060 600a 7069 7020 696e 7374  ``..```.pip inst
-000009d0: 616c 6c20 6d65 726b 6c79 0a60 6060 0a0a  all merkly.```..
-000009e0: 2323 2048 6f77 2074 6f20 776f 726b 730a  ## How to works.
-000009f0: 0a2d 202a 5765 2075 7365 206b 6563 6361  .- *We use kecca
-00000a00: 6b2d 3235 3620 756e 6465 722d 7468 652d  k-256 under-the-
-00000a10: 686f 6f64 2a0a 0a54 6869 7320 6c69 6272  hood*..This libr
-00000a20: 6172 7920 7072 6f76 6964 6573 2061 2063  ary provides a c
-00000a30: 6c65 616e 2061 6e64 2065 6173 7920 746f  lean and easy to
-00000a40: 2075 7365 2069 6d70 6c65 6d65 6e74 6174   use implementat
-00000a50: 696f 6e20 6f66 2074 6865 204d 6572 6b6c  ion of the Merkl
-00000a60: 6520 5472 6565 2077 6974 6820 7468 6520  e Tree with the 
-00000a70: 666f 6c6c 6f77 696e 6720 6665 6174 7572  following featur
-00000a80: 6573 3a0a 0a2d 2043 7265 6174 6520 4c65  es:..- Create Le
-00000a90: 6166 0a2d 2043 7265 6174 6520 526f 6f74  af.- Create Root
-00000aa0: 0a2d 2043 7265 6174 6520 5072 6f6f 660a  .- Create Proof.
-00000ab0: 2d20 5665 7269 6679 2050 726f 6f66 0a0a  - Verify Proof..
-00000ac0: 3c69 6d67 2077 6964 7468 3d22 3232 3136  <img width="2216
-00000ad0: 2220 616c 743d 226d 6572 6b6c 652d 7472  " alt="merkle-tr
-00000ae0: 6565 2220 7372 633d 2268 7474 7073 3a2f  ee" src="https:/
-00000af0: 2f75 7365 722d 696d 6167 6573 2e67 6974  /user-images.git
-00000b00: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000b10: 6f6d 2f35 3030 3337 3536 372f 3139 3336  om/50037567/1936
-00000b20: 3233 3031 332d 3363 3238 3838 6431 2d34  23013-3c2888d1-4
-00000b30: 3431 662d 3435 6131 2d39 3766 652d 3665  41f-45a1-97fe-6e
-00000b40: 3237 3565 6464 6538 3437 2e70 6e67 223e  275edde847.png">
-00000b50: 0a0a 0a23 2320 486f 7720 746f 2055 7365  ...## How to Use
-00000b60: 0a0a 2a2a 4372 6561 7465 2061 204d 6572  ..**Create a Mer
-00000b70: 6b6c 6520 5472 6565 2a2a 0a0a 6060 6070  kle Tree**..```p
-00000b80: 7974 686f 6e0a 6672 6f6d 206d 6572 6b6c  ython.from merkl
-00000b90: 792e 6d74 7265 6520 696d 706f 7274 204d  y.mtree import M
-00000ba0: 6572 6b6c 6554 7265 650a 0a23 2063 7265  erkleTree..# cre
-00000bb0: 6174 6520 6120 4d65 726b 6c65 2054 7265  ate a Merkle Tre
-00000bc0: 650a 6d74 7265 6520 3d20 4d65 726b 6c65  e.mtree = Merkle
-00000bd0: 5472 6565 285b 2761 272c 2027 6227 2c20  Tree(['a', 'b', 
-00000be0: 2763 272c 2027 6427 5d0a 0a23 2073 686f  'c', 'd']..# sho
-00000bf0: 7720 6f72 6967 696e 616c 2069 6e70 7574  w original input
-00000c00: 0a61 7373 6572 7420 6d74 7265 652e 7261  .assert mtree.ra
-00000c10: 775f 6c65 6166 7320 3d3d 205b 2761 272c  w_leafs == ['a',
-00000c20: 2027 6227 2c20 2763 272c 2027 6427 5d0a   'b', 'c', 'd'].
-00000c30: 0a23 2073 686f 7720 6c65 6166 7320 0a61  .# show leafs .a
-00000c40: 7373 6572 7420 6d74 7265 652e 6c65 6166  ssert mtree.leaf
-00000c50: 7320 3d3d 205b 5d0a 6060 600a 0a0a 2a2a  s == [].```...**
-00000c60: 4372 6561 7465 2061 2052 6f6f 742a 2a0a  Create a Root**.
-00000c70: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
-00000c80: 6d65 726b 6c79 2e6d 7472 6565 2069 6d70  merkly.mtree imp
-00000c90: 6f72 7420 4d65 726b 6c65 5472 6565 0a0a  ort MerkleTree..
-00000ca0: 2320 6372 6561 7465 2061 204d 6572 6b6c  # create a Merkl
-00000cb0: 6520 5472 6565 0a6d 7472 6565 203d 204d  e Tree.mtree = M
-00000cc0: 6572 6b6c 6554 7265 6528 5b27 6127 2c20  erkleTree(['a', 
-00000cd0: 2762 272c 2027 6327 2c20 2764 275d 290a  'b', 'c', 'd']).
-00000ce0: 0a23 2067 6574 2072 6f6f 7420 6f66 2074  .# get root of t
-00000cf0: 7265 650a 6173 7365 7274 206d 7472 6565  ree.assert mtree
-00000d00: 2e72 6f6f 7420 3d3d 2022 220a 6060 600a  .root == "".```.
-00000d10: 0a2a 2a43 7265 6174 6520 5072 6f6f 6620  .**Create Proof 
-00000d20: 6f66 2061 206c 6561 662a 2a0a 6060 6070  of a leaf**.```p
-00000d30: 7974 686f 6e0a 6672 6f6d 206d 6572 6b6c  ython.from merkl
-00000d40: 792e 6d74 7265 6520 696d 706f 7274 204d  y.mtree import M
-00000d50: 6572 6b6c 6554 7265 650a 0a23 2063 7265  erkleTree..# cre
-00000d60: 6174 6520 6120 4d65 726b 6c65 2054 7265  ate a Merkle Tre
-00000d70: 650a 6d74 7265 6520 3d20 4d65 726b 6c65  e.mtree = Merkle
-00000d80: 5472 6565 285b 2761 272c 2027 6227 2c20  Tree(['a', 'b', 
-00000d90: 2763 272c 2027 6427 5d29 0a0a 2320 6765  'c', 'd'])..# ge
-00000da0: 7420 7072 6f6f 6620 6f66 2061 206c 6561  t proof of a lea
-00000db0: 660a 6173 7365 7274 206d 7472 6565 2e70  f.assert mtree.p
-00000dc0: 726f 6f66 2822 6222 2920 3d3d 205b 5d0a  roof("b") == [].
-00000dd0: 6060 600a 0a2a 2a56 6572 6966 7920 5072  ```..**Verify Pr
-00000de0: 6f6f 6620 6f66 2061 206c 6561 662a 2a0a  oof of a leaf**.
-00000df0: 6060 6070 7974 686f 6e0a 6672 6f6d 206d  ```python.from m
-00000e00: 6572 6b6c 792e 6d74 7265 6520 696d 706f  erkly.mtree impo
-00000e10: 7274 204d 6572 6b6c 6554 7265 650a 0a23  rt MerkleTree..#
-00000e20: 2063 7265 6174 6520 6120 4d65 726b 6c65   create a Merkle
-00000e30: 2054 7265 650a 6d74 7265 6520 3d20 4d65   Tree.mtree = Me
-00000e40: 726b 6c65 5472 6565 285b 2761 272c 2027  rkleTree(['a', '
-00000e50: 6227 2c20 2763 272c 2027 6427 5d29 0a0a  b', 'c', 'd'])..
-00000e60: 2320 6765 7420 7072 6f6f 6620 6f66 2061  # get proof of a
-00000e70: 206c 6561 660a 7020 3d20 6d74 7265 652e   leaf.p = mtree.
-00000e80: 7072 6f6f 6628 2262 2229 0a0a 2320 7665  proof("b")..# ve
-00000e90: 7269 6679 2079 6f75 7220 7072 6f6f 660a  rify your proof.
-00000ea0: 6173 7365 7274 206d 7472 6565 2e76 6572  assert mtree.ver
-00000eb0: 6966 7928 7029 203d 3d20 5472 7565 0a60  ify(p) == True.`
-00000ec0: 6060 0a0a 0a23 2320 526f 6164 6d61 700a  ``...## Roadmap.
-00000ed0: 0a7c 2046 6561 7475 7265 207c 2053 7461  .| Feature | Sta
-00000ee0: 7475 7320 7c20 5072 696f 7269 7479 207c  tus | Priority |
-00000ef0: 0a7c 2d7c 2d7c 2d7c 0a7c 2043 7265 6174  .|-|-|-|.| Creat
-00000f00: 6520 526f 6f74 207c 20e2 9c85 207c 20f0  e Root | ... | .
-00000f10: 9f94 a520 7c0a 7c20 4372 6561 7465 2050  ... |.| Create P
-00000f20: 726f 6f66 207c 20e2 9c85 207c 20f0 9f94  roof | ... | ...
-00000f30: a520 7c0a 7c20 5665 7269 6679 2050 726f  . |.| Verify Pro
-00000f40: 6f66 207c 20e2 9c85 207c 20f0 9f94 a520  of | ... | .... 
-00000f50: 7c0a 7c20 5375 7070 6f72 7420 2a2a 5b4f  |.| Support **[O
-00000f60: 7065 6e5a 6570 7065 6c69 6e5d 2868 7474  penZeppelin](htt
-00000f70: 7073 3a2f 2f64 6f63 732e 6f70 656e 7a65  ps://docs.openze
-00000f80: 7070 656c 696e 2e63 6f6d 2f63 6f6e 7472  ppelin.com/contr
-00000f90: 6163 7473 2f34 2e78 2f75 7469 6c69 7469  acts/4.x/utiliti
-00000fa0: 6573 2376 6572 6966 7969 6e67 5f6d 6572  es#verifying_mer
-00000fb0: 6b6c 655f 7072 6f6f 6673 292a 2a20 7c20  kle_proofs)** | 
-00000fc0: e28f b020 7c20 f09f 94a5 207c 0a7c 2043  ... | .... |.| C
-00000fd0: 6f6d 7061 7469 626c 6520 7769 7468 202a  ompatible with *
-00000fe0: 2a5b 4d65 726b 6c65 5472 6565 4a73 5d28  *[MerkleTreeJs](
-00000ff0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001000: 6f6d 2f6d 6967 7565 6c6d 6f74 612f 6d65  om/miguelmota/me
-00001010: 726b 6c65 7472 6565 6a73 292a 2a20 7c20  rkletreejs)** | 
-00001020: e28f b020 7c20 f09f 94a5 207c 0a7c 2055  ... | .... |.| U
-00001030: 7365 2061 6e79 2048 6173 6820 6675 6e63  se any Hash func
-00001040: 7469 6f6e 207c 20e2 8fb0 207c 20f0 9fa7  tion | ... | ...
-00001050: 9020 7c0a 7c20 4c65 6166 7320 6f66 2061  . |.| Leafs of a
-00001060: 6e79 2073 697a 6520 7c20 e28f b020 7c20  ny size | ... | 
-00001070: f09f a790 207c 0a0a 2323 2043 6f6e 7472  .... |..## Contr
-00001080: 6962 7574 696e 670a 0a2d 2042 6566 6f72  ibuting..- Befor
-00001090: 6520 7265 6164 2061 2063 6f64 6520 6f66  e read a code of
-000010a0: 2063 6f6e 6475 6374 3a20 2a2a 5b43 4f44   conduct: **[COD
-000010b0: 455f 4f46 5f43 4f4e 4455 4354 5d28 434f  E_OF_CONDUCT](CO
-000010c0: 4445 5f4f 465f 434f 4e44 5543 542e 6d64  DE_OF_CONDUCT.md
-000010d0: 292a 2a0a 2d20 466f 6c6c 6f77 2074 6865  )**.- Follow the
-000010e0: 2067 7569 6465 206f 6620 6465 7665 6c6f   guide of develo
-000010f0: 706d 656e 743a 202a 2a5b 434f 4e54 5249  pment: **[CONTRI
-00001100: 4255 5449 4e47 5d28 434f 4e54 5249 4255  BUTING](CONTRIBU
-00001110: 5449 4e47 2e6d 6429 2a2a 0a0a 2323 204c  TING.md)**..## L
-00001120: 6963 656e 7365 0a0a 5b4d 4954 5d28 4c49  icense..[MIT](LI
-00001130: 4345 4e53 4529 0a0a 3c21 2d2d 2068 7474  CENSE)..<!-- htt
-00001140: 7073 3a2f 2f6d 6174 682e 6d69 742e 6564  ps://math.mit.ed
-00001150: 752f 7265 7365 6172 6368 2f68 6967 6873  u/research/highs
-00001160: 6368 6f6f 6c2f 7072 696d 6573 2f6d 6174  chool/primes/mat
-00001170: 6572 6961 6c73 2f32 3031 382f 4b75 737a  erials/2018/Kusz
-00001180: 6d61 756c 2e70 6466 202d 2d3e 0a0a       maul.pdf -->..
+00000720: 7922 3e0a 2020 2020 3c2f 613e 0a20 2020  y">.    </a>.   
+00000730: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000740: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 6c69  //github.com/oli
+00000750: 766d 6174 682f 6d65 726b 6c79 2f62 6c6f  vmath/merkly/blo
+00000760: 622f 6d61 696e 2f4c 4943 454e 5345 223e  b/main/LICENSE">
+00000770: 0a20 2020 2020 2020 203c 696d 6720 7372  .        <img sr
+00000780: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000790: 6869 656c 6473 2e69 6f2f 7079 7069 2f6c  hields.io/pypi/l
+000007a0: 2f6d 6572 6b6c 7922 3e0a 2020 2020 3c2f  /merkly">.    </
+000007b0: 613e 0a3c 2f70 3e0a 0a2d 2d2d 0a0a 2323  a>.</p>..---..##
+000007c0: 2054 6162 6c65 206f 6620 436f 6e74 656e   Table of Conten
+000007d0: 7473 0a0a 2d20 5b43 7265 6469 7473 5d28  ts..- [Credits](
+000007e0: 2363 7265 6469 7473 290a 2d20 5b48 6f77  #credits).- [How
+000007f0: 2074 6f20 696e 7374 616c 6c5d 2823 686f   to install](#ho
+00000800: 772d 746f 2d69 6e73 7461 6c6c 290a 2d20  w-to-install).- 
+00000810: 5b48 6f77 2069 7420 776f 726b 735d 2823  [How it works](#
+00000820: 686f 772d 6974 2d77 6f72 6b73 290a 2d20  how-it-works).- 
+00000830: 5b48 6f77 2074 6f20 7573 655d 2823 686f  [How to use](#ho
+00000840: 772d 746f 2d75 7365 290a 2d20 5b52 6f61  w-to-use).- [Roa
+00000850: 646d 6170 5d28 2372 6f61 646d 6170 290a  dmap](#roadmap).
+00000860: 2d20 5b43 6f6e 7472 6962 7574 696e 675d  - [Contributing]
+00000870: 2823 636f 6e74 7269 6275 7469 6e67 290a  (#contributing).
+00000880: 2d20 5b4c 6963 656e 7365 5d28 236c 6963  - [License](#lic
+00000890: 656e 7365 290a 0a23 2320 4372 6564 6974  ense)..## Credit
+000008a0: 730a 0a5b 215b 4769 7448 7562 2043 6f6e  s..[![GitHub Con
+000008b0: 7472 6962 7574 6f72 7320 496d 6167 655d  tributors Image]
+000008c0: 2868 7474 7073 3a2f 2f63 6f6e 7472 6962  (https://contrib
+000008d0: 2e72 6f63 6b73 2f69 6d61 6765 3f72 6570  .rocks/image?rep
+000008e0: 6f3d 6f6c 6976 6d61 7468 2f6d 6572 6b6c  o=olivmath/merkl
+000008f0: 7929 5d28 6874 7470 733a 2f2f 6769 7468  y)](https://gith
+00000900: 7562 2e63 6f6d 2f6f 6c69 766d 6174 682f  ub.com/olivmath/
+00000910: 6d65 726b 6c79 2f67 7261 7068 732f 636f  merkly/graphs/co
+00000920: 6e74 7269 6275 746f 7273 290a 0a23 2320  ntributors)..## 
+00000930: 486f 7720 746f 2069 6e73 7461 6c6c 0a0a  How to install..
+00000940: 6060 600a 706f 6574 7279 2061 6464 206d  ```.poetry add m
+00000950: 6572 6b6c 790a 6060 600a 0a60 6060 0a70  erkly.```..```.p
+00000960: 6970 2069 6e73 7461 6c6c 206d 6572 6b6c  ip install merkl
+00000970: 790a 6060 600a 0a23 2320 486f 7720 746f  y.```..## How to
+00000980: 2077 6f72 6b73 0a0a 2d20 5f57 6520 7573   works..- _We us
+00000990: 6520 6b65 6363 616b 2d32 3536 2075 6e64  e keccak-256 und
+000009a0: 6572 2d74 6865 2d68 6f6f 645f 0a0a 5468  er-the-hood_..Th
+000009b0: 6973 206c 6962 7261 7279 2070 726f 7669  is library provi
+000009c0: 6465 7320 6120 636c 6561 6e20 616e 6420  des a clean and 
+000009d0: 6561 7379 2074 6f20 7573 6520 696d 706c  easy to use impl
+000009e0: 656d 656e 7461 7469 6f6e 206f 6620 7468  ementation of th
+000009f0: 6520 4d65 726b 6c65 2054 7265 6520 7769  e Merkle Tree wi
+00000a00: 7468 2074 6865 2066 6f6c 6c6f 7769 6e67  th the following
+00000a10: 2066 6561 7475 7265 733a 0a0a 2d20 4372   features:..- Cr
+00000a20: 6561 7465 204c 6561 660a 2d20 4372 6561  eate Leaf.- Crea
+00000a30: 7465 2052 6f6f 740a 2d20 4372 6561 7465  te Root.- Create
+00000a40: 2050 726f 6f66 0a2d 2056 6572 6966 7920   Proof.- Verify 
+00000a50: 5072 6f6f 660a 0a23 2320 486f 7720 746f  Proof..## How to
+00000a60: 2055 7365 0a0a 2a2a 4372 6561 7465 2061   Use..**Create a
+00000a70: 204d 6572 6b6c 6520 5472 6565 2a2a 0a0a   Merkle Tree**..
+00000a80: 6060 6070 7974 686f 6e0a 6672 6f6d 206d  ```python.from m
+00000a90: 6572 6b6c 792e 6d74 7265 6520 696d 706f  erkly.mtree impo
+00000aa0: 7274 204d 6572 6b6c 6554 7265 650a 0a23  rt MerkleTree..#
+00000ab0: 2063 7265 6174 6520 6120 4d65 726b 6c65   create a Merkle
+00000ac0: 2054 7265 650a 6d74 7265 6520 3d20 4d65   Tree.mtree = Me
+00000ad0: 726b 6c65 5472 6565 285b 2761 272c 2027  rkleTree(['a', '
+00000ae0: 6227 2c20 2763 272c 2027 6427 5d29 0a0a  b', 'c', 'd'])..
+00000af0: 2320 7368 6f77 206f 7269 6769 6e61 6c20  # show original 
+00000b00: 696e 7075 740a 6173 7365 7274 206d 7472  input.assert mtr
+00000b10: 6565 2e72 6177 5f6c 6561 6673 203d 3d20  ee.raw_leafs == 
+00000b20: 5b27 6127 2c20 2762 272c 2027 6327 2c20  ['a', 'b', 'c', 
+00000b30: 2764 275d 0a0a 2320 6861 7368 6564 206c  'd']..# hashed l
+00000b40: 6561 6673 0a61 7373 6572 7420 6d74 7265  eafs.assert mtre
+00000b50: 652e 6c65 6166 7320 3d3d 205b 0a20 2020  e.leafs == [.   
+00000b60: 2027 3361 6332 3235 3136 3864 6635 3432   '3ac225168df542
+00000b70: 3132 6132 3563 3163 3031 6664 3335 6265  12a25c1c01fd35be
+00000b80: 6266 6561 3430 3866 6461 6332 6533 3164  bfea408fdac2e31d
+00000b90: 6464 3666 3830 6134 6262 6639 6135 6631  dd6f80a4bbf9a5f1
+00000ba0: 6362 272c 0a20 2020 2027 6235 3535 3364  cb',.    'b5553d
+00000bb0: 6533 3135 6530 6564 6635 3034 6439 3135  e315e0edf504d915
+00000bc0: 3061 6638 3264 6166 6135 6334 3636 3766  0af82dafa5c4667f
+00000bd0: 6136 3138 6564 3061 3666 3139 6336 3962  a618ed0a6f19c69b
+00000be0: 3431 3136 3663 3535 3130 272c 0a20 2020  41166c5510',.   
+00000bf0: 2027 3062 3432 6236 3339 3363 3166 3533   '0b42b6393c1f53
+00000c00: 3036 3066 6533 6464 6266 6364 3761 6164  060fe3ddbfcd7aad
+00000c10: 6363 6138 3934 3436 3561 3561 3433 3866  cca894465a5a438f
+00000c20: 3639 6338 3764 3739 3062 3232 3939 6239  69c87d790b2299b9
+00000c30: 6232 272c 0a20 2020 2027 6631 3931 3865  b2',.    'f1918e
+00000c40: 3835 3632 3233 3665 6231 3761 6463 3835  8562236eb17adc85
+00000c50: 3032 3333 3266 3463 3963 3832 6263 3134  02332f4c9c82bc14
+00000c60: 6531 3962 6663 3061 6131 3061 6236 3734  e19bfc0aa10ab674
+00000c70: 6666 3735 6233 6432 6633 270a 5d0a 0a23  ff75b3d2f3'.]..#
+00000c80: 2073 686f 7274 6564 2068 6173 6865 6420   shorted hashed 
+00000c90: 6c65 6166 730a 6173 7365 7274 206d 7472  leafs.assert mtr
+00000ca0: 6565 2e73 686f 7274 5f6c 6561 6673 203d  ee.short_leafs =
+00000cb0: 3d20 5b0a 2020 2020 2733 6163 322e 2e2e  = [.    '3ac2...
+00000cc0: 272c 0a20 2020 2027 6235 3535 2e2e 2e27  ',.    'b555...'
+00000cd0: 2c0a 2020 2020 2730 6234 322e 2e2e 272c  ,.    '0b42...',
+00000ce0: 0a20 2020 2027 6631 3931 2e2e 2e27 0a5d  .    'f191...'.]
+00000cf0: 0a60 6060 0a0a 2a2a 4372 6561 7465 2061  .```..**Create a
+00000d00: 2052 6f6f 742a 2a0a 0a60 6060 7079 7468   Root**..```pyth
+00000d10: 6f6e 0a66 726f 6d20 6d65 726b 6c79 2e6d  on.from merkly.m
+00000d20: 7472 6565 2069 6d70 6f72 7420 4d65 726b  tree import Merk
+00000d30: 6c65 5472 6565 0a0a 2320 6372 6561 7465  leTree..# create
+00000d40: 2061 204d 6572 6b6c 6520 5472 6565 0a6d   a Merkle Tree.m
+00000d50: 7472 6565 203d 204d 6572 6b6c 6554 7265  tree = MerkleTre
+00000d60: 6528 5b27 6127 2c20 2762 272c 2027 6327  e(['a', 'b', 'c'
+00000d70: 2c20 2764 275d 290a 0a23 2067 6574 2072  , 'd'])..# get r
+00000d80: 6f6f 7420 6f66 2074 7265 650a 6173 7365  oot of tree.asse
+00000d90: 7274 206d 7472 6565 2e72 6f6f 7420 3d3d  rt mtree.root ==
+00000da0: 2027 3131 3563 6262 3437 3735 6564 3439   '115cbb4775ed49
+00000db0: 3566 3364 3935 3464 6661 3437 3136 3433  5f3d954dfa471643
+00000dc0: 3539 6139 3737 3632 6234 3030 3539 6439  59a97762b40059d9
+00000dd0: 3530 3238 3935 6465 6631 3665 6564 3630  502895def16eed60
+00000de0: 3963 270a 6060 600a 0a2a 2a43 7265 6174  9c'.```..**Creat
+00000df0: 6520 5072 6f6f 6620 6f66 2061 206c 6561  e Proof of a lea
+00000e00: 662a 2a0a 0a60 6060 7079 7468 6f6e 0a66  f**..```python.f
+00000e10: 726f 6d20 6d65 726b 6c79 2e6d 7472 6565  rom merkly.mtree
+00000e20: 2069 6d70 6f72 7420 4d65 726b 6c65 5472   import MerkleTr
+00000e30: 6565 0a0a 2320 6372 6561 7465 2061 204d  ee..# create a M
+00000e40: 6572 6b6c 6520 5472 6565 0a6d 7472 6565  erkle Tree.mtree
+00000e50: 203d 204d 6572 6b6c 6554 7265 6528 5b27   = MerkleTree(['
+00000e60: 6127 2c20 2762 272c 2027 6327 2c20 2764  a', 'b', 'c', 'd
+00000e70: 275d 290a 0a23 2067 6574 2070 726f 6f66  '])..# get proof
+00000e80: 206f 6620 6120 6072 6177 6020 6c65 6166   of a `raw` leaf
+00000e90: 0a61 7373 6572 7420 6d74 7265 652e 7072  .assert mtree.pr
+00000ea0: 6f6f 6628 2762 2729 203d 3d20 5b0a 2020  oof('b') == [.  
+00000eb0: 2020 4e6f 6465 286c 6566 743a 2027 3361    Node(left: '3a
+00000ec0: 6332 2e2e 2e27 292c 0a20 2020 204e 6f64  c2...'),.    Nod
+00000ed0: 6528 7269 6768 743a 2027 6235 3535 2e2e  e(right: 'b555..
+00000ee0: 2e27 292c 0a20 2020 204e 6f64 6528 7269  .'),.    Node(ri
+00000ef0: 6768 743a 2027 3634 3637 2e2e 2e27 290a  ght: '6467...').
+00000f00: 5d0a 6060 600a 0a2a 2a56 6572 6966 7920  ].```..**Verify 
+00000f10: 5072 6f6f 6620 6f66 2061 206c 6561 662a  Proof of a leaf*
+00000f20: 2a0a 0a60 6060 7079 7468 6f6e 0a66 726f  *..```python.fro
+00000f30: 6d20 6d65 726b 6c79 2e6d 7472 6565 2069  m merkly.mtree i
+00000f40: 6d70 6f72 7420 4d65 726b 6c65 5472 6565  mport MerkleTree
+00000f50: 0a0a 2320 6372 6561 7465 2061 204d 6572  ..# create a Mer
+00000f60: 6b6c 6520 5472 6565 0a6d 7472 6565 203d  kle Tree.mtree =
+00000f70: 204d 6572 6b6c 6554 7265 6528 5b27 6127   MerkleTree(['a'
+00000f80: 2c20 2762 272c 2027 6327 2c20 2764 275d  , 'b', 'c', 'd']
+00000f90: 290a 0a23 2067 6574 2070 726f 6f66 206f  )..# get proof o
+00000fa0: 6620 6120 7261 7720 6c65 6166 0a70 203d  f a raw leaf.p =
+00000fb0: 206d 7472 6565 2e70 726f 6f66 2827 6227   mtree.proof('b'
+00000fc0: 290a 0a23 2076 6572 6966 7920 796f 7572  )..# verify your
+00000fd0: 2070 726f 6f66 206f 6620 7261 7720 6c65   proof of raw le
+00000fe0: 6166 0a61 7373 6572 7420 6d74 7265 652e  af.assert mtree.
+00000ff0: 7665 7269 6679 2870 2c20 2762 2729 203d  verify(p, 'b') =
+00001000: 3d20 5472 7565 0a60 6060 0a0a 2323 2052  = True.```..## R
+00001010: 6f61 646d 6170 0a0a 7c20 4665 6174 7572  oadmap..| Featur
+00001020: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00001030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 2020 2020 7c20 5374 6174 7573 207c 2050      | Status | P
+00001090: 7269 6f72 6974 7920 7c0a 7c20 2d2d 2d2d  riority |.| ----
+000010a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000010b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000010c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000010d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000010e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000010f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001100: 2d2d 2d2d 2d20 7c20 2d2d 2d2d 2d2d 207c  ----- | ------ |
+00001110: 202d 2d2d 2d2d 2d2d 2d20 7c0a 7c20 4372   -------- |.| Cr
+00001120: 6561 7465 2052 6f6f 7420 2020 2020 2020  eate Root       
+00001130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 2020 2020 2020 2020 7c20 e29c 8520 2020          | ...   
+00001190: 2020 7c20 f09f 94a5 2020 2020 2020 207c    | ....       |
+000011a0: 0a7c 2043 7265 6174 6520 5072 6f6f 6620  .| Create Proof 
+000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001200: 2020 2020 2020 2020 2020 2020 207c 20e2               | .
+00001210: 9c85 2020 2020 207c 20f0 9f94 a520 2020  ..     | ....   
+00001220: 2020 2020 7c0a 7c20 5665 7269 6679 2050      |.| Verify P
+00001230: 726f 6f66 2020 2020 2020 2020 2020 2020  roof            
+00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001290: 2020 7c20 e29c 8520 2020 2020 7c20 f09f    | ...     | ..
+000012a0: 94a5 2020 2020 2020 207c 0a7c 2053 7570  ..       |.| Sup
+000012b0: 706f 7274 202a 2a5b 4f70 656e 5a65 7070  port **[OpenZepp
+000012c0: 656c 696e 5d28 6874 7470 733a 2f2f 646f  elin](https://do
+000012d0: 6373 2e6f 7065 6e7a 6570 7065 6c69 6e2e  cs.openzeppelin.
+000012e0: 636f 6d2f 636f 6e74 7261 6374 732f 342e  com/contracts/4.
+000012f0: 782f 7574 696c 6974 6965 7323 7665 7269  x/utilities#veri
+00001300: 6679 696e 675f 6d65 726b 6c65 5f70 726f  fying_merkle_pro
+00001310: 6f66 7329 2a2a 207c 20e2 8fb0 2020 2020  ofs)** | ...    
+00001320: 207c 20f0 9f94 a520 2020 2020 2020 7c0a   | ....       |.
+00001330: 7c20 436f 6d70 6174 6962 6c65 2077 6974  | Compatible wit
+00001340: 6820 2a2a 5b4d 6572 6b6c 6554 7265 654a  h **[MerkleTreeJ
+00001350: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00001360: 622e 636f 6d2f 6d69 6775 656c 6d6f 7461  b.com/miguelmota
+00001370: 2f6d 6572 6b6c 6574 7265 656a 7329 2a2a  /merkletreejs)**
+00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001390: 2020 2020 2020 2020 2020 2020 7c20 e28f              | ..
+000013a0: b020 2020 2020 7c20 f09f 94a5 2020 2020  .     | ....    
+000013b0: 2020 207c 0a7c 2055 7365 2061 6e79 2048     |.| Use any H
+000013c0: 6173 6820 6675 6e63 7469 6f6e 2020 2020  ash function    
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001420: 207c 20e2 8fb0 2020 2020 207c 20f0 9fa7   | ...     | ...
+00001430: 9020 2020 2020 2020 7c0a 7c20 4c65 6166  .       |.| Leaf
+00001440: 7320 6f66 2061 6e79 2073 697a 6520 2020  s of any size   
+00001450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014a0: 2020 2020 2020 7c20 e28f b020 2020 2020        | ...     
+000014b0: 7c20 f09f a790 2020 2020 2020 207c 0a0a  | ....       |..
+000014c0: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+000014d0: 0a2d 2042 6566 6f72 6520 7265 6164 2061  .- Before read a
+000014e0: 2063 6f64 6520 6f66 2063 6f6e 6475 6374   code of conduct
+000014f0: 3a20 2a2a 5b43 4f44 455f 4f46 5f43 4f4e  : **[CODE_OF_CON
+00001500: 4455 4354 5d28 434f 4445 5f4f 465f 434f  DUCT](CODE_OF_CO
+00001510: 4e44 5543 542e 6d64 292a 2a0a 2d20 466f  NDUCT.md)**.- Fo
+00001520: 6c6c 6f77 2074 6865 2067 7569 6465 206f  llow the guide o
+00001530: 6620 6465 7665 6c6f 706d 656e 743a 202a  f development: *
+00001540: 2a5b 434f 4e54 5249 4255 5449 4e47 5d28  *[CONTRIBUTING](
+00001550: 434f 4e54 5249 4255 5449 4e47 2e6d 6429  CONTRIBUTING.md)
+00001560: 2a2a 0a0a 2323 204c 6963 656e 7365 0a0a  **..## License..
+00001570: 5b4d 4954 5d28 4c49 4345 4e53 4529 0a0a  [MIT](LICENSE)..
+00001580: 3c21 2d2d 2068 7474 7073 3a2f 2f6d 6174  <!-- https://mat
+00001590: 682e 6d69 742e 6564 752f 7265 7365 6172  h.mit.edu/resear
+000015a0: 6368 2f68 6967 6873 6368 6f6f 6c2f 7072  ch/highschool/pr
+000015b0: 696d 6573 2f6d 6174 6572 6961 6c73 2f32  imes/materials/2
+000015c0: 3031 382f 4b75 737a 6d61 756c 2e70 6466  018/Kuszmaul.pdf
+000015d0: 202d 2d3e 0a0a                            -->..
```

