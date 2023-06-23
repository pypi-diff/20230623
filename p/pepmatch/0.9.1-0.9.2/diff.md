# Comparing `tmp/pepmatch-0.9.1.tar.gz` & `tmp/pepmatch-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepmatch-0.9.1.tar", last modified: Tue May 23 23:15:53 2023, max compression
+gzip compressed data, was "pepmatch-0.9.2.tar", last modified: Fri Jun 23 07:36:29 2023, max compression
```

## Comparing `pepmatch-0.9.1.tar` & `pepmatch-0.9.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-23 23:15:53.081408 pepmatch-0.9.1/
--rw-r--r--   0 dan       (1000) dan       (1000)    11757 2021-03-17 17:44:53.000000 pepmatch-0.9.1/LICENSE
--rw-r--r--   0 dan       (1000) dan       (1000)     4847 2023-05-23 23:15:53.081408 pepmatch-0.9.1/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)     4541 2023-03-30 20:51:53.000000 pepmatch-0.9.1/README.md
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-23 23:15:53.078075 pepmatch-0.9.1/pepmatch/
--rw-r--r--   0 dan       (1000) dan       (1000)      139 2021-10-30 00:28:03.000000 pepmatch-0.9.1/pepmatch/__init__.py
--rw-r--r--   0 dan       (1000) dan       (1000)     2079 2023-01-19 01:48:10.000000 pepmatch-0.9.1/pepmatch/benchmarker.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1796 2023-03-28 21:36:21.000000 pepmatch-0.9.1/pepmatch/helpers.py
--rwxr-xr-x   0 dan       (1000) dan       (1000)    28307 2023-05-23 23:14:19.000000 pepmatch-0.9.1/pepmatch/matcher.py
--rwxr-xr-x   0 dan       (1000) dan       (1000)     9206 2023-04-11 22:13:38.000000 pepmatch-0.9.1/pepmatch/preprocessor.py
--rw-r--r--   0 dan       (1000) dan       (1000)       22 2023-05-23 23:14:03.000000 pepmatch-0.9.1/pepmatch/version.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-23 23:15:53.081408 pepmatch-0.9.1/pepmatch.egg-info/
--rw-r--r--   0 dan       (1000) dan       (1000)     4847 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/PKG-INFO
--rw-r--r--   0 dan       (1000) dan       (1000)      452 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/SOURCES.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/dependency_links.txt
--rw-r--r--   0 dan       (1000) dan       (1000)      104 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/entry_points.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        1 2021-01-26 17:40:31.000000 pepmatch-0.9.1/pepmatch.egg-info/not-zip-safe
--rw-r--r--   0 dan       (1000) dan       (1000)       80 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/requires.txt
--rw-r--r--   0 dan       (1000) dan       (1000)        9 2023-05-23 23:15:53.000000 pepmatch-0.9.1/pepmatch.egg-info/top_level.txt
--rw-r--r--   0 dan       (1000) dan       (1000)       38 2023-05-23 23:15:53.081408 pepmatch-0.9.1/setup.cfg
--rwxr-xr-x   0 dan       (1000) dan       (1000)     1081 2022-05-06 20:37:03.000000 pepmatch-0.9.1/setup.py
-drwxr-xr-x   0 dan       (1000) dan       (1000)        0 2023-05-23 23:15:53.081408 pepmatch-0.9.1/test/
--rw-r--r--   0 dan       (1000) dan       (1000)     1765 2023-05-23 05:17:53.000000 pepmatch-0.9.1/test/test_best_match.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1713 2023-05-23 05:18:00.000000 pepmatch-0.9.1/test/test_exact_match.py
--rw-r--r--   0 dan       (1000) dan       (1000)     1755 2023-05-23 05:18:04.000000 pepmatch-0.9.1/test/test_mismatch.py
+drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-06-23 07:36:29.343149 pepmatch-0.9.2/
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    11757 2023-03-01 21:01:30.000000 pepmatch-0.9.2/LICENSE
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4839 2023-06-23 07:36:29.342603 pepmatch-0.9.2/PKG-INFO
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4508 2023-05-30 05:21:03.000000 pepmatch-0.9.2/README.md
+drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-06-23 07:36:29.334154 pepmatch-0.9.2/pepmatch/
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      207 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/__init__.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     2096 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/benchmarker.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     2015 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/helpers.py
+-rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    31802 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/matcher.py
+-rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    10818 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/preprocessor.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       22 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/version.py
+drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-06-23 07:36:29.338614 pepmatch-0.9.2/pepmatch.egg-info/
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4839 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/PKG-INFO
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      486 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/SOURCES.txt
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        1 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/dependency_links.txt
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      104 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/entry_points.txt
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        1 2023-03-03 04:38:29.000000 pepmatch-0.9.2/pepmatch.egg-info/not-zip-safe
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       80 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/requires.txt
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        9 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/top_level.txt
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       38 2023-06-23 07:36:29.343323 pepmatch-0.9.2/setup.cfg
+-rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      999 2023-05-30 05:21:03.000000 pepmatch-0.9.2/setup.py
+drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-06-23 07:36:29.341243 pepmatch-0.9.2/test/
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1769 2023-05-30 05:21:03.000000 pepmatch-0.9.2/test/test_best_match.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      569 2023-05-30 05:21:03.000000 pepmatch-0.9.2/test/test_discontinuous_search.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1743 2023-05-30 05:21:03.000000 pepmatch-0.9.2/test/test_exact_match.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1785 2023-05-30 05:21:03.000000 pepmatch-0.9.2/test/test_mismatch.py
```

### Comparing `pepmatch-0.9.1/LICENSE` & `pepmatch-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.1/PKG-INFO` & `pepmatch-0.9.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pepmatch
-Version: 0.9.1
-Summary: Peptide and epitope search against a reference proteome with specified mismatches.
+Version: 0.9.2
+Summary: Search tool for peptides and epitopes within a proteome, while considering potential residue substitutions.
 Home-page: https://github.com/IEDB/PEPMatch
 Author: Daniel Marrama
 Author-email: dmarrama@lji.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img src="docs/logo.png">
 </p>
 
 --------------------------------------------------------------------
 
-![Unit Tests](https://github.com/IEDB/PEPMatch/actions/workflows/unittests.yml/badge.svg)
+![Unit Tests](https://github.com/IEDB/PEPMatch/actions/workflows/tests.yml/badge.svg)
 
 #### Author: Daniel Marrama
 
 Peptide search against a reference proteome, or sets of proteins, with residue subtitutions.
 
 Two step process: preprocessing and matching.
 
@@ -33,15 +33,15 @@
 - [NumPy](https://numpy.org/)
 - [Biopython](https://biopython.org/)
 - [Levenshtein](https://pypi.org/project/python-Levenshtein/)
 - [redis](https://redis.com/)
 
 ### Installation
 
-```
+```bash
 pip install pepmatch
 ```
 
 
 ### Inputs
 
 #### Preprocessor
@@ -78,39 +78,45 @@
 
 ### Exact Matching Example
 
 ```python
 from pepmatch import Preprocessor, Matcher
 
 # proteome, k, preprocessed_format, target directory, gene_priority_proteome
-Preprocessor('proteomes/human.fasta', '.' 'proteomes/human_gp.fasta').preprocess('sql', k=5)
-# PREPROCESSING ONLY NEEDS TO BE DONE ONCE!
+Preprocessor(
+  'proteomes/human.fasta', '.', 'proteomes/human_gp.fasta'
+).sql_proteome(k = 5) # preprocessing only needs to be done once!
 
 # query, proteome, max_mismatches, k, preprocessed files directory
-Matcher('queries/mhc_ligands_test.fasta', 'proteomes/human.fasta', 0, 5, '.').match()
+Matcher(
+  'queries/mhc_ligands_test.fasta', 'proteomes/human.fasta', 0, 5, '.'
+).match()
 ```
 
 ### Mismatching Example 
 
 ```python
 from pepmatch import Preprocessor, Matcher
 
 # proteome, k, preprocessed_format, target directory
-Preprocessor('proteomes/human.fasta').preprocess('pickle', k=3)
-# PREPROCESSING ONLY NEEDS TO BE DONE ONCE!
+Preprocessor('proteomes/human.fasta').pickle_proteome(k = 3)
 
 # query, proteome, max_mismatches, k, preprocessed files directory
-Matcher('queries/neoepitopes_test.fasta', 'proteomes/human.fasta', 3, 3).match()
+Matcher(
+  'queries/neoepitopes_test.fasta', 'proteomes/human.fasta', 3, 3
+).match()
 ```
 
 ### Best Match Example
 
 ```python
 from pepmatch import Preprocessor, Matcher
-Matcher('queries/milk_peptides.fasta', 'proteomes/human.fasta', best_match=True).match()
+Matcher(
+  'queries/milk_peptides.fasta', 'proteomes/human.fasta', best_match=True
+).match()
 ```
 
 The best match parameter without k or mismatch inputs will produce the best match for each peptide in the query, meaning the match with the least number of mismatches, the best protein existence level, and if the match exists in the gene priority proteome. No preprocessing beforehand is required, as the Matcher class will do this for you to find the best match.
 
 ### Outputs
 
 As mentioned above, outputs can be specified with the ```output_format``` parameter in the ```Matcher``` class. The following formats are allowed: `dataframe`, `csv`, `xlsx`, `json`, and `html`.
```

### Comparing `pepmatch-0.9.1/README.md` & `pepmatch-0.9.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <p align="center">
   <img src="docs/logo.png">
 </p>
 
 --------------------------------------------------------------------
 
-![Unit Tests](https://github.com/IEDB/PEPMatch/actions/workflows/unittests.yml/badge.svg)
+![Unit Tests](https://github.com/IEDB/PEPMatch/actions/workflows/tests.yml/badge.svg)
 
 #### Author: Daniel Marrama
 
 Peptide search against a reference proteome, or sets of proteins, with residue subtitutions.
 
 Two step process: preprocessing and matching.
 
@@ -23,15 +23,15 @@
 - [NumPy](https://numpy.org/)
 - [Biopython](https://biopython.org/)
 - [Levenshtein](https://pypi.org/project/python-Levenshtein/)
 - [redis](https://redis.com/)
 
 ### Installation
 
-```
+```bash
 pip install pepmatch
 ```
 
 
 ### Inputs
 
 #### Preprocessor
@@ -68,39 +68,45 @@
 
 ### Exact Matching Example
 
 ```python
 from pepmatch import Preprocessor, Matcher
 
 # proteome, k, preprocessed_format, target directory, gene_priority_proteome
-Preprocessor('proteomes/human.fasta', '.' 'proteomes/human_gp.fasta').preprocess('sql', k=5)
-# PREPROCESSING ONLY NEEDS TO BE DONE ONCE!
+Preprocessor(
+  'proteomes/human.fasta', '.', 'proteomes/human_gp.fasta'
+).sql_proteome(k = 5) # preprocessing only needs to be done once!
 
 # query, proteome, max_mismatches, k, preprocessed files directory
-Matcher('queries/mhc_ligands_test.fasta', 'proteomes/human.fasta', 0, 5, '.').match()
+Matcher(
+  'queries/mhc_ligands_test.fasta', 'proteomes/human.fasta', 0, 5, '.'
+).match()
 ```
 
 ### Mismatching Example 
 
 ```python
 from pepmatch import Preprocessor, Matcher
 
 # proteome, k, preprocessed_format, target directory
-Preprocessor('proteomes/human.fasta').preprocess('pickle', k=3)
-# PREPROCESSING ONLY NEEDS TO BE DONE ONCE!
+Preprocessor('proteomes/human.fasta').pickle_proteome(k = 3)
 
 # query, proteome, max_mismatches, k, preprocessed files directory
-Matcher('queries/neoepitopes_test.fasta', 'proteomes/human.fasta', 3, 3).match()
+Matcher(
+  'queries/neoepitopes_test.fasta', 'proteomes/human.fasta', 3, 3
+).match()
 ```
 
 ### Best Match Example
 
 ```python
 from pepmatch import Preprocessor, Matcher
-Matcher('queries/milk_peptides.fasta', 'proteomes/human.fasta', best_match=True).match()
+Matcher(
+  'queries/milk_peptides.fasta', 'proteomes/human.fasta', best_match=True
+).match()
 ```
 
 The best match parameter without k or mismatch inputs will produce the best match for each peptide in the query, meaning the match with the least number of mismatches, the best protein existence level, and if the match exists in the gene priority proteome. No preprocessing beforehand is required, as the Matcher class will do this for you to find the best match.
 
 ### Outputs
 
 As mentioned above, outputs can be specified with the ```output_format``` parameter in the ```Matcher``` class. The following formats are allowed: `dataframe`, `csv`, `xlsx`, `json`, and `html`.
```

### Comparing `pepmatch-0.9.1/pepmatch/benchmarker.py` & `pepmatch-0.9.2/pepmatch/benchmarker.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from .matcher import Matcher
 
-import os, glob
 
 class Benchmarker(Matcher):
-  '''
+  """
   Object used for benchmarking the PEPMatch code for the various applications.
   It uses three methods: 2 for preprocessing and 1 for searching as the benchmarking
   code is structured. PEPMatch does not do any query preprocessing so it raises
   a TypeError which is excepted in the benchmarking code.
   Inherits from Matcher object.
-  '''
+  """
   def __init__(self, query, proteome, lengths, max_mismatches, algorithm_parameters):
     self.query = query
     self.proteome = proteome
     self.max_mismatches = max_mismatches
     self.lengths = lengths
     self.algorithm_parameters = algorithm_parameters
     
-    super().__init__(query, proteome, max_mismatches, output_format=algorithm_parameters['output_format'], versioned_ids=False)
+    super().__init__(
+      query, proteome, max_mismatches, 
+      output_format=algorithm_parameters['output_format'], versioned_ids=False)
 
   def __str__(self):
     return 'PEPMatch'
 
-  def preprocess_query(self):
-    '''No query preprocessing, raise TypeError'''
+  def preprocess_query(self) -> None:
+    """No query preprocessing, raise TypeError"""
     raise TypeError(self.__str__() + ' does not preprocess queries.\n')
 
-  def preprocess_proteome(self):
-    '''Preprocess proteome once or multiple times for each split calculated.'''
+  def preprocess_proteome(self) -> None:
+    """Preprocess proteome once or multiple times for each split calculated."""
     if self.max_mismatches == -1:
       for k in self.best_match_ks():
         self.preprocess(k)
     else:
       for k in self.batch_query().keys():
         self.preprocess(k)
 
-  def search(self):
-    '''
-    Call overarching match function. Then convert results into the standard format
+  def search(self) -> list:
+    """Call overarching match function. Then convert results into the standard format
     needed to calculate accuracy.
-    '''
+    """
     if self.max_mismatches == -1:
       self.k_specified = True
       self.k = 2
       self.max_mismatches = 7
 
     matches = self.match()
```

### Comparing `pepmatch-0.9.1/pepmatch/helpers.py` & `pepmatch-0.9.2/pepmatch/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,49 @@
 #!/usr/bin/env python3
 
 import re
 
 from Bio import SeqIO
+from Bio.SeqRecord import SeqRecord
 
 
-def parse_fasta(file):
-  """Return a parsed Biopython SeqRecord object from a FASTA file."""
+def parse_fasta(file: str) -> list:
+  """Return a parsed Biopython SeqRecord object from a FASTA file.
+  Args:
+    file: path to FASTA file.
+  """
   return list(SeqIO.parse(file, 'fasta'))
 
-def split_sequence(sequence, k):
+
+def split_sequence(sequence: str, k: int) -> list:
   """
   Splits a peptide into equal sized k-mers on a rolling basis.
   Ex: k = 4, NSLFLTDLY --> ['NSLF', 'SLFL', 'LFLT', 'FLTD', 'LTDL', 'TDLY']
+
+  Args:
+    sequence: peptide sequence.
+    k: k-mer length.
   """
   return [sequence[i:i+k] for i in range(len(sequence) - k + 1)]
 
-def extract_metadata(record):
-  """Extract metadata from a FASTA header."""
+
+def extract_metadata(record: SeqRecord) -> list:
+  """Extract metadata from a FASTA header.
+  Args: 
+    record: protein SeqRecord from proteome FASTA file.
+  """
   regexes = {
-      'protein_id': re.compile(r"\|([^|]*)\|"),      # between | and |
-      'protein_name': re.compile(r"\s(.+?)\sOS"),    # between first space and space before OS
-      'species': re.compile(r"OS=(.+?)\sOX"),        # between OS= and space before OX (species can have spaces)
-      'taxon_id': re.compile(r"OX=(.+?)\s"),         # between OX= and space
-      'gene': re.compile(r"GN=(.+?)\s"),             # between GN= and space
-      'pe_level': re.compile(r"PE=(.+?)\s"),         # between PE= and space
-      'sequence_version': re.compile(r"SV=(.+?)\s"), # between SV= and space
-      'gene_priority': re.compile(r"GP=(.+?)\s"),    # between GP= and space
+      'protein_id': re.compile(r"\|([^|]*)\|"),     # between | and |
+      'protein_name': re.compile(r"\s(.+?)\sOS"),   # between space and space before OS
+      'species': re.compile(r"OS=(.+?)\sOX"),       # between OS= and space before OX
+      'taxon_id': re.compile(r"OX=(.+?)\s"),        # between OX= and space
+      'gene': re.compile(r"GN=(.+?)\s"),            # between GN= and space
+      'pe_level': re.compile(r"PE=(.+?)\s"),        # between PE= and space
+      'sequence_version': re.compile(r"SV=(.+?)\s"),# between SV= and space
+      'gene_priority': re.compile(r"GP=(.+?)\s"),   # between GP= and space
   }
   metadata = []
   for key in regexes: # loop through compiled regexes to extract metadata
     match = regexes[key].search(str(record.description))
     
     if match:
       metadata.append(match.group(1))
```

### Comparing `pepmatch-0.9.1/pepmatch/matcher.py` & `pepmatch-0.9.2/pepmatch/matcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import argparse
 import _pickle as pickle
 import sqlite3
 import pandas as pd
 import numpy as np
 
+from typing import Union
 from collections import Counter, defaultdict
 from Levenshtein import hamming
 
 from .helpers import parse_fasta, split_sequence, extract_metadata
 from .preprocessor import Preprocessor
 
 
@@ -43,115 +44,138 @@
                output_format='csv',
                output_name=''):
 
     if k < 0 or k == 1:
       raise ValueError('Invalid k value given. k cannot be negative or 1.')
 
     if output_format not in VALID_OUTPUT_FORMATS:
-      raise ValueError('Invalid output format, please choose `dataframe`, `csv`, `xlsx`, `json`, or `html`.')
+      raise ValueError(
+        'Invalid output format, please choose `dataframe`, '
+        '`csv`, `xlsx`, `json`, or `html`.'
+      )
 
     # initialize query and output name based on input type
     self.query = self._initialize_query(query, proteome_file, output_name)
     self.proteome = proteome_file
     self.proteome_name = proteome_file.split('/')[-1].split('.')[0]
 
     # discontinuous epitopes and linear epitopes handling - store separately
     self.discontinuous_epitopes = self._find_discontinuous_epitopes()
     self.query = self._clean_query()
-    assert self.query, 'Query is empty. Please check your input.'
+    
+    assert self.query or self.discontinuous_epitopes, 'Query is empty.'
     
     self.lengths = sorted(set(len(peptide) for peptide in self.query))
     self.max_mismatches = max_mismatches
     self.preprocessed_files_path = preprocessed_files_path
     self.best_match = best_match
     self.output_format = output_format
 
     # select format based on # of mismatches to pass to Preprocessor
     # SQLite for exact matching - pickle for mismatching
     self.preprocess_format = 'sql' if not max_mismatches else 'pickle'
     
     # initialize k and k_specified
-    self.k, self.k_specified = self._initialize_k(k)
+    if self.query:
+      self.k, self.k_specified = self._initialize_k(k)
 
     # for mismatching, if no k is specified, batch the peptides by length
     # then later we will use the ideal k to search them
     if max_mismatches > 0:
       self.batched_peptides = self._batch_query()
 
     # best match where no mismatches is specified means we will preprocess
     # the proteome by the smallest length, try to find exact matches,
     # then preprocess by half the length and search for more and repeat
     # until every peptide in the query has a match
     if max_mismatches == -1:
       self.ks = self._best_match_ks()
 
-  def _initialize_query(self, query, proteome_file, output_name):
-    """Initialize query and output name based on input type."""
+
+  def _initialize_query(
+    self, query: Union[str, list], proteome_file: str, output_name: str
+  ) -> list:
+    """Initialize query and output name based on input type.
+    
+    Args:
+      query: either a FASTA file or a Python list of peptides.
+      proteome_file: the proteome FASTA file.
+      output_name: the name of the output file.
+    """
     if isinstance(query, list):
       if output_name:
         self.output_name = output_name
       else:
         self.output_name = 'PEPMatch_results'
       
       return [seq.upper() for seq in query]
     
     else: # parse from FASTA if not Python list
       parsed_query = [str(record.seq) for record in parse_fasta(query)]
       if output_name:
         self.output_name = output_name
       else: # output_name = query_name_to_proteome_name
-        self.output_name = f"{query.split('/')[-1].split('.')[0]}_to_{proteome_file.split('/')[-1].split('.')[0]}"
-      
+        query_name = query.split('/')[-1].split('.')[0]
+        proteome_name = proteome_file.split('/')[-1].split('.')[0]
+        self.output_name = f'{query_name}_to_{proteome_name}'
+
       return [seq.upper() for seq in parsed_query]
 
-  def _find_discontinuous_epitopes(self):
+
+  def _find_discontinuous_epitopes(self) -> list:
     """Find discontinuous epitopes in query and store separately."""
     discontinuous_epitopes = []
     for peptide in self.query:
       try:
         discontinuous_epitope = [(x[0], int(x[1:])) for x in peptide.split(', ')]
         discontinuous_epitopes.append(discontinuous_epitope)
       except ValueError:
         continue
 
     return discontinuous_epitopes
 
-  def _clean_query(self):
+  def _clean_query(self) -> list:
     """Remove discontinous epitopes from query."""
-    query_without_discontinuous_epitopes = set(self.query) - set([', '.join([x[0] + str(x[1]) for x in self.discontinuous_epitopes[i]]) for i in range(len(self.discontinuous_epitopes))])
-    return list(query_without_discontinuous_epitopes)
+    epitopes = self.discontinuous_epitopes
+    discontinuous_epitope_strings = [
+      ', '.join([x[0] + str(x[1]) for x in epitopes[i]]) for i in range(len(epitopes))
+    ]
+    query_filtered = set(self.query) - set(discontinuous_epitope_strings)
+    return list(query_filtered)
   
-  def _initialize_k(self, k):
-    """Initialize k and k_specified values based on k and max_mismatches input."""
+  def _initialize_k(self, k: int) -> tuple:
+    """Initialize k and k_specified values based on k and max_mismatches input.
+    
+    Args:
+      k: the k-mer length to use for matching, 0 if not specified.
+    """
     if k > 1:
       return k, True
-    else: # use the length of the shortest peptide when k is not specified and exact matching is requested
+    else: # use the length of the shortest peptide for exact match 
       if not self.max_mismatches and not k:
         return self.lengths[0], False
       else:
         return 0, False
 
-  def _batch_query(self):
-    """
-    Batch peptides together by ideal k so it can be used when searching.
+  def _batch_query(self) -> dict:
+    """Batch peptides together by ideal k so it can be used when searching.
     If k is specified, just return the query as a dictionary with k as the key.
     """
     if self.k_specified:
       return {self.k: self.query}
     else:
       batched_peptides = defaultdict(list)
       for seq in self.query:
         key = len(seq) // (self.max_mismatches + 1)
         batched_peptides[key].append(seq)
       
       return dict(batched_peptides)
 
-  def _best_match_ks(self):
-    """
-    For the special case where mismatching is to be done, k is not 
+  def _best_match_ks(self) -> list:
+    """For the special case where mismatching is to be done, k is not 
     specified and best match is selected, we need to get all the k values
     to preprocess the proteome multiple times. Starting with the length 
     of the smallest peptide and then halving until we get to 2.
     """
     initial_k = self.lengths[0]
     ks = [initial_k]
 
@@ -166,17 +190,16 @@
         ks.append(initial_k)
 
     # mismatching function uses batched peptides, for best match, batch into one
     self.batched_peptides = {0: self.query}
 
     return ks
 
-  def match(self):
-    """
-    Overarching function that calls the appropriate search matching function
+  def match(self) -> list:
+    """Overarching function that calls the appropriate search matching function
     based on the parameters.
     """
     if self.query:
       
       if self.max_mismatches == -1:
         query_df = self._dataframe_matches(self.best_match_search())
 
@@ -201,87 +224,112 @@
     # return a dataframe instead of outputting file if specified
     if self.output_format == 'dataframe':
       return df
     
     else:
       self._output_matches(df)
 
-  def exact_match_search(self):
-    """
-    Using preprocessed data within a SQLite database and the query peptides,
+  def exact_match_search(self) -> list:
+    """Using preprocessed data within a SQLite database and the query peptides,
     find the peptide matches within the proteome without any residue 
     substitutions. 
     """
-    if not os.path.isfile(os.path.join(self.preprocessed_files_path, self.proteome_name + '.db')):
+    preprocessed_db = os.path.join(
+      self.preprocessed_files_path, self.proteome_name + '.db'
+    )
+    if not os.path.isfile(preprocessed_db):
       Preprocessor(self.proteome).sql_proteome(self.k)
 
     kmers_table_name = f'{self.proteome_name}_{str(self.k)}mers'
     metadata_table_name = f'{self.proteome_name}_metadata'
 
-    conn = sqlite3.connect(os.path.join(self.preprocessed_files_path, f'{self.proteome_name}.db'))
+    conn = sqlite3.connect(
+      os.path.join(self.preprocessed_files_path, f'{self.proteome_name}.db')
+    )
     cursor = conn.cursor()
 
     all_matches = []
     for peptide in self.query:
       
       if len(peptide) < self.k:
         continue
 
       # split peptide into kmers - only use kmers necessary that overlap entire peptide
       all_kmers = split_sequence(peptide, self.k)
       target_kmers = self._get_target_kmers(all_kmers)
 
       # SQL fetch
       sql_placeholders = ', '.join('?' * len(target_kmers))
-      sql_query = f'SELECT kmer, idx FROM "{kmers_table_name}" WHERE kmer IN ({sql_placeholders})'
+      sql_query = f"""
+                   SELECT kmer, idx FROM "{kmers_table_name}" 
+                   WHERE kmer IN ({sql_placeholders})
+                   """
       cursor.execute(sql_query, target_kmers)
       kmer_indexes = cursor.fetchall()
 
       kmer_hit_list = []
       for kmer, index in kmer_indexes:
         kmer_hit_list.append(index - all_kmers.index(kmer))
 
-      peptide_matches = []
+      matches = []
       sum_hits = Counter(kmer_hit_list)
       for hit, count in sum_hits.items():
-        if count == len(target_kmers): # number of index recordings that agree with the number of kmers used
-          peptide_matches.append(hit)
+        if count == len(target_kmers): # number of index recordings that 
+          matches.append(hit)  # agree with the number of kmers used
 
-      processed_matches = self._process_exact_matches(peptide, peptide_matches, cursor, metadata_table_name)
+      processed_matches = self._process_exact_matches(
+        peptide, matches, cursor, metadata_table_name
+      )
       all_matches.extend(processed_matches)
 
     cursor.close()
     conn.close()
 
     return all_matches
 
-  def _get_target_kmers(self, all_kmers):
-    """Return the target kmers that overlap the entire peptide."""
+  def _get_target_kmers(self, all_kmers: list) -> list:
+    """Return the target kmers that overlap the entire peptide.
+    
+    Args:
+      all_kmers: all possible kmers of the query peptide for a given k.
+    """
     if len(all_kmers) == self.k:
         return all_kmers
 
     target_kmers = all_kmers[::self.k]
     if all_kmers[-1] != target_kmers[-1]:
         target_kmers.append(all_kmers[-1])
     return target_kmers
 
-  def _process_exact_matches(self, peptide, peptide_matches, cursor, metadata_table_name):
-    """Extract all metadata for the exact matches and return as a list of tuples."""
+  def _process_exact_matches(
+    self, peptide: str, matches: list, cursor: sqlite3.Cursor, metadata_table_name: str
+  ) -> list:
+    """Extract all metadata for the exact matches and return as a list of tuples.
+    
+    Args:
+      peptide: the query peptide.
+      matches: the list of exact matches for the peptide.
+      cursor: the cursor object to execute SQL queries.
+      metadata_table_name: the name of the metadata table in the database.
+    """
     all_matches = []
-    if not peptide_matches:
+    if not matches:
       all_matches.append((peptide,) + (np.nan,) * 13)
     else:
-      for match in peptide_matches:
+      for match in matches:
         protein_number = (match - (match % 1000000)) // 1000000
-        query = f'SELECT * FROM "{metadata_table_name}" WHERE protein_number = "{protein_number}"'
+        query = f"""SELECT * 
+                 FROM "{metadata_table_name}" 
+                 WHERE protein_number = "{protein_number}"
+                 """
         cursor.execute(query)
         protein_data = cursor.fetchone()
         match_data = (
           peptide,                          # query peptide
-          peptide,                          # matched peptide (same as query for exact)
+          peptide,                          # matched peptide (same as query)
           protein_data[1],                  # protein ID
           protein_data[2],                  # protein name
           protein_data[3],                  # species
           protein_data[4],                  # taxon ID
           protein_data[5],                  # gene symbol
           0,                                # 0 mismatches for exact match
           [],                               # mutated positions (none)
@@ -291,239 +339,320 @@
           protein_data[7],                  # sequence version
           protein_data[8])                  # gene priority flag
         
         all_matches.append(match_data)
 
     return all_matches
 
-  def mismatch_search(self):
-    """
-    Using preprocessed data within a serialized pickle files, the query
+  def mismatch_search(self) -> list:
+    """Using preprocessed data within a serialized pickle files, the query
     peptides, and a maximum number of residue substitutions, find all peptide
     matches up to and including the maximum number of residue substitutions.
 
     This will utilize the pigeon hole principle to find all possible matches.
     We first search for any k-mer exact matches in the proteome and then
     check the left and right k-mer neighbors for mismatches. If the number of
     mismatches is less than or equal to the max, then it's a match.
     """
     all_matches = []
-    for k, peptides in self.batched_peptides.items(): # iterate through each batch - k: [peptides]
-      if not self.k_specified:
+    for k, peptides in self.batched_peptides.items(): # iterate through each batch
+      if not self.k_specified:                        # k: [peptides]
         self.k = k
 
-      try: # read in the preprocessed pickle files - create reverse kmer dictionary for neighbor seaches - index: kmer
+      try: # read in the preprocessed pickle files and create index: kmer dict
         kmer_dict, metadata_dict = self._read_pickle_files()
         rev_kmer_dict = {i: k for k, v in kmer_dict.items() for i in v}
       except FileNotFoundError: # do preprocessing if pickle files don't exist
         Preprocessor(self.proteome).pickle_proteome(self.k)
         kmer_dict, metadata_dict = self._read_pickle_files()
         rev_kmer_dict = {i: k for k, v in kmer_dict.items() for i in v}
 
       for peptide in peptides:
 
         all_kmers = split_sequence(peptide, self.k)
 
         # faster search if possible
         if len(peptide) % self.k == 0:
-          peptide_matches = self._find_even_split_matches(all_kmers, kmer_dict, rev_kmer_dict, len(peptide))
+          matches = self._find_even_split_matches(
+            all_kmers, kmer_dict, rev_kmer_dict, len(peptide)
+          )
 
         # slower search if necessary
         else:
-          peptide_matches = self._find_uneven_split_matches(all_kmers, kmer_dict, rev_kmer_dict, len(peptide))
-
-        processed_matches = self._process_mismatch_matches(peptide, peptide_matches, metadata_dict)
+          matches = self._find_uneven_split_matches(
+            all_kmers, kmer_dict, rev_kmer_dict, len(peptide)
+          )
+
+        processed_matches = self._process_mismatch_matches(
+          peptide, matches, metadata_dict
+        )
         all_matches.extend(processed_matches)
     
     return all_matches
 
-  def _read_pickle_files(self):
-    """
-    Read in the already created pickle files for each dictionary in the
+  def _read_pickle_files(self) -> tuple:
+    """Read in the already created pickle files for each dictionary in the
     preprocessing step.
     """
     with open(os.path.join(self.preprocessed_files_path, 
       f'{self.proteome_name}_{str(self.k)}mers.pickle'), 'rb') as f:
       kmer_dict = pickle.load(f)
 
     with open(os.path.join(self.preprocessed_files_path, 
       f'{self.proteome_name}_metadata.pickle'), 'rb') as f:
       names_dict = pickle.load(f)
 
     return kmer_dict, names_dict
 
-  def _find_even_split_matches(self, kmers, kmer_dict, rev_kmer_dict, peptide_length):
-    """
-    If the peptide length is evenly divisible by k, perform faster search. 
+  def _find_even_split_matches(
+    self, kmers: list, kmer_dict: dict, rev_kmer_dict: dict, peptide_length: int
+  ) -> list:
+    """If the peptide length is evenly divisible by k, perform faster search. 
     Check the associated k-mers for the left and right neighbors of any 
     exact matching k-mers in the proteome.
     
     EXAMPLE: "YLLDLHSYL", k=3 -> check only ["YLL", "DLH", "SYL"]. 
     If, say "DLH" is found somewhere in the proteome, check the neighboring
     k-mers to the left and right to see if "YLL" (left neighbor) and "SYL" 
     (right neighbor) have mismatches with the proteome k-mers, return any
     matches that are less than or equal to self.max_mismatches.
+
+    Args:
+      kmers: the k-mers of the query peptide.
+      kmer_dict: the k-mer -> index dictionary.
+      rev_kmer_dict: the index -> k-mer dictionary.
+      peptide_length: the length of the query peptide.
     """
-    peptide_matches = set()
+    matches = set()
     for idx in range(0, len(kmers), self.k): # gets only the k-mers to check
       try: # try to find an exact match hit for each k-mer
         for kmer_hit in kmer_dict[kmers[idx]]:
 
           mismatches = 0
-          mismatches = self._check_left_neighbors(kmers, idx, kmer_hit, rev_kmer_dict, mismatches)
+          mismatches = self._check_left_neighbors(
+            kmers, idx, kmer_hit, rev_kmer_dict, mismatches
+          )
 
           if not mismatches > self.max_mismatches:
-            mismatches = self._check_right_neighbors(kmers, idx, kmer_hit, rev_kmer_dict, mismatches)
+            mismatches = self._check_right_neighbors(
+              kmers, idx, kmer_hit, rev_kmer_dict, mismatches
+            )
           else:
             continue
           
           if mismatches <= self.max_mismatches:
-            matched_peptide = ''
-            for i in range(0, peptide_length, self.k): # add each proteome k-mer to get the full peptide
+            matched_peptide = '' # add k-mers to get the matched peptide 
+            for i in range(0, peptide_length, self.k): 
               matched_peptide += rev_kmer_dict[kmer_hit - idx + i]
 
-            peptide_matches.add((matched_peptide, mismatches, kmer_hit - idx))
+            matches.add((matched_peptide, mismatches, kmer_hit - idx))
 
-            # in case match is 0 mismatches and self.best_match is True, return right away
-            if self.best_match and not mismatches:
-              return list(peptide_matches)
+            if self.best_match and not mismatches: # can't have a better match
+              return list(matches)
           
           else:
             continue
       
       except KeyError:
         continue
     
-    return list(peptide_matches)
+    return list(matches)
 
-  def _find_uneven_split_matches(self, kmers, kmer_dict, rev_kmer_dict, peptide_length):
-    """
-    If the peptide length is NOT evenly divisible by k, perform slow search. 
+  def _find_uneven_split_matches(
+    self, kmers: list, kmer_dict: dict, rev_kmer_dict: dict, peptide_length: int
+  ) -> list:
+    """If the peptide length is NOT evenly divisible by k, perform slow search. 
     Check the associated residues for the left and right neighbors of any 
     exact matching k-mers in the proteome.
     
     EXAMPLE: "YLLDLHSYL", k=3 -> check all k-mers: 
     ["YLL", "LLD", "LDL", "DLH", "LHS", "HSY", "SYL"].
     
     If, say "DLH" is found somewhere in the proteome, check left "L" from "LDL",
     left "L" from "LLD", and "Y" from "YLL" to for any mismatches. Then do the 
     same for the residues of the right neighbors. Return any matches that are
     less than or equal to self.max_mismatches.
+
+    Args:
+      kmers: the k-mers of the query peptide.
+      kmer_dict: the k-mer -> index dictionary.
+      rev_kmer_dict: the index -> k-mer dictionary.
+      peptide_length: the length of the query peptide.
     """
-    peptide_matches = set()
+    matches = set()
     for idx in range(0, len(kmers)): # every k-mer
       try: # try to find an exact match hit for each k-mer
         for kmer_hit in kmer_dict[kmers[idx]]:
 
           mismatches = 0
-          mismatches = self._check_left_residues(kmers, idx, kmer_hit, rev_kmer_dict, mismatches)
+          mismatches = self._check_left_residues(
+            kmers, idx, kmer_hit, rev_kmer_dict, mismatches
+          )
 
           if not mismatches > self.max_mismatches:
-            mismatches = self._check_right_residues(kmers, idx, kmer_hit, rev_kmer_dict, mismatches)
+            mismatches = self._check_right_residues(
+              kmers, idx, kmer_hit, rev_kmer_dict, mismatches
+            )
             
           else:
             continue
           
           if mismatches <= self.max_mismatches:
             matched_peptide = rev_kmer_dict[kmer_hit - idx] # add the first k-mer
             for i in range(self.k - 1, peptide_length):
-              matched_peptide += rev_kmer_dict[kmer_hit - idx + i][-1] # add the last residue of each remaining k-mer
+              # add the last residue of each remaining k-mer
+              matched_peptide += rev_kmer_dict[kmer_hit - idx + i][-1]
 
             matched_peptide = matched_peptide[0:peptide_length]
-            peptide_matches.add((matched_peptide, mismatches, kmer_hit - idx))
+            matches.add((matched_peptide, mismatches, kmer_hit - idx))
 
-            # in case match is 0 mismatches and self.best_match is True, return right away
-            if self.best_match and not mismatches:
-              return peptide_matches
+            if self.best_match and not mismatches: # can't have a better match
+              return matches
 
       except KeyError:
         continue
 
-    return peptide_matches
+    return matches
 
-  def _check_left_neighbors(self, kmers, idx, kmer_hit, rev_kmer_dict, mismatches):
-    """Get mismatches of left k-mer neighbors in proteome."""
+  def _check_left_neighbors(
+    self, kmers: list, idx: int, kmer_hit: int, rev_kmer_dict: dict, mismatches: int
+  ) -> int:
+    """Get mismatches of left k-mer neighbors in proteome.
+    
+    Args:
+      kmers: the k-mers of the query peptide.
+      idx: the index of the k-mer in the query peptide.
+      kmer_hit: the index of the k-mer hit in the proteome.
+      rev_kmer_dict: the index -> k-mer dictionary.
+      mismatches: the number of mismatches so far.
+    """
     for i in range(0, idx, self.k):
       try: # get proteome k-mer from reverse dictionary and check associated query k-mer
         mismatches += hamming(rev_kmer_dict[kmer_hit + i - idx], kmers[i])
         if mismatches > self.max_mismatches:
           return 100
       except KeyError:
         return 100
     
     return mismatches
 
-  def _check_right_neighbors(self, kmers, idx, kmer_hit, rev_kmer_dict, mismatches):
-    """Get mismatches of right k-mer neighbors in proteome."""
+  def _check_right_neighbors(
+    self, kmers: list, idx: int, kmer_hit: int, rev_kmer_dict: dict, mismatches: int
+  ) -> int:
+    """Get mismatches of right k-mer neighbors in proteome.
+    
+    Args:
+      kmers: the k-mers of the query peptide.
+      idx: the index of the k-mer in the query peptide.
+      kmer_hit: the index of the k-mer hit in the proteome.
+      rev_kmer_dict: the index -> k-mer dictionary.
+      mismatches: the number of mismatches so far.
+    """
     for i in range(self.k + idx, len(kmers), self.k):
       try: # get proteome k-mer from reverse dictionary and check associated query k-mer
         mismatches += hamming(rev_kmer_dict[kmer_hit + i - idx], kmers[i])
         if mismatches > self.max_mismatches:
           return 100
       except KeyError:
         return 100
     
     return mismatches
 
-  def _check_left_residues(self, kmers, idx, kmer_hit, rev_kmer_dict, mismatches):
-    """Get mismatches of left residues of left k-mer neighbors in proteome."""
+  def _check_left_residues(
+    self, kmers: list, idx: int, kmer_hit: int, rev_kmer_dict: dict, mismatches: int
+  ) -> int:
+    """Get mismatches of left residues of left k-mer neighbors in proteome.
+    
+    Args:
+      kmers: the k-mers of the query peptide.
+      idx: the index of the k-mer in the query peptide.
+      kmer_hit: the index of the k-mer hit in the proteome.
+      rev_kmer_dict: the index -> k-mer dictionary.
+      mismatches: the number of mismatches so far.
+    """
     for i in range(0, idx):
-      try: # get proteome residue from reverse dictionary and check associated query residue
+      try: # get proteome residue from reverse dict and check associated query residue
         if rev_kmer_dict[kmer_hit + i - idx][0] != kmers[i][0]:
           mismatches += 1
         if mismatches > self.max_mismatches:
           return 100
       except KeyError:
         return 100
     
     return mismatches
 
-  def _check_right_residues(self, kmers, idx, kmer_hit, rev_kmer_dict, mismatches):
-    """Get mismatches of right residues of right k-mer neighbors in proteome."""
+  def _check_right_residues(
+    self, kmers: list, idx: int, kmer_hit: int, rev_kmer_dict: dict, mismatches: int
+  ) -> int:
+    """Get mismatches of right residues of right k-mer neighbors in proteome.
+    
+    Args:
+      kmers: the k-mers of the query peptide.
+      idx: the index of the k-mer in the query peptide.
+      kmer_hit: the index of the k-mer hit in the proteome.
+      rev_kmer_dict: the index -> k-mer dictionary.
+      mismatches: the number of mismatches so far.
+    """
     for i in range(idx + 1, len(kmers)):
-      try: # get proteome residue from reverse dictionary and check associated query residue
+      try: # get proteome residue from reverse dict and check associated query residue
         if rev_kmer_dict[kmer_hit + i - idx][-1] != kmers[i][-1]:
           mismatches += 1
         if mismatches > self.max_mismatches:
           return 100
       except KeyError:
         return 100
     
     return mismatches
 
-  def _process_mismatch_matches(self, peptide, peptide_matches, metadata_dict):
-    """Extract all metadata for the mismatch matches and return as a list of tuples."""
+  def _process_mismatch_matches(
+    self, peptide: str, matches: list, metadata_dict: dict
+  ) -> list:
+    """Extract all metadata for the mismatch matches and return as a list of tuples.
+    
+    Args:
+      peptide: the query peptide.
+      matches: the list of mismatch matches for the peptide.
+      metadata_dict: the protein number -> metadata dictionary.
+    """
     all_matches = []
-    if not peptide_matches:
+    if not matches:
       all_matches.append((peptide,) + (np.nan,) * 13)
     else:
-      for match in peptide_matches:
+      for match in matches:
+        metadata_key = (match[2] - (match[2] % 1000000)) // 1000000
+        metadata = metadata_dict[metadata_key]
+
+        mutated_positions = [
+          i+1 for i in range(len(peptide)) if peptide[i] != match[0][i]
+        ]
+        index_start = int((match[2] % 1000000) + 1)
+        index_end = int((match[2] % 1000000) + len(peptide))
+
         match_data = (
-          peptide,                                                         # query peptide
-          match[0],                                                        # matched peptide
-          metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][0],  # protein ID
-          metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][1],  # protein name
-          metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][2],  # species
-          int(metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][3]), # taxon ID
-          metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][4],  # gene symbol
-          int(match[1]),                                                   # mismatches count
-          [i+1 for i in range(len(peptide)) if peptide[i] != match[0][i]], # mutated positions
-          int((match[2] % 1000000) + 1),                                   # index start
-          int((match[2] % 1000000) + len(peptide)),                        # index end
-          int(metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][5]), # protein existence level
-          metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][6],  # sequence version
-          metadata_dict[(match[2] - (match[2] % 1000000)) // 1000000][7])  # gene priority flag
-        
+            peptide,                      # query peptide
+            match[0],                     # matched peptide
+            metadata[0],                  # protein ID
+            metadata[1],                  # protein name
+            metadata[2],                  # species
+            int(metadata[3]),             # taxon ID
+            metadata[4],                  # gene symbol
+            int(match[1]),                # mismatches count
+            mutated_positions,            # mutated positions
+            index_start,                  # index start
+            index_end,                    # index end
+            int(metadata[5]),             # protein existence level
+            metadata[6],                  # sequence version
+            metadata[7]                   # gene priority flag
+        )
         all_matches.append(match_data)
 
     return all_matches
 
-  def best_match_search(self):
-    """
-    After calculating the splits we would need (starting with lowest peptide
+  def best_match_search(self) -> list:
+    """After calculating the splits we would need (starting with lowest peptide
     length in query), we can then call the mismatch_search function. We use
     the maximum # of mismatches calculated from the each length and split.
     """
     all_matches = []
     for k in self.ks:
       self.k = k
       self.k_specified = True
@@ -564,114 +693,143 @@
           self.max_mismatches += 1
       
       # reset batched peptides
       self.batched_peptides = {0: self.query}
 
     return all_matches
 
-  def discontinuous_search(self):
+  def discontinuous_search(self) -> list:
     """Find matches for discontinuous epitopes."""
     all_matches = []
-    for discontinuous_epitope in self.discontinuous_epitopes:
+    for dis_epitope in self.discontinuous_epitopes:
       for protein_record in parse_fasta(self.proteome):
         try:
-          residue_matches = sum([x[0] == protein_record.seq[x[1] - 1] for x in discontinuous_epitope])
-          if residue_matches >= (len(discontinuous_epitope) - self.max_mismatches):
+          residue_matches = sum(
+            [x[0] == protein_record.seq[x[1] - 1] for x in dis_epitope]
+          )
+          if residue_matches >= (len(dis_epitope) - self.max_mismatches):
             metadata = extract_metadata(protein_record)
             match_data = (
-              ', '.join(   # query epitope
-                [x[0] + str(x[1]) for x in discontinuous_epitope]), 
-              ', '.join(   # matched epitope
-                [protein_record.seq[x[1] - 1] + str(x[1]) for x in discontinuous_epitope]), 
-              metadata[0], # protein ID
-              metadata[1], # protein name                  
-              metadata[2], # species               
-              metadata[3], # taxon ID              
-              metadata[4], # gene symbol       
-              len(discontinuous_epitope) - residue_matches, # mismatches count         
-              [x[1] for x in discontinuous_epitope if x[0] != protein_record.seq[x[1] - 1]], # mutated positions
-              discontinuous_epitope[0][1],  # index start           
-              discontinuous_epitope[-1][1], # index end  
-              metadata[5], # protein existence level         
-              metadata[6], # sequence version       
-              metadata[7]) # gene priority flag
+              ', '.join(                                    # query epitope
+                [x[0] + str(x[1]) for x in dis_epitope]),
+              ', '.join(                                    # matched epitope
+                [protein_record.seq[x[1] - 1] + str(x[1]) for x in dis_epitope]), 
+              metadata[0],                                  # protein ID
+              metadata[1],                                  # protein name
+              metadata[2],                                  # species
+              metadata[3],                                  # taxon ID
+              metadata[4],                                  # gene symbol
+              len(dis_epitope) - residue_matches,           # mismatches count
+                                                            # mutated positions
+              [x[1] for x in dis_epitope if x[0] != protein_record.seq[x[1] - 1]],
+              dis_epitope[0][1],                            # index start
+              dis_epitope[-1][1],                           # index end
+              metadata[5],                                  # protein existence level
+              metadata[6],                                  # sequence version
+              metadata[7])                                  # gene priority flag
             
             all_matches.append(match_data)
         
         except IndexError:
           continue
     
     return all_matches
 
-  def _dataframe_matches(self, all_matches):
-    """Return Pandas dataframe of the results."""
+  def _dataframe_matches(self, all_matches: list) -> pd.DataFrame:
+    """Return Pandas dataframe of the results.
+    
+    Args:
+      all_matches: the list of all matches for all peptides.
+    """
     df = pd.DataFrame(all_matches,
-                      columns=['Query Sequence', 'Matched Sequence', 'Protein ID', 
+                      columns=['Query Sequence', 'Matched Sequence', 'Protein ID',
                                'Protein Name', 'Species', 'Taxon ID', 'Gene',
                                'Mismatches', 'Mutated Positions','Index start',
-                               'Index end', 'Protein Existence Level', 'Sequence Version',
-                               'Gene Priority'])
+                               'Index end', 'Protein Existence Level',
+                               'Sequence Version', 'Gene Priority'])
 
     if self.best_match:
-      def filter_fragments(group):
-        """
-        Takes out matches with 'Fragment' in the protein name if there are other
+      def filter_fragments(group: pd.DataFrame) -> pd.DataFrame:
+        """Takes out matches with 'Fragment' in the protein name if there are other
         matches without 'Fragment'.
+
+        Args:
+          group: the group of matches for a given query peptide.
         """
+        group['Protein Name'] = group['Protein Name'].astype(str)
         no_fragments = group[~group['Protein Name'].str.contains('Fragment')]
         if len(no_fragments) > 0:
           return no_fragments
         else:
           return group
 
-      # take matches with the least number of mismatches   
-      idx = df.groupby(['Query Sequence'])['Mismatches'].transform(min) == df['Mismatches']
+      idx = df.groupby( # take matches with the least number of mismatches   
+        ['Query Sequence']
+      )['Mismatches'].transform(min) == df['Mismatches']
       df = df[idx]
 
-      # take matches that are in the gene priority proteome and with the best protein
-      # existence level - first fill NaN values with 0 - otherwise pandas will drop the rows
-      df[['Gene Priority', 'Protein Existence Level']] = df[['Gene Priority','Protein Existence Level']].fillna(value=0)
-      
-      idx = df.groupby(['Query Sequence'])['Gene Priority'].transform(max) == df['Gene Priority']
+      # fill NaN values with 0 - otherwise pandas will drop the rows
+      df[['Gene Priority', 'Protein Existence Level']] = df[
+         ['Gene Priority', 'Protein Existence Level']
+      ].fillna(value=0)
+
+      # take matches that are in the gene priority proteome 
+      idx = df.groupby(
+        ['Query Sequence']
+      )['Gene Priority'].transform(max) == df['Gene Priority']
       df = df[idx]
-
-      idx = df.groupby(['Query Sequence'])['Protein Existence Level'].transform(min) == df['Protein Existence Level']
+      
+      # and with the best protein existence level
+      idx = df.groupby(
+        ['Query Sequence']
+      )['Protein Existence Level'].transform(min) == df['Protein Existence Level']
       df = df[idx]
 
       # filter fragments
-      df = df.groupby('Query Sequence', group_keys=False).apply(filter_fragments).reset_index(drop=True)
+      df = df.groupby(
+        'Query Sequence', group_keys=False
+      ).apply(filter_fragments).reset_index(drop=True)
 
       # sort values by protein ID and drop duplicates, guaranteeing same results 
       df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start'], inplace=True)
       df.drop_duplicates(['Query Sequence'], inplace=True)
 
     # combine protein ID and sequence version
-    df['Sequence Version'] = df['Sequence Version'].apply(lambda x: f'.{int(x)}' if not pd.isna(x) else '')   
+    df['Sequence Version'] = df[
+       'Sequence Version'
+    ].apply(lambda x: f'.{int(x)}' if not pd.isna(x) else '')   
     df['Protein ID'] = df['Protein ID'] + df['Sequence Version']
     
     # drop "Sequence Version" and "Gene Priority" columns
     df.drop(columns=['Sequence Version'], inplace=True)
     df.drop(columns=['Gene Priority'], inplace=True)
 
     # force integers on some columns
-    int_cols = ['Taxon ID', 'Mismatches', 'Index start', 'Index end', 'Protein Existence Level']
+    int_cols = [
+      'Taxon ID', 'Mismatches', 'Index start', 'Index end', 'Protein Existence Level'
+    ]
     df[int_cols] = df[int_cols].astype('Int64')
 
     return df
 
-  def _output_matches(self, df):
-    """Write Pandas dataframe to format that is specified"""
+  def _output_matches(self, df: pd.DataFrame) -> None:
+    """Write Pandas dataframe to format that is specified
+    
+    Args:
+      df: the dataframe of the matches.
+    """
+    path = f'{self.preprocessed_files_path}/{self.output_name}'
     if self.output_format == 'csv':
-      return df.to_csv(f'{self.preprocessed_files_path}/{self.output_name}.csv', index=False)
+      return df.to_csv(f'{path}.csv', index=False)
     elif self.output_format == 'xlsx':
-      return df.to_excel(f'{self.preprocessed_files_path}/{self.output_name}.xlsx', index=False)
+      return df.to_excel(f'{path}.xlsx', index=False)
     elif self.output_format == 'json':
-      return df.to_json(f'{self.preprocessed_files_path}/{self.output_name}.json', index=False)
+      return df.to_json(f'{path}.json', index=False)
     elif self.output_format == 'html':
-      return df.to_html(f'{self.preprocessed_files_path}/{self.output_name}.html', index=False)
+      return df.to_html(f'{path}.html', index=False)
 
 
 
 # run via command line
 
 def parse_arguments():
   parser = argparse.ArgumentParser()
```

### Comparing `pepmatch-0.9.1/pepmatch/preprocessor.py` & `pepmatch-0.9.2/pepmatch/preprocessor.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,18 +48,23 @@
 
     # extracting the proteome name from the file path
     self.proteome_name = proteome.split('/')[-1].split('.')[0]
 
     # extract all the data from the proteome
     self.all_seqs, self.all_metadata = self._get_data_from_proteome()
 
-  def _append_gp_to_header(self, proteome, gene_priority_proteome):
-    """
-    Appends GP=1 or GP=0 to the FASTA header of a proteome depending on
+  def _append_gp_to_header(
+    self, proteome: str, gene_priority_proteome: str
+  ) -> list:
+    """Appends GP=1 or GP=0 to the FASTA header of a proteome depending on
     if the protein is in the gene priority proteome.
+
+    Args:
+      proteome: path to proteome FASTA file.
+      gene_priority_proteome: path to gene priority proteome FASTA file.
     """
     proteome_records = parse_fasta(proteome) # get regular proteome
     try: # try to get gene priority proteome
       gp_proteome_records = parse_fasta(gene_priority_proteome)
     except FileNotFoundError:
       gp_proteome_records = []
 
@@ -79,17 +84,16 @@
         GP = 'GP=0 '
 
       record.description += f' {GP}' # append notation to FASTA header
       records.append(record)
 
     return records
 
-  def _get_data_from_proteome(self):
-    """
-    Extract all the data from a FASTA file and returns two lists:
+  def _get_data_from_proteome(self) -> tuple:
+    """Extract all the data from a FASTA file and returns two lists:
 
     Use extract_metadata_from_fasta_header in helpers.py.
 
     1. A list of sequences
     2. A list of metadata in tuples. The metadata includes the protein ID,
        protein name, species, taxon ID, gene, protein existence level,
        sequence version, and gene priority label. 
@@ -104,40 +108,53 @@
       metadata.extend(extract_metadata(record))
 
       all_metadata.append(tuple(metadata))
       protein_number += 1
 
     return all_seqs, all_metadata
 
-  def sql_proteome(self, k):
-    """
-    Writes the kmers_table and metadata_table to a SQLite database.
+  def sql_proteome(self, k: int) -> None:
+    """Writes the kmers_table and metadata_table to a SQLite database.
+    
+    Args:
+      k: k-mer length to split the proteome into.
     """
     # create table names
     kmers_table = f'{self.proteome_name}_{str(k)}mers'
     metadata_table = f'{self.proteome_name}_metadata'
     
     # connect to database
     db_path = os.path.join(self.preprocessed_files_path, f'{self.proteome_name}.db')
     with sqlite3.connect(db_path) as conn:
       cursor = conn.cursor()
 
       # check if kmers table already exists and exit if it does
       # for some reason writing to the same table multiple times messes up results
-      if cursor.execute(f'SELECT name FROM sqlite_master WHERE type="table" AND name="{kmers_table}";').fetchone():
+      if cursor.execute(
+        f'SELECT name FROM sqlite_master WHERE type="table" AND name="{kmers_table}";'
+      ).fetchone():
         return
 
       self._create_tables(cursor, kmers_table, metadata_table)
       self._insert_kmers(cursor, kmers_table, k)
       self._insert_metadata(cursor, metadata_table)
       self._create_indexes(cursor, kmers_table, metadata_table)
 
       conn.commit()
 
-  def _create_tables(self, cursor, kmers_table, metadata_table):
+  def _create_tables(
+    self, cursor: sqlite3.Cursor, kmers_table: str, metadata_table: str
+  ) -> None:
+    """Creates the kmers_table and metadata_table in the SQLite database.
+
+    Args:
+      cursor: cursor object to execute SQL commands.
+      kmers_table: name of the k-mers table.
+      metadata_table: name of the metadata table.
+    """
     cursor.execute(
       f'CREATE TABLE IF NOT EXISTS {kmers_table} ('\
         'kmer TEXT NOT NULL,'\
         'idx  INTEGER NOT NULL)'
       )
     cursor.execute(
       f'CREATE TABLE IF NOT EXISTS {metadata_table} ('\
@@ -148,57 +165,91 @@
         'taxon_id         INTEGER NOT NULL,'\
         'gene             TEXT NOT NULL,'\
         'pe_level         INTEGER NOT NULL,'\
         'sequence_version INTEGER NOT NULL,'\
         'gene_priority    INTEGER NOT NULL)'\
     )
 
-  def _insert_kmers(self, cursor, kmers_table, k):
+  def _insert_kmers(self, cursor: sqlite3.Cursor, kmers_table: str, k: int) -> None:
+    """Inserts the k-mers into the kmers_table.
+
+    Args:
+      cursor: cursor object to execute SQL commands.
+      kmers_table: name of the k-mers table.
+      k: k-mer length to split the proteome into.
+    """
     kmer_rows = []
     for protein_count, seq in enumerate(self.all_seqs):
         for j, kmer in enumerate(split_sequence(seq, k)):
             kmer_rows.append((kmer, (protein_count + 1) * 1000000 + j))
     cursor.executemany(f'INSERT INTO {kmers_table} VALUES (?, ?)', kmer_rows)
 
-  def _insert_metadata(self, cursor, metadata_table):
-    cursor.executemany(f'INSERT INTO {metadata_table} VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?)', self.all_metadata)
+  def _insert_metadata(self, cursor: sqlite3.Cursor, metadata_table: str) -> None:
+    """Inserts the metadata into the metadata_table.
 
-  def _create_indexes(self, cursor, kmers_table, metadata_table):
-    cursor.execute(f'CREATE INDEX IF NOT EXISTS {kmers_table}_kmer_idx ON {kmers_table} (kmer)')
-    cursor.execute(f'CREATE INDEX IF NOT EXISTS {metadata_table}_protein_number_idx ON {metadata_table} (protein_number)')
+    Args:
+      cursor: cursor object to execute SQL commands.
+      metadata_table: name of the metadata table.
+    """
+    cursor.executemany(
+      f'INSERT INTO {metadata_table} VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?)', 
+      self.all_metadata
+    )
 
-  def pickle_proteome(self, k):
+  def _create_indexes(
+    self, cursor: sqlite3.Cursor, kmers_table: str, metadata_table: str
+  ) -> None:
+    """Creates indexes for the kmers_table and metadata_table.
+
+    Args:
+      cursor: cursor object to execute SQL commands.
+      kmers_table: name of the k-mers table.
+      metadata_table: name of the metadata table.
     """
-    Pickles the proteome into a dictionary of k-mers and a dictionary of metadata.
+    cursor.execute(
+      f'CREATE INDEX IF NOT EXISTS {kmers_table}_kmer_idx ON {kmers_table} (kmer)'
+    )
+    cursor.execute(
+      f'CREATE INDEX IF NOT EXISTS {metadata_table}_protein_number_idx '
+      f'ON {metadata_table} (protein_number)'
+    )
+
+  def pickle_proteome(self, k: int) -> None:
+    """Pickles the proteome into a dictionary of k-mers and a dictionary of metadata.
+
+    Args:
+      k: k-mer length to split the proteome into.
     """
     # create kmer_dict and metadata_dict out of self.all_seqs and self.all_metadata
     kmer_dict = {}
     for protein_count, seq in enumerate(self.all_seqs):
       for j, kmer in enumerate(split_sequence(seq, k)):
-        if kmer in kmer_dict.keys():
-          kmer_dict[kmer].append((protein_count + 1) * 1000000 + j) # add index to k-mer list
-        else:
-          kmer_dict[kmer] = [(protein_count + 1) * 1000000 + j] # create entry for new k-mer
+        if kmer in kmer_dict.keys(): # add index to k-mer list
+          kmer_dict[kmer].append((protein_count + 1) * 1000000 + j) 
+        else: # create entry for new k-mer
+          kmer_dict[kmer] = [(protein_count + 1) * 1000000 + j] 
     
     metadata_dict = {}
     for data in self.all_metadata:
       metadata_dict[data[0]] = data[1:]
     
     # write kmer_dict and metadata_dict to pickle files
     with open(os.path.join(self.preprocessed_files_path, 
       f'{self.proteome_name}_{str(k)}mers.pickle'), 'wb') as f:
       pickle.dump(kmer_dict, f)
 
     with open(os.path.join(self.preprocessed_files_path, 
       f'{self.proteome_name}_metadata.pickle'), 'wb') as f:
       pickle.dump(metadata_dict, f)
 
-  def redis_proteome(self, k):
-    """
-    Writes the k-mers and metadata to a Redis database.
+  def redis_proteome(self, k: int) -> None:
+    """Writes the k-mers and metadata to a Redis database.
+
+    Args:
+      k: k-mer length to split the proteome into.
     """
     import redis
     r = redis.Redis(host='localhost', port=6379, db=0)
 
     # store k-mers
     for protein_count, seq in enumerate(self.all_seqs):
       for j, kmer in enumerate(split_sequence(seq, k)):
@@ -209,33 +260,37 @@
     # store metadata
     for data in self.all_metadata:
       protein_number = data[0]
       metadata_values = ','.join([str(val) for val in data[1:]])
       key = f'metadata:{protein_number}'
       r.set(key, metadata_values)
 
-  def preprocess(self, preprocess_format, k):
-    """
-    Preprocesses the proteome and stores it in the specified format.
-    """
-    if not preprocess_format in ('sql', 'pickle', 'redis'):
-      raise AssertionError('Unexpected value of preprocessing format:', preprocess_format)
+  def preprocess(self, preprocess_format: str, k: int) -> None:
+    """Preprocesses the proteome and stores it in the specified format.
+
+    Args:
+      preprocess_format: format to store the proteome in (sql, pickle, redis).
+      k: k-mer length to split the proteome into.
+    """
+    if preprocess_format not in ('sql', 'pickle', 'redis'):
+      raise AssertionError(
+        'Unexpected value of preprocessing format:', preprocess_format
+      )
 
     assert k >= 2, 'k-sized split is invalid. Cannot be less than 2.'
 
     # store data based on format specified
     if preprocess_format == 'pickle':
       self.pickle_proteome(k)
     elif preprocess_format == 'sql':
       self.sql_proteome(k)
     elif preprocess_format == 'redis':
       self.redis_proteome(k)
 
 
-
 # run via command line
 def parse_arguments():
   parser = argparse.ArgumentParser()
 
   parser.add_argument('-p', '--proteome', required=True)
   parser.add_argument('-k', '--kmer_size', type=int, required=True)
   parser.add_argument('-f', '--preprocess_format', required=True)
```

### Comparing `pepmatch-0.9.1/pepmatch.egg-info/PKG-INFO` & `pepmatch-0.9.2/pepmatch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pepmatch
-Version: 0.9.1
-Summary: Peptide and epitope search against a reference proteome with specified mismatches.
+Version: 0.9.2
+Summary: Search tool for peptides and epitopes within a proteome, while considering potential residue substitutions.
 Home-page: https://github.com/IEDB/PEPMatch
 Author: Daniel Marrama
 Author-email: dmarrama@lji.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img src="docs/logo.png">
 </p>
 
 --------------------------------------------------------------------
 
-![Unit Tests](https://github.com/IEDB/PEPMatch/actions/workflows/unittests.yml/badge.svg)
+![Unit Tests](https://github.com/IEDB/PEPMatch/actions/workflows/tests.yml/badge.svg)
 
 #### Author: Daniel Marrama
 
 Peptide search against a reference proteome, or sets of proteins, with residue subtitutions.
 
 Two step process: preprocessing and matching.
 
@@ -33,15 +33,15 @@
 - [NumPy](https://numpy.org/)
 - [Biopython](https://biopython.org/)
 - [Levenshtein](https://pypi.org/project/python-Levenshtein/)
 - [redis](https://redis.com/)
 
 ### Installation
 
-```
+```bash
 pip install pepmatch
 ```
 
 
 ### Inputs
 
 #### Preprocessor
@@ -78,39 +78,45 @@
 
 ### Exact Matching Example
 
 ```python
 from pepmatch import Preprocessor, Matcher
 
 # proteome, k, preprocessed_format, target directory, gene_priority_proteome
-Preprocessor('proteomes/human.fasta', '.' 'proteomes/human_gp.fasta').preprocess('sql', k=5)
-# PREPROCESSING ONLY NEEDS TO BE DONE ONCE!
+Preprocessor(
+  'proteomes/human.fasta', '.', 'proteomes/human_gp.fasta'
+).sql_proteome(k = 5) # preprocessing only needs to be done once!
 
 # query, proteome, max_mismatches, k, preprocessed files directory
-Matcher('queries/mhc_ligands_test.fasta', 'proteomes/human.fasta', 0, 5, '.').match()
+Matcher(
+  'queries/mhc_ligands_test.fasta', 'proteomes/human.fasta', 0, 5, '.'
+).match()
 ```
 
 ### Mismatching Example 
 
 ```python
 from pepmatch import Preprocessor, Matcher
 
 # proteome, k, preprocessed_format, target directory
-Preprocessor('proteomes/human.fasta').preprocess('pickle', k=3)
-# PREPROCESSING ONLY NEEDS TO BE DONE ONCE!
+Preprocessor('proteomes/human.fasta').pickle_proteome(k = 3)
 
 # query, proteome, max_mismatches, k, preprocessed files directory
-Matcher('queries/neoepitopes_test.fasta', 'proteomes/human.fasta', 3, 3).match()
+Matcher(
+  'queries/neoepitopes_test.fasta', 'proteomes/human.fasta', 3, 3
+).match()
 ```
 
 ### Best Match Example
 
 ```python
 from pepmatch import Preprocessor, Matcher
-Matcher('queries/milk_peptides.fasta', 'proteomes/human.fasta', best_match=True).match()
+Matcher(
+  'queries/milk_peptides.fasta', 'proteomes/human.fasta', best_match=True
+).match()
 ```
 
 The best match parameter without k or mismatch inputs will produce the best match for each peptide in the query, meaning the match with the least number of mismatches, the best protein existence level, and if the match exists in the gene priority proteome. No preprocessing beforehand is required, as the Matcher class will do this for you to find the best match.
 
 ### Outputs
 
 As mentioned above, outputs can be specified with the ```output_format``` parameter in the ```Matcher``` class. The following formats are allowed: `dataframe`, `csv`, `xlsx`, `json`, and `html`.
```

### Comparing `pepmatch-0.9.1/setup.py` & `pepmatch-0.9.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 from setuptools import setup
 import re
 
 
 with open('README.md', 'r', encoding='utf-8') as f:
-    long_description = f.read()
+  long_description = f.read()
+
 
 with open('pepmatch/version.py', 'r') as f:
-    version = re.search(
-        r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
-        f.read(),
-        re.MULTILINE).group(1)
+  version = re.search(
+    r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
+    f.read(),
+    re.MULTILINE).group(1)
+
 
 setup(
-    name='pepmatch',
-    version=version,
-    description='Peptide and epitope search against a reference proteome with specified mismatches.',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/IEDB/PEPMatch',
-    author='Daniel Marrama',
-    author_email='dmarrama@lji.org',
-    packages=['pepmatch'],
-    install_requires=['numpy>=1.18',
-                      'pandas>=1.1',
-                      'biopython>=1.5',
-                      'python-Levenshtein>=0.11',
-                      'openpyxl>=3.0.0'],
-    zip_safe=False,
-    entry_points={
-        'console_scripts': [
-            'pepmatch-preprocess = pepmatch.preprocessor:run',
-            'pepmatch-match = pepmatch.matcher:run'
-        ]
-    }
+  name='pepmatch',
+  version=version,
+  description='Search tool for peptides and epitopes within a proteome, '
+              'while considering potential residue substitutions.',
+  long_description=long_description,
+  long_description_content_type='text/markdown',
+  url='https://github.com/IEDB/PEPMatch',
+  author='Daniel Marrama',
+  author_email='dmarrama@lji.org',
+  packages=['pepmatch'],
+  install_requires=[
+    'numpy>=1.18',
+    'pandas>=1.1',
+    'biopython>=1.5',
+    'python-Levenshtein>=0.11',
+    'openpyxl>=3.0.0'
+  ],
+  zip_safe=False,
+  entry_points={
+    'console_scripts': [
+      'pepmatch-preprocess = pepmatch.preprocessor:run',
+      'pepmatch-match = pepmatch.matcher:run'
+    ]
+  }
 )
```

### Comparing `pepmatch-0.9.1/test/test_best_match.py` & `pepmatch-0.9.2/test/test_best_match.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #!/usr/bin/env python3
 
 import os
-import glob
 
 import pandas as pd
 import pandas.testing as pdt
 
-from pepmatch import Preprocessor, Matcher
+from pepmatch import Matcher
   
 def test_mismatch():
 
   # paths
   test_script_dir = os.path.dirname(os.path.realpath(__file__))
-  proteome_fasta = os.path.join(test_script_dir, '../benchmarking/proteomes/human.fasta')
-  query_fasta = os.path.join(test_script_dir, '../benchmarking/queries/milk_peptides_test.fasta')
-  expected_csv = os.path.join(test_script_dir, '../benchmarking/expected/milk_peptides_expected.csv')
+  proteome_fasta = os.path.join(
+    test_script_dir, '../benchmarking/proteomes/human.fasta')
+  query_fasta = os.path.join(
+    test_script_dir, '../benchmarking/queries/milk_peptides_test.fasta')
+  expected_csv = os.path.join(
+    test_script_dir, '../benchmarking/expected/milk_peptides_expected.csv')
 
   # match neoepitopes to human proteome
   df = Matcher(
     query=query_fasta,
     proteome_file=proteome_fasta,
     best_match=True,
     output_format='dataframe').match()
@@ -31,19 +33,22 @@
   os.remove('human_metadata.pickle')
 
   # load the expected data
   expected_df = pd.read_csv(expected_csv)
 
   # select only the necessary columns to test for
   df = df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
-  expected_df = expected_df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
+  expected_df = expected_df[
+    ['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
 
   # convert Index start to int64 for comparison
   df['Index start'] = df['Index start'].astype('int64')
   expected_df['Index start'] = expected_df['Index start'].astype('int64')
 
   # sort dataframes by Query Sequence, Protein ID, and Index start
-  df = df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
-  expected_df = expected_df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
+  df = df.sort_values(
+    by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
+  expected_df = expected_df.sort_values(
+    by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
 
   # assert dataframes are equal
   pdt.assert_frame_equal(df, expected_df, check_dtype=False, check_exact=True)
```

### Comparing `pepmatch-0.9.1/test/test_exact_match.py` & `pepmatch-0.9.2/test/test_exact_match.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 
 from pepmatch import Preprocessor, Matcher
 
 
 def test_exact_match():
   # paths
   test_script_dir = os.path.dirname(os.path.realpath(__file__))
-  proteome_fasta = os.path.join(test_script_dir, '../benchmarking/proteomes/human.fasta')
-  query_fasta = os.path.join(test_script_dir, '../benchmarking/queries/mhc_ligands_test.fasta')
-  expected_csv = os.path.join(test_script_dir, '../benchmarking/expected/mhc_ligands_expected.csv')
+  proteome_fasta = os.path.join(
+    test_script_dir, '../benchmarking/proteomes/human.fasta')
+  query_fasta = os.path.join(
+    test_script_dir, '../benchmarking/queries/mhc_ligands_test.fasta')
+  expected_csv = os.path.join(
+    test_script_dir, '../benchmarking/expected/mhc_ligands_expected.csv')
 
   # preprocess human proteome
   k=9
   Preprocessor(proteome_fasta).sql_proteome(k)
 
   # match MHC ligands (9-mers) to human proteome
   df = Matcher(
@@ -31,19 +34,22 @@
   os.remove('human.db')
 
   # load the expected data
   expected_df = pd.read_csv(expected_csv)
 
   # select only the necessary columns to test for
   df = df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
-  expected_df = expected_df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
+  expected_df = expected_df[
+    ['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
 
   # convert Index start to int64 for comparison
   df['Index start'] = df['Index start'].astype('int64')
   expected_df['Index start'] = expected_df['Index start'].astype('int64')
 
   # sort dataframes by Query Sequence, Protein ID, and Index start
-  df = df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
-  expected_df = expected_df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
+  df = df.sort_values(
+    by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
+  expected_df = expected_df.sort_values(
+    by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
 
   # assert dataframes are equal
   pdt.assert_frame_equal(df, expected_df, check_dtype=False, check_exact=True)
```

### Comparing `pepmatch-0.9.1/test/test_mismatch.py` & `pepmatch-0.9.2/test/test_mismatch.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 import pandas.testing as pdt
 
 from pepmatch import Preprocessor, Matcher
   
 def test_mismatch():
   # paths
   test_script_dir = os.path.dirname(os.path.realpath(__file__))
-  proteome_fasta = os.path.join(test_script_dir, '../benchmarking/proteomes/human.fasta')
-  query_fasta = os.path.join(test_script_dir, '../benchmarking/queries/neoepitopes_test.fasta')
-  expected_csv = os.path.join(test_script_dir, '../benchmarking/expected/neoepitopes_expected.csv')
+  proteome_fasta = os.path.join(
+    test_script_dir, '../benchmarking/proteomes/human.fasta')
+  query_fasta = os.path.join(
+    test_script_dir, '../benchmarking/queries/neoepitopes_test.fasta')
+  expected_csv = os.path.join(
+    test_script_dir, '../benchmarking/expected/neoepitopes_expected.csv')
 
   # preprocess human proteome
   k = 3
   Preprocessor(proteome_fasta).pickle_proteome(k)
 
   # match neoepitopes to human proteome
   df = Matcher(
@@ -31,19 +34,22 @@
   os.remove('human_metadata.pickle')
 
   # load the expected data
   expected_df = pd.read_csv(expected_csv)
 
   # select only the necessary columns to test for
   df = df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
-  expected_df = expected_df[['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
+  expected_df = expected_df[
+    ['Query Sequence', 'Matched Sequence', 'Protein ID', 'Index start']]
 
   # convert Index start to int64 for comparison
   df['Index start'] = df['Index start'].astype('int64')
   expected_df['Index start'] = expected_df['Index start'].astype('int64')
 
   # sort dataframes by Query Sequence, Protein ID, and Index start
-  df = df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
-  expected_df = expected_df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
+  df = df.sort_values(
+    by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
+  expected_df = expected_df.sort_values(
+    by=['Query Sequence', 'Protein ID', 'Index start']).reset_index(drop=True)
 
   # assert dataframes are equal
   pdt.assert_frame_equal(df, expected_df, check_dtype=False, check_exact=True)
```

