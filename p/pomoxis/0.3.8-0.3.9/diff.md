# Comparing `tmp/pomoxis-0.3.8.tar.gz` & `tmp/pomoxis-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pomoxis-0.3.8.tar", last modified: Wed Jun 23 08:44:09 2021, max compression
+gzip compressed data, was "pomoxis-0.3.9.tar", last modified: Wed Aug 18 15:01:28 2021, max compression
```

## Comparing `pomoxis-0.3.8.tar` & `pomoxis-0.3.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 08:44:09.348260 pomoxis-0.3.8/
--rw-rw-rw-   0 root         (0) root         (0)    15820 2021-06-23 08:43:43.000000 pomoxis-0.3.8/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      115 2021-06-23 08:43:43.000000 pomoxis-0.3.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     5964 2021-06-23 08:43:43.000000 pomoxis-0.3.8/Makefile
--rw-r--r--   0 root         (0) root         (0)     6041 2021-06-23 08:44:09.348260 pomoxis-0.3.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5721 2021-06-23 08:43:43.000000 pomoxis-0.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 08:44:09.344260 pomoxis-0.3.8/images/
--rw-rw-rw-   0 root         (0) root         (0)    35610 2021-06-23 08:43:43.000000 pomoxis-0.3.8/images/ONT_logo_590x106.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 08:44:09.344260 pomoxis-0.3.8/pomoxis/
--rw-rw-rw-   0 root         (0) root         (0)     1466 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20228 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/assess_homopolymers.py
--rw-rw-rw-   0 root         (0) root         (0)     2577 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/bio.py
--rw-rw-rw-   0 root         (0) root         (0)    46389 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/catalogue_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     6482 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/common_errors_from_bam.py
--rw-rw-rw-   0 root         (0) root         (0)     3853 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/coverage_from_bam.py
--rw-rw-rw-   0 root         (0) root         (0)     5160 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/find_indels.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/qscores_from_summary.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/ref_seqs_from_bam.py
--rw-rw-rw-   0 root         (0) root         (0)     9628 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/stats_from_bam.py
--rw-rw-rw-   0 root         (0) root         (0)    12156 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/subsample_bam.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/summary_from_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     4332 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/trim_alignments.py
--rw-rw-rw-   0 root         (0) root         (0)    15442 2021-06-23 08:43:43.000000 pomoxis-0.3.8/pomoxis/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 08:44:09.348260 pomoxis-0.3.8/pomoxis.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6041 2021-06-23 08:44:09.000000 pomoxis-0.3.8/pomoxis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2021-06-23 08:44:09.000000 pomoxis-0.3.8/pomoxis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-23 08:44:09.000000 pomoxis-0.3.8/pomoxis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      866 2021-06-23 08:44:09.000000 pomoxis-0.3.8/pomoxis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-06-23 08:44:09.000000 pomoxis-0.3.8/pomoxis.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       85 2021-06-23 08:44:09.000000 pomoxis-0.3.8/pomoxis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2021-06-23 08:44:09.000000 pomoxis-0.3.8/pomoxis.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      286 2021-06-23 08:43:43.000000 pomoxis-0.3.8/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-06-23 08:44:09.348260 pomoxis-0.3.8/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     4408 2021-06-23 08:43:43.000000 pomoxis-0.3.8/scripts/assess_assembly
--rwxrwxrwx   0 root         (0) root         (0)     2094 2021-06-23 08:43:43.000000 pomoxis-0.3.8/scripts/intersect_assembly_errors
--rwxrwxrwx   0 root         (0) root         (0)     4876 2021-06-23 08:43:43.000000 pomoxis-0.3.8/scripts/mini_align
--rwxrwxrwx   0 root         (0) root         (0)     7841 2021-06-23 08:43:43.000000 pomoxis-0.3.8/scripts/mini_assemble
--rw-r--r--   0 root         (0) root         (0)       38 2021-06-23 08:44:09.348260 pomoxis-0.3.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5469 2021-06-23 08:43:43.000000 pomoxis-0.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 15:01:28.360728 pomoxis-0.3.9/
+-rw-rw-rw-   0 root         (0) root         (0)    15820 2021-08-18 11:13:05.000000 pomoxis-0.3.9/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      115 2021-08-18 11:13:05.000000 pomoxis-0.3.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     5964 2021-08-18 11:13:05.000000 pomoxis-0.3.9/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6041 2021-08-18 15:01:28.360728 pomoxis-0.3.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2021-08-18 11:13:05.000000 pomoxis-0.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 15:01:28.324725 pomoxis-0.3.9/images/
+-rw-rw-rw-   0 root         (0) root         (0)    35610 2021-08-18 11:13:05.000000 pomoxis-0.3.9/images/ONT_logo_590x106.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 15:01:28.356728 pomoxis-0.3.9/pomoxis/
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2021-08-18 15:00:49.000000 pomoxis-0.3.9/pomoxis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22740 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/assess_homopolymers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/bio.py
+-rw-rw-rw-   0 root         (0) root         (0)    48547 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/catalogue_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     6482 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/common_errors_from_bam.py
+-rw-rw-rw-   0 root         (0) root         (0)     3853 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/coverage_from_bam.py
+-rw-rw-rw-   0 root         (0) root         (0)     5160 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/find_indels.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/qscores_from_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/ref_seqs_from_bam.py
+-rw-rw-rw-   0 root         (0) root         (0)     9628 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/stats_from_bam.py
+-rw-rw-rw-   0 root         (0) root         (0)    12156 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/subsample_bam.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/summary_from_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     4332 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/trim_alignments.py
+-rw-rw-rw-   0 root         (0) root         (0)    15893 2021-08-18 11:13:05.000000 pomoxis-0.3.9/pomoxis/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 15:01:28.360728 pomoxis-0.3.9/pomoxis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6041 2021-08-18 15:01:28.000000 pomoxis-0.3.9/pomoxis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      777 2021-08-18 15:01:28.000000 pomoxis-0.3.9/pomoxis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-18 15:01:28.000000 pomoxis-0.3.9/pomoxis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      866 2021-08-18 15:01:28.000000 pomoxis-0.3.9/pomoxis.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-08-18 15:01:28.000000 pomoxis-0.3.9/pomoxis.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       85 2021-08-18 15:01:28.000000 pomoxis-0.3.9/pomoxis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2021-08-18 15:01:28.000000 pomoxis-0.3.9/pomoxis.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      286 2021-08-18 11:13:05.000000 pomoxis-0.3.9/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-18 15:01:28.360728 pomoxis-0.3.9/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     4432 2021-08-18 11:13:05.000000 pomoxis-0.3.9/scripts/assess_assembly
+-rwxrwxrwx   0 root         (0) root         (0)     2094 2021-08-18 11:13:05.000000 pomoxis-0.3.9/scripts/intersect_assembly_errors
+-rwxrwxrwx   0 root         (0) root         (0)     4876 2021-08-18 11:13:05.000000 pomoxis-0.3.9/scripts/mini_align
+-rwxrwxrwx   0 root         (0) root         (0)     7841 2021-08-18 11:13:05.000000 pomoxis-0.3.9/scripts/mini_assemble
+-rw-r--r--   0 root         (0) root         (0)       38 2021-08-18 15:01:28.360728 pomoxis-0.3.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5469 2021-08-18 11:13:05.000000 pomoxis-0.3.9/setup.py
```

### Comparing `pomoxis-0.3.8/LICENSE.md` & `pomoxis-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/Makefile` & `pomoxis-0.3.9/Makefile`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/PKG-INFO` & `pomoxis-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomoxis
-Version: 0.3.8
+Version: 0.3.9
 Summary: Assembly, consensensus, and analysis tools by ONT research.
 Home-page: UNKNOWN
 Author: cwright
 Author-email: cwright@nanoporetech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `pomoxis-0.3.8/README.md` & `pomoxis-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/images/ONT_logo_590x106.png` & `pomoxis-0.3.9/images/ONT_logo_590x106.png`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis/__init__.py` & `pomoxis-0.3.9/pomoxis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 
 import argparse
 import os
 import sys
 import platform
 import subprocess
```

### Comparing `pomoxis-0.3.8/pomoxis/assess_homopolymers.py` & `pomoxis-0.3.9/pomoxis/assess_homopolymers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import argparse
 import collections
+import concurrent.futures
+from functools import partial
+from math import ceil
 import os
 import pickle
 import re
+import shutil
 
 import matplotlib
 matplotlib.use('Agg', force=True)
 
 import  matplotlib.pyplot as plt
 from matplotlib.ticker import MaxNLocator
 import numpy as np
@@ -220,35 +224,70 @@
     fig.savefig(fname)
     plt.close(fig)
 
 
 def count_homopolymers(args):
     os.mkdir(args.output_dir)
 
-    score = AverageScore()
-    headers = [
-        'query_name', 'ref_name', 'ref_start', 'rev_comp', 'query_start',
-        'ref_base', 'query_base', 'ref_len', 'query_len']
+    # create a slice of reads to process in each thread to avoid looping through
+    # bam n read times and reduce mp overhead
+    ranges = [(0, 0, float('inf'))]
+    if args.threads > 1:
+        with pysam.AlignmentFile(args.bam) as bam:
+            n_reads = bam.count(until_eof=True)
+        n_reads_per_proc = ceil(n_reads / args.threads)
+        ranges = [(thread, thread * n_reads_per_proc, min((thread + 1) * n_reads_per_proc, n_reads))
+                   for thread in range(args.threads)]
+
+    headers = ['query_name', 'ref_name', 'ref_start', 'rev_comp', 'query_start',
+               'ref_base', 'query_base', 'ref_len', 'query_len']
 
     prefix = os.path.join(args.output_dir, 'hp')
 
+    total_score = AverageScore()
+    total_counts = collections.defaultdict(counts_factory)
+    total_aligned_length = 0
+
     if args.bed is not None:
         filter_trees = pomoxis.util.intervaltrees_from_bed(args.bed)
     else:
         filter_trees = None
 
+    f = partial(process_bam, args.bam, prefix, args.homo_len, filter_trees=filter_trees)
+
+    with concurrent.futures.ProcessPoolExecutor(max_workers=args.threads) as ex:
+        for returned in ex.map(f, ranges):
+            if returned is None:
+                continue
+            else:
+                score, counts, aligned_length = returned
+                for base in counts:
+                    for rlen in counts[base]:
+                        total_counts[base][rlen].update(counts[base][rlen])
+                total_score += score
+                total_aligned_length += aligned_length
+
+    print("Found {} homopolymers in {}. Average score: {}".format(
+        total_score.count, args.bam, total_score))
+    total_counts['length'] = total_aligned_length
+
     with open(prefix + '_catalogue.txt', 'w') as txt_fh:
         txt_fh.write('\t'.join(headers) + "\n")
-        score, counts, aligned_length = process_bam(args.bam, txt_fh, args.homo_len, score,
-                                                    filter_trees=filter_trees)
-    print("Found {} homopolymers in {}. Average score: {}".format(
-        score.count, args.bam, score))
-    counts['length'] = aligned_length
-    save_counts(counts, prefix + '_counts.pkl')
-    analyse_counts(counts, prefix, aligned_length)
+        for f in [prefix + '_catalogue_{}.txt'.format(n) for n in range(args.threads)]:
+            try:
+                with open(f, 'r') as infile:
+                    shutil.copyfileobj(infile, txt_fh)
+            except:
+                print("Error merging file {}".format(f))
+            else:
+                print("Merged file {}, deleting".format(f))
+                os.remove(f)
+
+    save_counts(total_counts, prefix + '_counts.pkl')
+    analyse_counts(total_counts, prefix, total_aligned_length)
 
 
 def save_counts(counts, fp):
     # convert counts from nested defaultdict with factory function to plain dict
     counts = {k: v if type(v) == int else dict(v) for k,v in counts.items()}
     with open(fp, 'wb') as pkl_fh:
         pickle.dump(counts, pkl_fh)
@@ -376,21 +415,43 @@
     return query_sequence[query_start + extend_backward + 1:query_end + extend_fwd]
 
 
 def counts_factory():
     return collections.defaultdict(collections.Counter)
 
 
-def process_bam(input_file, out_fh, homo_len, score, filter_trees=None):
-    # counts[query_base][ref_len][query_len]
+def process_bam(bam, prefix, homo_len, read_range, filter_trees=None):
+    """Count HPs in a chunk of reads.
+
+    :param bam: str, path to bam file
+    :param prefix: str, prefix for output paths
+    :param homo_len: int, minimum ref length of HPs to count
+    :param read_range: (int, int, int), chunk number, read index start and end
+    :param filter_trees: intervalTree, regions to analyse
+    :returns: score, counts, aligned_ref_len
+        score, AverageScore object
+        counts, defaultdict of defaultdicts of Counters, counts by contig, ref length,
+            query length
+        aligned_ref_len, int
+    """
     counts = collections.defaultdict(counts_factory)
+    score = AverageScore()
+    aligned_ref_len = 0
 
-    with pysam.AlignmentFile(input_file, 'r') as bam:
+    catalogue_path = prefix + '_catalogue_{}.txt'.format(read_range[0])
+    out_fh = open(catalogue_path, 'w')
+
+    with pysam.AlignmentFile(bam, 'r') as bam_obj:
         aligned_ref_len = 0
-        for seq in bam:
+        for i, seq in enumerate(bam_obj.fetch(until_eof=True)):
+            if i < read_range[1]:
+                continue
+            elif i == read_range[2]:
+                break
+
             if seq.is_secondary or seq.is_supplementary or seq.is_unmapped:
                 continue
             seq_reference_start = seq.reference_start  # avoid recomputing for each HP
             seq_reference_end = seq.reference_end  # avoid recomputing for each HP
 
             if (filter_trees is not None and not
                 filter_trees[seq.reference_name].overlaps(seq_reference_start, seq_reference_end)):
@@ -463,14 +524,17 @@
                     orginal_base,
                     base,
                     ref_hp_len,
                     call_len)])
                 out_fh.write(out_str + '\n')
                 # update counts of calls
                 counts[base][ref_hp_len][call_len] += 1
+
+    out_fh.close()
+
     return score, counts, aligned_ref_len
 
 
 def main():
     """Entry point for homopolymer accuracy counting."""
     parser = argparse.ArgumentParser(
         prog='assess_homopolymers',
@@ -484,14 +548,16 @@
     cparser = subparsers.add_parser('count',
         help='Count homopolymers starting from a bam. ',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     cparser.set_defaults(func=count_homopolymers)
     cparser.add_argument('bam', help='Input bam file.')
     cparser.add_argument('-o', '--output_dir', default='homopolymers',
         help="Output directory (will be created).")
+    cparser.add_argument('-t', '--threads', type=int, default=1,
+        help='Number of threads for parallel execution.')
     cparser.add_argument('-l', '--homo_len', default=3, type=int,
         help='Minimum homopolymer length, default 3')
     cparser.add_argument('-b', '--bed',
         help='Bed file to limit search.')
 
     aparser = subparsers.add_parser('analyse',
         help='Analyse existing counts, optionally merging multiple counters.',
```

### Comparing `pomoxis-0.3.8/pomoxis/bio.py` & `pomoxis-0.3.9/pomoxis/bio.py`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis/catalogue_errors.py` & `pomoxis-0.3.9/pomoxis/catalogue_errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import argparse
 from collections import defaultdict, Counter, namedtuple
 import concurrent.futures
 from functools import partial
 import itertools
 import logging
+import shutil
+from math import ceil
 from operator import attrgetter
 import os
 import pickle
 import re
 import unittest
 import warnings
 
@@ -553,61 +555,90 @@
     if l_i == len(sizes):
         size = "> {}".format(sizes[-1])
     else:
         size = "<= {}".format(sizes[l_i])
     return size
 
 
-def _process_read(bam, read_num, bed_file=None):
+def _process_read(bam, outdir, read_range, bed_file=None):
     """Load an alignment from bam and return result of `_process_seg`.
 
     :param bam: str, bam file.
-    :param read_num: int, index of alignment to process.
+    :param outdir: str, output path
+    :param read_range: (int, int, int), process number, range of alignments to process.
     :param bed_file: path to .bed file of regions to include in analysis.
     :returns: result of `_process_seg`.
     """
     trees = None
     if bed_file is not None:
         trees = intervaltrees_from_bed(bed_file)
 
-    with pysam.AlignmentFile(bam, 'rb') as bam_obj:
-        gen = (r for r in bam_obj)
-        for i in range(read_num + 1):
-            rec = next(gen)
-        if rec.is_unmapped or rec.is_supplementary or rec.is_secondary:
-            return
+    total_ref_length = defaultdict(int)
+    total_n_ref_sites_masked = defaultdict(int)
+    error_count = defaultdict(Counter)
+
+    db_path = os.path.join(outdir, 'error_catalogue_db_{}.txt'.format(read_range[0]))
+    txt_path = os.path.join(outdir, 'error_catalogue_{}.txt'.format(read_range[0]))
+    db_fh = open(db_path, 'w')
+    txt_fh = open(txt_path, 'w')
+    headers = get_headers()
 
-        if bed_file is not None:
-            tree = trees[rec.reference_name]
+    with pysam.AlignmentFile(bam, 'rb') as bam_obj:
+        for i, rec in enumerate(bam_obj.fetch(until_eof=True)):
+            if i < read_range[1]:
+                continue
+            elif i == read_range[2]:
+                break
 
-            if not tree.overlaps(rec.reference_start, rec.reference_end):
-                #sys.stderr.write('read {} does not overlap with any regions in bedfile\n'.format(rec.query_name))
+            if rec.is_unmapped or rec.is_supplementary or rec.is_secondary:
                 return
-        else:
-            tree = None
 
-        seg = AlignSeg(rname=rec.reference_name, qname=rec.query_name,
-                       pairs=list(get_trimmed_pairs(rec)), rlen=rec.reference_length
-                      )
-        logging.debug('Loaded query {}'.format(seg.qname))
-        return _process_seg(seg, tree)
+            if bed_file is not None:
+                tree = trees[rec.reference_name]
+
+                if not tree.overlaps(rec.reference_start, rec.reference_end):
+                    #sys.stderr.write('read {} does not overlap with any regions in bedfile\n'.format(rec.query_name))
+                    continue
+            else:
+                tree = None
+
+            seg = AlignSeg(rname=rec.reference_name, qname=rec.query_name,
+                           pairs=list(get_trimmed_pairs(rec)), rlen=rec.reference_length
+                          )
+            logging.debug('Loaded query {}'.format(seg.qname))
 
+            seg_result = _process_seg(seg, db_fh, txt_fh, headers, tree)
+            if seg_result is None:
+                continue
+
+            ref_name, ref_length, counts, n_masked = seg_result
+            
+            error_count[ref_name].update(counts)
+            total_ref_length[ref_name] += ref_length
+            total_n_ref_sites_masked[ref_name] += n_masked
+
+    db_fh.close()
+    txt_fh.close()
+
+    return error_count, total_ref_length, total_n_ref_sites_masked
 
-def _process_seg(seg, tree=None):
+
+def _process_seg(seg, db_fh, txt_fh, headers, tree=None):
     """Classify and count errors within an `AlignSeg` object.
 
     :param seg: `AlignSeg` object.
+    :param db_fh: file object, catalogue db file
+    :param txt_fh: file object, catalogue file
+    :param headers: list of tuples, error properties and their label ids
     :param tree: `intervaltree.IntervalTree` object of regions to analyse.
-    :returns: (seg.rname, aligned_ref_len, error_count, errors, n_masked)
+    :returns: (seg.rname, aligned_ref_len, error_count, n_masked)
         error_count: `Counter` of error classes
-        errors: list of `Error` objects
         n_masked: number of reference positions excluded by tree.
     """
     error_count = Counter()
-    errors = []
     err_result = get_errors(seg.pairs, tree)
     if err_result is None:  # no matches within bed regions
         logging.debug('Skipping {} since all bed regions were deleted'.format(
                       seg.qname))
         return None
 
     pos_and_errors, aligned_ref_len, n_masked = err_result
@@ -618,24 +649,32 @@
 
         rp = ri
         qp = qi
         if rp is None:
             rp = "~{}".format(approx_pos[0])
         if qp is None:
             qp = "~{}".format(approx_pos[1])
-        errors.append(Error(rp=rp, rname=seg.rname, qp=qp, qname=seg.qname, ref=ref,
-                            match=match, read=read, counts=counts, klass=klass,
-                            aggr_klass=get_aggr_klass(klass)))
+
+        e = Error(rp=rp, rname=seg.rname, qp=qp, qname=seg.qname, ref=ref,
+                  match=match, read=read, counts=counts, klass=klass,
+                  aggr_klass=get_aggr_klass(klass))
         error_count[klass] += 1
 
+        db_fh.write(_sep_.join((str(h[1](e)) for h in headers)) + '\n')
+        txt_fh.write("Ref Pos: {}, {} Pos {}, {}, {}\n".format(e.rp, e.qname, e.qp, e.klass, e.aggr_klass))
+        txt_fh.write(e.ref + "\n")
+        txt_fh.write(e.match + "\n")
+        txt_fh.write(e.read + "\n")
+        txt_fh.write(".\n")
+
     if tree is None:
         assert seg.rlen == aligned_ref_len
 
     logging.debug('Done processing {} aligned to {}'.format(seg.qname, seg.rname))
-    return seg.rname, aligned_ref_len, error_count, errors, n_masked
+    return seg.rname, aligned_ref_len, error_count, n_masked
 
 
 def qscore(d):
     """Calculate a qscore"""
     with warnings.catch_warnings():
         # some values might be zero
         warnings.simplefilter("ignore")
@@ -698,15 +737,14 @@
                 aggr_klass = '{} {}'.format(error_type, max_indel)
             else:
                 aggr_klass = error_type
             break
     return aggr_klass
 
 
-
 def analyse_errors(args):
     # load and merge existing counts
     error_count = defaultdict(Counter)
     total_ref_length = Counter()
     total_n_ref_sites_masked = Counter()
     for pkl in args.pkl:
         with open(pkl, 'rb') as fh:
@@ -725,67 +763,89 @@
             error_count[ref].update(d_counts)
         total_ref_length.update(counts['ref_lengths'])
         total_n_ref_sites_masked.update(counts['n_ref_sites_masked'])
 
     aggr_and_output(args, error_count, total_ref_length, total_n_ref_sites_masked)
 
 
+def get_headers():
+    # make an approximate position into int
+    helper = lambda x: int(x.replace('~','')) if isinstance(x, str) else x
+
+    return [('ref_name', attrgetter('rname')),
+            ('ref_pos', helper(attrgetter('rp'))),
+            ('ref_context', attrgetter('ref')),
+            ('query_name', attrgetter('qname')),
+            ('query_pos', helper(attrgetter('qp'))),
+            ('query_context', attrgetter('read')),
+            ('class', attrgetter('klass')),
+            ('aggr_class', attrgetter('aggr_klass')),
+            ('n_ins', lambda e: len(e.counts['ins'])),
+            ('n_del', lambda e: len(e.counts['del'])),
+            ('n_sub', lambda e: len(e.counts['sub'])),
+            ('context_len', lambda e: len(e.ref)),
+    ]
+
+
 def count_errors(args):
-    with pysam.AlignmentFile(args.bam, 'rb') as bam:
-        n_reads = bam.count()
+    # create a slice of reads to process in each thread to avoid looping through
+    # bam n read times and reduce mp overhead
+    ranges = [(0, 0, float('inf'))]
+    if args.threads > 1:
+        with pysam.AlignmentFile(args.bam) as bam:
+            n_reads = bam.count(until_eof=True)
+        n_reads_per_proc = ceil(n_reads / args.threads)
+        ranges = [(thread, thread * n_reads_per_proc, min((thread + 1) * n_reads_per_proc, n_reads))
+                   for thread in range(args.threads)]
 
     total_ref_length = defaultdict(int)
     total_n_ref_sites_masked = defaultdict(int)
     error_count = defaultdict(Counter)
-    f = partial(_process_read, args.bam, bed_file=args.bed)
 
     # record draft start position of each long multi indel
     multi_errs = {}
-    # make an approximate position into int
-    helper = lambda x: int(x.replace('~','')) if isinstance(x, str) else x
-    db_fh = open(os.path.join(args.outdir, 'error_catalogue_db.txt'), 'w')
-    txt_fh = open(os.path.join(args.outdir, 'error_catalogue.txt'), 'w')
 
-    headers = [('ref_name', attrgetter('rname')),
-                ('ref_pos', helper(attrgetter('rp'))),
-                ('ref_context', attrgetter('ref')),
-                ('query_name', attrgetter('qname')),
-                ('query_pos', helper(attrgetter('qp'))),
-                ('query_context', attrgetter('read')),
-                ('class', attrgetter('klass')),
-                ('aggr_class', attrgetter('aggr_klass')),
-                ('n_ins', lambda e: len(e.counts['ins'])),
-                ('n_del', lambda e: len(e.counts['del'])),
-                ('n_sub', lambda e: len(e.counts['sub'])),
-                ('context_len', lambda e: len(e.ref)),
-    ]
-    db_fh.write(_sep_.join((h[0] for h in headers)) + '\n')
+    f = partial(_process_read, args.bam, args.outdir, bed_file=args.bed)
 
     with concurrent.futures.ProcessPoolExecutor(max_workers=args.threads) as ex:
-        for returned in ex.map(f, range(n_reads)):
+        for returned in ex.map(f, ranges):
             if returned is None:
                 continue
             else:
-                ref_name, ref_length, counts, errors, n_masked = returned
-            error_count[ref_name].update(counts)
-            total_ref_length[ref_name] += ref_length
-            total_n_ref_sites_masked[ref_name] += n_masked
-            for e in errors:
-                db_fh.write(_sep_.join((str(h[1](e)) for h in headers)) + '\n')
-                txt_fh.write("Ref Pos: {}, {} Pos {}, {}, {}\n".format(e.rp, e.qname, e.qp, e.klass, e.aggr_klass))
-                txt_fh.write(e.ref + "\n")
-                txt_fh.write(e.match + "\n")
-                txt_fh.write(e.read + "\n")
-                txt_fh.write(".\n")
+                counts, ref_length, n_masked = returned
+
+            for ref_name in counts:
+                error_count[ref_name].update(counts[ref_name])
+                total_ref_length[ref_name] += ref_length[ref_name]
+                total_n_ref_sites_masked[ref_name] += n_masked[ref_name]
+
+    db_fh = open(os.path.join(args.outdir, 'error_catalogue_db.txt'), 'w')
+    db_fh.write(_sep_.join((h[0] for h in get_headers())) + '\n')
+    merge_catalogues(db_fh, [os.path.join(args.outdir, 'error_catalogue_db_{}.txt'.format(n)) for n in range(args.threads)])
     db_fh.close()
+
+    txt_fh = open(os.path.join(args.outdir, 'error_catalogue.txt'), 'w')
+    merge_catalogues(txt_fh, [os.path.join(args.outdir, 'error_catalogue_{}.txt'.format(n)) for n in range(args.threads)])
     txt_fh.close()
 
     aggr_and_output(args, error_count, total_ref_length, total_n_ref_sites_masked)
 
 
+def merge_catalogues(outfile, filenames):
+    for f in filenames:
+        try:
+            with open(f, 'r') as infile:
+                shutil.copyfileobj(infile, outfile)
+        except:
+            logging.info("Error merging file {}".format(f))
+        else:
+            logging.info("Merged file {}, deleting".format(f))
+            os.remove(f)
+
+
 def aggr_and_output(args, error_count, total_ref_length, total_n_ref_sites_masked):
     total_counts = Counter()
     aggr_by_ref = {}
     for ref_name, counts in error_count.items():
         df = analyze_counts(counts, total_ref_length[ref_name])
         fp = os.path.join(args.outdir, '{}_error_summary.txt'.format(ref_name))
         df.to_csv(fp, sep=_sep_, index=False)
```

### Comparing `pomoxis-0.3.8/pomoxis/common_errors_from_bam.py` & `pomoxis-0.3.9/pomoxis/common_errors_from_bam.py`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis/coverage_from_bam.py` & `pomoxis-0.3.9/pomoxis/coverage_from_bam.py`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis/find_indels.py` & `pomoxis-0.3.9/pomoxis/find_indels.py`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis/qscores_from_summary.py` & `pomoxis-0.3.9/pomoxis/qscores_from_summary.py`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis/ref_seqs_from_bam.py` & `pomoxis-0.3.9/pomoxis/ref_seqs_from_bam.py`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis/stats_from_bam.py` & `pomoxis-0.3.9/pomoxis/stats_from_bam.py`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis/subsample_bam.py` & `pomoxis-0.3.9/pomoxis/subsample_bam.py`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis/summary_from_stats.py` & `pomoxis-0.3.9/pomoxis/summary_from_stats.py`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis/trim_alignments.py` & `pomoxis-0.3.9/pomoxis/trim_alignments.py`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis/util.py` & `pomoxis-0.3.9/pomoxis/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                 if qual is None:
                     for i, s in enumerate(chunks(seq, chunksize)):
                         chunk_name = '{}_chunk{}'.format(name, i)
                         fout.write(chunk_name, s, comment=comment)
                 else:
                     for i, (s, q) in enumerate(zip(chunks(seq, chunksize), chunks(qual, chunksize))):
                         chunk_name = '{}_chunk{}'.format(name, i)
-                        fout.write(chunk_name, s, q, comment)
+                        fout.write(chunk_name, ''.join(s), ''.join(q), comment)
 
 
 def split_fastx_cmdline():
     """Split records in a fasta/q file into chunks of a maximum size."""
     parser = argparse.ArgumentParser(
         prog='split_fastx',
         description='Split records in a fasta/q file into chunks of a maximum size.',
@@ -151,17 +151,21 @@
         pass # default
     else:
         raise ValueError("convert must be 'qq', 'aq', 'qa', or 'aa'\n")
 
     with FastxWrite('-', force_q=out_fmt=='fastq', mock_q=args.mock_q) as fh_out:
         with pysam.FastxFile('-') as fh_in:
             for rec in fh_in:
-                qual = rec.quality
-                if qflag and (in_fmt=='fasta' or args.discard_q):
+                if out_fmt == 'fasta':
+                    qual = None
+                elif qflag:
                     qual = chr(33 + args.mock_q) * len(rec.sequence)
+                else:
+                    qual = rec.quality
+
                 fh_out.write(rec.name, rec.sequence, qual, rec.comment)
 
 
 def extract_long_reads():
     """Filter fastq to longest reads."""
 
     parser = argparse.ArgumentParser(description='Extract longest reads from a fastq.')
@@ -207,14 +211,26 @@
 
     with FastxWrite(args.output, 'w') as out:
         for i in longest:
             name = ids[i]
             rec = record_dict[ids[i]]
             out.write(name, *rec)
 
+    if args.others is not None:
+        if args.bases is None:
+            others = np.argpartition(lengths, -max_reads)[:-max_reads]
+        else:
+            others = order[last:]
+
+        with FastxWrite(args.others, 'w') as out:
+            for i in others:
+                name = ids[i]
+                rec = record_dict[ids[i]]
+                out.write(name, *rec)
+
 
 def parse_regions(regions, ref_lengths=None):
     """Parse region strings into `Region` objects.
 
     :param regions: iterable of str
     :param ref_lengths: {str ref_names: int ref_lengths}, if provided Region.end
         will default to the reference length instead of None.
```

### Comparing `pomoxis-0.3.8/pomoxis.egg-info/PKG-INFO` & `pomoxis-0.3.9/pomoxis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomoxis
-Version: 0.3.8
+Version: 0.3.9
 Summary: Assembly, consensensus, and analysis tools by ONT research.
 Home-page: UNKNOWN
 Author: cwright
 Author-email: cwright@nanoporetech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `pomoxis-0.3.8/pomoxis.egg-info/SOURCES.txt` & `pomoxis-0.3.9/pomoxis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/pomoxis.egg-info/entry_points.txt` & `pomoxis-0.3.9/pomoxis.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/scripts/assess_assembly` & `pomoxis-0.3.9/scripts/assess_assembly`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 grep 'Percentage Errors' -A 7 -m 1 ${PREFIX}_summ.txt
 grep 'Q Scores' -A 7 -m 1 ${PREFIX}_summ.txt
 
 if $homopolymer_flag; then
     OUTDIR=${PREFIX}_homopolymer
     echo "Running homopolymer count, saving data to ${OUTDIR}"
     if $bed_flag; then
-        assess_homopolymers count ${PREFIX}.bam -o ${OUTDIR} ${BED}
+        assess_homopolymers count ${PREFIX}.bam -t $THREADS -o ${OUTDIR} ${BED}
     else
-        assess_homopolymers count ${PREFIX}.bam -o ${OUTDIR}
+        assess_homopolymers count ${PREFIX}.bam -t $THREADS -o ${OUTDIR}
     fi
 fi
 
 
 echo "All done, output written to ${PREFIX}_stats.txt, ${PREFIX}_summ.txt and ${PREFIX}_indel_ge${MIN_INDEL_LEN}.txt"
```

### Comparing `pomoxis-0.3.8/scripts/intersect_assembly_errors` & `pomoxis-0.3.9/scripts/intersect_assembly_errors`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/scripts/mini_align` & `pomoxis-0.3.9/scripts/mini_align`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/scripts/mini_assemble` & `pomoxis-0.3.9/scripts/mini_assemble`

 * *Files identical despite different names*

### Comparing `pomoxis-0.3.8/setup.py` & `pomoxis-0.3.9/setup.py`

 * *Files identical despite different names*

