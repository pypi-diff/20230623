# Comparing `tmp/cnmfsns-1.5.1.tar.gz` & `tmp/cnmfsns-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmfsns-1.5.1.tar", last modified: Fri Jun 23 16:45:40 2023, max compression
+gzip compressed data, was "cnmfsns-1.5.2.tar", last modified: Fri Jun 23 17:05:18 2023, max compression
```

## Comparing `cnmfsns-1.5.1.tar` & `cnmfsns-1.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 16:45:40.150011 cnmfsns-1.5.1/
--rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.5.1/LICENSE
--rw-rw-rw-   0        0        0     4246 2023-06-23 16:45:40.150011 cnmfsns-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     3731 2023-06-23 16:41:17.000000 cnmfsns-1.5.1/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.5.1/pyproject.toml
--rw-rw-rw-   0        0        0      980 2023-06-23 16:45:40.150011 cnmfsns-1.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-23 16:45:40.118734 cnmfsns-1.5.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 16:45:40.134373 cnmfsns-1.5.1/src/cnmfsns/
--rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.5.1/src/cnmfsns/__init__.py
--rw-rw-rw-   0        0        0    52028 2023-06-23 16:38:54.000000 cnmfsns-1.5.1/src/cnmfsns/cli.py
--rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.5.1/src/cnmfsns/cnmf.py
--rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.5.1/src/cnmfsns/colors.py
--rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.5.1/src/cnmfsns/config.py
--rw-rw-rw-   0        0        0    35838 2023-06-23 16:14:21.000000 cnmfsns-1.5.1/src/cnmfsns/dataset.py
--rw-rw-rw-   0        0        0    21163 2023-06-23 16:39:53.000000 cnmfsns-1.5.1/src/cnmfsns/integration.py
--rw-rw-rw-   0        0        0    59406 2023-06-23 16:40:44.000000 cnmfsns-1.5.1/src/cnmfsns/plots.py
--rw-rw-rw-   0        0        0    41117 2023-06-21 18:18:46.000000 cnmfsns-1.5.1/src/cnmfsns/sns.py
--rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.5.1/src/cnmfsns/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:45:40.150011 cnmfsns-1.5.1/src/cnmfsns.egg-info/
--rw-rw-rw-   0        0        0     4246 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      189 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 17:05:18.737539 cnmfsns-1.5.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0     4320 2023-06-23 17:05:18.737539 cnmfsns-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3805 2023-06-23 17:03:58.000000 cnmfsns-1.5.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0      980 2023-06-23 17:05:18.740532 cnmfsns-1.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 17:05:18.680345 cnmfsns-1.5.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 17:05:18.703354 cnmfsns-1.5.2/src/cnmfsns/
+-rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.5.2/src/cnmfsns/__init__.py
+-rw-rw-rw-   0        0        0    52062 2023-06-23 16:52:38.000000 cnmfsns-1.5.2/src/cnmfsns/cli.py
+-rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.5.2/src/cnmfsns/cnmf.py
+-rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.5.2/src/cnmfsns/colors.py
+-rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.5.2/src/cnmfsns/config.py
+-rw-rw-rw-   0        0        0    35838 2023-06-23 16:14:21.000000 cnmfsns-1.5.2/src/cnmfsns/dataset.py
+-rw-rw-rw-   0        0        0    21163 2023-06-23 16:39:53.000000 cnmfsns-1.5.2/src/cnmfsns/integration.py
+-rw-rw-rw-   0        0        0    59406 2023-06-23 17:03:17.000000 cnmfsns-1.5.2/src/cnmfsns/plots.py
+-rw-rw-rw-   0        0        0    41117 2023-06-21 18:18:46.000000 cnmfsns-1.5.2/src/cnmfsns/sns.py
+-rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.5.2/src/cnmfsns/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:05:18.735474 cnmfsns-1.5.2/src/cnmfsns.egg-info/
+-rw-rw-rw-   0        0        0     4320 2023-06-23 17:05:18.000000 cnmfsns-1.5.2/src/cnmfsns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-06-23 17:05:18.000000 cnmfsns-1.5.2/src/cnmfsns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 17:05:18.000000 cnmfsns-1.5.2/src/cnmfsns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-23 17:05:18.000000 cnmfsns-1.5.2/src/cnmfsns.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      189 2023-06-23 17:05:18.000000 cnmfsns-1.5.2/src/cnmfsns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 17:05:18.000000 cnmfsns-1.5.2/src/cnmfsns.egg-info/top_level.txt
```

### Comparing `cnmfsns-1.5.1/LICENSE` & `cnmfsns-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.1/PKG-INFO` & `cnmfsns-1.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.5.1
+Version: 1.5.2
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.5.1-blue)
+![version badge](https://img.shields.io/badge/version-1.5.2-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
@@ -51,35 +51,37 @@
 - Two interfaces: command-line interface for rapid data exploration and python
   interface for extensibility and flexibility
 
 ## 🔧 Install
 
 ### ☁️ Public Release
 
-Install the package with conda:
+Install the package with conda (in an isolated conda environment)
 ```bash
-conda install -c conda-forge cnmfsns
+conda env create cnmfsns -c conda-forge cnmfsns
+conda activate cnmfsns
 ```
 
 ### ✨ Latest version from GitHub
 
 Before installing cNMF-SNS using pip, it is recommended to first set up a separate conda environment and have conda manage as many dependencies as possible.
 
 ```bash
-conda create --name cnmfsns -c conda-forge python=3.10 anndata pandas numpy scipy matplotlib upsetplot httplib2 tomli tomli-w click pygraphviz python-igraph semantic_version pyyaml scikit-learn fastcluster scanpy pyyaml
+conda create --name cnmfsns -c conda-forge python=3.10 anndata pandas numpy scipy matplotlib upsetplot httplib2 tomli tomli-w click pygraphviz python-igraph pyyaml scikit-learn fastcluster scanpy pyyaml
 conda activate cnmfsns
 pip install git+https://github.com/MorrissyLab/cNMF-SNS.git
 ```
 
 ## 📖 Documentation
 
-### 🗐 Data requirements
+### 🗐 Data guidelines
 
 cNMF-SNS can factorize a wide variety of datasets, but will work optimally in these conditions:
-  - Use untransformed (raw) data where possible. For (sc)RNA-Seq data, use feature counts, not TPM or other log-transformed values.
+  - Use untransformed (raw) data where possible.
+  - For single-cell or spatial RNA-Seq data, use feature counts, not TPM or other log-transformed values.
 
 
 ### 📓 Python interface
 
 To get started, sample proteomics datasets and a Jupyter notebook tutorial is available [here](/tutorial/tutorial.ipynb).
 
 Detailed API reference can be found on [ReadTheDocs](https://cnmf-sns.readthedocs.io/).
```

### Comparing `cnmfsns-1.5.1/README.md` & `cnmfsns-1.5.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2070 6f77 6572 6675 6c20 6661 6374 6f72   powerful factor
 00000050: 697a 6174 696f 6e2d 6261 7365 6420 6d75  ization-based mu
 00000060: 6c74 692d 6f6d 6963 7320 696e 7465 6772  lti-omics integr
 00000070: 6174 696f 6e20 746f 6f6c 6b69 740d 0a0d  ation toolkit...
 00000080: 0a21 5b76 6572 7369 6f6e 2062 6164 6765  .![version badge
 00000090: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
 000000a0: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-000000b0: 6572 7369 6f6e 2d31 2e35 2e31 2d62 6c75  ersion-1.5.1-blu
+000000b0: 6572 7369 6f6e 2d31 2e35 2e32 2d62 6c75  ersion-1.5.2-blu
 000000c0: 6529 0d0a 5b21 5b50 7950 4920 4c61 7465  e)..[![PyPI Late
 000000d0: 7374 2052 656c 6561 7365 5d28 6874 7470  st Release](http
 000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 000000f0: 696f 2f70 7970 692f 762f 636e 6d66 736e  io/pypi/v/cnmfsn
 00000100: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
 00000110: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000120: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b43  /cnmfsns/)..[![C
@@ -141,94 +141,98 @@
 000008c0: 2065 7874 656e 7369 6269 6c69 7479 2061   extensibility a
 000008d0: 6e64 2066 6c65 7869 6269 6c69 7479 0d0a  nd flexibility..
 000008e0: 0d0a 2323 20f0 9f94 a720 496e 7374 616c  ..## .... Instal
 000008f0: 6c0d 0a0d 0a23 2323 20e2 9881 efb8 8f20  l....### ...... 
 00000900: 5075 626c 6963 2052 656c 6561 7365 0d0a  Public Release..
 00000910: 0d0a 496e 7374 616c 6c20 7468 6520 7061  ..Install the pa
 00000920: 636b 6167 6520 7769 7468 2063 6f6e 6461  ckage with conda
-00000930: 3a0d 0a60 6060 6261 7368 0d0a 636f 6e64  :..```bash..cond
-00000940: 6120 696e 7374 616c 6c20 2d63 2063 6f6e  a install -c con
-00000950: 6461 2d66 6f72 6765 2063 6e6d 6673 6e73  da-forge cnmfsns
-00000960: 0d0a 6060 600d 0a0d 0a23 2323 20e2 9ca8  ..```....### ...
-00000970: 204c 6174 6573 7420 7665 7273 696f 6e20   Latest version 
-00000980: 6672 6f6d 2047 6974 4875 620d 0a0d 0a42  from GitHub....B
-00000990: 6566 6f72 6520 696e 7374 616c 6c69 6e67  efore installing
-000009a0: 2063 4e4d 462d 534e 5320 7573 696e 6720   cNMF-SNS using 
-000009b0: 7069 702c 2069 7420 6973 2072 6563 6f6d  pip, it is recom
-000009c0: 6d65 6e64 6564 2074 6f20 6669 7273 7420  mended to first 
-000009d0: 7365 7420 7570 2061 2073 6570 6172 6174  set up a separat
-000009e0: 6520 636f 6e64 6120 656e 7669 726f 6e6d  e conda environm
-000009f0: 656e 7420 616e 6420 6861 7665 2063 6f6e  ent and have con
-00000a00: 6461 206d 616e 6167 6520 6173 206d 616e  da manage as man
-00000a10: 7920 6465 7065 6e64 656e 6369 6573 2061  y dependencies a
-00000a20: 7320 706f 7373 6962 6c65 2e0d 0a0d 0a60  s possible.....`
-00000a30: 6060 6261 7368 0d0a 636f 6e64 6120 6372  ``bash..conda cr
-00000a40: 6561 7465 202d 2d6e 616d 6520 636e 6d66  eate --name cnmf
-00000a50: 736e 7320 2d63 2063 6f6e 6461 2d66 6f72  sns -c conda-for
-00000a60: 6765 2070 7974 686f 6e3d 332e 3130 2061  ge python=3.10 a
-00000a70: 6e6e 6461 7461 2070 616e 6461 7320 6e75  nndata pandas nu
-00000a80: 6d70 7920 7363 6970 7920 6d61 7470 6c6f  mpy scipy matplo
-00000a90: 746c 6962 2075 7073 6574 706c 6f74 2068  tlib upsetplot h
-00000aa0: 7474 706c 6962 3220 746f 6d6c 6920 746f  ttplib2 tomli to
-00000ab0: 6d6c 692d 7720 636c 6963 6b20 7079 6772  mli-w click pygr
-00000ac0: 6170 6876 697a 2070 7974 686f 6e2d 6967  aphviz python-ig
-00000ad0: 7261 7068 2073 656d 616e 7469 635f 7665  raph semantic_ve
-00000ae0: 7273 696f 6e20 7079 7961 6d6c 2073 6369  rsion pyyaml sci
-00000af0: 6b69 742d 6c65 6172 6e20 6661 7374 636c  kit-learn fastcl
-00000b00: 7573 7465 7220 7363 616e 7079 2070 7979  uster scanpy pyy
-00000b10: 616d 6c0d 0a63 6f6e 6461 2061 6374 6976  aml..conda activ
-00000b20: 6174 6520 636e 6d66 736e 730d 0a70 6970  ate cnmfsns..pip
-00000b30: 2069 6e73 7461 6c6c 2067 6974 2b68 7474   install git+htt
-00000b40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000b50: 4d6f 7272 6973 7379 4c61 622f 634e 4d46  MorrissyLab/cNMF
-00000b60: 2d53 4e53 2e67 6974 0d0a 6060 600d 0a0d  -SNS.git..```...
-00000b70: 0a23 2320 f09f 9396 2044 6f63 756d 656e  .## .... Documen
-00000b80: 7461 7469 6f6e 0d0a 0d0a 2323 2320 f09f  tation....### ..
-00000b90: 9790 2044 6174 6120 7265 7175 6972 656d  .. Data requirem
-00000ba0: 656e 7473 0d0a 0d0a 634e 4d46 2d53 4e53  ents....cNMF-SNS
-00000bb0: 2063 616e 2066 6163 746f 7269 7a65 2061   can factorize a
-00000bc0: 2077 6964 6520 7661 7269 6574 7920 6f66   wide variety of
-00000bd0: 2064 6174 6173 6574 732c 2062 7574 2077   datasets, but w
-00000be0: 696c 6c20 776f 726b 206f 7074 696d 616c  ill work optimal
-00000bf0: 6c79 2069 6e20 7468 6573 6520 636f 6e64  ly in these cond
-00000c00: 6974 696f 6e73 3a0d 0a20 202d 2055 7365  itions:..  - Use
-00000c10: 2075 6e74 7261 6e73 666f 726d 6564 2028   untransformed (
-00000c20: 7261 7729 2064 6174 6120 7768 6572 6520  raw) data where 
-00000c30: 706f 7373 6962 6c65 2e20 466f 7220 2873  possible. For (s
-00000c40: 6329 524e 412d 5365 7120 6461 7461 2c20  c)RNA-Seq data, 
-00000c50: 7573 6520 6665 6174 7572 6520 636f 756e  use feature coun
-00000c60: 7473 2c20 6e6f 7420 5450 4d20 6f72 206f  ts, not TPM or o
-00000c70: 7468 6572 206c 6f67 2d74 7261 6e73 666f  ther log-transfo
-00000c80: 726d 6564 2076 616c 7565 732e 0d0a 0d0a  rmed values.....
-00000c90: 0d0a 2323 2320 f09f 9393 2050 7974 686f  ..### .... Pytho
-00000ca0: 6e20 696e 7465 7266 6163 650d 0a0d 0a54  n interface....T
-00000cb0: 6f20 6765 7420 7374 6172 7465 642c 2073  o get started, s
-00000cc0: 616d 706c 6520 7072 6f74 656f 6d69 6373  ample proteomics
-00000cd0: 2064 6174 6173 6574 7320 616e 6420 6120   datasets and a 
-00000ce0: 4a75 7079 7465 7220 6e6f 7465 626f 6f6b  Jupyter notebook
-00000cf0: 2074 7574 6f72 6961 6c20 6973 2061 7661   tutorial is ava
-00000d00: 696c 6162 6c65 205b 6865 7265 5d28 2f74  ilable [here](/t
-00000d10: 7574 6f72 6961 6c2f 7475 746f 7269 616c  utorial/tutorial
-00000d20: 2e69 7079 6e62 292e 0d0a 0d0a 4465 7461  .ipynb).....Deta
-00000d30: 696c 6564 2041 5049 2072 6566 6572 656e  iled API referen
-00000d40: 6365 2063 616e 2062 6520 666f 756e 6420  ce can be found 
-00000d50: 6f6e 205b 5265 6164 5468 6544 6f63 735d  on [ReadTheDocs]
-00000d60: 2868 7474 7073 3a2f 2f63 6e6d 662d 736e  (https://cnmf-sn
-00000d70: 732e 7265 6164 7468 6564 6f63 732e 696f  s.readthedocs.io
-00000d80: 2f29 2e0d 0a0d 0a0d 0a23 2323 20e2 8ca8  /).......### ...
-00000d90: efb8 8f20 436f 6d6d 616e 6420 6c69 6e65  ... Command line
-00000da0: 2069 6e74 6572 6661 6365 0d0a 0d0a 5365   interface....Se
-00000db0: 6520 7468 6520 5b63 6f6d 6d61 6e64 206c  e the [command l
-00000dc0: 696e 6520 696e 7465 7266 6163 6520 646f  ine interface do
-00000dd0: 6375 6d65 6e74 6174 696f 6e5d 282f 434c  cumentation](/CL
-00000de0: 492e 6d64 292e 0d0a 0d0a 2323 20f0 9f92  I.md).....## ...
-00000df0: ad20 4765 7474 696e 6720 4865 6c70 0d0a  . Getting Help..
-00000e00: 0d0a 466f 7220 6572 726f 7273 2061 7269  ..For errors ari
-00000e10: 7369 6e67 2064 7572 696e 6720 7573 6520  sing during use 
-00000e20: 6f66 2063 4e4d 462d 534e 532c 2063 7265  of cNMF-SNS, cre
-00000e30: 6174 6520 616e 6420 6272 6f77 7365 2069  ate and browse i
-00000e40: 7373 7565 7320 696e 2074 6865 205b 4769  ssues in the [Gi
-00000e50: 7448 7562 2022 6973 7375 6573 2220 7461  tHub "issues" ta
-00000e60: 625d 2868 7474 7073 3a2f 2f67 6974 6875  b](https://githu
-00000e70: 622e 636f 6d2f 4d6f 7272 6973 7379 4c61  b.com/MorrissyLa
-00000e80: 622f 634e 4d46 2d53 4e53 2f69 7373 7565  b/cNMF-SNS/issue
-00000e90: 7329 2e                                  s).
+00000930: 2028 696e 2061 6e20 6973 6f6c 6174 6564   (in an isolated
+00000940: 2063 6f6e 6461 2065 6e76 6972 6f6e 6d65   conda environme
+00000950: 6e74 290d 0a60 6060 6261 7368 0d0a 636f  nt)..```bash..co
+00000960: 6e64 6120 656e 7620 6372 6561 7465 2063  nda env create c
+00000970: 6e6d 6673 6e73 202d 6320 636f 6e64 612d  nmfsns -c conda-
+00000980: 666f 7267 6520 636e 6d66 736e 730d 0a63  forge cnmfsns..c
+00000990: 6f6e 6461 2061 6374 6976 6174 6520 636e  onda activate cn
+000009a0: 6d66 736e 730d 0a60 6060 0d0a 0d0a 2323  mfsns..```....##
+000009b0: 2320 e29c a820 4c61 7465 7374 2076 6572  # ... Latest ver
+000009c0: 7369 6f6e 2066 726f 6d20 4769 7448 7562  sion from GitHub
+000009d0: 0d0a 0d0a 4265 666f 7265 2069 6e73 7461  ....Before insta
+000009e0: 6c6c 696e 6720 634e 4d46 2d53 4e53 2075  lling cNMF-SNS u
+000009f0: 7369 6e67 2070 6970 2c20 6974 2069 7320  sing pip, it is 
+00000a00: 7265 636f 6d6d 656e 6465 6420 746f 2066  recommended to f
+00000a10: 6972 7374 2073 6574 2075 7020 6120 7365  irst set up a se
+00000a20: 7061 7261 7465 2063 6f6e 6461 2065 6e76  parate conda env
+00000a30: 6972 6f6e 6d65 6e74 2061 6e64 2068 6176  ironment and hav
+00000a40: 6520 636f 6e64 6120 6d61 6e61 6765 2061  e conda manage a
+00000a50: 7320 6d61 6e79 2064 6570 656e 6465 6e63  s many dependenc
+00000a60: 6965 7320 6173 2070 6f73 7369 626c 652e  ies as possible.
+00000a70: 0d0a 0d0a 6060 6062 6173 680d 0a63 6f6e  ....```bash..con
+00000a80: 6461 2063 7265 6174 6520 2d2d 6e61 6d65  da create --name
+00000a90: 2063 6e6d 6673 6e73 202d 6320 636f 6e64   cnmfsns -c cond
+00000aa0: 612d 666f 7267 6520 7079 7468 6f6e 3d33  a-forge python=3
+00000ab0: 2e31 3020 616e 6e64 6174 6120 7061 6e64  .10 anndata pand
+00000ac0: 6173 206e 756d 7079 2073 6369 7079 206d  as numpy scipy m
+00000ad0: 6174 706c 6f74 6c69 6220 7570 7365 7470  atplotlib upsetp
+00000ae0: 6c6f 7420 6874 7470 6c69 6232 2074 6f6d  lot httplib2 tom
+00000af0: 6c69 2074 6f6d 6c69 2d77 2063 6c69 636b  li tomli-w click
+00000b00: 2070 7967 7261 7068 7669 7a20 7079 7468   pygraphviz pyth
+00000b10: 6f6e 2d69 6772 6170 6820 7079 7961 6d6c  on-igraph pyyaml
+00000b20: 2073 6369 6b69 742d 6c65 6172 6e20 6661   scikit-learn fa
+00000b30: 7374 636c 7573 7465 7220 7363 616e 7079  stcluster scanpy
+00000b40: 2070 7979 616d 6c0d 0a63 6f6e 6461 2061   pyyaml..conda a
+00000b50: 6374 6976 6174 6520 636e 6d66 736e 730d  ctivate cnmfsns.
+00000b60: 0a70 6970 2069 6e73 7461 6c6c 2067 6974  .pip install git
+00000b70: 2b68 7474 7073 3a2f 2f67 6974 6875 622e  +https://github.
+00000b80: 636f 6d2f 4d6f 7272 6973 7379 4c61 622f  com/MorrissyLab/
+00000b90: 634e 4d46 2d53 4e53 2e67 6974 0d0a 6060  cNMF-SNS.git..``
+00000ba0: 600d 0a0d 0a23 2320 f09f 9396 2044 6f63  `....## .... Doc
+00000bb0: 756d 656e 7461 7469 6f6e 0d0a 0d0a 2323  umentation....##
+00000bc0: 2320 f09f 9790 2044 6174 6120 6775 6964  # .... Data guid
+00000bd0: 656c 696e 6573 0d0a 0d0a 634e 4d46 2d53  elines....cNMF-S
+00000be0: 4e53 2063 616e 2066 6163 746f 7269 7a65  NS can factorize
+00000bf0: 2061 2077 6964 6520 7661 7269 6574 7920   a wide variety 
+00000c00: 6f66 2064 6174 6173 6574 732c 2062 7574  of datasets, but
+00000c10: 2077 696c 6c20 776f 726b 206f 7074 696d   will work optim
+00000c20: 616c 6c79 2069 6e20 7468 6573 6520 636f  ally in these co
+00000c30: 6e64 6974 696f 6e73 3a0d 0a20 202d 2055  nditions:..  - U
+00000c40: 7365 2075 6e74 7261 6e73 666f 726d 6564  se untransformed
+00000c50: 2028 7261 7729 2064 6174 6120 7768 6572   (raw) data wher
+00000c60: 6520 706f 7373 6962 6c65 2e0d 0a20 202d  e possible...  -
+00000c70: 2046 6f72 2073 696e 676c 652d 6365 6c6c   For single-cell
+00000c80: 206f 7220 7370 6174 6961 6c20 524e 412d   or spatial RNA-
+00000c90: 5365 7120 6461 7461 2c20 7573 6520 6665  Seq data, use fe
+00000ca0: 6174 7572 6520 636f 756e 7473 2c20 6e6f  ature counts, no
+00000cb0: 7420 5450 4d20 6f72 206f 7468 6572 206c  t TPM or other l
+00000cc0: 6f67 2d74 7261 6e73 666f 726d 6564 2076  og-transformed v
+00000cd0: 616c 7565 732e 0d0a 0d0a 0d0a 2323 2320  alues.......### 
+00000ce0: f09f 9393 2050 7974 686f 6e20 696e 7465  .... Python inte
+00000cf0: 7266 6163 650d 0a0d 0a54 6f20 6765 7420  rface....To get 
+00000d00: 7374 6172 7465 642c 2073 616d 706c 6520  started, sample 
+00000d10: 7072 6f74 656f 6d69 6373 2064 6174 6173  proteomics datas
+00000d20: 6574 7320 616e 6420 6120 4a75 7079 7465  ets and a Jupyte
+00000d30: 7220 6e6f 7465 626f 6f6b 2074 7574 6f72  r notebook tutor
+00000d40: 6961 6c20 6973 2061 7661 696c 6162 6c65  ial is available
+00000d50: 205b 6865 7265 5d28 2f74 7574 6f72 6961   [here](/tutoria
+00000d60: 6c2f 7475 746f 7269 616c 2e69 7079 6e62  l/tutorial.ipynb
+00000d70: 292e 0d0a 0d0a 4465 7461 696c 6564 2041  ).....Detailed A
+00000d80: 5049 2072 6566 6572 656e 6365 2063 616e  PI reference can
+00000d90: 2062 6520 666f 756e 6420 6f6e 205b 5265   be found on [Re
+00000da0: 6164 5468 6544 6f63 735d 2868 7474 7073  adTheDocs](https
+00000db0: 3a2f 2f63 6e6d 662d 736e 732e 7265 6164  ://cnmf-sns.read
+00000dc0: 7468 6564 6f63 732e 696f 2f29 2e0d 0a0d  thedocs.io/)....
+00000dd0: 0a0d 0a23 2323 20e2 8ca8 efb8 8f20 436f  ...### ...... Co
+00000de0: 6d6d 616e 6420 6c69 6e65 2069 6e74 6572  mmand line inter
+00000df0: 6661 6365 0d0a 0d0a 5365 6520 7468 6520  face....See the 
+00000e00: 5b63 6f6d 6d61 6e64 206c 696e 6520 696e  [command line in
+00000e10: 7465 7266 6163 6520 646f 6375 6d65 6e74  terface document
+00000e20: 6174 696f 6e5d 282f 434c 492e 6d64 292e  ation](/CLI.md).
+00000e30: 0d0a 0d0a 2323 20f0 9f92 ad20 4765 7474  ....## .... Gett
+00000e40: 696e 6720 4865 6c70 0d0a 0d0a 466f 7220  ing Help....For 
+00000e50: 6572 726f 7273 2061 7269 7369 6e67 2064  errors arising d
+00000e60: 7572 696e 6720 7573 6520 6f66 2063 4e4d  uring use of cNM
+00000e70: 462d 534e 532c 2063 7265 6174 6520 616e  F-SNS, create an
+00000e80: 6420 6272 6f77 7365 2069 7373 7565 7320  d browse issues 
+00000e90: 696e 2074 6865 205b 4769 7448 7562 2022  in the [GitHub "
+00000ea0: 6973 7375 6573 2220 7461 625d 2868 7474  issues" tab](htt
+00000eb0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000ec0: 4d6f 7272 6973 7379 4c61 622f 634e 4d46  MorrissyLab/cNMF
+00000ed0: 2d53 4e53 2f69 7373 7565 7329 2e         -SNS/issues).
```

### Comparing `cnmfsns-1.5.1/setup.cfg` & `cnmfsns-1.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6e6d 6673 6e73 0d0a 7665 7273   = cnmfsns..vers
-00000020: 696f 6e20 3d20 312e 352e 310d 0a61 7574  ion = 1.5.1..aut
+00000020: 696f 6e20 3d20 312e 352e 320d 0a61 7574  ion = 1.5.2..aut
 00000030: 686f 7220 3d20 5465 6420 5665 7268 6579  hor = Ted Verhey
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2074 6276 6572 6865 7940 7563 616c 6761   tbverhey@ucalga
 00000060: 7279 2e63 610d 0a64 6573 6372 6970 7469  ry.ca..descripti
 00000070: 6f6e 203d 2063 4e4d 4620 536f 6c75 7469  on = cNMF Soluti
 00000080: 6f6e 204e 6574 776f 726b 2053 7061 6365  on Network Space
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `cnmfsns-1.5.1/src/cnmfsns/__init__.py` & `cnmfsns-1.5.2/src/cnmfsns/__init__.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.1/src/cnmfsns/cli.py` & `cnmfsns-1.5.2/src/cnmfsns/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -722,24 +722,24 @@
             fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "correlation_bar", dataset_name, layer + ".pdf"))
             plt.close(fig)
 
 
     logging.info("Creating community-level network plots")
 
     # Community-level, categorical data, overrepresentation network
-    for dataset_name in integration.datasets:
+    for dataset_name, dataset in integration.datasets.items():
         os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_network", dataset_name), exist_ok=True)
         for layer in dataset.get_metadata_df(include_numerical=False):
             fig = plot_overrepresentation_community_network(snsmap, colors, layer=layer, subset_datasets=dataset_name)   
             fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_network", dataset_name, layer + ".pdf"))
             fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_network", dataset_name, layer + ".png"), dpi=600)
             plt.close(fig)
  
     # Community-level, numerical data, correlation network
-    for dataset_name in integration.datasets:
+    for dataset_name, dataset in integration.datasets.items():
         os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "correlation_network", dataset_name), exist_ok=True)
         for layer in dataset.get_metadata_df(include_categorical=False):
             fig = plot_metadata_correlation_community_network(snsmap, colors, layer=layer, subset_datasets=dataset_name)   
             fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "correlation_network", dataset_name, layer + ".pdf"))
             fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "correlation_network", dataset_name, layer + ".png"), dpi=600)
             plt.close(fig)
```

### Comparing `cnmfsns-1.5.1/src/cnmfsns/cnmf.py` & `cnmfsns-1.5.2/src/cnmfsns/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.1/src/cnmfsns/colors.py` & `cnmfsns-1.5.2/src/cnmfsns/colors.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.1/src/cnmfsns/config.py` & `cnmfsns-1.5.2/src/cnmfsns/config.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.1/src/cnmfsns/dataset.py` & `cnmfsns-1.5.2/src/cnmfsns/dataset.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.1/src/cnmfsns/integration.py` & `cnmfsns-1.5.2/src/cnmfsns/integration.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.1/src/cnmfsns/plots.py` & `cnmfsns-1.5.2/src/cnmfsns/plots.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.1/src/cnmfsns/sns.py` & `cnmfsns-1.5.2/src/cnmfsns/sns.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.1/src/cnmfsns/utils.py` & `cnmfsns-1.5.2/src/cnmfsns/utils.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.1/src/cnmfsns.egg-info/PKG-INFO` & `cnmfsns-1.5.2/src/cnmfsns.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.5.1
+Version: 1.5.2
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.5.1-blue)
+![version badge](https://img.shields.io/badge/version-1.5.2-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
@@ -51,35 +51,37 @@
 - Two interfaces: command-line interface for rapid data exploration and python
   interface for extensibility and flexibility
 
 ## 🔧 Install
 
 ### ☁️ Public Release
 
-Install the package with conda:
+Install the package with conda (in an isolated conda environment)
 ```bash
-conda install -c conda-forge cnmfsns
+conda env create cnmfsns -c conda-forge cnmfsns
+conda activate cnmfsns
 ```
 
 ### ✨ Latest version from GitHub
 
 Before installing cNMF-SNS using pip, it is recommended to first set up a separate conda environment and have conda manage as many dependencies as possible.
 
 ```bash
-conda create --name cnmfsns -c conda-forge python=3.10 anndata pandas numpy scipy matplotlib upsetplot httplib2 tomli tomli-w click pygraphviz python-igraph semantic_version pyyaml scikit-learn fastcluster scanpy pyyaml
+conda create --name cnmfsns -c conda-forge python=3.10 anndata pandas numpy scipy matplotlib upsetplot httplib2 tomli tomli-w click pygraphviz python-igraph pyyaml scikit-learn fastcluster scanpy pyyaml
 conda activate cnmfsns
 pip install git+https://github.com/MorrissyLab/cNMF-SNS.git
 ```
 
 ## 📖 Documentation
 
-### 🗐 Data requirements
+### 🗐 Data guidelines
 
 cNMF-SNS can factorize a wide variety of datasets, but will work optimally in these conditions:
-  - Use untransformed (raw) data where possible. For (sc)RNA-Seq data, use feature counts, not TPM or other log-transformed values.
+  - Use untransformed (raw) data where possible.
+  - For single-cell or spatial RNA-Seq data, use feature counts, not TPM or other log-transformed values.
 
 
 ### 📓 Python interface
 
 To get started, sample proteomics datasets and a Jupyter notebook tutorial is available [here](/tutorial/tutorial.ipynb).
 
 Detailed API reference can be found on [ReadTheDocs](https://cnmf-sns.readthedocs.io/).
```

