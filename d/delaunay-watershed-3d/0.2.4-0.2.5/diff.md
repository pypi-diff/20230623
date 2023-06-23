# Comparing `tmp/delaunay_watershed_3d-0.2.4.tar.gz` & `tmp/delaunay_watershed_3d-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/delaunay-watershed/dist/.tmp-fkmjxki_/delaunay_watershed_3d-0.2.4.tar", last modified: Thu Apr 13 08:11:29 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/delaunay-watershed/dist/.tmp-55fbnwhl/delaunay_watershed_3d-0.2.5.tar", last modified: Fri Jun 23 13:51:50 2023, max compression
```

## Comparing `delaunay_watershed_3d-0.2.4.tar` & `delaunay_watershed_3d-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 08:11:29.288559 delaunay_watershed_3d-0.2.4/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-13 08:11:29.288720 delaunay_watershed_3d-0.2.4/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5343 2023-04-12 12:26:50.000000 delaunay_watershed_3d-0.2.4/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     1019 2023-04-13 08:11:29.289679 delaunay_watershed_3d-0.2.4/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 08:11:29.270991 delaunay_watershed_3d-0.2.4/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 08:11:29.275760 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6029 2023-04-13 08:11:29.000000 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-04-13 08:11:29.000000 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-04-13 08:11:29.000000 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      163 2023-04-13 08:11:29.000000 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-04-13 08:11:29.000000 delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/top_level.txt
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-04-13 08:11:29.288155 delaunay_watershed_3d-0.2.4/src/dw3d/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    12409 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Curvature.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    21891 2023-04-13 08:05:19.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Dcel.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6880 2023-04-12 17:10:03.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Geometric_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    16784 2023-04-13 08:01:40.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Geometry.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Graph_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Mask_reconstruction.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10499 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/Networkx_functions.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/__init__.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-03-18 13:41:24.000000 delaunay_watershed_3d-0.2.4/src/dw3d/functions.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:51:50.357334 delaunay_watershed_3d-0.2.5/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     7904 2023-06-23 13:51:50.357451 delaunay_watershed_3d-0.2.5/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     7218 2023-06-23 13:44:43.000000 delaunay_watershed_3d-0.2.5/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     1008 2023-06-23 13:51:50.358058 delaunay_watershed_3d-0.2.5/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:51:50.339478 delaunay_watershed_3d-0.2.5/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:51:50.344512 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     7904 2023-06-23 13:51:50.000000 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      531 2023-06-23 13:51:50.000000 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-06-23 13:51:50.000000 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      152 2023-06-23 13:51:50.000000 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        5 2023-06-23 13:51:50.000000 delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:51:50.356707 delaunay_watershed_3d-0.2.5/src/dw3d/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    12255 2023-06-23 13:30:42.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Curvature.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    21852 2023-06-23 13:29:29.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Dcel.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6929 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Geometric_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    16784 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Geometry.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     6334 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Graph_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     2827 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Mask_reconstruction.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10499 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     3506 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/Networkx_functions.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       87 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/__init__.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     5033 2023-06-23 13:22:16.000000 delaunay_watershed_3d-0.2.5/src/dw3d/functions.py
```

### Comparing `delaunay_watershed_3d-0.2.4/PKG-INFO` & `delaunay_watershed_3d-0.2.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: delaunay_watershed_3d
-Version: 0.2.4
-Summary: Geometrical reconstruction of cell assemblies from instance segmentations
-Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
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
 # Delaunay-Watershed 3D
 
 <img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Figure_logo_white_arrow.png" alt="drawing" width="300"/>
 
 
 **Delaunay-Watershed-3D** is an algorithm designed to reconstruct a sparse representation of the geometry of tissues and cell nuclei from instance segmentations, in 3D. It accomplishes this by building multimaterial meshes from segmentation masks. These multimaterial meshes are perfectly suited for **storage, geometrical analysis, sharing** and **visualisation of data**. We provide high level APIs to extract geometrical features from the meshes, as well as visualisation tools based on [polyscope](https://polyscope.run) and [napari](https://napari.org).
 
@@ -119,7 +102,22 @@
 
 
 ### Credits, contact, citations
 If you use this tool, please cite the associated preprint.
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **Delaunay-Watershed** could help biologists and physicists to shed light on the mechanical aspects of early development.
 
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
+
```

### Comparing `delaunay_watershed_3d-0.2.4/README.md` & `delaunay_watershed_3d-0.2.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: delaunay_watershed_3d
+Version: 0.2.5
+Summary: Geometrical reconstruction of cell assemblies from instance segmentations
+Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
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
 # Delaunay-Watershed 3D
 
 <img src="https://raw.githubusercontent.com/sacha-ichbiah/delaunay_watershed_3d/main/Figures_readme/Figure_logo_white_arrow.png" alt="drawing" width="300"/>
 
 
 **Delaunay-Watershed-3D** is an algorithm designed to reconstruct a sparse representation of the geometry of tissues and cell nuclei from instance segmentations, in 3D. It accomplishes this by building multimaterial meshes from segmentation masks. These multimaterial meshes are perfectly suited for **storage, geometrical analysis, sharing** and **visualisation of data**. We provide high level APIs to extract geometrical features from the meshes, as well as visualisation tools based on [polyscope](https://polyscope.run) and [napari](https://napari.org).
 
@@ -102,7 +119,22 @@
 
 
 ### Credits, contact, citations
 If you use this tool, please cite the associated preprint.
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **Delaunay-Watershed** could help biologists and physicists to shed light on the mechanical aspects of early development.
 
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
+
```

### Comparing `delaunay_watershed_3d-0.2.4/setup.cfg` & `delaunay_watershed_3d-0.2.5/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = delaunay_watershed_3d
-version = 0.2.4
+version = 0.2.5
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Geometrical reconstruction of cell assemblies from instance segmentations
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/VirtualEmbryo/delaunay-watershed
 project_urls = 
@@ -28,15 +28,15 @@
 	scipy>=1.4.1
 	polyscope>=1.2.0
 	matplotlib>=3.3.1
 	networkx>=2.5.1
 	torch>=1.6.0
 	edt>=2.2.0
 	trimesh>=3.8.12
-	robust-laplacian>=0.2.2
+	tqdm>=4.60.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/PKG-INFO` & `delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-watershed-3d
-Version: 0.2.4
+Version: 0.2.5
 Summary: Geometrical reconstruction of cell assemblies from instance segmentations
 Home-page: https://github.com/VirtualEmbryo/delaunay-watershed
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -119,7 +119,22 @@
 
 
 ### Credits, contact, citations
 If you use this tool, please cite the associated preprint.
 Do not hesitate to contact Sacha Ichbiah and Hervé Turlier for practical questions and applications. 
 We hope that **Delaunay-Watershed** could help biologists and physicists to shed light on the mechanical aspects of early development.
 
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
+
```

### Comparing `delaunay_watershed_3d-0.2.4/src/delaunay_watershed_3d.egg-info/SOURCES.txt` & `delaunay_watershed_3d-0.2.5/src/delaunay_watershed_3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.4/src/dw3d/Curvature.py` & `delaunay_watershed_3d-0.2.5/src/dw3d/Curvature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #Sacha Ichbiah, Sept 2021
 import numpy as np 
 import scipy.sparse as sp
-import robust_laplacian
 import trimesh
 
-#TODO: IMPLEMENT THE EDGE_BASED CURVATURE FORMULA
+#TODO: IMPLEMENT THE EDGE_BASED CURVATURE FORMULA (Paper from Julicher)
 
 def find_key_multiplier(num_points): 
     key_multiplier = 1
     while num_points//key_multiplier != 0 : 
         key_multiplier*=10
     return(key_multiplier)   
 
@@ -74,28 +73,14 @@
     L, inv_areas=laplacian_cot(verts,faces)
     inv_areas = inv_areas.reshape(-1)
     sum_cols = np.array(L.sum(axis=1))
     Laplacian = L@verts - verts*sum_cols
     norm = (0.75*inv_areas).reshape(-1,1)
     return(Laplacian*norm,inv_areas)
 
-def compute_laplacian_robust(Mesh): 
-    ### Robust Laplacian using implicit triangulations : 
-    # from "A Laplacian for Nonmanifold Triangle Meshes", N.Sharp, K.Crane, 2020
-    verts = Mesh.v
-    faces = Mesh.f[:,[0,1,2]]
-    L, M=robust_laplacian.mesh_laplacian(Mesh.v,Mesh.f[:,[0,1,2]])
-    inv_areas = 1/M.diagonal().reshape(-1)/3
-    Sum_cols = np.array(L.sum(axis=1)) #Useless as it is already 0 (sum comprised in the central term) see http://rodolphe-vaillant.fr/entry/101/definition-laplacian-matrix-for-triangle-meshes
-    first_term = np.dot(L.toarray(),verts)
-    second_term = verts*Sum_cols
-    Laplacian = (first_term-second_term)
-    norm = (1.5*inv_areas).reshape(-1,1)
-    return(-Laplacian*norm,inv_areas)
-
 def compute_gaussian_curvature_vertices(Mesh):
     mesh_trimesh =trimesh.Trimesh(vertices=Mesh.v,
                   faces = Mesh.f[:,:3]) 
     G = trimesh.curvature.discrete_gaussian_curvature_measure(mesh_trimesh, Mesh.v,0.)
     return(G)
 
     
@@ -107,34 +92,18 @@
     Sum_cols = np.array(L.sum(axis=1))
     first_term = np.dot(L.toarray(),verts)
     second_term = verts*Sum_cols
     Laplacian = (first_term-second_term)/2
     H = np.linalg.norm(Laplacian,axis=1)*3*inv_areas/2
     return(H,inv_areas,Laplacian*3*(np.array([inv_areas]*3).transpose())/2)
 
-def compute_curvature_vertices_robust_laplacian(Mesh): 
-    verts = Mesh.v
-    faces = Mesh.f[:,[0,1,2]]
-    L, M=robust_laplacian.mesh_laplacian(Mesh.v,Mesh.f[:,[0,1,2]])
-    inv_areas = 1/M.diagonal().reshape(-1)/3
-    Sum_cols = np.array(L.sum(axis=1))
-    first_term = np.dot(L.toarray(),verts)
-    second_term = verts*Sum_cols
-    Laplacian = (first_term-second_term)
-    H = np.linalg.norm(Laplacian,axis=1)*3*inv_areas/2
-    return(H,inv_areas,Laplacian*3*(np.array([inv_areas]*3).transpose())/2)
 
+def compute_curvature_interfaces(Mesh,weighted=True): 
 
-def compute_curvature_interfaces(Mesh,laplacian = "robust",weighted=True): 
-    Interfaces={}
-    Interfaces_weights={}
-    if laplacian =="robust" : 
-        L,inv_areas = compute_laplacian_robust(Mesh)
-    elif laplacian =="cotan" : 
-        L,inv_areas = compute_laplacian_cotan(Mesh)
+    L,inv_areas = compute_laplacian_cotan(Mesh)
 
     vertex_normals = Mesh.compute_vertex_normals()
     H = np.sign(np.sum(np.multiply(L,vertex_normals),axis=1))*np.linalg.norm(L,axis=1)
     
     
     Vertices_on_interfaces ={}
     for edge in Mesh.half_edges : 
@@ -357,7 +326,37 @@
     Diffs = np.array([Half_perimeters]*3).transpose() - Lengths_sides
     Areas = (Half_perimeters*Diffs[:,0]*Diffs[:,1]*Diffs[:,2])**(0.5)
     return(Areas)
 
 
 
 
+"""
+import robust-laplacian
+def compute_laplacian_robust(Mesh): 
+    ### Robust Laplacian using implicit triangulations : 
+    # from "A Laplacian for Nonmanifold Triangle Meshes", N.Sharp, K.Crane, 2020
+    verts = Mesh.v
+    faces = Mesh.f[:,[0,1,2]]
+    L, M=robust_laplacian.mesh_laplacian(Mesh.v,Mesh.f[:,[0,1,2]])
+    inv_areas = 1/M.diagonal().reshape(-1)/3
+    Sum_cols = np.array(L.sum(axis=1)) #Useless as it is already 0 (sum comprised in the central term) see http://rodolphe-vaillant.fr/entry/101/definition-laplacian-matrix-for-triangle-meshes
+    first_term = np.dot(L.toarray(),verts)
+    second_term = verts*Sum_cols
+    Laplacian = (first_term-second_term)
+    norm = (1.5*inv_areas).reshape(-1,1)
+    return(-Laplacian*norm,inv_areas)
+
+
+def compute_curvature_vertices_robust_laplacian(Mesh): 
+    verts = Mesh.v
+    faces = Mesh.f[:,[0,1,2]]
+    L, M=robust_laplacian.mesh_laplacian(Mesh.v,Mesh.f[:,[0,1,2]])
+    inv_areas = 1/M.diagonal().reshape(-1)/3
+    Sum_cols = np.array(L.sum(axis=1))
+    first_term = np.dot(L.toarray(),verts)
+    second_term = verts*Sum_cols
+    Laplacian = (first_term-second_term)
+    H = np.linalg.norm(Laplacian,axis=1)*3*inv_areas/2
+    return(H,inv_areas,Laplacian*3*(np.array([inv_areas]*3).transpose())/2)
+
+"""
```

### Comparing `delaunay_watershed_3d-0.2.4/src/dw3d/Dcel.py` & `delaunay_watershed_3d-0.2.5/src/dw3d/Dcel.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,41 +371,41 @@
     
     def compute_areas_cells(self):
         return(compute_areas_cells(self))
 
     def compute_areas_interfaces(self): 
         return(compute_areas_interfaces(self))
     
-    def compute_area_derivatives(self): 
+    def compute_area_derivatives_slow(self): 
         return(compute_area_derivative_dict(self))
 
-    def compute_area_derivatives_fast(self): 
+    def compute_area_derivatives(self): 
         return(compute_area_derivative_autodiff(self))
 
     def compute_volumes_cells(self): 
         return(compute_volume_cells(self))
     
-    def compute_volume_derivatives(self):
+    def compute_volume_derivatives_slow(self):
         return(compute_volume_derivative_dict(self))
     
-    def compute_volume_derivatives_fast(self):
+    def compute_volume_derivatives(self):
         return(compute_volume_derivative_autodiff_dict(self))
     
     def compute_length_derivatives(self):
         return(compute_length_derivative_autodiff(self))
 
     def compute_angles_junctions(self,unique=True):
         return(compute_angles_tri(self,unique=unique)[0])
 
     def compute_angles_tri(self,unique=True):
         return(compute_angles_tri(self,unique=unique))
 
-    def compute_curvatures_interfaces(self,laplacian="robust",weighted=True):
+    def compute_curvatures_interfaces(self,weighted=True):
         #"robust" or "cotan"
-        return(compute_curvature_interfaces(self,laplacian=laplacian,weighted=weighted))
+        return(compute_curvature_interfaces(self,weighted=weighted))
 
 
     def save(self, filename):
         with open(filename, "wb") as f:
             # Pickle the 'data' dictionary using the highest protocol available.
             pickle.dump(self.vertices, f, pickle.HIGHEST_PROTOCOL)
             pickle.dump(self.half_edges, f, pickle.HIGHEST_PROTOCOL)
```

### Comparing `delaunay_watershed_3d-0.2.4/src/dw3d/Geometric_utilities.py` & `delaunay_watershed_3d-0.2.5/src/dw3d/Geometric_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,14 @@
 
 def build_triangulation(labels,min_distance=5,mode='torch',prints=False):
     if mode == 'torch': 
         return(build_triangulation_torch(labels,(min_distance//2)*2 +1,prints))
     else : 
         return(build_triangulation_skimage(labels,min_distance,prints))
 
-
 def build_triangulation_torch(labels,min_distance=5,prints=False):#,size_shell=2,dist_shell=4):
     if prints : 
         print("Mode == Torch")
         print("Kernel size =",min_distance)
         print("Computing EDT ...")
     t1 = time()
     b = StandardLabelToBoundary()(labels)[0]
@@ -127,16 +126,18 @@
         seeds_coords.append(table_coords[f_i][seed])
         
     seeds_coords = np.array(seeds_coords)
     seeds_indices = values_lbls
 
     corners = give_corners(Total_EDT)
     
+    
     t3 = time()
     if prints : print("Searching local extremas ...")
+    np.random.seed(42)
     EDT =Total_EDT + np.random.rand(nx,ny,nz)*1e-5
     T = torch.tensor(EDT).unsqueeze(0)
     kernel_size = min_distance
     padding = kernel_size//2
     F = torch.nn.MaxPool3d((kernel_size,kernel_size,kernel_size), stride=(1,1,1), padding=padding, dilation=1, return_indices=False, ceil_mode=False)
 
     minpooled = F(-T)[0].numpy()
@@ -161,15 +162,14 @@
     t5 = time()
     if prints : print("Triangulation build in ",np.round(t5-t4,2))
     
     return(seeds_coords,seeds_indices, tesselation,Total_EDT)
 
 
 
-
 def build_triangulation_skimage(labels,min_distance=5,prints=False):
     if prints : 
         print("Mode == Skimage")
         print("min_distance =",min_distance)
         print("Computing EDT ...")
     t1 = time()
 
@@ -201,14 +201,15 @@
     seeds_indices = values_lbls
 
     corners = give_corners(Total_EDT)
     
     
     t3 = time()
     if prints : print("Searching local extremas ...")
+    np.random.seed(42)
     EDT = Total_EDT + np.random.rand(nx,ny,nz)*1e-5
     
     local_mins = peak_local_max(-EDT,min_distance=min_distance,exclude_border=False)
     if prints : print("Number of local minimas :",len(local_mins))
 
     local_maxes = peak_local_max(EDT,min_distance=min_distance,exclude_border=False)
     if prints : print("Number of local maxes :",len(local_maxes))
```

### Comparing `delaunay_watershed_3d-0.2.4/src/dw3d/Geometry.py` & `delaunay_watershed_3d-0.2.5/src/dw3d/Geometry.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.4/src/dw3d/Graph_functions.py` & `delaunay_watershed_3d-0.2.5/src/dw3d/Graph_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.4/src/dw3d/Mask_reconstruction.py` & `delaunay_watershed_3d-0.2.5/src/dw3d/Mask_reconstruction.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.4/src/dw3d/Mesh_utilities.py` & `delaunay_watershed_3d-0.2.5/src/dw3d/Mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.4/src/dw3d/Networkx_functions.py` & `delaunay_watershed_3d-0.2.5/src/dw3d/Networkx_functions.py`

 * *Files identical despite different names*

### Comparing `delaunay_watershed_3d-0.2.4/src/dw3d/functions.py` & `delaunay_watershed_3d-0.2.5/src/dw3d/functions.py`

 * *Files identical despite different names*

