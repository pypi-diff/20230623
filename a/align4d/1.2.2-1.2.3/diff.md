# Comparing `tmp/align4d-1.2.2.tar.gz` & `tmp/align4d-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "align4d-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "align4d-1.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `align4d-1.2.2.tar` & `align4d-1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    13824 2023-05-24 15:58:19.921621 align4d-1.2.2/README.md
--rw-r--r--   0        0        0      822 2023-05-25 00:05:08.864830 align4d-1.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-22 15:58:38.000000 align4d-1.2.2/src/align4d/__init__.py
--rw-r--r--   0        0        0     6865 2023-05-24 23:55:09.226943 align4d-1.2.2/src/align4d/align.py
--rw-r--r--   0        0        0     1126 2023-05-09 01:39:20.296078 align4d-1.2.2/src/align4d/align4d.py
--rw-r--r--   0        0        0    10873 2023-05-06 05:20:19.306748 align4d-1.2.2/src/align4d/cpp/align.cpp
--rw-r--r--   0        0        0      739 2023-05-20 18:31:44.397330 align4d-1.2.2/src/align4d/cpp/align.h
--rw-r--r--   0        0        0    11216 2023-05-06 05:19:22.245690 align4d-1.2.2/src/align4d/cpp/align4d_cpython_extension.cpp
--rw-r--r--   0        0        0    17229 2023-05-23 22:36:06.537819 align4d-1.2.2/src/align4d/cpp/msa.cpp
--rw-r--r--   0        0        0     1199 2023-05-06 00:02:45.112359 align4d-1.2.2/src/align4d/cpp/msa.h
--rw-r--r--   0        0        0     4479 2023-05-06 05:17:40.301355 align4d-1.2.2/src/align4d/cpp/postprocess.cpp
--rw-r--r--   0        0        0     2175 2023-05-06 05:17:40.309160 align4d-1.2.2/src/align4d/cpp/postprocess.h
--rw-r--r--   0        0        0    10501 2023-05-23 22:36:06.535319 align4d-1.2.2/src/align4d/cpp/preprocess.cpp
--rw-r--r--   0        0        0     1375 2023-02-23 22:03:46.707574 align4d-1.2.2/src/align4d/cpp/preprocess.h
--rw-r--r--   0        0        0     1255 2023-05-24 14:55:30.141829 align4d-1.2.2/src/align4d/cpp/setup.py
--rw-r--r--   0        0        0    14549 1970-01-01 00:00:00.000000 align4d-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    14105 2023-06-23 16:44:39.286568 align4d-1.2.3/README.md
+-rw-r--r--   0        0        0      822 2023-06-23 16:46:01.978384 align4d-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-22 15:58:38.000000 align4d-1.2.3/src/align4d/__init__.py
+-rw-r--r--   0        0        0     7231 2023-06-23 16:40:53.463997 align4d-1.2.3/src/align4d/align.py
+-rw-r--r--   0        0        0     1126 2023-05-09 01:39:20.296078 align4d-1.2.3/src/align4d/align4d.py
+-rw-r--r--   0        0        0    10873 2023-05-06 05:20:19.306748 align4d-1.2.3/src/align4d/cpp/align.cpp
+-rw-r--r--   0        0        0      739 2023-05-20 18:31:44.397330 align4d-1.2.3/src/align4d/cpp/align.h
+-rw-r--r--   0        0        0    11216 2023-05-06 05:19:22.245690 align4d-1.2.3/src/align4d/cpp/align4d_cpython_extension.cpp
+-rw-r--r--   0        0        0    17229 2023-05-23 22:36:06.537819 align4d-1.2.3/src/align4d/cpp/msa.cpp
+-rw-r--r--   0        0        0     1199 2023-05-06 00:02:45.112359 align4d-1.2.3/src/align4d/cpp/msa.h
+-rw-r--r--   0        0        0     4479 2023-06-22 16:40:01.529884 align4d-1.2.3/src/align4d/cpp/postprocess.cpp
+-rw-r--r--   0        0        0     2175 2023-05-06 05:17:40.309160 align4d-1.2.3/src/align4d/cpp/postprocess.h
+-rw-r--r--   0        0        0    10501 2023-05-23 22:36:06.535319 align4d-1.2.3/src/align4d/cpp/preprocess.cpp
+-rw-r--r--   0        0        0     1375 2023-02-23 22:03:46.707574 align4d-1.2.3/src/align4d/cpp/preprocess.h
+-rw-r--r--   0        0        0     1255 2023-05-24 14:55:30.141829 align4d-1.2.3/src/align4d/cpp/setup.py
+-rw-r--r--   0        0        0    14830 1970-01-01 00:00:00.000000 align4d-1.2.3/PKG-INFO
```

### Comparing `align4d-1.2.2/README.md` & `align4d-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -162,54 +162,54 @@
 The criterion for determining the matching result are the following (also mentioned in the **Mechanism**):
 
 1. fully match: Levenshtein Distance = 0
 2. partially match: Levenshtein Distance ≤ boundary (default to be 2)
 3. mismatch: Levenshtein Distance > boundary (default to be 2)
 4. gap: aligned to a gap
 
-The `token_match()` requires 2 parameter, the `align_result` which is the direct return value from the previous three alignment functions, and an optional parameter `partial_bound` which must be the same as the `partial_bound` used in `align()` function. 
+The `token_match()` requires 3 parameter, the `align_result` which is the direct return value from the previous three alignment functions, an optional parameter `partial_bound` which must be the same as the `partial_bound` used in `align()` function (default to be 2), and an optional parameter `strip_punctuation` which must be the same as the `strip_punctuation` used in `align()` function (default to be True). 
 
 ```python
 hypothesis = "ok I am a fish. Are you? Hello there. How are you? ok"
 reference = [
         ["A", "I am a fish. "],
         ["B", "okay. "],
         ["C", "Are you? "],
         ["D", "Hello there. "],
         ["E", "How are you? "]
 ]
 align_result = align.align(hypothesis, reference)
-token_match_result = align.get_token_match_result(align_result)
+token_match_result = align.token_match(align_result)
 print(token_match_result)
 ```
 
 The return value is a list of strings that shows the token matching result and can either be fully match, partially match, mismatch, or gap.
 
 ```python
 # possible output for get_token_match_result()
 ['mismatch', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'gap']
 ```
 
 ### Retrieve mapping from reference to hypothesis
 
 Based on the alignment result, this tool provide function to retrieve the mapping from each token in the reference sequences to the hypothesis sequence. Each index shows the relative position (index) in the hypothesis sequence of the non-gap token (fully match, partially match, or mismatch) from the separated reference sequences. If the index is -1, it means that the current token does not aligned to any token in the hypothesis (align to a gap).
 
-To achieve this, use function `align_indices()`. This function requires one parameter, the `align_result` which is the direct return value from the previous `align()` function. 
+To achieve this, use function `align_indices()`. This function requires 2 parameters, the `align_result` which is the direct return value from the previous `align()` functionand an optional parameter `strip_punctuation` which must be the same as the `strip_punctuation` used in `align()` function (default to be True). 
 
 ```python
 hypothesis = "ok I am a fish. Are you? Hello there. How are you? ok"
 reference = [
         ["A", "I am a fish. "],
         ["B", "okay. "],
         ["C", "Are you? "],
         ["D", "Hello there. "],
         ["E", "How are you? "]
 ]
 align_result = align.align(hypothesis, reference)
-align_indices = align.get_token_match_result(align_result)
+align_indices = align.align_indices(align_result)
 print(align_indices)
 ```
 
 The return value is a dictionary containing list of integers that shows the mapping between tokens from separated reference to hypothesis. The integers are the indices of the tokens in reference sequence map to the hypothesis sequence (for example, the first token in sequence “C” is mapped to the token in hypothesis with index 5).
 
 ```python
 # possible output
```

### Comparing `align4d-1.2.2/pyproject.toml` & `align4d-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "align4d"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Peilin Wu", email="pwu54@emory.edu" },
 ]
 description = "align4d: Multi-sequence alignment tools for aligning ASR and Speaker Diarization result"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `align4d-1.2.2/src/align4d/align.py` & `align4d-1.2.3/src/align4d/align.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,16 +31,16 @@
                 reference_temp.extend(utterance[1].split())
                 reference_label.extend([utterance[0]] * len(utterance[1].split()))
             elif type(utterance[1]) == list:
                 reference_temp.extend(utterance[1])
                 reference_label.extend([utterance[0]] * len(utterance[1]))
     if strip_punctuation:
         TRANS = str.maketrans('', '', string.punctuation)
-        hypothesis_strip = [s.translate(TRANS) for s in hypothesis_temp]
-        reference_strip = [s.translate(TRANS) for s in reference_temp]
+        hypothesis_strip = [s.translate(TRANS) if not all(c in string.punctuation for c in s) else s for s in hypothesis_temp]
+        reference_strip = [s.translate(TRANS) if not all(c in string.punctuation for c in s) else s for s in reference_temp]
     else:
         hypothesis_strip = hypothesis_temp
         reference_strip = reference_temp
 
     # align
     if (segment_length is None and barrier_length is not None) or (barrier_length is None and segment_length is not None):
         raise Exception("Segment length or barrier length parameter incorrect or missing.")
@@ -76,30 +76,32 @@
     align_result = [[s if s != '-' else '' for s in seq] for seq in align_result]
     output = {"hypothesis": align_result[0], "reference": {}}
     for i in range(len(unique_speaker_label)):
         output["reference"][f"{unique_speaker_label[i]}"] = align_result[i + 1]
     return output
 
 
-def token_match(output: dict, partial_bound: int = 2) -> list[str]:
+def token_match(output: dict, partial_bound: int = 2, strip_punctuation: bool = True) -> list[str]:
     align_result = [output["hypothesis"]]
     for value in output["reference"].values():
         align_result.append(value)
-    TRANS = str.maketrans('', '', string.punctuation)
-    align_result = [[token.translate(TRANS) for token in row] for row in align_result]
+    if strip_punctuation:
+        TRANS = str.maketrans('', '', string.punctuation)
+        align_result = [[token.translate(TRANS) if not all(c in string.punctuation for c in token) else token for token in row] for row in align_result]
     align_result = [[token if token != '' else '-' for token in row] for row in align_result]
     return align4d.get_token_match_result(align_result, partial_bound)
 
 
-def align_indices(output: dict) -> dict:
+def align_indices(output: dict, strip_punctuation: bool = True) -> dict:
     align_result = [output["hypothesis"]]
     for value in output["reference"].values():
         align_result.append(value)
-    TRANS = str.maketrans('', '', string.punctuation)
-    align_result = [[token.translate(TRANS) for token in row] for row in align_result]
+    if strip_punctuation:
+        TRANS = str.maketrans('', '', string.punctuation)
+        align_result = [[token.translate(TRANS) if not all(c in string.punctuation for c in token) else token for token in row] for row in align_result]
     align_result = [[token if token != '' else '-' for token in row] for row in align_result]
     align_indices_list = align4d.get_align_indices(align_result)
     align_indices = {}
     for index, speaker_label in enumerate(output["reference"].keys()):
         align_indices[speaker_label] = align_indices_list[index]
     return align_indices
```

### Comparing `align4d-1.2.2/src/align4d/align4d.py` & `align4d-1.2.3/src/align4d/align4d.py`

 * *Files identical despite different names*

### Comparing `align4d-1.2.2/src/align4d/cpp/align.cpp` & `align4d-1.2.3/src/align4d/cpp/align.cpp`

 * *Files identical despite different names*

### Comparing `align4d-1.2.2/src/align4d/cpp/align.h` & `align4d-1.2.3/src/align4d/cpp/align.h`

 * *Files identical despite different names*

### Comparing `align4d-1.2.2/src/align4d/cpp/align4d_cpython_extension.cpp` & `align4d-1.2.3/src/align4d/cpp/align4d_cpython_extension.cpp`

 * *Files identical despite different names*

### Comparing `align4d-1.2.2/src/align4d/cpp/msa.cpp` & `align4d-1.2.3/src/align4d/cpp/msa.cpp`

 * *Files identical despite different names*

### Comparing `align4d-1.2.2/src/align4d/cpp/msa.h` & `align4d-1.2.3/src/align4d/cpp/msa.h`

 * *Files identical despite different names*

### Comparing `align4d-1.2.2/src/align4d/cpp/postprocess.cpp` & `align4d-1.2.3/src/align4d/cpp/postprocess.cpp`

 * *Files identical despite different names*

### Comparing `align4d-1.2.2/src/align4d/cpp/postprocess.h` & `align4d-1.2.3/src/align4d/cpp/postprocess.h`

 * *Files identical despite different names*

### Comparing `align4d-1.2.2/src/align4d/cpp/preprocess.cpp` & `align4d-1.2.3/src/align4d/cpp/preprocess.cpp`

 * *Files identical despite different names*

### Comparing `align4d-1.2.2/src/align4d/cpp/preprocess.h` & `align4d-1.2.3/src/align4d/cpp/preprocess.h`

 * *Files identical despite different names*

### Comparing `align4d-1.2.2/src/align4d/cpp/setup.py` & `align4d-1.2.3/src/align4d/cpp/setup.py`

 * *Files identical despite different names*

### Comparing `align4d-1.2.2/PKG-INFO` & `align4d-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: align4d
-Version: 1.2.2
+Version: 1.2.3
 Summary: align4d: Multi-sequence alignment tools for aligning ASR and Speaker Diarization result
 Author-email: Peilin Wu <pwu54@emory.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -178,54 +178,54 @@
 The criterion for determining the matching result are the following (also mentioned in the **Mechanism**):
 
 1. fully match: Levenshtein Distance = 0
 2. partially match: Levenshtein Distance ≤ boundary (default to be 2)
 3. mismatch: Levenshtein Distance > boundary (default to be 2)
 4. gap: aligned to a gap
 
-The `token_match()` requires 2 parameter, the `align_result` which is the direct return value from the previous three alignment functions, and an optional parameter `partial_bound` which must be the same as the `partial_bound` used in `align()` function. 
+The `token_match()` requires 3 parameter, the `align_result` which is the direct return value from the previous three alignment functions, an optional parameter `partial_bound` which must be the same as the `partial_bound` used in `align()` function (default to be 2), and an optional parameter `strip_punctuation` which must be the same as the `strip_punctuation` used in `align()` function (default to be True). 
 
 ```python
 hypothesis = "ok I am a fish. Are you? Hello there. How are you? ok"
 reference = [
         ["A", "I am a fish. "],
         ["B", "okay. "],
         ["C", "Are you? "],
         ["D", "Hello there. "],
         ["E", "How are you? "]
 ]
 align_result = align.align(hypothesis, reference)
-token_match_result = align.get_token_match_result(align_result)
+token_match_result = align.token_match(align_result)
 print(token_match_result)
 ```
 
 The return value is a list of strings that shows the token matching result and can either be fully match, partially match, mismatch, or gap.
 
 ```python
 # possible output for get_token_match_result()
 ['mismatch', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'fully match', 'gap']
 ```
 
 ### Retrieve mapping from reference to hypothesis
 
 Based on the alignment result, this tool provide function to retrieve the mapping from each token in the reference sequences to the hypothesis sequence. Each index shows the relative position (index) in the hypothesis sequence of the non-gap token (fully match, partially match, or mismatch) from the separated reference sequences. If the index is -1, it means that the current token does not aligned to any token in the hypothesis (align to a gap).
 
-To achieve this, use function `align_indices()`. This function requires one parameter, the `align_result` which is the direct return value from the previous `align()` function. 
+To achieve this, use function `align_indices()`. This function requires 2 parameters, the `align_result` which is the direct return value from the previous `align()` functionand an optional parameter `strip_punctuation` which must be the same as the `strip_punctuation` used in `align()` function (default to be True). 
 
 ```python
 hypothesis = "ok I am a fish. Are you? Hello there. How are you? ok"
 reference = [
         ["A", "I am a fish. "],
         ["B", "okay. "],
         ["C", "Are you? "],
         ["D", "Hello there. "],
         ["E", "How are you? "]
 ]
 align_result = align.align(hypothesis, reference)
-align_indices = align.get_token_match_result(align_result)
+align_indices = align.align_indices(align_result)
 print(align_indices)
 ```
 
 The return value is a dictionary containing list of integers that shows the mapping between tokens from separated reference to hypothesis. The integers are the indices of the tokens in reference sequence map to the hypothesis sequence (for example, the first token in sequence “C” is mapped to the token in hypothesis with index 5).
 
 ```python
 # possible output
```

