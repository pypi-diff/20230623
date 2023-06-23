# Comparing `tmp/ms1searchpy-2.4.1-py3-none-any.whl.zip` & `tmp/ms1searchpy-2.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 36962 bytes, number of entries: 15
+Zip file size: 36864 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-16 13:01 ms1searchpy/__init__.py
 -rw-r--r--  2.0 unx     4185 b- defN 23-Mar-16 13:01 ms1searchpy/combine.py
 -rw-r--r--  2.0 unx     2746 b- defN 23-Mar-16 13:01 ms1searchpy/combine_proteins.py
 -rw-r--r--  2.0 unx    16453 b- defN 23-Mar-16 13:01 ms1searchpy/directms1quant.py
--rw-r--r--  2.0 unx    74207 b- defN 23-Jun-15 09:03 ms1searchpy/main.py
+-rw-r--r--  2.0 unx    74513 b- defN 23-Jun-23 14:08 ms1searchpy/main.py
 -rw-r--r--  2.0 unx     7413 b- defN 23-Mar-16 13:01 ms1searchpy/ms1todiffacto.py
 -rw-r--r--  2.0 unx     4528 b- defN 23-Jun-15 09:03 ms1searchpy/search.py
 -rw-r--r--  2.0 unx    14882 b- defN 23-Jun-15 09:03 ms1searchpy/utils.py
 -rw-r--r--  2.0 unx    12868 b- defN 23-Mar-16 13:01 ms1searchpy/utils_figures.py
--rwxr-xr-x  2.0 unx      551 b- defN 23-Jun-15 09:04 ms1searchpy-2.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6264 b- defN 23-Jun-15 09:04 ms1searchpy-2.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 09:04 ms1searchpy-2.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      283 b- defN 23-Jun-15 09:04 ms1searchpy-2.4.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-15 09:04 ms1searchpy-2.4.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1240 b- defN 23-Jun-15 09:04 ms1searchpy-2.4.1.dist-info/RECORD
-15 files, 145724 bytes uncompressed, 34912 bytes compressed:  76.0%
+-rwxr-xr-x  2.0 unx      551 b- defN 23-Jun-23 14:08 ms1searchpy-2.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5795 b- defN 23-Jun-23 14:08 ms1searchpy-2.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 14:08 ms1searchpy-2.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      283 b- defN 23-Jun-23 14:08 ms1searchpy-2.4.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-23 14:08 ms1searchpy-2.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1240 b- defN 23-Jun-23 14:08 ms1searchpy-2.4.2.dist-info/RECORD
+15 files, 145561 bytes uncompressed, 34814 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: ms1searchpy/utils.py
 Comment: 
 
 Filename: ms1searchpy/utils_figures.py
 Comment: 
 
-Filename: ms1searchpy-2.4.1.dist-info/LICENSE
+Filename: ms1searchpy-2.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: ms1searchpy-2.4.1.dist-info/METADATA
+Filename: ms1searchpy-2.4.2.dist-info/METADATA
 Comment: 
 
-Filename: ms1searchpy-2.4.1.dist-info/WHEEL
+Filename: ms1searchpy-2.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: ms1searchpy-2.4.1.dist-info/entry_points.txt
+Filename: ms1searchpy-2.4.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ms1searchpy-2.4.1.dist-info/top_level.txt
+Filename: ms1searchpy-2.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ms1searchpy-2.4.1.dist-info/RECORD
+Filename: ms1searchpy-2.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ms1searchpy/main.py

```diff
@@ -935,15 +935,18 @@
                 train_RT.append(float(RT))
             outcalib.close()
 
             subprocess.call([deeplc_path, '--file_pred', outcalib_name, '--file_cal', outtrain_name, '--file_pred_out', outres_name] + deeplc_extra_args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 
             pepdict = dict()
             for seq, x in zip(train_seq, open(outres_name).readlines()[1:]):
-                _, RT = x.strip().split(',')
+                try:
+                    _, _, _, _, RT = x.strip().split(',')
+                except:
+                    _, RT = x.strip().split(',')
                 pepdict[seq] = float(RT)
 
 
             train_RT = np.array(train_RT)
             RT_pred = np.array([pepdict[s] for s in train_seq])
 
             rt_diff_tmp = RT_pred - train_RT
@@ -1076,15 +1079,18 @@
             outtrain.close()
 
             # [:int(len(ns)/2)]
 
             subprocess.call([deeplc_path, '--file_pred', outtrain_name, '--file_cal', outcal_name, '--file_pred_out', outres_name] + deeplc_extra_args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
             pepdict = dict()
             for seq, x in zip(train_seq, open(outres_name).readlines()[1:]):
-                _, RT = x.strip().split(',')
+                try:
+                    _, _, _, _, RT = x.strip().split(',')
+                except:
+                    _, RT = x.strip().split(',')
                 pepdict[seq] = float(RT)
 
 
             train_RT = np.array(train_RT)
             RT_pred = np.array([pepdict[s] for s in train_seq])
 
             rt_diff_tmp = RT_pred - train_RT
@@ -1203,15 +1209,18 @@
             mods_tmp = utils.mods_for_deepLC(seq, aa_to_psi)
             outtest.write(seq + ',' + str(mods_tmp) + '\n')
             test_seqs.append(seq)
         outtest.close()
 
         subprocess.call([deeplc_path, '--file_pred', outtest_name, '--file_cal', outtrain_name, '--file_pred_out', outres_name] + deeplc_extra_args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         for seq, x in zip(test_seqs, open(outres_name).readlines()[1:]):
-            _, RT = x.strip().split(',')
+            try:
+                _, _, _, RT = x.strip().split(',')
+            except:
+                _, RT = x.strip().split(',')
             pepdict[seq] = float(RT)
 
     else:
 
         if n == 1 or os.name == 'nt':
             qin = list(p1)
             qout = []
```

## Comparing `ms1searchpy-2.4.1.dist-info/LICENSE` & `ms1searchpy-2.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ms1searchpy-2.4.1.dist-info/METADATA` & `ms1searchpy-2.4.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: ms1searchpy
-Version: 2.4.1
+Version: 2.4.2
 Summary: A proteomics search engine for LC-MS1 spectra.
 Author: Mark Ivanov
 Author-email: pyteomics@googlegroups.com
 License: License :: OSI Approved :: Apache Software License
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
@@ -38,28 +37,29 @@
 
     ms1searchpy *_peptideFeatures.tsv -d path_to.FASTA
 
 Read further for detailed info, including quantitative analysis.
 
 ## Citing ms1searchpy
 
+Ivanov et al. DirectMS1Quant: Ultrafast Quantitative Proteomics with MS/MS-Free Mass Spectrometry. https://pubs.acs.org/doi/10.1021/acs.analchem.2c02255
+
 Ivanov et al. Boosting MS1-only Proteomics with Machine Learning Allows 2000 Protein Identifications in Single-Shot Human Proteome Analysis Using 5 min HPLC Gradient. https://doi.org/10.1021/acs.jproteome.0c00863
 
 Ivanov et al. DirectMS1: MS/MS-free identification of 1000 proteins of cellular proteomes in 5 minutes. https://doi.org/10.1021/acs.analchem.9b05095
 
 ## Installation
 
 Using pip:
 
     pip install ms1searchpy
 
-It is recommended to additionally install [DeepLC](https://github.com/compomics/DeepLC) version 2.2.0+; you may also want to install
-[diffacto](https://github.com/statisticalbiotechnology/diffacto):
+It is recommended to additionally install [DeepLC](https://github.com/compomics/DeepLC) version 1.1.2 (newer version has some issues right now):
 
-    pip install deeplc diffacto
+    pip install deeplc==1.1.2
 
 This should work on recent versions of Python (3.8-3.10).
 
 ## Usage tutorial: protein identification
 
 The script used for protein identification is called `ms1searchpy`. It needs input files (mzML or tsv) and a FASTA database.
 
@@ -114,34 +114,23 @@
 
     ms1combine sample_rep_*.features_PFMs_ML.tsv
 
 ## Usage tutorial: Quantitation
 
 After obtaining the protein identification results, you can proceed to compare your samples using LFQ.
 
-### Using diffacto
-
-Here's an example where we use Bourne Shell syntax for brevity. Each sample contains three replicates:
-
-    ms1todiffacto -dif diffacto -S1 sample1_r{1,2,3}.features_proteins.tsv -S2 sample2_r{1,2,3}.features_proteins.tsv -norm median -out diffacto_output.tsv -min_samples 3
-
-`ms1todiffacto` prepares input file for [diffacto](https://github.com/statisticalbiotechnology/diffacto) from ms1searchpy output and to automatically runs diffacto.
-
 ### Using directms1quant
 
 New LFQ method designed specifically for DirectMS1 is invoked like this:
 
-    directms1quant -S1 sample1_r{1,2,3}.features_proteins_full.tsv -S2 sample2_r{1,2,3}.features_proteins_full.tsv -min_samples 3
+    directms1quant -S1 sample1_r{1,2,3}.features_proteins_full.tsv -S2 sample2_r{1,2,3}.features_proteins_full.tsv
 
 It produces a filtered table of significantly changed proteins with p-values and fold changes,
 as well as the full protein table and a separate file simply listing all
 IDs of significantly modified proteins (e.g. for easy copy-paste into a StringDB search window).
 
 ## Links
 
 - GitHub repo & issue tracker: https://github.com/markmipt/ms1searchpy
 - Mailing list: markmipt@gmail.com
 
-- Diffacto repo: https://github.com/statisticalbiotechnology/diffacto
 - DeepLC repo: https://github.com/compomics/DeepLC
-
-
```

## Comparing `ms1searchpy-2.4.1.dist-info/RECORD` & `ms1searchpy-2.4.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ms1searchpy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ms1searchpy/combine.py,sha256=AOnPa_7Meqst5H6qM6faa4GbSIYzURmiH9cOUerKOq0,4185
 ms1searchpy/combine_proteins.py,sha256=LFJuwkb8UBy-1T-kAT3H4zxkqQ6VTso6SOLP7s8o0Ow,2746
 ms1searchpy/directms1quant.py,sha256=XnjMzwK3E3R2V_OrqycpRSA7pYk9Q7oRvHt3CI0pMCU,16453
-ms1searchpy/main.py,sha256=BEB-ZKrEJTHIOa3qR83EFbwMZ7pSS-esug7DEMHZPTg,74207
+ms1searchpy/main.py,sha256=sPMb29-n6twrU-WsFD-O8OgzeTxz7ZqONhunQBFYIbo,74513
 ms1searchpy/ms1todiffacto.py,sha256=xGxcIe8-C_vSLx5Qz5qwSKa4oULJ-8cgq4DtCTXKe3s,7413
 ms1searchpy/search.py,sha256=btcqQcUoVr49QwFLCpD0FOo6_z2VY8JNyucq_ywr-ws,4528
 ms1searchpy/utils.py,sha256=Krqh2oQJEFLeF1HCA9j2aHL5yKFDyUyVARV9KECN_pE,14882
 ms1searchpy/utils_figures.py,sha256=8COdbQsgrHcmaiVzPiEVge3PTAAvdk2TMrZkx-vz9cI,12868
-ms1searchpy-2.4.1.dist-info/LICENSE,sha256=WanbJHdVmtsm-QgIuB0GDMrtkwBHY6WmTzwvX6ZZtgs,551
-ms1searchpy-2.4.1.dist-info/METADATA,sha256=x2JuZHMSEFg41Ch5cfyyr19vrysBC_mQshErIm16iZs,6264
-ms1searchpy-2.4.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-ms1searchpy-2.4.1.dist-info/entry_points.txt,sha256=o8muZPvEPb8wlQ2pwAcB2shJdht4gN6levpHaObftbI,283
-ms1searchpy-2.4.1.dist-info/top_level.txt,sha256=pyjbWV_odwavqf6q4mSj2P0L0zLqKEDftX53QvxeJlc,12
-ms1searchpy-2.4.1.dist-info/RECORD,,
+ms1searchpy-2.4.2.dist-info/LICENSE,sha256=WanbJHdVmtsm-QgIuB0GDMrtkwBHY6WmTzwvX6ZZtgs,551
+ms1searchpy-2.4.2.dist-info/METADATA,sha256=cWxc6mUGuX8sOi70JVj8n9ynDLt4yz0Ri_sTcpvCaKo,5795
+ms1searchpy-2.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ms1searchpy-2.4.2.dist-info/entry_points.txt,sha256=o8muZPvEPb8wlQ2pwAcB2shJdht4gN6levpHaObftbI,283
+ms1searchpy-2.4.2.dist-info/top_level.txt,sha256=pyjbWV_odwavqf6q4mSj2P0L0zLqKEDftX53QvxeJlc,12
+ms1searchpy-2.4.2.dist-info/RECORD,,
```

