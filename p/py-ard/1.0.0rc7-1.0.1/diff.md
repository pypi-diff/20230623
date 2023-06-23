# Comparing `tmp/py-ard-1.0.0rc7.tar.gz` & `tmp/py-ard-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ard-1.0.0rc7.tar", last modified: Mon Apr 17 19:05:16 2023, max compression
+gzip compressed data, was "py-ard-1.0.1.tar", last modified: Fri Jun 23 21:44:53 2023, max compression
```

## Comparing `py-ard-1.0.0rc7.tar` & `py-ard-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:05:16.217231 py-ard-1.0.0rc7/
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-04-17 19:05:16.217231 py-ard-1.0.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:05:16.213231 py-ard-1.0.0rc7/py_ard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20003 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 19:05:16.000000 py-ard-1.0.0rc7/py_ard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:05:16.217231 py-ard-1.0.0rc7/pyard/
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/CWD2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27740 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/ard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/blender.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/broad_splits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16015 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/dna_relshp.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/drbx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9345 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/pyard/smart_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:05:16.217231 py-ard-1.0.0rc7/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3260 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/scripts/pyard
--rwxr-xr-x   0 runner    (1001) docker     (123)     5192 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/scripts/pyard-import
--rwxr-xr-x   0 runner    (1001) docker     (123)    15408 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/scripts/pyard-reduce-csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     3997 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/scripts/pyard-status
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-17 19:05:16.217231 py-ard-1.0.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-17 19:05:06.000000 py-ard-1.0.0rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:44:53.928184 py-ard-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-23 21:44:42.000000 py-ard-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-23 21:44:42.000000 py-ard-1.0.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-23 21:44:42.000000 py-ard-1.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-23 21:44:42.000000 py-ard-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-23 21:44:42.000000 py-ard-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20077 2023-06-23 21:44:53.928184 py-ard-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15574 2023-06-23 21:44:42.000000 py-ard-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:44:53.924184 py-ard-1.0.1/py_ard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20077 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 21:44:53.000000 py-ard-1.0.1/py_ard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:44:53.928184 py-ard-1.0.1/pyard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/CWD2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28985 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/ard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/blender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/broad_splits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/dna_relshp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/drbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-23 21:44:42.000000 py-ard-1.0.1/pyard/smart_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 21:44:42.000000 py-ard-1.0.1/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 21:44:42.000000 py-ard-1.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:44:53.928184 py-ard-1.0.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3969 2023-06-23 21:44:42.000000 py-ard-1.0.1/scripts/pyard
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5192 2023-06-23 21:44:42.000000 py-ard-1.0.1/scripts/pyard-import
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15408 2023-06-23 21:44:42.000000 py-ard-1.0.1/scripts/pyard-reduce-csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3997 2023-06-23 21:44:42.000000 py-ard-1.0.1/scripts/pyard-status
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-23 21:44:53.928184 py-ard-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-23 21:44:42.000000 py-ard-1.0.1/setup.py
```

### Comparing `py-ard-1.0.0rc7/CONTRIBUTING.rst` & `py-ard-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc7/COPYING` & `py-ard-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc7/LICENSE` & `py-ard-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc7/PKG-INFO` & `py-ard-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.0.0rc7
+Version: 1.0.1
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
         
@@ -180,14 +180,15 @@
         | `G`            | Reduce to G Group Level                         |
         | `P`            | Reduce to P Group Level                         |
         | `lg`           | Reduce to 2 field ARD level (append `g`)        |
         | `lgx`          | Reduce to 2 field ARD level                     |
         | `W`            | Reduce/Expand to 3 field WHO nomenclature level |
         | `exon`         | Reduce/Expand to exon level                     |
         | `U2`           | Reduce to 2 field unambiguous level             |
+        | `S`            | Reduce to Serological level                     |
         
         ### Perform DRB1 blending with DRB3, DRB4 and DRB5
         
         ```python
         import pyard
         
         pyard.dr_blender(drb1='HLA-DRB1*03:01+DRB1*04:01', drb3='DRB3*01:01', drb4='DRB4*01:03')
```

### Comparing `py-ard-1.0.0rc7/README.md` & `py-ard-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,15 @@
 | `G`            | Reduce to G Group Level                         |
 | `P`            | Reduce to P Group Level                         |
 | `lg`           | Reduce to 2 field ARD level (append `g`)        |
 | `lgx`          | Reduce to 2 field ARD level                     |
 | `W`            | Reduce/Expand to 3 field WHO nomenclature level |
 | `exon`         | Reduce/Expand to exon level                     |
 | `U2`           | Reduce to 2 field unambiguous level             |
+| `S`            | Reduce to Serological level                     |
 
 ### Perform DRB1 blending with DRB3, DRB4 and DRB5
 
 ```python
 import pyard
 
 pyard.dr_blender(drb1='HLA-DRB1*03:01+DRB1*04:01', drb3='DRB3*01:01', drb4='DRB4*01:03')
```

### Comparing `py-ard-1.0.0rc7/py_ard.egg-info/PKG-INFO` & `py-ard-1.0.1/py_ard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.0.0rc7
+Version: 1.0.1
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
         
@@ -180,14 +180,15 @@
         | `G`            | Reduce to G Group Level                         |
         | `P`            | Reduce to P Group Level                         |
         | `lg`           | Reduce to 2 field ARD level (append `g`)        |
         | `lgx`          | Reduce to 2 field ARD level                     |
         | `W`            | Reduce/Expand to 3 field WHO nomenclature level |
         | `exon`         | Reduce/Expand to exon level                     |
         | `U2`           | Reduce to 2 field unambiguous level             |
+        | `S`            | Reduce to Serological level                     |
         
         ### Perform DRB1 blending with DRB3, DRB4 and DRB5
         
         ```python
         import pyard
         
         pyard.dr_blender(drb1='HLA-DRB1*03:01+DRB1*04:01', drb3='DRB3*01:01', drb4='DRB4*01:03')
```

### Comparing `py-ard-1.0.0rc7/py_ard.egg-info/SOURCES.txt` & `py-ard-1.0.1/py_ard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc7/pyard/CWD2.csv` & `py-ard-1.0.1/pyard/CWD2.csv`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 DPB1,DPB1*02:01
 DPB1,DPB1*02:02
 DPB1,DPB1*03:01
 DPB1,DPB1*04:01
 DPB1,DPB1*04:02
 DPB1,DPB1*05:01
 DPB1,DPB1*06:01
-DPB1,DPB1*105:0
+DPB1,DPB1*105:01
 DPB1,DPB1*09:01
 DPB1,DPB1*10:01
 DPB1,DPB1*11:01
 DPB1,DPB1*13:01
 DPB1,DPB1*14:01
 DPB1,DPB1*15:01
 DPB1,DPB1*16:01
```

### Comparing `py-ard-1.0.0rc7/pyard/__init__.py` & `py-ard-1.0.1/pyard/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 from .blender import blender as dr_blender
 from .broad_splits import find_splits as find_broad_splits
 from .constants import DEFAULT_CACHE_SIZE
 from .misc import get_imgt_db_versions as db_versions
 
 __author__ = """NMDP Bioinformatics"""
-__version__ = "1.0.0rc7"
+__version__ = "1.0.1"
 
 
 def init(
     imgt_version: str = "Latest",
     data_dir: str = None,
     load_mac: bool = True,
     cache_size: int = DEFAULT_CACHE_SIZE,
```

### Comparing `py-ard-1.0.0rc7/pyard/ard.py` & `py-ard-1.0.1/pyard/ard.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from . import broad_splits, smart_sort
 from . import data_repository as dr
 from . import db
 from .exceptions import InvalidAlleleError, InvalidMACError, InvalidTypingError
 from .misc import (
     get_n_field_allele,
     get_2field_allele,
+    is_2_field_allele,
     validate_reduction_type,
 )
 from .constants import (
     HLA_regex,
     VALID_REDUCTION_TYPES,
     expression_chars,
     DEFAULT_CACHE_SIZE,
@@ -49,25 +50,26 @@
     "reduce_P": True,
     "reduce_XX": True,
     "reduce_MAC": True,
     "reduce_shortnull": True,
     "ping": False,
     "map_drb345_to_drbx": True,
     "verbose_log": True,
+    "ARS_as_lg": False,
 }
 
 
 # Typing information
 
 
 class ARD(object):
     """
     ARD reduction for HLA
     Allows reducing alleles, allele code(MAC), Serology to
-    G, lg, lgx, W, exon and U2 levels.
+    G, lg, lgx, W, exon, S and U2 levels.
     """
 
     def __init__(
         self,
         imgt_version: str = "Latest",
         data_dir: str = None,
         load_mac: bool = True,
@@ -165,16 +167,14 @@
         :type: str
         :param redux_type: reduction type.
         :type: str
         :return: reduced allele
         :rtype: str
         """
 
-        validate_reduction_type(redux_type)
-
         # deal with leading 'HLA-'
         if HLA_regex.search(allele):
             hla, allele_name = allele.split("-")
             redux_allele = self._redux_allele(allele_name, redux_type)
             if redux_allele:
                 return "HLA-" + redux_allele
             else:
@@ -209,14 +209,17 @@
             elif allele in self.ars_mappings.lgx_group:
                 redux_allele = self.ars_mappings.lgx_group[allele]
             else:
                 # for 'lgx' or 'lg' mode when allele is not in G group,
                 # return allele with only first 2 field
                 redux_allele = ":".join(allele.split(":")[0:2])
             if redux_type == "lg":
+                # ARS suffix maybe used instead of g
+                if self._config["ARS_as_lg"]:
+                    return redux_allele + "ARS"
                 # lg mode has g appended with lgx reduction
                 return redux_allele + "g"
             return redux_allele
         elif redux_type == "W":
             # new redux_type which is full WHO expansion
             if self._is_who_allele(allele):
                 return allele
@@ -249,14 +252,32 @@
             # If the 2 field reduction is unambiguous, reduce to 2 field level
             allele_2_fields = get_n_field_allele(allele, 2, preserve_expression=True)
             if self._is_valid_allele(allele_2_fields):
                 return allele_2_fields
             else:
                 # If ambiguous, reduce to G group level
                 return self._redux_allele(allele, "lgx")
+        elif redux_type == "S":
+            # find serology equivalent in serology_mapping
+            serology_mapping = db.find_serology_for_allele(self.db_connection, allele)
+            serology_set = set()
+            if is_2_field_allele(allele):
+                for serology, allele_list in serology_mapping.items():
+                    allele_list_lgx = self.redux(allele_list, "lgx")
+                    if allele in allele_list_lgx:
+                        serology_set.add(serology)
+            else:
+                for serology, allele_list in serology_mapping.items():
+                    if allele in allele_list:
+                        serology_set.add(serology)
+            return "/".join(
+                sorted(
+                    serology_set, key=functools.cmp_to_key(self.smart_sort_comparator)
+                )
+            )
         else:
             # Make this an explicit lookup to the g_group or p_group table
             # for stringent validation
             if allele.endswith("P"):
                 if allele in self.ars_mappings.p_group.values():
                     return allele
             elif allele.endswith("G"):
@@ -289,15 +310,15 @@
             )
 
         # generate a unique list over a delimiter
         # e.g. [A, A/B] => [ A, B ] for / delimiter
         all_gls = []
         for gl in gls:
             all_gls += gl.split(delim)
-        unique_gls = set(all_gls)
+        unique_gls = filter(lambda s: s != "", set(all_gls))
         return delim.join(
             sorted(unique_gls, key=functools.cmp_to_key(self.smart_sort_comparator))
         )
 
     @functools.lru_cache(maxsize=DEFAULT_CACHE_SIZE)
     def redux(self, glstring: str, redux_type: VALID_REDUCTION_TYPES) -> str:
         """
@@ -619,22 +640,26 @@
             and not self.is_v2(allele)
             and not self.is_shortnull(allele)
         ):
             # Alleles ending with P or G are valid_alleles
             if allele.endswith(("P", "G")):
                 # remove the last character
                 allele = allele[:-1]
-                if self._is_valid_allele(allele):
-                    return True
-                else:
-                    allele = get_2field_allele(allele)
-                    if self._is_valid_allele(allele):
-                        return True
+            # validate format: there are no empty fields eg, 2 :: together
+            if "*" in allele:
+                _, fields = allele.split("*")
+                if not all(map(str.isalnum, fields.split(":"))):
+                    return False
+            # The allele is valid as whole or as a 2 field version
+            if self._is_valid_allele(allele):
+                return True
+            else:
+                allele = get_2field_allele(allele)
+                return self._is_valid_allele(allele)
 
-            return self._is_valid_allele(allele)
         return True
 
     def _is_valid_gl(self, glstring: str) -> bool:
         """
         Determines validity of glstring
 
         :param glstring
```

### Comparing `py-ard-1.0.0rc7/pyard/blender.py` & `py-ard-1.0.1/pyard/blender.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc7/pyard/broad_splits.py` & `py-ard-1.0.1/pyard/broad_splits.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc7/pyard/constants.py` & `py-ard-1.0.1/pyard/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 #
 import re
 
 DEFAULT_CACHE_SIZE = 1_000
 
 HLA_regex = re.compile("^HLA-")
 
-VALID_REDUCTION_TYPES = ["G", "P", "lg", "lgx", "W", "exon", "U2"]
+VALID_REDUCTION_TYPES = ["G", "P", "lg", "lgx", "W", "exon", "U2", "S"]
 expression_chars = ["N", "Q", "L", "S"]
 # List of P and G characters
 PandG_chars = ["P", "G"]
```

### Comparing `py-ard-1.0.0rc7/pyard/data_repository.py` & `py-ard-1.0.1/pyard/data_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,14 @@
         return db.load_ars_mappings(db_connection)
 
     import pandas as pd
 
     df_g_group = load_g_group(imgt_version)
     df_p_group = load_p_group(imgt_version)
 
-    # Extract p group mapping
-    p_group = df_p_group.set_index("A")["P"].to_dict()
-
     # compare df_p_group["2d"] with df_g_group["2d"] to find 2-field alleles in the
     # P-group that aren't in the G-group
     p_not_in_g = set(df_p_group["2d"]) - set(df_g_group["2d"])
 
     # filter to find these 2-field alleles (2d) in the P-group data frame
     df_p_not_g = df_p_group[df_p_group["2d"].isin(p_not_in_g)]
 
@@ -120,35 +117,47 @@
         df_g_group[df_g_group["2d"].isin(multiple_lgx_list)][["lgx", "2d"]]
         .drop_duplicates()
         .groupby("2d", as_index=True)
         .agg("/".join)
         .to_dict()["lgx"]
     )
 
-    # Creating dictionaries with mac_code->ARD group mapping
+    # Extract G group mapping
     df_g = pd.concat(
         [
             df_g_group[["2d", "G"]].rename(columns={"2d": "A"}),
             df_g_group[["3d", "G"]].rename(columns={"3d": "A"}),
             df_g_group[["A", "G"]],
         ],
         ignore_index=True,
     )
     g_group = df_g.set_index("A")["G"].to_dict()
 
+    # Extract P group mapping
+    df_p = pd.concat(
+        [
+            df_p_group[["2d", "P"]].rename(columns={"2d": "A"}),
+            df_p_group[["3d", "P"]].rename(columns={"3d": "A"}),
+            df_p_group[["A", "P"]],
+        ],
+        ignore_index=True,
+    )
+    p_group = df_p.set_index("A")["P"].to_dict()
+
+    # Extract lgx group mapping
     df_lgx = pd.concat(
         [
             df_g_group[["2d", "lgx"]].rename(columns={"2d": "A"}),
             df_g_group[["3d", "lgx"]].rename(columns={"3d": "A"}),
             df_g_group[["A", "lgx"]],
         ]
     )
     lgx_group = df_lgx.set_index("A")["lgx"].to_dict()
 
-    # exon
+    # Extract exon mapping
     df_exon = pd.concat(
         [
             df_g_group[["A", "3d"]].rename(columns={"3d": "exon"}),
         ]
     )
     exon_group = df_exon.set_index("A")["exon"].to_dict()
```

### Comparing `py-ard-1.0.0rc7/pyard/db.py` & `py-ard-1.0.1/pyard/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         return sqlite3.connect(file_uri, check_same_thread=False, uri=True), db_filename
 
     # Check the imgt_version is a valid IMGT DB Version
     # by querying the IMGT site
     if imgt_version != "Latest":
         if not pathlib.Path(db_filename).exists():
             all_imgt_versions = get_imgt_db_versions()
-            if imgt_version not in all_imgt_versions:
+            if str(imgt_version) not in all_imgt_versions:
                 raise ValueError(
                     f"{imgt_version} is not a valid IMGT database version."
                 )
 
     # Create the data directory if it doesn't exist
     if not pathlib.Path(data_dir).exists():
         pathlib.Path(data_dir).mkdir(parents=True, exist_ok=True)
@@ -366,14 +366,35 @@
     # fetchall() returns a list of tuples of results
     # e.g. [('C*04:09N',)]
     # Get out the first value of the tuple from the result list
     alleles = set(map(lambda t: t[0], result))
     return alleles
 
 
+def find_serology_for_allele(
+    connection: sqlite3.Connection, allele_name: str
+) -> Dict[str, str]:
+    """
+    Find similar alleles starting with the provided allele_name.
+
+    :param connection: db connection of type sqlite.Connection
+    :param allele_name: Allele name to use as a prefix to find similar alleles
+    :return: list of similar alleles
+    """
+    query = (
+        "SELECT serology, allele_list FROM serology_mapping WHERE allele_list LIKE ?"
+    )
+    cursor = connection.execute(query, (f"%{allele_name}%",))
+    results = cursor.fetchall()
+    # fetchall() returns a list of tuples of results
+    # e.g. [('A1', ''A*01:01:01:01/A*01:01:01:03')]
+    serology_mapping = {serology: allele_list for serology, allele_list in results}
+    return serology_mapping
+
+
 def get_user_version(connection: sqlite3.Connection) -> int:
     """
     Retrieve user_version from db
 
     :connection: sqlite3.Connection: SQLite DB Connection
     """
     query = "PRAGMA user_version"
```

### Comparing `py-ard-1.0.0rc7/pyard/drbx.py` & `py-ard-1.0.1/pyard/drbx.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc7/pyard/exceptions.py` & `py-ard-1.0.1/pyard/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc7/pyard/load.py` & `py-ard-1.0.1/pyard/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,25 +106,27 @@
             ars_p_url, skiprows=6, names=["Locus", "A", "P"], sep=";"
         ).dropna()
     except URLError as e:
         print(f"Error downloading {ars_p_url}", e, file=sys.stderr)
         sys.exit(1)
 
     # the P-group is named for its first allele
-    df_p["P"] = df_p["A"].apply(get_P_name)
+    # The P column is already present in the file
+    # df_p["P"] = df_p["A"].apply(get_P_name)
     # convert slash delimited string to a list
     df_p["A"] = df_p["A"].apply(lambda a: a.split("/"))
     df_p = df_p.explode("A")
     # C* 06:06:01:01/06:06:01:02/06:271 06:06P
     df_p["A"] = df_p["Locus"] + df_p["A"]
     df_p["P"] = df_p["Locus"] + df_p["P"]
     # C* 06:06:01:01 06:06P
     # C* 06:06:01:02 06:06P
     # C* 06:271 06:06P
     df_p["2d"] = df_p["A"].apply(get_2field_allele)
+    df_p["3d"] = df_p["A"].apply(get_3field_allele)
     # lgx has the P-group name without the P for comparison
     df_p["lgx"] = df_p["P"].apply(get_2field_allele)
     return df_p
 
 
 def load_allele_list(imgt_version):
     """
```

### Comparing `py-ard-1.0.0rc7/pyard/mappings.py` & `py-ard-1.0.1/pyard/mappings.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc7/pyard/misc.py` & `py-ard-1.0.1/pyard/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,18 @@
     return get_n_field_allele(a, 1)
 
 
 def number_of_fields(allele: str) -> int:
     return len(allele.split(":"))
 
 
+def is_2_field_allele(allele: str) -> bool:
+    return number_of_fields(allele) == 2
+
+
 # computes a valid G name based on the ambiguity string
 def get_G_name(a: str) -> str:
     a = a.split("/")[0]
     last_char = a[-1]
     if last_char in PandG_chars + expression_chars:
         a = a[:-1]
     if len(a.split(":")) == 2:
```

### Comparing `py-ard-1.0.0rc7/pyard/smart_sort.py` & `py-ard-1.0.1/pyard/smart_sort.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,19 @@
     a1 = re.sub(expr_regex, "", a1)
     a2 = re.sub(expr_regex, "", a2)
 
     # Check to see if they are still the same alleles
     if a1 == a2:
         return 0
 
-    # Extract and Compare first fields first
+    # Handle serology
+    if ":" not in a1:
+        return 1 if a1 > a2 else -1
+
+    # Extract and Compare 1st fields first
     a1_f1 = int(a1[a1.find("*") + 1 : a1.find(":")])
     a2_f1 = int(a2[a2.find("*") + 1 : a2.find(":")])
 
     if a1_f1 < a2_f1:
         return -1
     if a1_f1 > a2_f1:
         return 1
```

### Comparing `py-ard-1.0.0rc7/scripts/pyard` & `py-ard-1.0.1/scripts/pyard-status`

 * *Files 27% similar despite different names*

```diff
@@ -18,82 +18,91 @@
 #    along with this library;  if not, write to the Free Software Foundation,
 #    Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA.
 #
 #    > http://www.fsf.org/licensing/licenses/lgpl.html
 #    > http://www.opensource.org/licenses/lgpl-license.php
 #
 import argparse
-import sys
+import os
+import re
+
+import pyard
+import pyard.mappings
+from pyard import db, data_repository
+from pyard.misc import get_data_dir
+
+
+def get_latest_imgt_version() -> int:
+    """
+    Gets the list of db versions and returns the maximum
+    version numbered db
+    @return: int
+    """
+    return max(map(int, pyard.db_versions()[:-1]))
+
+
+def get_file_size(file_name: str) -> float:
+    return os.path.getsize(file_name) / 1024 / 1024
 
-from pyard.constants import VALID_REDUCTION_TYPES
-import pyard.misc
-from pyard.exceptions import InvalidAlleleError
-from pyard.misc import get_data_dir, get_imgt_version
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
         description="""
-        py-ard tool to redux GL String
-        """,
-    )
-    parser.add_argument(
-        "-v",
-        "--version",
-        dest="version",
-        action="store_true",
-        help="IPD-IMGT/HLA DB Version number",
+        py-ard tool to provide a status report for reference SQLite databases.
+        """
     )
     parser.add_argument(
         "-d",
         "--data-dir",
         dest="data_dir",
         help="Data directory to store imported data",
     )
-    parser.add_argument(
-        "-i",
-        "--imgt-version",
-        dest="imgt_version",
-        help="IPD-IMGT/HLA db to use for redux",
-    )
-    parser.add_argument("-g", "--gl", dest="gl_string", help="GL String to reduce")
-    parser.add_argument(
-        "-r",
-        "--redux-type",
-        choices=VALID_REDUCTION_TYPES,
-        dest="redux_type",
-        help="Reduction Method",
-    )
-    parser.add_argument("--splits", dest="splits", help="Find Broad and Splits")
 
     args = parser.parse_args()
-
-    imgt_version = get_imgt_version(args.imgt_version)
     data_dir = get_data_dir(args.data_dir)
-    ard = pyard.init(imgt_version=imgt_version, data_dir=data_dir)
-
-    if args.version:
-        version = ard.get_db_version()
-        print(f"IPD-IMGT/HLA version:", version)
-        print(f"py-ard version:", pyard.__version__)
-        sys.exit(0)
-
-    if args.splits:
-        mapping = pyard.find_broad_splits(args.splits)
-        if mapping:
-            print(f"{mapping[0]} = {'/'.join(mapping[1])}")
-        sys.exit(0)
-
-    try:
-        if args.redux_type:
-            print(ard.redux(args.gl_string, args.redux_type))
-        else:
-            for redux_type in VALID_REDUCTION_TYPES:
-                redux_type_info = f"Reduction Method: {redux_type}"
-                print(redux_type_info)
-                print("-" * len(redux_type_info))
-                print(ard.redux(args.gl_string, redux_type))
-                print()
-    except InvalidAlleleError as e:
-        print("Error:", e)
 
-    # Remove ard and close db connection
-    del ard
+    imgt_regex = re.compile(r"pyard-(.+)\.sqlite3")
+    for _, _, filenames in os.walk(data_dir):
+        for filename in filenames:
+            # Get imgt version from the filename
+            # eg: get 3440 from 'pyard-3440.sqlite3'
+            match = imgt_regex.match(filename)
+            imgt_version = match.group(1)  # Get first group
+            db_connection, db_filename = db.create_db_connection(
+                data_dir, imgt_version, ro=True
+            )
+            print("-" * 43)
+            if imgt_version == "Latest":
+                db_version = data_repository.get_db_version(db_connection)
+                print(f"IMGT DB Version: {imgt_version} ({db_version})")
+                latest_version = get_latest_imgt_version()
+                if latest_version == db_version:
+                    print(
+                        f"You're up to date. {db_version} is the most recent version."
+                    )
+                else:
+                    print(f"There is a newer IMGT release than version {db_version}")
+                    print(
+                        f"Upgrade to latest version '{latest_version}'",
+                        "with 'pyard-import --re-install'",
+                    )
+            else:
+                print(f"IMGT DB Version: {imgt_version}")
+            file_size = get_file_size(db_filename)
+            print(f"File: {db_filename}")
+            print(f"Size: {file_size:.2f}MB")
+            print("-" * 43)
+            print(f"|{'Table Name':20}|{'Rows':20}|")
+            print(f"|{'-' * 41}|")
+            for table in (
+                pyard.mappings.ars_mapping_tables
+                + pyard.mappings.code_mapping_tables
+                + pyard.mappings.allele_tables
+                + ["mac_codes"]
+            ):
+                if db.table_exists(db_connection, table):
+                    total_rows = db.count_rows(db_connection, table)
+                    print(f"|{table:20}|{total_rows:20}|")
+                else:
+                    print(f"MISSING: {table} table")
+            print("-" * 43)
+            db_connection.close()
```

### Comparing `py-ard-1.0.0rc7/scripts/pyard-import` & `py-ard-1.0.1/scripts/pyard-import`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc7/scripts/pyard-reduce-csv` & `py-ard-1.0.1/scripts/pyard-reduce-csv`

 * *Files identical despite different names*

### Comparing `py-ard-1.0.0rc7/setup.cfg` & `py-ard-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.0rc7
+current_version = 1.0.1
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `py-ard-1.0.0rc7/setup.py` & `py-ard-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="py-ard",
-    version="1.0.0rc7",
+    version="1.0.1",
     description="ARD reduction for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="CIBMTR",
     author_email="cibmtr-pypi@nmdp.org",
     url="https://github.com/nmdp-bioinformatics/py-ard",
     packages=[
```

