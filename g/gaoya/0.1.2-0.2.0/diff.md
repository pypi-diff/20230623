# Comparing `tmp/gaoya-0.1.2-cp37-abi3-win_amd64.whl.zip` & `tmp/gaoya-0.2.0-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 386394 bytes, number of entries: 7
--rw-r--r--  4.6 unx     2324 b- defN 22-Jul-15 17:44 gaoya-0.1.2.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 22-Jul-15 17:44 gaoya-0.1.2.dist-info/WHEEL
--rw-r--r--  4.6 unx     9096 b- defN 22-Jul-15 17:44 gaoya/minhash.py
--rw-r--r--  4.6 unx     5870 b- defN 22-Jul-15 17:44 gaoya/simhash.py
--rw-r--r--  4.6 unx       73 b- defN 22-Jul-15 17:44 gaoya/__init__.py
--rwxr-xr-x  4.6 unx  1249280 b- defN 22-Jul-15 17:44 gaoya/gaoya.pyd
--rw-r--r--  4.6 unx      493 b- defN 22-Jul-15 17:44 gaoya-0.1.2.dist-info/RECORD
-7 files, 1267231 bytes uncompressed, 385542 bytes compressed:  69.6%
+Zip file size: 485654 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     2283 b- defN 23-Jun-23 06:36 gaoya-0.2.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-Jun-23 06:36 gaoya-0.2.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     9778 b- defN 23-Jun-23 06:36 gaoya/minhash.py
+-rw-r--r--  4.6 unx     5870 b- defN 23-Jun-23 06:36 gaoya/simhash.py
+-rw-r--r--  4.6 unx       73 b- defN 23-Jun-23 06:36 gaoya/__init__.py
+-rwxr-xr-x  4.6 unx  1914880 b- defN 23-Jun-23 06:36 gaoya/gaoya.pyd
+-rw-r--r--  4.6 unx      493 b- defN 23-Jun-23 06:36 gaoya-0.2.0.dist-info/RECORD
+7 files, 1933472 bytes uncompressed, 484802 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: gaoya-0.1.2.dist-info/METADATA
+Filename: gaoya-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: gaoya-0.1.2.dist-info/WHEEL
+Filename: gaoya-0.2.0.dist-info/WHEEL
 Comment: 
 
 Filename: gaoya/minhash.py
 Comment: 
 
 Filename: gaoya/simhash.py
 Comment: 
 
 Filename: gaoya/__init__.py
 Comment: 
 
 Filename: gaoya/gaoya.pyd
 Comment: 
 
-Filename: gaoya-0.1.2.dist-info/RECORD
+Filename: gaoya-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gaoya/minhash.py

```diff
@@ -1,14 +1,14 @@
 from typing import List, Union, Tuple
 
 from .gaoya import minhash as m
 
 class MinHashStringIndex:
     """
-    MinHashStringIndex for indexing and searching text documents based jaccard similarity.
+    MinHashStringIndex for indexing and searching text documents (strings) on jaccard similarity.
 
 
     Reference: `Chapter 3, Mining of Massive Datasets <http://www.mmds.org/>`
     If  `hash_size` and `num_bands` is specified `num_hashes` is not used, otherwise
         `hash_size` and `num_bands` will be calculated according to S-curve.
 
     Parameters
@@ -49,14 +49,22 @@
         The lower and upper boundary of the range of n-values for different
         n-grams to be extracted. All values of n such that min_n <= n <= max_n
         will be used. For example an `ngram_range` of `(1, 1)`  means only
         unigrams, `(1, 2)` means unigrams and bigrams, and `(2, 2)` means
         only bigrams.
         Only applies if `analyzer` is not callable.
 
+    id_container: str, default="set"
+        The data structure used as a bucket to hold ids of documents in bands.
+        When efficient removals required use "set".
+        When removals are not required or rare use "vec"
+        When the number of similar documents (near duplicates) is expected to be small use "smallvec" which
+        can store up to two ids inline without allocation, which reduces memory usage
+        and improves performamance.
+
     Examples
     --------
             >>> index = gaoya.minhash.MinHashStringIndex(32, 0.5, 42, 3, None, 'word', True, (1,1))
             >>> corpus = [
             ...     'This is the first document.',
             ...     'This document is the second document.',
             ...     'And this is the third document.',
@@ -77,50 +85,68 @@
     def __init__(self, hash_size=32,
                  jaccard_threshold=0.75,
                  num_bands=20,
                  band_size=5,
                  num_hashes=None,
                  analyzer='word',
                  lowercase=False,
-                 ngram_range=None):
+                 ngram_range=None,
+                 id_container='set'):
         if hash_size not in [8, 16, 32, 64]:
             raise ValueError(f"Invalid hash_size {hash_size}. hash_size must be on of 8, 16, 32 or 64")
         if jaccard_threshold < 0.0 or jaccard_threshold > 1.0:
             raise ValueError(f"Jaccard threshold must be between 0 and 1")
+        if id_container not in ("set", "vec", "smallvec"):
+            raise ValueError(f"id_container must be one of ('set', 'vec', 'smallvec')")
         self.analyzer = analyzer
         # if analyzer is callable we need to pass something to index's constructor.
         analyzer = 'word' if callable(self.analyzer) else analyzer
-        if hash_size == 64:
-            self.index = m.MinHash64StringIntIndex(jaccard_threshold, num_bands, band_size, num_hashes, analyzer, lowercase, ngram_range)
-        elif hash_size == 32:
-            self.index = m.MinHash32StringIntIndex(jaccard_threshold, num_bands, band_size, num_hashes, analyzer, lowercase, ngram_range)
-        elif hash_size == 16:
-            self.index = m.MinHash16StringIntIndex(jaccard_threshold, num_bands, band_size, num_hashes, analyzer, lowercase, ngram_range)
-        elif hash_size == 8:
-            self.index = m.MinHash8StringIntIndex(jaccard_threshold, num_bands, band_size, num_hashes, analyzer, lowercase, ngram_range)
-        else:
-            raise ValueError(f"Invalid hash size {hash_size}")
 
+        constructors = {
+            64: {
+                'set': m.MinHash64StringIntIndexHashSet,
+                'vec': m.MinHash64StringIntIndexVec,
+                'smallvec': m.MinHash64StringIntIndexSmallVec,
+            },
+            32: {
+                'set': m.MinHash32StringIntIndexHashSet,
+                'vec': m.MinHash32StringIntIndexVec,
+                'smallvec': m.MinHash32StringIntIndexSmallVec,
+            },
+            16: {
+                'set': m.MinHash16StringIntIndexHashSet,
+                'vec': m.MinHash16StringIntIndexVec,
+                'smallvec': m.MinHash16StringIntIndexSmallVec,
+            },
+            8: {
+                'set': m.MinHash8StringIntIndexHashSet,
+                'vec': m.MinHash8StringIntIndexVec,
+                'smallvec': m.MinHash8StringIntIndexSmallVec,
+            }
+        }
+
+        type = constructors[hash_size][id_container]
+        self.minhash_index = type(jaccard_threshold, num_bands, band_size, num_hashes, analyzer, lowercase, ngram_range)
 
-    def insert_document(self, id, doc):
+    def insert_document(self, id: int, doc: str):
         """
         Inserts a document `doc` with id `id` into the index.
 
         Parameters
         ----------
 
         id: int
             Id of the document
         doc: str
             Document text
         """
         if callable(self.analyzer):
-            self.index.insert_tokens(id, self.analyzer(doc))
+            self.minhash_index.insert_tokens(id, self.analyzer(doc))
         else:
-            self.index.insert_document(id, doc)
+            self.minhash_index.insert_document(id, doc)
 
     def query(self, doc: str, return_similarity=False) -> Union[List[int], List[Tuple[int, float]]]:
         """
         Searches the index for documents similar to `doc`.
         Returns list of similar document ids.
         If return_similarity is `True` method returns a list of tuples where the first element
         is document id and the second is jaccard similarity. The result is sorted by similarity from
@@ -134,22 +160,22 @@
 
         Returns:
         ----------
         List of ids or list of tuples
         """
         if callable(self.analyzer):
             if return_similarity:
-                return self.index.query_tokens_return_similarity(self.analyzer(doc))
+                return self.minhash_index.query_tokens_return_similarity(self.analyzer(doc))
             else:
-                return self.index.query_tokens(self.analyzer(doc))
+                return self.minhash_index.query_tokens(self.analyzer(doc))
         else:
             if return_similarity:
-                return self.index.query_return_similarity(doc)
+                return self.minhash_index.query_return_similarity(doc)
             else:
-                return self.index.query(doc)
+                return self.minhash_index.query(doc)
 
     def par_bulk_query(self, docs: List[str], return_similarity=False):
         """
         Searches the index for documents similar to `docs`.
         This method uses multiple native threads to execute `query` operation on a batch of documents
         Returns list of lists of similar document ids or list of lists of tuples
         Parameters
@@ -163,22 +189,22 @@
         ----------
         List Lists of ids or list of lists of tuples
         """
 
         if callable(self.analyzer):
             analyzed_docs = [self.analyzer(doc) for doc in docs]
             if return_similarity:
-                return self.index.par_bulk_query_tokens_return_similarity(analyzed_docs)
+                return self.minhash_index.par_bulk_query_tokens_return_similarity(analyzed_docs)
             else:
-                return self.index.par_bulk_query_tokens(analyzed_docs)
+                return self.minhash_index.par_bulk_query_tokens(analyzed_docs)
         else:
             if return_similarity:
-                return self.index.par_bulk_query_return_similarity(docs)
+                return self.minhash_index.par_bulk_query_return_similarity(docs)
             else:
-                return self.index.par_bulk_query(docs)
+                return self.minhash_index.par_bulk_query(docs)
 
 
 
     def par_bulk_insert_docs(self, ids: List[int], docs: List[str]):
         """
         Inserts a batch of documents. This method will use multiple cores to insert a batch
         of documents into the index. If analyzer is callable tokenization will be single threaded.
@@ -189,40 +215,33 @@
             List of ids
 
         docs: list
             List of strings
         """
         if callable(self.analyzer):
             tokens = [self.analyzer(doc) for doc in docs]
-            self.index.bulk_insert_tokens(ids, tokens)
+            self.minhash_index.bulk_insert_tokens(ids, tokens)
         else:
-            self.index.par_bulk_insert_docs(ids, docs)
+            self.minhash_index.par_bulk_insert_docs(ids, docs)
 
     def remove(self, id: int):
         """
         Removes id from the index.
 
-        Currently, this method may not remove the minhash associated with `id` from memory if there is another minhash
-        with the same value at any band.
-        To fully remove minhash from memory gaoya needs to be compiled on nightly Rust channel with `--features "unstable"`
-        This will work on the stable when this issue is resolved
-        https://github.com/rust-lang/rust/issues/56167
-
-
         Parameters
         ----------
         id: int
             Id of the document
         """
-        self.index.remove(id)
+        self.minhash_index.remove(id)
 
     def size(self):
         """
         Returns the number of documents in the index
         """
-        return self.index.size()
+        return self.minhash_index.size()
 
     def __str__(self):
-        return self.index.__str__()
+        return self.minhash_index.__str__()
 
     def __repr__(self):
-        return self.index.__repr__()
+        return self.minhash_index.__repr__()
```

## gaoya/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 from . import minhash
 from . import simhash
```

## Comparing `gaoya-0.1.2.dist-info/METADATA` & `gaoya-0.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 Metadata-Version: 2.1
 Name: gaoya
-Version: 0.1.2
-Classifier: Programming Language :: Rust
+Version: 0.2.0
 Summary: Locality Sensitive Hashing
 Home-Page: https://github.com/serega/gaoya
 Author: Sergey Melderis <sergey.melderis@gmail.com>
 Author-email: Sergey Melderis <sergey.melderis@gmail.com>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

