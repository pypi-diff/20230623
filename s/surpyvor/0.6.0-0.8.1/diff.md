# Comparing `tmp/surpyvor-0.6.0.tar.gz` & `tmp/surpyvor-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/surpyvor-0.6.0.tar", last modified: Tue Oct 29 07:04:48 2019, max compression
+gzip compressed data, was "dist/surpyvor-0.8.1.tar", last modified: Wed May 20 20:31:41 2020, max compression
```

## Comparing `surpyvor-0.6.0.tar` & `surpyvor-0.8.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-10-29 07:04:48.000000 surpyvor-0.6.0/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     2960 2019-10-29 07:04:48.000000 surpyvor-0.6.0/PKG-INFO
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1861 2019-07-17 12:44:51.000000 surpyvor-0.6.0/README.md
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       38 2019-10-29 07:04:48.000000 surpyvor-0.6.0/setup.cfg
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1453 2019-07-17 12:37:39.000000 surpyvor-0.6.0/setup.py
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-10-29 07:04:48.000000 surpyvor-0.6.0/surpyvor/
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)       40 2019-02-27 12:29:59.000000 surpyvor-0.6.0/surpyvor/__init__.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)    10999 2019-09-17 08:02:44.000000 surpyvor-0.6.0/surpyvor/parse_arguments.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     3538 2019-09-17 07:52:36.000000 surpyvor-0.6.0/surpyvor/plots.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     5306 2019-09-17 08:02:58.000000 surpyvor-0.6.0/surpyvor/surpyvor.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     6617 2019-09-17 07:54:46.000000 surpyvor-0.6.0/surpyvor/utils.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)       22 2019-09-17 07:55:31.000000 surpyvor-0.6.0/surpyvor/version.py
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2019-10-29 07:04:48.000000 surpyvor-0.6.0/surpyvor.egg-info/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     2960 2019-10-29 07:04:47.000000 surpyvor-0.6.0/surpyvor.egg-info/PKG-INFO
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      338 2019-10-29 07:04:47.000000 surpyvor-0.6.0/surpyvor.egg-info/SOURCES.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        1 2019-10-29 07:04:47.000000 surpyvor-0.6.0/surpyvor.egg-info/dependency_links.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       53 2019-10-29 07:04:47.000000 surpyvor-0.6.0/surpyvor.egg-info/entry_points.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       50 2019-10-29 07:04:47.000000 surpyvor-0.6.0/surpyvor.egg-info/requires.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        9 2019-10-29 07:04:47.000000 surpyvor-0.6.0/surpyvor.egg-info/top_level.txt
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2020-05-20 20:31:41.000000 surpyvor-0.8.1/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     2960 2020-05-20 20:31:41.000000 surpyvor-0.8.1/PKG-INFO
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     2022 2020-05-20 20:31:41.000000 surpyvor-0.8.1/README.rst
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       38 2020-05-20 20:31:41.000000 surpyvor-0.8.1/setup.cfg
+-rw-r--r--   0 wouter    (1000) wouter    (1000)     1603 2020-04-19 12:34:38.000000 surpyvor-0.8.1/setup.py
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2020-05-20 20:31:41.000000 surpyvor-0.8.1/surpyvor/
+-rw-r--r--   0 wouter    (1000) wouter    (1000)       40 2020-03-10 09:42:43.000000 surpyvor-0.8.1/surpyvor/__init__.py
+-rw-r--r--   0 wouter    (1000) wouter    (1000)     3163 2020-03-12 10:18:48.000000 surpyvor-0.8.1/surpyvor/haplomerge.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     3046 2020-05-16 10:46:10.000000 surpyvor-0.8.1/surpyvor/improve_insertion_sequence.py
+-rw-r--r--   0 wouter    (1000) wouter    (1000)    17568 2020-05-20 20:26:13.000000 surpyvor-0.8.1/surpyvor/parse_arguments.py
+-rw-r--r--   0 wouter    (1000) wouter    (1000)     3617 2020-03-12 10:10:24.000000 surpyvor-0.8.1/surpyvor/plots.py
+-rw-r--r--   0 wouter    (1000) wouter    (1000)     3708 2020-04-19 12:35:37.000000 surpyvor-0.8.1/surpyvor/purge2d.py
+-rw-r--r--   0 wouter    (1000) wouter    (1000)     6824 2020-05-20 20:26:21.000000 surpyvor-0.8.1/surpyvor/surpyvor.py
+-rw-r--r--   0 wouter    (1000) wouter    (1000)     8411 2020-03-16 11:27:41.000000 surpyvor-0.8.1/surpyvor/utils.py
+-rw-r--r--   0 wouter    (1000) wouter    (1000)       22 2020-05-20 20:26:31.000000 surpyvor-0.8.1/surpyvor/version.py
+drwxrwxr-x   0 wouter    (1000) wouter    (1000)        0 2020-05-20 20:31:41.000000 surpyvor-0.8.1/surpyvor.egg-info/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     2960 2020-05-20 20:31:41.000000 surpyvor-0.8.1/surpyvor.egg-info/PKG-INFO
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      421 2020-05-20 20:31:41.000000 surpyvor-0.8.1/surpyvor.egg-info/SOURCES.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)        1 2020-05-20 20:31:41.000000 surpyvor-0.8.1/surpyvor.egg-info/dependency_links.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       53 2020-05-20 20:31:41.000000 surpyvor-0.8.1/surpyvor.egg-info/entry_points.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       62 2020-05-20 20:31:41.000000 surpyvor-0.8.1/surpyvor.egg-info/requires.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)        9 2020-05-20 20:31:41.000000 surpyvor-0.8.1/surpyvor.egg-info/top_level.txt
```

### Comparing `surpyvor-0.6.0/PKG-INFO` & `surpyvor-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surpyvor
-Version: 0.6.0
+Version: 0.8.1
 Summary: Manipulate vcf files of structural variants using SURVIVOR
 Home-page: https://github.com/wdecoster/surpyvor
 Author: Wouter De Coster
 Author-email: decosterwouter@gmail.com
 License: MIT
 Description: # surpyvor
         A python wrapper around [SURVIVOR](https://github.com/fritzsedlazeck/SURVIVOR), with additional convenience functions.
```

### Comparing `surpyvor-0.6.0/setup.py` & `surpyvor-0.8.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,21 @@
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
     ],
     keywords='nanopore',
     packages=find_packages(),
     python_requires='>=3',
-    install_requires=['matplotlib', 'matplotlib-venn', 'cyvcf2', 'numpy', 'UpSetPlot'],
+    install_requires=['matplotlib',
+                      'matplotlib-venn',
+                      'cyvcf2',
+                      'numpy',
+                      'UpSetPlot',
+                      'pysam',
+                      'cigar'],
     package_data={'surpyvor': []},
     package_dir={'surpyvor': 'surpyvor'},
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'surpyvor=surpyvor.surpyvor:main',
         ],
```

### Comparing `surpyvor-0.6.0/surpyvor/plots.py` & `surpyvor-0.8.1/surpyvor/plots.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from cyvcf2 import VCF
 import matplotlib.pyplot as plt
-from surpyvor import utils
-import numpy as np
-from matplotlib_venn import venn2, venn3
-from upsetplot import plot as upsetplot
 
 
 def bar_chart(vcf, outname="stacked_bar.png"):
     """
     Make a stacked bar chart for length of the SV split by validation status
     This ignores zygosity.
     """
+    from cyvcf2 import VCF
+    from surpyvor import utils
+    import numpy as np
+
     len_dict = {"True": [], "False": [], "Missed": []}
     for v in VCF(vcf):
         if not v.INFO.get('SVTYPE') == 'TRA' and abs(v.INFO.get('SVLEN')) >= 50:
             calls = [utils.is_variant(call) for call in v.gt_types]
             if calls == [True, True]:
                 len_dict['True'].append(v.INFO.get('SVLEN'))
             elif calls == [False, True]:
@@ -44,23 +43,25 @@
                fontsize="small")
     plt.tight_layout()
     plt.savefig(outname)
     plt.close()
 
 
 def upset_plot(upsets, outname="UpSetPlot.png"):
+    from upsetplot import plot as upsetplot
     upsetplot(upsets, sort_by='cardinality')
     plt.savefig(outname)
 
 
 def venn_diagram(sets, labels, num_samples=2, outname="venn.png"):
+    from matplotlib_venn import venn2, venn3
     if num_samples == 2:
-        venn = venn2
+        from matplotlib_venn import venn2 as venn
     else:
-        venn = venn3
+        from matplotlib_venn import venn3 as venn
     venn(sets, set_labels=labels)
     plt.savefig(outname)
     plt.close()
 
 
 def length_plot(dict_of_lengths, output):
     """Makes two stacked bar charts
```

### Comparing `surpyvor-0.6.0/surpyvor/utils.py` & `surpyvor-0.8.1/surpyvor/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import os
 import sys
-from shutil import which
 import tempfile
-from cyvcf2 import VCF
+from cyvcf2 import VCF, Writer
 import subprocess
 import shlex
 import pandas as pd
-import gzip
-from collections import defaultdict
 
 
 def is_variant(call):
     """Check if a variant position qualifies as a variant
 
     0,1,2,3==HOM_REF, HET, UNKNOWN, HOM_ALT"""
     if call == 1 or call == 3:
         return True
     else:
         return False
 
 
 def normalize_vcf(vcff):
     """Normalize a vcf by changing DUP to INS"""
+    import gzip
+
     handle, name = tempfile.mkstemp(suffix='.vcf')
     out = open(name, 'w')
     if vcff.endswith('.gz'):
         vcf = gzip.open(vcff, 'rt')
     else:
         vcf = open(vcff)
     for line in vcf:
@@ -66,14 +65,15 @@
     return ''.join([str(i) for i in binary_calls])
 
 
 def make_sets(vcf, names):
     """From the merged SV file, return pd.Series of overlapping sets.
 
     Intended for making an upset plot"""
+    from collections import defaultdict
     calls = defaultdict(int)
     for v in VCF(vcf):
         calls[gt_types_to_binary_comparison(v.gt_types)] += 1
     tf_array = [[True, False]] * len(list(calls.keys())[0])
     index = pd.MultiIndex.from_product(tf_array, names=names)
     values = [calls[''.join([str(int(j)) for j in i])] for i in index]
     return pd.Series(values, index=index)
@@ -123,14 +123,16 @@
         subprocess.call(shlex.split("bgzip -cd {}".format(vcf)), stdout=handle)
         return output
     else:
         return vcf
 
 
 def test_dependencies():
+    from shutil import which
+
     for dependency in ['bcftools', 'bgzip', 'tabix', 'SURVIVOR']:
         if not which(dependency):
             sys.exit("ERROR: Could not find required executable '{}'.\n"
                      "Make sure it is installed and in $PATH".format(dependency))
 
 
 def vcf_sort(input, output):
@@ -164,14 +166,15 @@
     df.columns.name = names[1]
     df.index = ['nocall', 'hom_ref', 'het', 'hom_alt']
     df.index.name = names[0]
     print(df)
 
 
 def get_svlengths(vcf):
+    from collections import defaultdict
     len_dict = defaultdict(list)
     vcf = VCF(vcf)
     if len(vcf.samples) > 1:
         sys.stderr.write("\n\nWarning: this script does not support multiple samples in a vcf.\n")
         sys.stderr.write("Plotting and counting only for {}.".format(vcf.samples[0]))
     for v in vcf:
         if is_variant(v.gt_types[0]) and not v.INFO.get('SVTYPE') == 'TRA':
@@ -198,7 +201,54 @@
         return "INV"
     else:
         return v.INFO.get('SVTYPE').split(':')[0].split('/')[0]
 
 
 def get_svlen(v):
     return abs(v.INFO.get('SVLEN'))
+
+
+def filter_vcf(vcf, output, minlength=0, truncate_svlen=float("inf"), suffix=""):
+    vcf_in = VCF(vcf)
+    if not output:
+        output = vcf.replace(".vcf", "_{}.vcf".format(suffix))
+    vcf_in.add_info_to_header({'ID': 'TRUNCATED',
+                               'Description': "SVLEN truncated",
+                               'Type': 'Flag', 'Number': '0'})
+    vcf_out = Writer(output, vcf_in)
+    records_truncated = 0
+    records_filtered = 0
+    for v in vcf_in:
+        svlen = get_svlen(v)
+        if svlen >= minlength:
+            if svlen > truncate_svlen:
+                v.INFO['SVLEN'] = 1
+                v.INFO['END'] = v.start + 1
+                v.INFO['TRUNCATED'] = True
+                records_truncated += 1
+            vcf_out.write_record(v)
+        else:
+            records_filtered += 1
+    if records_truncated != 0:
+        sys.stderr.write("Truncated {} records where SVLEN > {}\n".format(
+            records_truncated, int(truncate_svlen)))
+    if records_filtered != 0:
+        sys.stderr.write("Filtered {} records where SVLEN < {}\n".format(
+            records_filtered, int(minlength)))
+
+
+def fix_vcf(vcf, output):
+    vcf_in = VCF(vcf)
+    if not output:
+        output = vcf.replace(".vcf", "_{}.vcf".format("fixed"))
+    vcf_in.add_info_to_header({'ID': 'TRUNCATED',
+                               'Description': "SVLEN truncated",
+                               'Type': 'Flag', 'Number': '0'})
+    vcf_out = Writer(output, vcf_in)
+    records_fixed = 0
+    for v in vcf_in:
+        if v.start == -1:
+            v.set_pos(0)
+            records_fixed += 1
+        vcf_out.write_record(v)
+    if records_fixed != 0:
+        sys.stderr.write("Fixed {} records.\n".format(records_fixed))
```

### Comparing `surpyvor-0.6.0/surpyvor.egg-info/PKG-INFO` & `surpyvor-0.8.1/surpyvor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surpyvor
-Version: 0.6.0
+Version: 0.8.1
 Summary: Manipulate vcf files of structural variants using SURVIVOR
 Home-page: https://github.com/wdecoster/surpyvor
 Author: Wouter De Coster
 Author-email: decosterwouter@gmail.com
 License: MIT
 Description: # surpyvor
         A python wrapper around [SURVIVOR](https://github.com/fritzsedlazeck/SURVIVOR), with additional convenience functions.
```

