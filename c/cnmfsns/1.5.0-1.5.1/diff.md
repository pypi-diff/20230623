# Comparing `tmp/cnmfsns-1.5.0.tar.gz` & `tmp/cnmfsns-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmfsns-1.5.0.tar", last modified: Wed Jun 21 20:06:38 2023, max compression
+gzip compressed data, was "cnmfsns-1.5.1.tar", last modified: Fri Jun 23 16:45:40 2023, max compression
```

## Comparing `cnmfsns-1.5.0.tar` & `cnmfsns-1.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 20:06:38.944065 cnmfsns-1.5.0/
--rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.5.0/LICENSE
--rw-rw-rw-   0        0        0     4246 2023-06-21 20:06:38.944065 cnmfsns-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3731 2023-06-21 20:02:01.000000 cnmfsns-1.5.0/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      980 2023-06-21 20:06:38.944065 cnmfsns-1.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-21 20:06:38.888950 cnmfsns-1.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-21 20:06:38.908788 cnmfsns-1.5.0/src/cnmfsns/
--rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.5.0/src/cnmfsns/__init__.py
--rw-rw-rw-   0        0        0    51994 2023-06-21 19:58:59.000000 cnmfsns-1.5.0/src/cnmfsns/cli.py
--rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.5.0/src/cnmfsns/cnmf.py
--rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.5.0/src/cnmfsns/colors.py
--rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.5.0/src/cnmfsns/config.py
--rw-rw-rw-   0        0        0    35838 2023-06-14 22:17:36.000000 cnmfsns-1.5.0/src/cnmfsns/dataset.py
--rw-rw-rw-   0        0        0    21163 2023-06-19 20:28:23.000000 cnmfsns-1.5.0/src/cnmfsns/integration.py
--rw-rw-rw-   0        0        0    59336 2023-06-15 03:48:57.000000 cnmfsns-1.5.0/src/cnmfsns/plots.py
--rw-rw-rw-   0        0        0    41117 2023-06-21 18:18:46.000000 cnmfsns-1.5.0/src/cnmfsns/sns.py
--rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.5.0/src/cnmfsns/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-21 20:06:38.944065 cnmfsns-1.5.0/src/cnmfsns.egg-info/
--rw-rw-rw-   0        0        0     4246 2023-06-21 20:06:38.000000 cnmfsns-1.5.0/src/cnmfsns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-06-21 20:06:38.000000 cnmfsns-1.5.0/src/cnmfsns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 20:06:38.000000 cnmfsns-1.5.0/src/cnmfsns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-21 20:06:38.000000 cnmfsns-1.5.0/src/cnmfsns.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      189 2023-06-21 20:06:38.000000 cnmfsns-1.5.0/src/cnmfsns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-21 20:06:38.000000 cnmfsns-1.5.0/src/cnmfsns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 16:45:40.150011 cnmfsns-1.5.1/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0     4246 2023-06-23 16:45:40.150011 cnmfsns-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3731 2023-06-23 16:41:17.000000 cnmfsns-1.5.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      980 2023-06-23 16:45:40.150011 cnmfsns-1.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 16:45:40.118734 cnmfsns-1.5.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 16:45:40.134373 cnmfsns-1.5.1/src/cnmfsns/
+-rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.5.1/src/cnmfsns/__init__.py
+-rw-rw-rw-   0        0        0    52028 2023-06-23 16:38:54.000000 cnmfsns-1.5.1/src/cnmfsns/cli.py
+-rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.5.1/src/cnmfsns/cnmf.py
+-rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.5.1/src/cnmfsns/colors.py
+-rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.5.1/src/cnmfsns/config.py
+-rw-rw-rw-   0        0        0    35838 2023-06-23 16:14:21.000000 cnmfsns-1.5.1/src/cnmfsns/dataset.py
+-rw-rw-rw-   0        0        0    21163 2023-06-23 16:39:53.000000 cnmfsns-1.5.1/src/cnmfsns/integration.py
+-rw-rw-rw-   0        0        0    59406 2023-06-23 16:40:44.000000 cnmfsns-1.5.1/src/cnmfsns/plots.py
+-rw-rw-rw-   0        0        0    41117 2023-06-21 18:18:46.000000 cnmfsns-1.5.1/src/cnmfsns/sns.py
+-rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.5.1/src/cnmfsns/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:45:40.150011 cnmfsns-1.5.1/src/cnmfsns.egg-info/
+-rw-rw-rw-   0        0        0     4246 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      189 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 16:45:40.000000 cnmfsns-1.5.1/src/cnmfsns.egg-info/top_level.txt
```

### Comparing `cnmfsns-1.5.0/LICENSE` & `cnmfsns-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.0/PKG-INFO` & `cnmfsns-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.5.0
+Version: 1.5.1
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
 
-![version badge](https://img.shields.io/badge/version-1.5.0-blue)
+![version badge](https://img.shields.io/badge/version-1.5.1-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```

### Comparing `cnmfsns-1.5.0/README.md` & `cnmfsns-1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2070 6f77 6572 6675 6c20 6661 6374 6f72   powerful factor
 00000050: 697a 6174 696f 6e2d 6261 7365 6420 6d75  ization-based mu
 00000060: 6c74 692d 6f6d 6963 7320 696e 7465 6772  lti-omics integr
 00000070: 6174 696f 6e20 746f 6f6c 6b69 740d 0a0d  ation toolkit...
 00000080: 0a21 5b76 6572 7369 6f6e 2062 6164 6765  .![version badge
 00000090: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
 000000a0: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-000000b0: 6572 7369 6f6e 2d31 2e35 2e30 2d62 6c75  ersion-1.5.0-blu
+000000b0: 6572 7369 6f6e 2d31 2e35 2e31 2d62 6c75  ersion-1.5.1-blu
 000000c0: 6529 0d0a 5b21 5b50 7950 4920 4c61 7465  e)..[![PyPI Late
 000000d0: 7374 2052 656c 6561 7365 5d28 6874 7470  st Release](http
 000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 000000f0: 696f 2f70 7970 692f 762f 636e 6d66 736e  io/pypi/v/cnmfsn
 00000100: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
 00000110: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000120: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b43  /cnmfsns/)..[![C
```

### Comparing `cnmfsns-1.5.0/setup.cfg` & `cnmfsns-1.5.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6e6d 6673 6e73 0d0a 7665 7273   = cnmfsns..vers
-00000020: 696f 6e20 3d20 312e 352e 300d 0a61 7574  ion = 1.5.0..aut
+00000020: 696f 6e20 3d20 312e 352e 310d 0a61 7574  ion = 1.5.1..aut
 00000030: 686f 7220 3d20 5465 6420 5665 7268 6579  hor = Ted Verhey
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2074 6276 6572 6865 7940 7563 616c 6761   tbverhey@ucalga
 00000060: 7279 2e63 610d 0a64 6573 6372 6970 7469  ry.ca..descripti
 00000070: 6f6e 203d 2063 4e4d 4620 536f 6c75 7469  on = cNMF Soluti
 00000080: 6f6e 204e 6574 776f 726b 2053 7061 6365  on Network Space
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `cnmfsns-1.5.0/src/cnmfsns/__init__.py` & `cnmfsns-1.5.1/src/cnmfsns/__init__.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.0/src/cnmfsns/cli.py` & `cnmfsns-1.5.1/src/cnmfsns/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -701,24 +701,24 @@
         for layer in dataset.get_metadata_df(include_categorical=False):
             df = snsmap.get_community_metadata_correlation(layer=layer, subset_datasets=dataset_name, method="pearson")
             df.to_csv(os.path.join(sns_output_dir, "annotated_communities", "correlation", dataset_name, layer + ".txt"), sep='\t')
 
     logging.info("Creating community-level bar plots")
 
     # Community-level, categorical data, overrepresentation bar plots
-    for dataset_name in integration.datasets:
+    for dataset_name, dataset in integration.datasets.items():
         os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_bar", dataset_name), exist_ok=True)
         for layer in dataset.get_metadata_df(include_numerical=False):
             fig = plot_overrepresentation_community_bar(snsmap, colors, layer=layer, subset_datasets=dataset_name)
             os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_bar"), exist_ok=True)
             fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "overrepresentation_bar", dataset_name, layer + ".pdf"))
             plt.close(fig)
         
     # Community-level, numerical metadata, correlation bar plots
-    for dataset_name in integration.datasets:
+    for dataset_name, dataset in integration.datasets.items():
         os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "correlation_bar", dataset_name), exist_ok=True)
         for layer in dataset.get_metadata_df(include_categorical=False):
             fig = plot_metadata_correlation_community_bar(snsmap, colors, layer=layer, subset_datasets=dataset_name)
             os.makedirs(os.path.join(sns_output_dir, "annotated_communities", "correlation_bar"), exist_ok=True)
             fig.savefig(os.path.join(sns_output_dir, "annotated_communities", "correlation_bar", dataset_name, layer + ".pdf"))
             plt.close(fig)
```

### Comparing `cnmfsns-1.5.0/src/cnmfsns/cnmf.py` & `cnmfsns-1.5.1/src/cnmfsns/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.0/src/cnmfsns/colors.py` & `cnmfsns-1.5.1/src/cnmfsns/colors.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.0/src/cnmfsns/config.py` & `cnmfsns-1.5.1/src/cnmfsns/config.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.0/src/cnmfsns/dataset.py` & `cnmfsns-1.5.1/src/cnmfsns/dataset.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.0/src/cnmfsns/integration.py` & `cnmfsns-1.5.1/src/cnmfsns/integration.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.0/src/cnmfsns/plots.py` & `cnmfsns-1.5.1/src/cnmfsns/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,16 @@
         gs2 = mpl.gridspec.GridSpecFromSubplotSpec(metadata.shape[1], 1, subplot_spec=gs0[2])
         for i, (track, annot) in enumerate(metadata.items()):
             ax = fig.add_subplot(gs2[i], sharex=ax_heatmap)
             ax.set_facecolor(missing_data_color)
             if pd.api.types.is_categorical_dtype(annot) or pd.api.types.is_object_dtype(annot):
                 ordered_rgb = annot.iloc[xind].replace(metadata_colors[track])
                 if ordered_rgb.isnull().any():
-                    ordered_rgb = ordered_rgb.cat.add_categories(missing_data_color)
+                    if pd.api.types.is_categorical_dtype(annot):
+                        ordered_rgb = ordered_rgb.cat.add_categories(missing_data_color)
                     ordered_rgb = ordered_rgb.fillna(missing_data_color)
                 ordered_rgb = ordered_rgb.astype("object").map(mpl.colors.to_rgb)
                 ordered_rgb = np.array([list(rgb) for rgb in ordered_rgb])
                 ax.imshow(np.stack([ordered_rgb, ordered_rgb]), aspect='auto', extent=[xmin,xmax,0,1], interpolation='none')
             else:
                 ax.imshow(np.stack([annot.iloc[xind],annot.iloc[xind]]), aspect='auto', extent=[xmin,xmax,0,1], cmap='Blues', interpolation='none')
             ax.set_yticks([])
```

### Comparing `cnmfsns-1.5.0/src/cnmfsns/sns.py` & `cnmfsns-1.5.1/src/cnmfsns/sns.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.0/src/cnmfsns/utils.py` & `cnmfsns-1.5.1/src/cnmfsns/utils.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.5.0/src/cnmfsns.egg-info/PKG-INFO` & `cnmfsns-1.5.1/src/cnmfsns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.5.0
+Version: 1.5.1
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
 
-![version badge](https://img.shields.io/badge/version-1.5.0-blue)
+![version badge](https://img.shields.io/badge/version-1.5.1-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```

