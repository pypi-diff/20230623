# Comparing `tmp/foambryo-0.2.5.tar.gz` & `tmp/foambryo-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-c0f11wrk/foambryo-0.2.5.tar", last modified: Fri Jun 23 13:54:25 2023, max compression
+gzip compressed data, was "/Users/sachaichbiah/Documents/PHD/Gitlab/pip_libraries/foambryo/dist/.tmp-ix2twqku/foambryo-0.2.6.tar", last modified: Fri Jun 23 14:05:56 2023, max compression
```

## Comparing `foambryo-0.2.5.tar` & `foambryo-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:54:25.452247 foambryo-0.2.5/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11270 2023-06-23 13:54:25.452469 foambryo-0.2.5/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10640 2023-06-23 13:48:40.000000 foambryo-0.2.5/README.md
--rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:21:07.000000 foambryo-0.2.5/pyproject.toml
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      905 2023-06-23 13:54:25.453207 foambryo-0.2.5/setup.cfg
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:54:25.445184 foambryo-0.2.5/src/
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:54:25.449376 foambryo-0.2.5/src/foambryo/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    25142 2023-06-23 13:32:33.000000 foambryo-0.2.5/src/foambryo/Force_viewer.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/Inference_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/Mesh_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    10498 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/Plotting_utilities.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)     8921 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/Pressure_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/Tension_inference.py
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-06-23 13:21:07.000000 foambryo-0.2.5/src/foambryo/__init__.py
-drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 13:54:25.451926 foambryo-0.2.5/src/foambryo.egg-info/
--rw-r--r--   0 sachaichbiah   (503) staff       (20)    11270 2023-06-23 13:54:25.000000 foambryo-0.2.5/src/foambryo.egg-info/PKG-INFO
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-06-23 13:54:25.000000 foambryo-0.2.5/src/foambryo.egg-info/SOURCES.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-06-23 13:54:25.000000 foambryo-0.2.5/src/foambryo.egg-info/dependency_links.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-06-23 13:54:25.000000 foambryo-0.2.5/src/foambryo.egg-info/requires.txt
--rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-06-23 13:54:25.000000 foambryo-0.2.5/src/foambryo.egg-info/top_level.txt
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 14:05:56.112203 foambryo-0.2.6/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11270 2023-06-23 14:05:56.112351 foambryo-0.2.6/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10640 2023-06-23 13:48:40.000000 foambryo-0.2.6/README.md
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)       84 2023-06-23 13:21:07.000000 foambryo-0.2.6/pyproject.toml
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      905 2023-06-23 14:05:56.113259 foambryo-0.2.6/setup.cfg
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 14:05:56.095753 foambryo-0.2.6/src/
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 14:05:56.102244 foambryo-0.2.6/src/foambryo/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    25160 2023-06-23 13:57:19.000000 foambryo-0.2.6/src/foambryo/Force_viewer.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     4235 2023-06-23 13:21:07.000000 foambryo-0.2.6/src/foambryo/Inference_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     9713 2023-06-23 13:21:07.000000 foambryo-0.2.6/src/foambryo/Mesh_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    10498 2023-06-23 13:21:07.000000 foambryo-0.2.6/src/foambryo/Plotting_utilities.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)     8843 2023-06-23 14:01:15.000000 foambryo-0.2.6/src/foambryo/Pressure_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    28964 2023-06-23 13:21:07.000000 foambryo-0.2.6/src/foambryo/Tension_inference.py
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      223 2023-06-23 13:21:07.000000 foambryo-0.2.6/src/foambryo/__init__.py
+drwxr-xr-x   0 sachaichbiah   (503) staff       (20)        0 2023-06-23 14:05:56.111679 foambryo-0.2.6/src/foambryo.egg-info/
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)    11270 2023-06-23 14:05:56.000000 foambryo-0.2.6/src/foambryo.egg-info/PKG-INFO
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      438 2023-06-23 14:05:56.000000 foambryo-0.2.6/src/foambryo.egg-info/SOURCES.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        1 2023-06-23 14:05:56.000000 foambryo-0.2.6/src/foambryo.egg-info/dependency_links.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)      107 2023-06-23 14:05:56.000000 foambryo-0.2.6/src/foambryo.egg-info/requires.txt
+-rw-r--r--   0 sachaichbiah   (503) staff       (20)        9 2023-06-23 14:05:56.000000 foambryo-0.2.6/src/foambryo.egg-info/top_level.txt
```

### Comparing `foambryo-0.2.5/PKG-INFO` & `foambryo-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.2.5
+Version: 0.2.6
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `foambryo-0.2.5/README.md` & `foambryo-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.5/setup.cfg` & `foambryo-0.2.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = foambryo
-version = 0.2.5
+version = 0.2.6
 author = Sacha Ichbiah
 author_email = sacha.ichbiah@college-de-france.fr
 description = Tension inference for 3D cell assemblies
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sacha-ichbiah/foambryo
 project_urls =
```

### Comparing `foambryo-0.2.5/src/foambryo/Force_viewer.py` & `foambryo-0.2.6/src/foambryo/Force_viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from numpy.linalg import eig
 import networkx as nx
 from .Tension_inference import infer_forces, infer_tension, infer_pressure, compute_residual_junctions_dict
 
 from dw3d.Dcel import compute_faces_areas,compute_normal_Faces, update_graph_with_scattered_values
-from dw3d.Curvature import compute_curvature_vertices_robust_laplacian, compute_gaussian_curvature_vertices, compute_curvature_vertices_cotan,compute_sphere_fit_residues_dict
+from dw3d.Curvature import compute_gaussian_curvature_vertices, compute_curvature_vertices_cotan,compute_sphere_fit_residues_dict
 
 from .Plotting_utilities import *
 
 def plot_force_inference(Mesh,dict_tensions = None, dict_pressure = None,alpha = 0.05, scalar_quantities = False,scattered = False,scatter_coeff=0.2):
     
     if dict_tensions == None : 
         dict_tensions,dict_pressure = infer_forces(Mesh)
@@ -200,25 +200,15 @@
     print("Extremas of volume derivatives plotted: ",vmin,vmax)
     Derivatives_verts = Derivatives_verts.clip(vmin,vmax)
     
     ps_mesh = view_vertex_values_on_embryo(Mesh,Derivatives_verts,ps_mesh = ps_mesh, name_values = "Volume Derivatives",remove_trijunctions=remove_trijunctions,clean_before = clean_before, clean_after = clean_after,show=show, scattered = scattered)
     
     return(ps_mesh)
 
-def view_mean_curvature_robust(Mesh,alpha = 0.05,ps_mesh = None, remove_trijunctions=True,clean_before = True, clean_after = True,show=True,scattered = False):
-    
-    H,_,_=compute_curvature_vertices_robust_laplacian(Mesh)
-    
-    vmin, vmax = np.quantile(H,alpha),np.quantile(H,1-alpha)
-    print("Extremas of mean curvature (robust) plotted: ",vmin,vmax)
-    H = H.clip(vmin,vmax)
 
-    ps_mesh = view_vertex_values_on_embryo(Mesh,H,ps_mesh = ps_mesh,name_values="Mean Curvature Robust",remove_trijunctions=remove_trijunctions,clean_before = clean_before, clean_after = clean_after,show=show, scattered = scattered)
-        
-    return(ps_mesh)
 
 
 def view_mean_curvature_cotan(Mesh,alpha = 0.05,ps_mesh = None, remove_trijunctions=True,clean_before = True, clean_after = True,show=True,scattered = False):
     
     H,_,_=compute_curvature_vertices_cotan(Mesh)
     
     vmin, vmax = np.quantile(H,alpha),np.quantile(H,1-alpha)
@@ -241,15 +231,15 @@
         
     return(ps_mesh)
 
 
 
 def view_discrepancy_of_principal_curvatures(Mesh,alpha = 0.05,ps_mesh = None, remove_trijunctions=True,clean_before = True, clean_after = True,show=True,scattered = False):
     
-    H,_,_=compute_curvature_vertices_robust_laplacian(Mesh)
+    H,_,_=compute_curvature_vertices_cotan(Mesh)
     H/=9
     H[H==0]=np.mean(H)
     
     G = compute_gaussian_curvature_vertices(Mesh)
     Kdiff =  np.abs((H**2-G)/(H**2))
 
     vmin, vmax = np.quantile(Kdiff,alpha),np.quantile(Kdiff,1-alpha)
@@ -581,8 +571,22 @@
         view_mean_curvature_cotan(Mesh, alpha = alpha,ps_mesh = ps_mesh, clean_before = False, clean_after = False,show=False)
         view_mean_curvature_robust(Mesh, alpha = alpha,ps_mesh = ps_mesh, clean_before = False, clean_after = False,show=False)
         view_gaussian_curvature(Mesh, alpha = alpha,ps_mesh = ps_mesh, clean_before = False, clean_after = False,show=False)
         view_discrepancy_of_principal_curvatures(Mesh, alpha = alpha,ps_mesh = ps_mesh, clean_before = False, clean_after = False,show=False)
 
     ps.show()
 
+from dw3d.Curvature import compute_curvature_vertices_robust_laplacian
+
+def view_mean_curvature_robust(Mesh,alpha = 0.05,ps_mesh = None, remove_trijunctions=True,clean_before = True, clean_after = True,show=True,scattered = False):
+    
+    H,_,_=compute_curvature_vertices_robust_laplacian(Mesh)
+    
+    vmin, vmax = np.quantile(H,alpha),np.quantile(H,1-alpha)
+    print("Extremas of mean curvature (robust) plotted: ",vmin,vmax)
+    H = H.clip(vmin,vmax)
+
+    ps_mesh = view_vertex_values_on_embryo(Mesh,H,ps_mesh = ps_mesh,name_values="Mean Curvature Robust",remove_trijunctions=remove_trijunctions,clean_before = clean_before, clean_after = clean_after,show=show, scattered = scattered)
+        
+    return(ps_mesh)
+
 """
```

### Comparing `foambryo-0.2.5/src/foambryo/Inference_utilities.py` & `foambryo-0.2.6/src/foambryo/Inference_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.5/src/foambryo/Mesh_utilities.py` & `foambryo-0.2.6/src/foambryo/Mesh_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.5/src/foambryo/Plotting_utilities.py` & `foambryo-0.2.6/src/foambryo/Plotting_utilities.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.5/src/foambryo/Pressure_inference.py` & `foambryo-0.2.6/src/foambryo/Pressure_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     new_faces = faces.copy()
     for key in mapping : 
         new_faces[faces[:,3]==key][:,3]=mapping[key]
         new_faces[faces[:,4]==key][:,4]=mapping[key]
     return(new_faces)
 
 
-def infer_pressure_laplace(Mesh,dict_tensions,P0=0,laplacian="robust",weighted=False):
+def infer_pressure_laplace(Mesh,dict_tensions,P0=0,weighted=False):
     dict_areas = Mesh.compute_areas_interfaces()
-    dict_curvature = Mesh.compute_curvatures_interfaces(laplacian=laplacian,weighted=weighted)
+    dict_curvature = Mesh.compute_curvatures_interfaces(weighted=weighted)
     
     M,B = build_matrix_laplace(dict_curvature,dict_areas,dict_tensions,Mesh.n_materials,Mesh.materials,P0)
     x, resid, rank, sigma = linalg.lstsq(M, B)
     
     nc = Mesh.n_materials
     
     dict_pressures = {0:P0}
@@ -56,17 +56,17 @@
     P=np.linalg.inv(G_p)@G_g@x
         
     for i,key in enumerate(Mesh.materials[1:]): 
         dict_pressures[key]=P[i]+P0
     
     return(x,dict_pressures,0)
 
-def infer_pressure(Mesh,dict_tensions,mode='Variational',P0=0,laplacian="robust",weighted=False):
+def infer_pressure(Mesh,dict_tensions,mode='Variational',P0=0,weighted=False):
     if mode =="Laplace":
-        return(infer_pressure_laplace(Mesh,dict_tensions,P0,laplacian=laplacian,weighted=weighted))
+        return(infer_pressure_laplace(Mesh,dict_tensions,P0,weighted=weighted))
     elif mode =='Variational': 
         return(infer_pressure_variational(Mesh,dict_tensions,P0))
     else : 
         print("Unimplemented method")
         return(None)
```

### Comparing `foambryo-0.2.5/src/foambryo/Tension_inference.py` & `foambryo-0.2.6/src/foambryo/Tension_inference.py`

 * *Files identical despite different names*

### Comparing `foambryo-0.2.5/src/foambryo.egg-info/PKG-INFO` & `foambryo-0.2.6/src/foambryo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foambryo
-Version: 0.2.5
+Version: 0.2.6
 Summary: Tension inference for 3D cell assemblies
 Home-page: https://github.com/sacha-ichbiah/foambryo
 Author: Sacha Ichbiah
 Author-email: sacha.ichbiah@college-de-france.fr
 Project-URL: Team website, https://www.turlierlab.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

