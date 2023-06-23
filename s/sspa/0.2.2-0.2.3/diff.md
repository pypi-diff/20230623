# Comparing `tmp/sspa-0.2.2.tar.gz` & `tmp/sspa-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sspa-0.2.2.tar", last modified: Tue Feb 21 11:14:40 2023, max compression
+gzip compressed data, was "sspa-0.2.3.tar", last modified: Fri Jun 23 21:25:54 2023, max compression
```

## Comparing `sspa-0.2.2.tar` & `sspa-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-02-21 11:14:40.282414 sspa-0.2.2/
--rw-r--r--   0 cw2019     (501) staff       (20)    35149 2021-12-28 11:48:17.000000 sspa-0.2.2/LICENSE
--rw-r--r--   0 cw2019     (501) staff       (20)     6194 2023-02-21 11:14:40.281802 sspa-0.2.2/PKG-INFO
--rw-r--r--   0 cw2019     (501) staff       (20)     5766 2023-01-06 14:29:14.000000 sspa-0.2.2/README.md
--rw-r--r--   0 cw2019     (501) staff       (20)       38 2023-02-21 11:14:40.282701 sspa-0.2.2/setup.cfg
--rw-r--r--   0 cw2019     (501) staff       (20)      986 2023-02-21 11:14:18.000000 sspa-0.2.2/setup.py
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-02-21 11:14:40.020472 sspa-0.2.2/src/
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-02-21 11:14:40.029909 sspa-0.2.2/src/sspa/
--rw-r--r--   0 cw2019     (501) staff       (20)      608 2023-01-06 11:27:15.000000 sspa-0.2.2/src/sspa/__init__.py
--rw-r--r--   0 cw2019     (501) staff       (20)     7091 2022-10-06 11:06:14.000000 sspa-0.2.2/src/sspa/download_pathways.py
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-02-21 11:14:40.086417 sspa-0.2.2/src/sspa/example_data/
--rw-r--r--   0 cw2019     (501) staff       (20)  3458958 2022-02-15 11:17:29.000000 sspa-0.2.2/src/sspa/example_data/BXD_mouse_metabolomics.csv
--rw-r--r--   0 cw2019     (501) staff       (20)  3269754 2022-02-15 12:04:44.000000 sspa-0.2.2/src/sspa/example_data/BXD_mouse_metabolomics_raw_data.csv
--rw-r--r--   0 cw2019     (501) staff       (20)  1742398 2021-12-28 17:58:04.000000 sspa-0.2.2/src/sspa/example_data/Su_covid_metabolomics_processed.csv
--rw-r--r--   0 cw2019     (501) staff       (20)  2768383 2022-02-18 15:51:44.000000 sspa-0.2.2/src/sspa/example_data/Su_metab_data_raw.csv
--rw-r--r--   0 cw2019     (501) staff       (20)     2201 2022-10-11 12:11:57.000000 sspa-0.2.2/src/sspa/identifier_conversion.py
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-02-21 11:14:40.277341 sspa-0.2.2/src/sspa/pathway_databases/
--rw-r--r--   0 cw2019     (501) staff       (20) 30485396 2021-12-28 17:59:39.000000 sspa-0.2.2/src/sspa/pathway_databases/ChEBI2Reactome_All_Levels_R78.txt
--rw-r--r--   0 cw2019     (501) staff       (20)   172723 2021-06-07 08:24:37.000000 sspa-0.2.2/src/sspa/pathway_databases/KEGG_human_pathways_compounds_R98.csv
--rw-r--r--   0 cw2019     (501) staff       (20)   259274 2022-07-07 13:45:17.000000 sspa-0.2.2/src/sspa/pathway_databases/wikipathways-20220610-gmt-Homo_sapiens.gmt
--rw-r--r--   0 cw2019     (501) staff       (20)     4243 2022-09-16 11:23:22.000000 sspa-0.2.2/src/sspa/process_pathways.py
--rw-r--r--   0 cw2019     (501) staff       (20)     2897 2022-02-14 15:21:22.000000 sspa-0.2.2/src/sspa/process_pathways_dictionary.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1699 2022-09-16 19:04:09.000000 sspa-0.2.2/src/sspa/sspa_cluster.py
--rw-r--r--   0 cw2019     (501) staff       (20)     2621 2023-01-06 14:47:35.000000 sspa-0.2.2/src/sspa/sspa_fgsea.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1971 2023-01-05 16:12:18.000000 sspa-0.2.2/src/sspa/sspa_gsea.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1878 2023-01-06 14:47:35.000000 sspa-0.2.2/src/sspa/sspa_gsva.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1508 2022-09-16 19:01:36.000000 sspa-0.2.2/src/sspa/sspa_kpca.py
--rw-r--r--   0 cw2019     (501) staff       (20)     5359 2022-10-25 10:55:24.000000 sspa-0.2.2/src/sspa/sspa_ora.py
--rw-r--r--   0 cw2019     (501) staff       (20)     2476 2023-01-05 16:12:18.000000 sspa-0.2.2/src/sspa/sspa_ssGSEA.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1576 2022-09-16 19:02:23.000000 sspa-0.2.2/src/sspa/sspa_svd.py
--rw-r--r--   0 cw2019     (501) staff       (20)     1613 2022-09-16 19:02:38.000000 sspa-0.2.2/src/sspa/sspa_zscore.py
--rw-r--r--   0 cw2019     (501) staff       (20)     3890 2023-02-21 10:51:51.000000 sspa-0.2.2/src/sspa/utils.py
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-02-21 11:14:40.033030 sspa-0.2.2/src/sspa.egg-info/
--rw-r--r--   0 cw2019     (501) staff       (20)     6194 2023-02-21 11:14:40.000000 sspa-0.2.2/src/sspa.egg-info/PKG-INFO
--rw-r--r--   0 cw2019     (501) staff       (20)     1018 2023-02-21 11:14:40.000000 sspa-0.2.2/src/sspa.egg-info/SOURCES.txt
--rw-r--r--   0 cw2019     (501) staff       (20)        1 2023-02-21 11:14:40.000000 sspa-0.2.2/src/sspa.egg-info/dependency_links.txt
--rw-r--r--   0 cw2019     (501) staff       (20)       76 2023-02-21 11:14:40.000000 sspa-0.2.2/src/sspa.egg-info/requires.txt
--rw-r--r--   0 cw2019     (501) staff       (20)        5 2023-02-21 11:14:40.000000 sspa-0.2.2/src/sspa.egg-info/top_level.txt
-drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-02-21 11:14:40.280805 sspa-0.2.2/tests/
--rw-r--r--   0 cw2019     (501) staff       (20)      586 2022-10-30 19:06:06.000000 sspa-0.2.2/tests/test_download_pathways.py
--rw-r--r--   0 cw2019     (501) staff       (20)     2782 2023-01-08 14:18:53.000000 sspa-0.2.2/tests/test_utils.py
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.610908 sspa-0.2.3/
+-rw-r--r--   0 cw2019     (501) staff       (20)    35149 2021-12-28 11:48:17.000000 sspa-0.2.3/LICENSE
+-rw-r--r--   0 cw2019     (501) staff       (20)     6479 2023-06-23 21:25:54.610496 sspa-0.2.3/PKG-INFO
+-rw-r--r--   0 cw2019     (501) staff       (20)     6051 2023-06-23 21:24:36.000000 sspa-0.2.3/README.md
+-rw-r--r--   0 cw2019     (501) staff       (20)       38 2023-06-23 21:25:54.611046 sspa-0.2.3/setup.cfg
+-rw-r--r--   0 cw2019     (501) staff       (20)      986 2023-06-23 21:10:23.000000 sspa-0.2.3/setup.py
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.255398 sspa-0.2.3/src/
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.274906 sspa-0.2.3/src/sspa/
+-rw-r--r--   0 cw2019     (501) staff       (20)      608 2023-01-06 11:27:15.000000 sspa-0.2.3/src/sspa/__init__.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     7133 2023-06-21 17:20:00.000000 sspa-0.2.3/src/sspa/download_pathways.py
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.334696 sspa-0.2.3/src/sspa/example_data/
+-rw-r--r--   0 cw2019     (501) staff       (20)  3458958 2022-02-15 11:17:29.000000 sspa-0.2.3/src/sspa/example_data/BXD_mouse_metabolomics.csv
+-rw-r--r--   0 cw2019     (501) staff       (20)  3269754 2022-02-15 12:04:44.000000 sspa-0.2.3/src/sspa/example_data/BXD_mouse_metabolomics_raw_data.csv
+-rw-r--r--   0 cw2019     (501) staff       (20)  1742398 2021-12-28 17:58:04.000000 sspa-0.2.3/src/sspa/example_data/Su_covid_metabolomics_processed.csv
+-rw-r--r--   0 cw2019     (501) staff       (20)  2768383 2022-02-18 15:51:44.000000 sspa-0.2.3/src/sspa/example_data/Su_metab_data_raw.csv
+-rw-r--r--   0 cw2019     (501) staff       (20)     2201 2022-10-11 12:11:57.000000 sspa-0.2.3/src/sspa/identifier_conversion.py
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.603366 sspa-0.2.3/src/sspa/pathway_databases/
+-rw-r--r--   0 cw2019     (501) staff       (20) 30485396 2021-12-28 17:59:39.000000 sspa-0.2.3/src/sspa/pathway_databases/ChEBI2Reactome_All_Levels_R78.txt
+-rw-r--r--   0 cw2019     (501) staff       (20)   172723 2021-06-07 08:24:37.000000 sspa-0.2.3/src/sspa/pathway_databases/KEGG_human_pathways_compounds_R98.csv
+-rw-r--r--   0 cw2019     (501) staff       (20)   259274 2022-07-07 13:45:17.000000 sspa-0.2.3/src/sspa/pathway_databases/wikipathways-20220610-gmt-Homo_sapiens.gmt
+-rw-r--r--   0 cw2019     (501) staff       (20)     4243 2022-09-16 11:23:22.000000 sspa-0.2.3/src/sspa/process_pathways.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     2897 2022-02-14 15:21:22.000000 sspa-0.2.3/src/sspa/process_pathways_dictionary.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1699 2022-09-16 19:04:09.000000 sspa-0.2.3/src/sspa/sspa_cluster.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     2621 2023-01-06 14:47:35.000000 sspa-0.2.3/src/sspa/sspa_fgsea.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1971 2023-01-05 16:12:18.000000 sspa-0.2.3/src/sspa/sspa_gsea.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1878 2023-01-06 14:47:35.000000 sspa-0.2.3/src/sspa/sspa_gsva.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1508 2022-09-16 19:01:36.000000 sspa-0.2.3/src/sspa/sspa_kpca.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     5359 2022-10-25 10:55:24.000000 sspa-0.2.3/src/sspa/sspa_ora.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     2476 2023-01-05 16:12:18.000000 sspa-0.2.3/src/sspa/sspa_ssGSEA.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1576 2022-09-16 19:02:23.000000 sspa-0.2.3/src/sspa/sspa_svd.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     1613 2022-09-16 19:02:38.000000 sspa-0.2.3/src/sspa/sspa_zscore.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     3890 2023-02-21 10:51:51.000000 sspa-0.2.3/src/sspa/utils.py
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.277949 sspa-0.2.3/src/sspa.egg-info/
+-rw-r--r--   0 cw2019     (501) staff       (20)     6479 2023-06-23 21:25:54.000000 sspa-0.2.3/src/sspa.egg-info/PKG-INFO
+-rw-r--r--   0 cw2019     (501) staff       (20)     1018 2023-06-23 21:25:54.000000 sspa-0.2.3/src/sspa.egg-info/SOURCES.txt
+-rw-r--r--   0 cw2019     (501) staff       (20)        1 2023-06-23 21:25:54.000000 sspa-0.2.3/src/sspa.egg-info/dependency_links.txt
+-rw-r--r--   0 cw2019     (501) staff       (20)       76 2023-06-23 21:25:54.000000 sspa-0.2.3/src/sspa.egg-info/requires.txt
+-rw-r--r--   0 cw2019     (501) staff       (20)        5 2023-06-23 21:25:54.000000 sspa-0.2.3/src/sspa.egg-info/top_level.txt
+drwxr-xr-x   0 cw2019     (501) staff       (20)        0 2023-06-23 21:25:54.609507 sspa-0.2.3/tests/
+-rw-r--r--   0 cw2019     (501) staff       (20)      586 2022-10-30 19:06:06.000000 sspa-0.2.3/tests/test_download_pathways.py
+-rw-r--r--   0 cw2019     (501) staff       (20)     2782 2023-01-08 14:18:53.000000 sspa-0.2.3/tests/test_utils.py
```

### Comparing `sspa-0.2.2/LICENSE` & `sspa-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/PKG-INFO` & `sspa-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspa
-Version: 0.2.2
+Version: 0.2.3
 Summary: Single sample pathway analysis tools for omics data
 Home-page: https://github.com/cwieder/sspa
 Author: Cecilia Wieder
 Author-email: cw2019@ic.ac.uk
 License: GNU 3.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -171,16 +171,24 @@
 }
 
 ```
 
 ## Contributing
 Read our [contributor's guide](https://github.com/cwieder/py-ssPA/blob/main/CONTRIBUTING.md) to get started
 
+### Contributors
+We are grateful for our contributors who help develop and maintain py-ssPA:
+- Maëlick Brochut [@mbrochut](https://github.com/mbrochut)
+
 ## News 
 
+### [v0.2.3] - 23/06/23
+- @mbrochut Bug fix in KEGG pathway downloader 
+- @mbrochut Add tqdm progress bar for long KEGG downloads
+
 ### [v0.2.1] - 05/01/23
 - Removal of rpy2 dependency for improved compatibility across systems
 - Use [GSEApy](https://github.com/zqfang/GSEApy) as backend for GSEA and ssGSEA 
 - Minor syntax changes
    - `ora.ttest_res` is now `ora.DA_test_res` (as we can implement t-test or MWU tests)
    - `sspa_fgsea()` is now `sspa_gsea()` and uses gseapy as the backend rather than R fgsea
    - `sspa_gsva()` is temporarily deprecated due to the need for the rpy2 compatability - use the [GSVA R package](https://bioconductor.org/packages/release/bioc/html/GSVA.html)
```

### Comparing `sspa-0.2.2/README.md` & `sspa-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -157,16 +157,24 @@
 }
 
 ```
 
 ## Contributing
 Read our [contributor's guide](https://github.com/cwieder/py-ssPA/blob/main/CONTRIBUTING.md) to get started
 
+### Contributors
+We are grateful for our contributors who help develop and maintain py-ssPA:
+- Maëlick Brochut [@mbrochut](https://github.com/mbrochut)
+
 ## News 
 
+### [v0.2.3] - 23/06/23
+- @mbrochut Bug fix in KEGG pathway downloader 
+- @mbrochut Add tqdm progress bar for long KEGG downloads
+
 ### [v0.2.1] - 05/01/23
 - Removal of rpy2 dependency for improved compatibility across systems
 - Use [GSEApy](https://github.com/zqfang/GSEApy) as backend for GSEA and ssGSEA 
 - Minor syntax changes
    - `ora.ttest_res` is now `ora.DA_test_res` (as we can implement t-test or MWU tests)
    - `sspa_fgsea()` is now `sspa_gsea()` and uses gseapy as the backend rather than R fgsea
    - `sspa_gsva()` is temporarily deprecated due to the need for the rpy2 compatability - use the [GSVA R package](https://bioconductor.org/packages/release/bioc/html/GSVA.html)
```

### Comparing `sspa-0.2.2/setup.py` & `sspa-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='sspa',
-    version='0.2.2',
+    version='0.2.3',
     packages=['sspa'],
     package_dir={'':'src'},
     url='https://github.com/cwieder/sspa',
     license='GNU 3.0',
     author='Cecilia Wieder',
     author_email='cw2019@ic.ac.uk',
     description='Single sample pathway analysis tools for omics data',
```

### Comparing `sspa-0.2.2/src/sspa/__init__.py` & `sspa-0.2.3/src/sspa/__init__.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/download_pathways.py` & `sspa-0.2.3/src/sspa/download_pathways.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Similar to KEGGREST R in principle
 
 import requests
 import re
 import pandas as pd
 import warnings
 import json
+from tqdm import tqdm
 
 def download_KEGG(organism, filepath=None):
     '''
     Function for KEGG pathway download
     Args:
         organism (str): KEGG 3 letter organism code
         filepath (str): filepath to save pathway file to, default is None - save to variable
@@ -21,32 +22,31 @@
     url = 'http://rest.kegg.jp/list/pathway/'+organism
     # change organism name
     data = requests.get(url)
     pathways = data.text
     pathways = pathways.split("\n")
     pathways = filter(None, pathways)
     pathway_dict = dict()
-
+    
     for path in pathways:
         path = path.split("\t")
         name = path[1]
-        pathid = re.search(r"path:(.*)", path[0]).group(1)
+        pathid = re.search(r"(.*)", path[0]).group(1)
         pathway_dict[pathid] = name
 
     # get compounds for each pathway
     base_url = 'http://rest.kegg.jp/get/'
 
     pathway_ids = [*pathway_dict]
     pathway_names = list(pathway_dict.values())
     pathway_compound_mapping = dict()
 
-    for i in pathway_ids:
+    for index,i in enumerate(tqdm(pathway_ids)):
         complist = []
-        current_url = base_url + "pathway:" + i
-
+        current_url = base_url + "pathway:" +i
         # parse the pathway description page
         page = requests.get(current_url)
         lines = page.text.split("\n")
 
         try:
             cpds_start = [lines.index(i) for i in lines if i.startswith("COMPOUND")][0]
             reference_start = [lines.index(i) for i in lines if i.startswith("REFERENCE") or i.startswith("REL_PATHWAY")][0]
```

### Comparing `sspa-0.2.2/src/sspa/example_data/BXD_mouse_metabolomics.csv` & `sspa-0.2.3/src/sspa/example_data/BXD_mouse_metabolomics.csv`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/example_data/BXD_mouse_metabolomics_raw_data.csv` & `sspa-0.2.3/src/sspa/example_data/BXD_mouse_metabolomics_raw_data.csv`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/example_data/Su_covid_metabolomics_processed.csv` & `sspa-0.2.3/src/sspa/example_data/Su_covid_metabolomics_processed.csv`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/example_data/Su_metab_data_raw.csv` & `sspa-0.2.3/src/sspa/example_data/Su_metab_data_raw.csv`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/identifier_conversion.py` & `sspa-0.2.3/src/sspa/identifier_conversion.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/pathway_databases/ChEBI2Reactome_All_Levels_R78.txt` & `sspa-0.2.3/src/sspa/pathway_databases/ChEBI2Reactome_All_Levels_R78.txt`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/pathway_databases/KEGG_human_pathways_compounds_R98.csv` & `sspa-0.2.3/src/sspa/pathway_databases/KEGG_human_pathways_compounds_R98.csv`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/pathway_databases/wikipathways-20220610-gmt-Homo_sapiens.gmt` & `sspa-0.2.3/src/sspa/pathway_databases/wikipathways-20220610-gmt-Homo_sapiens.gmt`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/process_pathways.py` & `sspa-0.2.3/src/sspa/process_pathways.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/process_pathways_dictionary.py` & `sspa-0.2.3/src/sspa/process_pathways_dictionary.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/sspa_cluster.py` & `sspa-0.2.3/src/sspa/sspa_cluster.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/sspa_fgsea.py` & `sspa-0.2.3/src/sspa/sspa_fgsea.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/sspa_gsea.py` & `sspa-0.2.3/src/sspa/sspa_gsea.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/sspa_gsva.py` & `sspa-0.2.3/src/sspa/sspa_gsva.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/sspa_kpca.py` & `sspa-0.2.3/src/sspa/sspa_kpca.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/sspa_ora.py` & `sspa-0.2.3/src/sspa/sspa_ora.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/sspa_ssGSEA.py` & `sspa-0.2.3/src/sspa/sspa_ssGSEA.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/sspa_svd.py` & `sspa-0.2.3/src/sspa/sspa_svd.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/sspa_zscore.py` & `sspa-0.2.3/src/sspa/sspa_zscore.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa/utils.py` & `sspa-0.2.3/src/sspa/utils.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/src/sspa.egg-info/PKG-INFO` & `sspa-0.2.3/src/sspa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sspa
-Version: 0.2.2
+Version: 0.2.3
 Summary: Single sample pathway analysis tools for omics data
 Home-page: https://github.com/cwieder/sspa
 Author: Cecilia Wieder
 Author-email: cw2019@ic.ac.uk
 License: GNU 3.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -171,16 +171,24 @@
 }
 
 ```
 
 ## Contributing
 Read our [contributor's guide](https://github.com/cwieder/py-ssPA/blob/main/CONTRIBUTING.md) to get started
 
+### Contributors
+We are grateful for our contributors who help develop and maintain py-ssPA:
+- Maëlick Brochut [@mbrochut](https://github.com/mbrochut)
+
 ## News 
 
+### [v0.2.3] - 23/06/23
+- @mbrochut Bug fix in KEGG pathway downloader 
+- @mbrochut Add tqdm progress bar for long KEGG downloads
+
 ### [v0.2.1] - 05/01/23
 - Removal of rpy2 dependency for improved compatibility across systems
 - Use [GSEApy](https://github.com/zqfang/GSEApy) as backend for GSEA and ssGSEA 
 - Minor syntax changes
    - `ora.ttest_res` is now `ora.DA_test_res` (as we can implement t-test or MWU tests)
    - `sspa_fgsea()` is now `sspa_gsea()` and uses gseapy as the backend rather than R fgsea
    - `sspa_gsva()` is temporarily deprecated due to the need for the rpy2 compatability - use the [GSVA R package](https://bioconductor.org/packages/release/bioc/html/GSVA.html)
```

### Comparing `sspa-0.2.2/src/sspa.egg-info/SOURCES.txt` & `sspa-0.2.3/src/sspa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/tests/test_download_pathways.py` & `sspa-0.2.3/tests/test_download_pathways.py`

 * *Files identical despite different names*

### Comparing `sspa-0.2.2/tests/test_utils.py` & `sspa-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

