# Comparing `tmp/jellyfish-0.8.9.tar.gz` & `tmp/jellyfish-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jellyfish-0.8.9.tar", last modified: Tue Oct 26 15:19:05 2021, max compression
+gzip compressed data, was "jellyfish-0.9.0.tar", last modified: Fri Jan  7 20:19:05 2022, max compression
```

## Comparing `jellyfish-0.8.9.tar` & `jellyfish-0.9.0.tar`

### file list

```diff
@@ -1,54 +1,50 @@
-drwxrwxrwx   0        0        0        0 2021-10-26 15:19:05.748419 jellyfish-0.8.9/
--rw-rw-rw-   0        0        0     1377 2021-10-26 15:18:33.000000 jellyfish-0.8.9/LICENSE
--rw-rw-rw-   0        0        0      112 2021-10-26 15:18:33.000000 jellyfish-0.8.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2899 2021-10-26 15:19:05.748419 jellyfish-0.8.9/PKG-INFO
--rw-rw-rw-   0        0        0     2146 2021-10-26 15:18:33.000000 jellyfish-0.8.9/README.rst
-drwxrwxrwx   0        0        0        0 2021-10-26 15:19:05.728418 jellyfish-0.8.9/cjellyfish/
--rw-rw-rw-   0        0        0     5175 2021-10-26 15:18:35.000000 jellyfish-0.8.9/cjellyfish/damerau_levenshtein.c
--rw-rw-rw-   0        0        0      521 2021-10-26 15:18:35.000000 jellyfish-0.8.9/cjellyfish/hamming.c
--rw-rw-rw-   0        0        0     4486 2021-10-26 15:18:35.000000 jellyfish-0.8.9/cjellyfish/jaro.c
--rw-rw-rw-   0        0        0     1746 2021-10-26 15:18:35.000000 jellyfish-0.8.9/cjellyfish/jellyfish.h
--rw-rw-rw-   0        0        0    11068 2021-10-26 15:18:35.000000 jellyfish-0.8.9/cjellyfish/jellyfishmodule.c
--rw-rw-rw-   0        0        0     1140 2021-10-26 15:18:35.000000 jellyfish-0.8.9/cjellyfish/levenshtein.c
--rw-rw-rw-   0        0        0     5463 2021-10-26 15:18:35.000000 jellyfish-0.8.9/cjellyfish/metaphone.c
--rw-rw-rw-   0        0        0     2723 2021-10-26 15:18:35.000000 jellyfish-0.8.9/cjellyfish/mra.c
--rw-rw-rw-   0        0        0     4683 2021-10-26 15:18:35.000000 jellyfish-0.8.9/cjellyfish/nysiis.c
--rw-rw-rw-   0        0        0    12381 2021-10-26 15:18:35.000000 jellyfish-0.8.9/cjellyfish/porter.c
--rw-rw-rw-   0        0        0     1415 2021-10-26 15:18:35.000000 jellyfish-0.8.9/cjellyfish/soundex.c
-drwxrwxrwx   0        0        0        0 2021-10-26 15:19:05.733418 jellyfish-0.8.9/docs/
--rw-rw-rw-   0        0        0     6951 2021-10-26 15:18:33.000000 jellyfish-0.8.9/docs/Makefile
--rw-rw-rw-   0        0        0     3946 2021-10-26 15:18:33.000000 jellyfish-0.8.9/docs/changelog.rst
--rw-rw-rw-   0        0        0     3820 2021-10-26 15:18:33.000000 jellyfish-0.8.9/docs/comparison.rst
--rw-rw-rw-   0        0        0     8545 2021-10-26 15:18:33.000000 jellyfish-0.8.9/docs/conf.py
--rw-rw-rw-   0        0        0     1209 2021-10-26 15:18:33.000000 jellyfish-0.8.9/docs/index.rst
--rw-rw-rw-   0        0        0     2460 2021-10-26 15:18:33.000000 jellyfish-0.8.9/docs/phonetic.rst
--rw-rw-rw-   0        0        0      485 2021-10-26 15:18:33.000000 jellyfish-0.8.9/docs/stemming.rst
-drwxrwxrwx   0        0        0        0 2021-10-26 15:19:05.737417 jellyfish-0.8.9/jellyfish/
--rw-rw-rw-   0        0        0      785 2021-10-26 15:18:33.000000 jellyfish-0.8.9/jellyfish/__init__.py
--rw-rw-rw-   0        0        0      555 2021-10-26 15:18:33.000000 jellyfish-0.8.9/jellyfish/__init__.pyi
--rw-rw-rw-   0        0        0    13522 2021-10-26 15:18:33.000000 jellyfish-0.8.9/jellyfish/_jellyfish.py
--rw-rw-rw-   0        0        0     7218 2021-10-26 15:18:33.000000 jellyfish-0.8.9/jellyfish/porter.py
--rw-rw-rw-   0        0        0        0 2021-10-26 15:18:33.000000 jellyfish-0.8.9/jellyfish/py.typed
--rw-rw-rw-   0        0        0     7394 2021-10-26 15:18:33.000000 jellyfish-0.8.9/jellyfish/test.py
-drwxrwxrwx   0        0        0        0 2021-10-26 15:19:05.739419 jellyfish-0.8.9/jellyfish.egg-info/
--rw-rw-rw-   0        0        0     2899 2021-10-26 15:19:05.000000 jellyfish-0.8.9/jellyfish.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1030 2021-10-26 15:19:05.000000 jellyfish-0.8.9/jellyfish.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-10-26 15:19:05.000000 jellyfish-0.8.9/jellyfish.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2021-10-26 15:19:05.000000 jellyfish-0.8.9/jellyfish.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-10-26 15:19:05.748419 jellyfish-0.8.9/setup.cfg
--rw-rw-rw-   0        0        0     4784 2021-10-26 15:18:33.000000 jellyfish-0.8.9/setup.py
-drwxrwxrwx   0        0        0        0 2021-10-26 15:19:05.747419 jellyfish-0.8.9/testdata/
--rw-rw-rw-   0        0        0       77 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/README.md
--rw-rw-rw-   0        0        0      164 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/damerau_levenshtein.csv
--rw-rw-rw-   0        0        0      105 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/hamming.csv
--rw-rw-rw-   0        0        0      142 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/jaro_distance.csv
--rw-rw-rw-   0        0        0      303 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/jaro_winkler.csv
--rw-rw-rw-   0        0        0      197 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/jaro_winkler_longtol.csv
--rw-rw-rw-   0        0        0       68 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/levenshtein.csv
--rw-rw-rw-   0        0        0      129 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/match_rating_codex.csv
--rw-rw-rw-   0        0        0      110 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/match_rating_comparison.csv
--rw-rw-rw-   0        0        0      475 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/metaphone.csv
--rw-rw-rw-   0        0        0      449 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/nysiis.csv
--rw-rw-rw-   0        0        0   377012 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/porter.csv
--rw-rw-rw-   0        0        0      131 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/soundex.csv
--rw-rw-rw-   0        0        0       98 2021-10-26 15:18:36.000000 jellyfish-0.8.9/testdata/wagner_fischer.csv
+drwxrwxrwx   0        0        0        0 2022-01-07 20:19:05.388511 jellyfish-0.9.0/
+-rw-rw-rw-   0        0        0     1377 2022-01-07 20:18:31.000000 jellyfish-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      112 2022-01-07 20:18:31.000000 jellyfish-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2417 2022-01-07 20:19:05.387510 jellyfish-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1622 2022-01-07 20:18:31.000000 jellyfish-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-01-07 20:19:05.364510 jellyfish-0.9.0/cjellyfish/
+-rw-rw-rw-   0        0        0     5175 2022-01-07 20:18:35.000000 jellyfish-0.9.0/cjellyfish/damerau_levenshtein.c
+-rw-rw-rw-   0        0        0      527 2022-01-07 20:18:35.000000 jellyfish-0.9.0/cjellyfish/hamming.c
+-rw-rw-rw-   0        0        0     4486 2022-01-07 20:18:35.000000 jellyfish-0.9.0/cjellyfish/jaro.c
+-rw-rw-rw-   0        0        0     1883 2022-01-07 20:18:35.000000 jellyfish-0.9.0/cjellyfish/jellyfish.h
+-rw-rw-rw-   0        0        0    14067 2022-01-07 20:18:35.000000 jellyfish-0.9.0/cjellyfish/jellyfishmodule.c
+-rw-rw-rw-   0        0        0     1140 2022-01-07 20:18:35.000000 jellyfish-0.9.0/cjellyfish/levenshtein.c
+-rw-rw-rw-   0        0        0     5463 2022-01-07 20:18:35.000000 jellyfish-0.9.0/cjellyfish/metaphone.c
+-rw-rw-rw-   0        0        0     3003 2022-01-07 20:18:35.000000 jellyfish-0.9.0/cjellyfish/mra.c
+-rw-rw-rw-   0        0        0     4683 2022-01-07 20:18:35.000000 jellyfish-0.9.0/cjellyfish/nysiis.c
+-rw-rw-rw-   0        0        0    12382 2022-01-07 20:18:35.000000 jellyfish-0.9.0/cjellyfish/porter.c
+-rw-rw-rw-   0        0        0     1415 2022-01-07 20:18:35.000000 jellyfish-0.9.0/cjellyfish/soundex.c
+drwxrwxrwx   0        0        0        0 2022-01-07 20:19:05.367508 jellyfish-0.9.0/docs/
+-rw-rw-rw-   0        0        0     4145 2022-01-07 20:18:31.000000 jellyfish-0.9.0/docs/changelog.md
+-rw-rw-rw-   0        0        0     6718 2022-01-07 20:18:31.000000 jellyfish-0.9.0/docs/functions.md
+-rw-rw-rw-   0        0        0     2354 2022-01-07 20:18:31.000000 jellyfish-0.9.0/docs/index.md
+drwxrwxrwx   0        0        0        0 2022-01-07 20:19:05.372510 jellyfish-0.9.0/jellyfish/
+-rw-rw-rw-   0        0        0      785 2022-01-07 20:18:31.000000 jellyfish-0.9.0/jellyfish/__init__.py
+-rw-rw-rw-   0        0        0      555 2022-01-07 20:18:31.000000 jellyfish-0.9.0/jellyfish/__init__.pyi
+-rw-rw-rw-   0        0        0    13524 2022-01-07 20:18:31.000000 jellyfish-0.9.0/jellyfish/_jellyfish.py
+-rw-rw-rw-   0        0        0     7218 2022-01-07 20:18:31.000000 jellyfish-0.9.0/jellyfish/porter.py
+-rw-rw-rw-   0        0        0        0 2022-01-07 20:18:31.000000 jellyfish-0.9.0/jellyfish/py.typed
+-rw-rw-rw-   0        0        0     7394 2022-01-07 20:18:31.000000 jellyfish-0.9.0/jellyfish/test.py
+drwxrwxrwx   0        0        0        0 2022-01-07 20:19:05.375510 jellyfish-0.9.0/jellyfish.egg-info/
+-rw-rw-rw-   0        0        0     2417 2022-01-07 20:19:05.000000 jellyfish-0.9.0/jellyfish.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      962 2022-01-07 20:19:05.000000 jellyfish-0.9.0/jellyfish.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-07 20:19:05.000000 jellyfish-0.9.0/jellyfish.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2022-01-07 20:19:05.000000 jellyfish-0.9.0/jellyfish.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-01-07 20:19:05.388511 jellyfish-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     4826 2022-01-07 20:18:31.000000 jellyfish-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-07 20:19:05.386510 jellyfish-0.9.0/testdata/
+-rw-rw-rw-   0        0        0       77 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/README.md
+-rw-rw-rw-   0        0        0      164 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/damerau_levenshtein.csv
+-rw-rw-rw-   0        0        0      105 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/hamming.csv
+-rw-rw-rw-   0        0        0      142 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/jaro_distance.csv
+-rw-rw-rw-   0        0        0      303 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/jaro_winkler.csv
+-rw-rw-rw-   0        0        0      197 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/jaro_winkler_longtol.csv
+-rw-rw-rw-   0        0        0       68 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/levenshtein.csv
+-rw-rw-rw-   0        0        0      129 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/match_rating_codex.csv
+-rw-rw-rw-   0        0        0      139 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/match_rating_comparison.csv
+-rw-rw-rw-   0        0        0      475 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/metaphone.csv
+-rw-rw-rw-   0        0        0      449 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/nysiis.csv
+-rw-rw-rw-   0        0        0   377012 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/porter.csv
+-rw-rw-rw-   0        0        0      131 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/soundex.csv
+-rw-rw-rw-   0        0        0       98 2022-01-07 20:18:35.000000 jellyfish-0.9.0/testdata/wagner_fischer.csv
```

### Comparing `jellyfish-0.8.9/LICENSE` & `jellyfish-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jellyfish-0.8.9/README.rst` & `jellyfish-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,44 @@
-=========
-jellyfish
-=========
+Metadata-Version: 2.1
+Name: jellyfish
+Version: 0.9.0
+Summary: a library for doing approximate and phonetic matching of strings.
+Home-page: http://github.com/jamesturk/jellyfish
+License: UNKNOWN
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Text Processing :: Linguistic
+Requires-Python: >3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Overview
+
+**jellyfish** is a library for approximate & phonetic matching of strings.
+
+Source: [https://github.com/jamesturk/jellyfish](https://github.com/jamesturk/jellyfish)
+
+Documentation: [https://jamesturk.github.io/jellyfish/](https://jamesturk.github.io/jellyfish/)
+
+Issues: [https://github.com/jamesturk/jellyfish/issues](https://github.com/jamesturk/jellyfish/issues)
+
+[![PyPI badge](https://badge.fury.io/py/jellyfish.svg)](https://badge.fury.io/py/jellyfish)
+[![Test badge](https://github.com/jamesturk/jellyfish/workflows/Python%20package/badge.svg)](https://github.com/jamesturk/jellyfish/actions?query=workflow%3A%22Python+package)
+[![Coveralls](https://coveralls.io/repos/jamesturk/jellyfish/badge.png?branch=master)](https://coveralls.io/r/jamesturk/jellyfish)
 
-.. image:: https://github.com/jamesturk/jellyfish/workflows/Python%20package/badge.svg
 
-.. image:: https://coveralls.io/repos/jamesturk/jellyfish/badge.png?branch=master
-    :target: https://coveralls.io/r/jamesturk/jellyfish
-
-.. image:: https://img.shields.io/pypi/v/jellyfish.svg
-    :target: https://pypi.python.org/pypi/jellyfish
-
-.. image:: https://readthedocs.org/projects/jellyfish/badge/?version=latest
-    :target: https://readthedocs.org/projects/jellyfish/?badge=latest
-    :alt: Documentation Status
-
-Jellyfish is a python library for doing approximate and phonetic matching of strings.
-
-Written by James Turk <dev@jamesturk.net> and Michael Stephens.
-
-See https://github.com/jamesturk/jellyfish/graphs/contributors for contributors.
-
-See http://jellyfish.readthedocs.io for documentation.
-
-Source is available at http://github.com/jamesturk/jellyfish.
-
-**Jellyfish >= 0.7 only supports Python 3, if you need Python 2 please use 0.6.x.**
-
-Included Algorithms
-===================
+## Included Algorithms
 
 String comparison:
 
 * Levenshtein Distance
 * Damerau-Levenshtein Distance
 * Jaro Distance
 * Jaro-Winkler Distance
@@ -41,17 +48,17 @@
 Phonetic encoding:
 
 * American Soundex
 * Metaphone
 * NYSIIS (New York State Identification and Intelligence System)
 * Match Rating Codex
 
-Example Usage
-=============
+## Example Usage
 
+``` python
 >>> import jellyfish
 >>> jellyfish.levenshtein_distance(u'jellyfish', u'smellyfish')
 2
 >>> jellyfish.jaro_distance(u'jellyfish', u'smellyfish')
 0.89629629629629637
 >>> jellyfish.damerau_levenshtein_distance(u'jellyfish', u'jellyfihs')
 1
@@ -60,20 +67,10 @@
 'JLFX'
 >>> jellyfish.soundex(u'Jellyfish')
 'J412'
 >>> jellyfish.nysiis(u'Jellyfish')
 'JALYF'
 >>> jellyfish.match_rating_codex(u'Jellyfish')
 'JLLFSH'
+```
 
-Running Tests
-=============
-
-If you are interested in contributing to Jellyfish, you may want to
-run tests locally. Jellyfish uses tox_ to run tests, which you can
-setup and run as follows::
-
-  pip install tox
-  # cd jellyfish/
-  tox
 
-.. _tox: https://tox.readthedocs.io/en/latest/
```

### Comparing `jellyfish-0.8.9/cjellyfish/damerau_levenshtein.c` & `jellyfish-0.9.0/cjellyfish/damerau_levenshtein.c`

 * *Files identical despite different names*

### Comparing `jellyfish-0.8.9/cjellyfish/jaro.c` & `jellyfish-0.9.0/cjellyfish/jaro.c`

 * *Files identical despite different names*

### Comparing `jellyfish-0.8.9/cjellyfish/jellyfish.h` & `jellyfish-0.9.0/cjellyfish/jellyfish.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 #ifndef _JELLYFISH_H_
 #define _JELLYFISH_H_
 
 #include <stdlib.h>
 
 #if CJELLYFISH_PYTHON
 #include <Python.h>
-#define JFISH_UNICODE Py_UNICODE
+#define JFISH_UNICODE Py_UCS4
+#define ISALPHA Py_UNICODE_ISALPHA
+#else
+#include <wctype.h>
+#include <wchar.h>
+#define JFISH_UNICODE wint_t
+#define ISALPHA iswalpha
 #endif
 
 #ifndef MIN
 #define MIN(a, b) ((a) < (b) ? (a) : (b))
 #endif
 
 static inline void* safe_malloc(size_t num, size_t size)
```

### Comparing `jellyfish-0.8.9/cjellyfish/levenshtein.c` & `jellyfish-0.9.0/cjellyfish/levenshtein.c`

 * *Files identical despite different names*

### Comparing `jellyfish-0.8.9/cjellyfish/metaphone.c` & `jellyfish-0.9.0/cjellyfish/metaphone.c`

 * *Files identical despite different names*

### Comparing `jellyfish-0.8.9/cjellyfish/mra.c` & `jellyfish-0.9.0/cjellyfish/mra.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 #include "jellyfish.h"
 #include <string.h>
 #include <ctype.h>
 
+#define ISVOWEL(c) ((c) == 'A' || (c) == 'E' || (c) == 'I' || \
+                    (c) == 'O' || (c) == 'U')
+
+#define TRUE 1
+#define FALSE 0
+
 static size_t compute_match_rating_codex(const JFISH_UNICODE *str, size_t len, JFISH_UNICODE codex[7]);
 
 int match_rating_comparison(const JFISH_UNICODE *s1, size_t len1, const JFISH_UNICODE *s2, size_t len2) {
+    /* s1 and s2 are already in uppercase when this function is called */
     size_t s1c_len, s2c_len;
     size_t i, j;
     int diff;
     JFISH_UNICODE *longer;
 
     JFISH_UNICODE s1_codex[7], s2_codex[7];
     s1c_len = compute_match_rating_codex(s1, len1, s1_codex);
@@ -85,36 +92,37 @@
     }
     compute_match_rating_codex(str, len, codex);
 
     return codex;
 }
 
 static size_t compute_match_rating_codex(const JFISH_UNICODE *str, size_t len, JFISH_UNICODE codex[7]) {
+    /* str is already in uppercase when this function is called */
     size_t i, j;
+    int first;
     JFISH_UNICODE c, prev;
 
     prev = '\0';
+    first = TRUE;
     for(i = 0, j = 0; i < len && j < 7; i++) {
-        c = toupper(str[i]);
-
-        if (c == ' ' || (i != 0 && (c == 'A' || c == 'E' || c == 'I' ||
-                                    c == 'O' || c == 'U'))) {
+        c = str[i];
+        if (!ISALPHA(c)) {
+            prev = c;
             continue;
         }
 
-        if (c == prev) {
-            continue;
-        }
+        if (first || (!ISVOWEL(c) && c != prev)) {
+            if (j == 6) {
+                codex[3] = codex[4];
+                codex[4] = codex[5];
+                j = 5;
+            }
 
-        if (j == 6) {
-            codex[3] = codex[4];
-            codex[4] = codex[5];
-            j = 5;
+            codex[j++] = c;
         }
-
-        codex[j++] = c;
         prev = c;
+        first = FALSE;
     }
 
     codex[j] = '\0';
     return j;
 }
```

### Comparing `jellyfish-0.8.9/cjellyfish/nysiis.c` & `jellyfish-0.9.0/cjellyfish/nysiis.c`

 * *Files identical despite different names*

### Comparing `jellyfish-0.8.9/cjellyfish/porter.c` & `jellyfish-0.9.0/cjellyfish/porter.c`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
    It may be be regarded as cononical, in that it follows the algorithm
    presented in
 
    Porter, 1980, An algorithm for suffix stripping, Program, Vol. 14,
    no. 3, pp 130-137,
 
-   only differing from it at the points maked --DEPARTURE-- below.
+   only differing from it at the points marked --DEPARTURE-- below.
 
    See also http://www.tartarus.org/~martin/PorterStemmer
 
    The algorithm as described in the paper could be exactly replicated
    by adjusting the points of DEPARTURE, but this is barely necessary,
    because (a) the points of DEPARTURE are definitely improvements, and
    (b) no encoding of the Porter stemmer I have seen is anything like
```

### Comparing `jellyfish-0.8.9/cjellyfish/soundex.c` & `jellyfish-0.9.0/cjellyfish/soundex.c`

 * *Files identical despite different names*

### Comparing `jellyfish-0.8.9/docs/changelog.rst` & `jellyfish-0.9.0/docs/changelog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.9.0 - 7 January 2021
+----------------------
+* updated documentation available at https://jamesturk.github.io/jellyfish/
+* support for Python 3.10+
+* handle spaces correctly in MRA algorithm
+
 0.8.9 - 26 October 2021
 -----------------------
 * fix buffer overflow in NYSIIS
 * remove unnecessary/undocumented special casing of digits in Jaro-Winkler
 
 0.8.8 - 17 August 2021
 ----------------------
```

### Comparing `jellyfish-0.8.9/jellyfish/__init__.py` & `jellyfish-0.9.0/jellyfish/__init__.py`

 * *Files identical despite different names*

### Comparing `jellyfish-0.8.9/jellyfish/__init__.pyi` & `jellyfish-0.9.0/jellyfish/__init__.pyi`

 * *Files identical despite different names*

### Comparing `jellyfish-0.8.9/jellyfish/_jellyfish.py` & `jellyfish-0.9.0/jellyfish/_jellyfish.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         ("L", "4"),
         ("MN", "5"),
         ("R", "6"),
     )
     result = [s[0]]
     count = 1
 
-    # find would-be replacment for first character
+    # find would-be replacement for first character
     for lset, sub in replacements:
         if s[0] in lset:
             last = sub
             break
     else:
         last = None
 
@@ -331,26 +331,28 @@
 
     return key
 
 
 def match_rating_codex(s):
     _check_type(s)
 
-    s = s.upper()
+    # we ignore spaces
+    s = s.upper().replace(" ", "")
     codex = []
 
     prev = None
-    for i, c in enumerate(s):
-        # not a space OR
-        # starting character & vowel
+    first = True
+    for c in s:
+        # starting character
         # or consonant not preceded by same consonant
-        if c != " " and (i == 0 and c in "AEIOU") or (c not in "AEIOU" and c != prev):
+        if first or (c not in "AEIOU" and c != prev):
             codex.append(c)
 
         prev = c
+        first = False
 
     # just use first/last 3
     if len(codex) > 6:
         return "".join(codex[:3] + codex[-3:])
     else:
         return "".join(codex)
```

### Comparing `jellyfish-0.8.9/jellyfish/porter.py` & `jellyfish-0.9.0/jellyfish/porter.py`

 * *Files identical despite different names*

### Comparing `jellyfish-0.8.9/jellyfish/test.py` & `jellyfish-0.9.0/jellyfish/test.py`

 * *Files identical despite different names*

### Comparing `jellyfish-0.8.9/jellyfish.egg-info/SOURCES.txt` & `jellyfish-0.9.0/jellyfish.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 setup.py
 cjellyfish/damerau_levenshtein.c
 cjellyfish/hamming.c
 cjellyfish/jaro.c
 cjellyfish/jellyfish.h
 cjellyfish/jellyfishmodule.c
 cjellyfish/levenshtein.c
 cjellyfish/metaphone.c
 cjellyfish/mra.c
 cjellyfish/nysiis.c
 cjellyfish/porter.c
 cjellyfish/soundex.c
-docs/Makefile
-docs/changelog.rst
-docs/comparison.rst
-docs/conf.py
-docs/index.rst
-docs/phonetic.rst
-docs/stemming.rst
+docs/changelog.md
+docs/functions.md
+docs/index.md
 jellyfish/__init__.py
 jellyfish/__init__.pyi
 jellyfish/_jellyfish.py
 jellyfish/porter.py
 jellyfish/py.typed
 jellyfish/test.py
 jellyfish.egg-info/PKG-INFO
```

### Comparing `jellyfish-0.8.9/setup.py` & `jellyfish-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
             '''The command args string passed to
                                     unittest framework, such as --args="-v -f"''',
         )
     ]
 
     def initialize_options(self):
         self.args = ""
-        pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         self.run_command("build")
         bld = self.distribution.get_command_obj("build")
@@ -101,37 +100,38 @@
                 )
             ],
             cmdclass=dict(build_ext=ve_build_ext, test=TestCommand),
         )
     else:
         kw = dict(cmdclass=dict(test=TestCommand))
 
-    with open("README.rst") as readme:
+    with open("README.md") as readme:
         long_description = readme.read()
 
     setup(
         name="jellyfish",
-        version="0.8.9",
-        python_requires=">3.5",
+        version="0.9.0",
+        python_requires=">3.6",
         platforms=["any"],
         description=(
             "a library for doing approximate and " "phonetic matching of strings."
         ),
         url="http://github.com/jamesturk/jellyfish",
         long_description=long_description,
+        long_description_content_type="text/markdown",
         classifiers=[
             "Development Status :: 4 - Beta",
             "Intended Audience :: Developers",
             "License :: OSI Approved :: BSD License",
             "Natural Language :: English",
             "Operating System :: OS Independent",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
             "Topic :: Text Processing :: Linguistic",
         ],
         packages=["jellyfish"],
         package_data={"jellyfish": ["*.pyi", "py.typed"]},
         **kw
     )
```

### Comparing `jellyfish-0.8.9/testdata/porter.csv` & `jellyfish-0.9.0/testdata/porter.csv`

 * *Files identical despite different names*

