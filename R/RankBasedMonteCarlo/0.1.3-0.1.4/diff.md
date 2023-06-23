# Comparing `tmp/RankBasedMonteCarlo-0.1.3.tar.gz` & `tmp/rankbasedmontecarlo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RankBasedMonteCarlo-0.1.3.tar", last modified: Mon Nov  4 12:39:43 2019, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `RankBasedMonteCarlo-0.1.3.tar` & `rankbasedmontecarlo-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,11 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2019-11-04 12:39:43.000000 RankBasedMonteCarlo-0.1.3/
--rw-r--r--   0 ben        (501) staff       (20)      887 2019-11-04 12:39:43.000000 RankBasedMonteCarlo-0.1.3/PKG-INFO
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2019-11-04 12:39:43.000000 RankBasedMonteCarlo-0.1.3/RankBasedMonteCarlo/
--rw-r--r--   0 ben        (501) staff       (20)    11259 2019-11-04 12:11:01.000000 RankBasedMonteCarlo-0.1.3/RankBasedMonteCarlo/Methods.py
--rw-r--r--   0 ben        (501) staff       (20)      115 2019-10-31 12:23:07.000000 RankBasedMonteCarlo-0.1.3/RankBasedMonteCarlo/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)       39 2019-11-02 16:22:02.000000 RankBasedMonteCarlo-0.1.3/setup.cfg
--rw-r--r--   0 ben        (501) staff       (20)     1035 2019-11-04 12:33:03.000000 RankBasedMonteCarlo-0.1.3/setup.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rankbasedmontecarlo-0.1.4/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 rankbasedmontecarlo-0.1.4/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rankbasedmontecarlo-0.1.4/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rankbasedmontecarlo-0.1.4/src/RankBasedMonteCarlo/.DS_Store
+-rw-r--r--   0        0        0    11298 2020-02-02 00:00:00.000000 rankbasedmontecarlo-0.1.4/src/RankBasedMonteCarlo/Methods.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 rankbasedmontecarlo-0.1.4/src/RankBasedMonteCarlo/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 rankbasedmontecarlo-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 rankbasedmontecarlo-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 rankbasedmontecarlo-0.1.4/README.md
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 rankbasedmontecarlo-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 rankbasedmontecarlo-0.1.4/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `RankBasedMonteCarlo-0.1.3/PKG-INFO` & `rankbasedmontecarlo-0.1.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,38 @@
-Metadata-Version: 1.1
-Name: RankBasedMonteCarlo
-Version: 0.1.3
-Summary: A set of Monte Carlo based tools to create test statistics for four non-parametric rank-based tests: Mann-Whitney (MW), Kruskal-Wallis (KW), Kolmogorov-Smirnov (KS) and Kuiper (K).
-Home-page: https://github.com/tazzben/RankBasedMonteCarlo
-Author: Ben Smith
-Author-email: bosmith@unomaha.edu
-License: MIT
-Download-URL: https://github.com/tazzben/RankBasedMonteCarlo/archive/v0.1.3.tar.gz
-Description: UNKNOWN
-Keywords: Monte Carlo,Rank based,Statistics
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "RankBasedMonteCarlo"
+version = "0.1.4"
+description = "A set of Monte Carlo based tools to create test statistics for four non-parametric rank-based tests: Mann-Whitney (MW), Kruskal-Wallis (KW), Kolmogorov-Smirnov (KS) and Kuiper (K)."
+license = "MIT"
+authors = [
+  { name="Ben Smith", email="bosmith@unomaha.edu" },
+]
+maintainers = [
+  { name="Ben Smith", email="bosmith@unomaha.edu" },
+]
+readme = "README.md"
+homepage = "https://github.com/tazzben/RankBasedMonteCarlo"
+repository = "https://github.com/tazzben/RankBasedMonteCarlo"
+keywords = ["Monte Carlo", "Rank based", "Statistics"]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
+]
+requires-python = ">=3.8"
+dependencies = [
+    "numpy>=1.21.0",
+    "pandas>=1.3.0",
+    "tqdm>=4.26.0",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/tazzben/RankBasedMonteCarlo"
+"Bug Tracker" = "https://github.com/tazzben/RankBasedMonteCarlo/issues"
```

### Comparing `RankBasedMonteCarlo-0.1.3/RankBasedMonteCarlo/Methods.py` & `rankbasedmontecarlo-0.1.4/src/RankBasedMonteCarlo/Methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy
 import pandas
 import sys
 import multiprocessing
-
+from tqdm import tqdm
 
 class _RankBasedMonteCarlo:
     def _RandomRank(self, ns):
         objects = numpy.concatenate(
             [numpy.repeat((i + 1), n) for i, n in enumerate(ns)], axis=None
         )
         numpy.random.shuffle(objects)
@@ -18,15 +18,15 @@
         sample = self._RandomRank(sampleSizes)
         return self._CalculateStatistic(sample)
 
     def _PoolMonteCarlo(self, ns, reps):
         p = multiprocessing.Pool()
         r = []
         for i, result in enumerate(
-            p.imap_unordered(self._RandomStatistic, (ns,) * reps)
+            tqdm(p.imap_unordered(self._RandomStatistic, (ns,) * reps), total=reps)
         ):
             r.append(result)
             sys.stderr.write("\r{: .2f}% done".format(100 * i / reps))
         p.close()
         p.join()
         return numpy.array(r)
```

