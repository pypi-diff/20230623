# Comparing `tmp/foambryo-0.2.3.tar.gz` & `tmp/foambryo-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/foambryo/dist/.tmp-k42zj9do/foambryo-0.2.3.tar", last modified: Thu Apr 13 07:51:29 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-c0f11wrk/foambryo-0.2.5.tar", last modified: Fri Jun 23 13:54:25 2023, max compression
```

## Comparing `foambryo-0.2.3.tar` & `foambryo-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 07:51:29.011943 foambryo-0.2.3/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     9396 2023-04-13 07:51:29.012174 foambryo-0.2.3/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     8766 2023-04-12 17:06:40.000000 foambryo-0.2.3/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2022-07-13 10:39:51.000000 foambryo-0.2.3/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      905 2023-04-13 07:51:29.012871 foambryo-0.2.3/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 07:51:29.007141 foambryo-0.2.3/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 07:51:29.009166 foambryo-0.2.3/src/foambryo/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-03-03 13:34:52.000000 foambryo-0.2.3/src/foambryo/__init__.py
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 07:51:29.011544 foambryo-0.2.3/src/foambryo.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     9396 2023-04-13 07:51:28.000000 foambryo-0.2.3/src/foambryo.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      238 2023-04-13 07:51:29.000000 foambryo-0.2.3/src/foambryo.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-04-13 07:51:28.000000 foambryo-0.2.3/src/foambryo.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-04-13 07:51:28.000000 foambryo-0.2.3/src/foambryo.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-04-13 07:51:28.000000 foambryo-0.2.3/src/foambryo.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:54:25.452247 foambryo-0.2.5/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11270 2023-06-23 13:54:25.452469 foambryo-0.2.5/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10640 2023-06-23 13:48:40.000000 foambryo-0.2.5/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:21:07.000000 foambryo-0.2.5/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      905 2023-06-23 13:54:25.453207 foambryo-0.2.5/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:54:25.445184 foambryo-0.2.5/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:54:25.449376 foambryo-0.2.5/src/foambryo/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    25142 2023-06-23 13:32:33.000000 foambryo-0.2.5/src/foambryo/Force_viewer.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/Inference_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10498 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/Plotting_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     8921 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/Pressure_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/Tension_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/__init__.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:54:25.451926 foambryo-0.2.5/src/foambryo.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11270 2023-06-23 13:54:25.000000 foambryo-0.2.5/src/foambryo.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-06-23 13:54:25.000000 foambryo-0.2.5/src/foambryo.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-06-23 13:54:25.000000 foambryo-0.2.5/src/foambryo.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-06-23 13:54:25.000000 foambryo-0.2.5/src/foambryo.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-06-23 13:54:25.000000 foambryo-0.2.5/src/foambryo.egg-info/top_level.txt
```

### Comparing `foambryo-0.2.3/PKG-INFO` & `foambryo-0.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: foambryo
-Version: 0.2.3
-Summary: Tension inference for 3D cell assemblies
-Home-page: https://github.com/sacha-ichbiah/foambryo
-Author: Sacha Ichbiah
-Author-email: sacha.ichbiah@college-de-france.fr
-Project-URL: Team website, https://www.turlierlab.com/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 ### foambryo
 
 **foambryo** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids.
 
 Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. They embody important features: symmetries, polarisations, patterning.
 Mechanics is at the heart of the development of these structures, yet tools to investigate forces at play during development in 3D are scarse. Characterizing and quantifying precisely their shapes allows us to match them to a simple physical model, and to reveal the forces shaping cells.
 
@@ -159,9 +142,23 @@
 ### Credits, contact, citations
 If you use this tool, please cite the associated preprint: 
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **foambryo** could help biologists and physicists to shed light on the mechanical aspects of early development.
 
 
 
+```
+@article {Ichbiah2023.04.12.536641,
+	author = {Sacha Ichbiah and Fabrice Delbary and Alex McDougall and R{\'e}mi Dumollard and Herv{\'e} Turlier},
+	title = {Embryo mechanics cartography: inference of 3D force atlases from fluorescence microscopy},
+	elocation-id = {2023.04.12.536641},
+	year = {2023},
+	doi = {10.1101/2023.04.12.536641},
+	publisher = {Cold Spring Harbor Laboratory},
+	abstract = {The morphogenesis of tissues and embryos results from a tight interplay between gene expression, biochemical signaling and mechanics. Although sequencing methods allow the generation of cell-resolved spatio-temporal maps of gene expression in developing tissues, creating similar maps of cell mechanics in 3D has remained a real challenge. Exploiting the foam-like geometry of cells in embryos, we propose a robust end-to-end computational method to infer spatiotemporal atlases of cellular forces from fluorescence microscopy images of cell membranes. Our method generates precise 3D meshes of cell geometry and successively predicts relative cell surface tensions and pressures in the tissue. We validate it with 3D active foam simulations, study its noise sensitivity, and prove its biological relevance in mouse, ascidian and C. elegans embryos. 3D inference allows us to recover mechanical features identified previously, but also predicts new ones, unveiling potential new insights on the spatiotemporal regulation of cell mechanics in early embryos. Our code is freely available and paves the way for unraveling the unknown mechanochemical feedbacks that control embryo and tissue morphogenesis.Competing Interest StatementThe authors have declared no competing interest.},
+	URL = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641},
+	eprint = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641.full.pdf},
+	journal = {bioRxiv}
+}
+```
```

### Comparing `foambryo-0.2.3/README.md` & `foambryo-0.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: foambryo
+Version: 0.2.5
+Summary: Tension inference for 3D cell assemblies
+Home-page: https://github.com/sacha-ichbiah/foambryo
+Author: Sacha Ichbiah
+Author-email: sacha.ichbiah@college-de-france.fr
+Project-URL: Team website, https://www.turlierlab.com/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 ### foambryo
 
 **foambryo** is a python package based on Polyscope designed to infer surface tensions, pressures and stresses from the geometry of epithelial-cell-clusters, namely early-embryos and structures encoutered in stem cell cultures, as organoids and embryoids.
 
 Living structures encountered in the field of developmental biology have intricate shapes and structures, that reflectes their physiological functions. They embody important features: symmetries, polarisations, patterning.
 Mechanics is at the heart of the development of these structures, yet tools to investigate forces at play during development in 3D are scarse. Characterizing and quantifying precisely their shapes allows us to match them to a simple physical model, and to reveal the forces shaping cells.
 
@@ -142,9 +159,23 @@
 ### Credits, contact, citations
 If you use this tool, please cite the associated preprint: 
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **foambryo** could help biologists and physicists to shed light on the mechanical aspects of early development.
 
 
 
+```
+@article {Ichbiah2023.04.12.536641,
+	author = {Sacha Ichbiah and Fabrice Delbary and Alex McDougall and R{\'e}mi Dumollard and Herv{\'e} Turlier},
+	title = {Embryo mechanics cartography: inference of 3D force atlases from fluorescence microscopy},
+	elocation-id = {2023.04.12.536641},
+	year = {2023},
+	doi = {10.1101/2023.04.12.536641},
+	publisher = {Cold Spring Harbor Laboratory},
+	abstract = {The morphogenesis of tissues and embryos results from a tight interplay between gene expression, biochemical signaling and mechanics. Although sequencing methods allow the generation of cell-resolved spatio-temporal maps of gene expression in developing tissues, creating similar maps of cell mechanics in 3D has remained a real challenge. Exploiting the foam-like geometry of cells in embryos, we propose a robust end-to-end computational method to infer spatiotemporal atlases of cellular forces from fluorescence microscopy images of cell membranes. Our method generates precise 3D meshes of cell geometry and successively predicts relative cell surface tensions and pressures in the tissue. We validate it with 3D active foam simulations, study its noise sensitivity, and prove its biological relevance in mouse, ascidian and C. elegans embryos. 3D inference allows us to recover mechanical features identified previously, but also predicts new ones, unveiling potential new insights on the spatiotemporal regulation of cell mechanics in early embryos. Our code is freely available and paves the way for unraveling the unknown mechanochemical feedbacks that control embryo and tissue morphogenesis.Competing Interest StatementThe authors have declared no competing interest.},
+	URL = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641},
+	eprint = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641.full.pdf},
+	journal = {bioRxiv}
+}
+```
```

### Comparing `foambryo-0.2.3/setup.cfg` & `foambryo-0.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foambryo
-version = 0.2.3
+version = 0.2.5
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Tension inference for 3D cell assemblies
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sacha-ichbiah/foambryo
 project_urls = 
@@ -23,15 +23,15 @@
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy>=1.21.6
 	polyscope>=1.2.0
 	scipy>=1.4.1
-	delaunay-watershed-3d>=0.2.0
+	delaunay-watershed-3d>=0.2.5
 	networkx>=2.5.1
 	matplotlib>=3.3.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `foambryo-0.2.3/src/foambryo.egg-info/PKG-INFO` & `foambryo-0.2.5/src/foambryo.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.2.3
+Version: 0.2.5
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -159,9 +159,23 @@
 ### Credits, contact, citations
 If you use this tool, please cite the associated preprint: 
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **foambryo** could help biologists and physicists to shed light on the mechanical aspects of early development.
 
 
 
+```
+@article {Ichbiah2023.04.12.536641,
+	author = {Sacha Ichbiah and Fabrice Delbary and Alex McDougall and R{\'e}mi Dumollard and Herv{\'e} Turlier},
+	title = {Embryo mechanics cartography: inference of 3D force atlases from fluorescence microscopy},
+	elocation-id = {2023.04.12.536641},
+	year = {2023},
+	doi = {10.1101/2023.04.12.536641},
+	publisher = {Cold Spring Harbor Laboratory},
+	abstract = {The morphogenesis of tissues and embryos results from a tight interplay between gene expression, biochemical signaling and mechanics. Although sequencing methods allow the generation of cell-resolved spatio-temporal maps of gene expression in developing tissues, creating similar maps of cell mechanics in 3D has remained a real challenge. Exploiting the foam-like geometry of cells in embryos, we propose a robust end-to-end computational method to infer spatiotemporal atlases of cellular forces from fluorescence microscopy images of cell membranes. Our method generates precise 3D meshes of cell geometry and successively predicts relative cell surface tensions and pressures in the tissue. We validate it with 3D active foam simulations, study its noise sensitivity, and prove its biological relevance in mouse, ascidian and C. elegans embryos. 3D inference allows us to recover mechanical features identified previously, but also predicts new ones, unveiling potential new insights on the spatiotemporal regulation of cell mechanics in early embryos. Our code is freely available and paves the way for unraveling the unknown mechanochemical feedbacks that control embryo and tissue morphogenesis.Competing Interest StatementThe authors have declared no competing interest.},
+	URL = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641},
+	eprint = {https://www.biorxiv.org/content/early/2023/04/13/2023.04.12.536641.full.pdf},
+	journal = {bioRxiv}
+}
+```
```

