# Comparing `tmp/orr_sommerfeld_convmix_cgb-0.2.7.tar.gz` & `tmp/orr_sommerfeld_convmix_cgb-0.2.8.tar.gz`

## Comparing `orr_sommerfeld_convmix_cgb-0.2.7.tar` & `orr_sommerfeld_convmix_cgb-0.2.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.7/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.7/src/Orr_Sommerfeld_convmix_CGB/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.7/LICENSE
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.7/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/src/Orr_Sommerfeld_convmix_CGB/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/LICENSE
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 orr_sommerfeld_convmix_cgb-0.2.8/PKG-INFO
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.7/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py` & `orr_sommerfeld_convmix_cgb-0.2.8/src/Orr_Sommerfeld_convmix_CGB/OS_CM.py`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.2.7/LICENSE` & `orr_sommerfeld_convmix_cgb-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `orr_sommerfeld_convmix_cgb-0.2.7/README.md` & `orr_sommerfeld_convmix_cgb-0.2.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Orr-Sommerfeld-convmix-CGB Package
 It is a python package developed in order to solve the Orr Sommerfeld equations. It is free for the community and allows to calculate disturbances for one flow of interest: Mixed convection in vertical rectangular channels like the following one: 
 
 <p align="center">
   <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/Canal.png" alt="Descripción de la imagen" width="300px">
 </p>
 
+[Link to channel description image on Gitlab repository](https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/Canal.png)
+
 The perturbations can be used to analyze the phenomenon of the laminar-turbulent transition. 
 
 ## Table of contents
 * [General info](#general-info)
 * [Technologies](#technologies)
 * [Installation](#installation)
 * [Examples](#examples)
@@ -27,17 +29,20 @@
 * [Plotly](https://plotly.com/)
 * [Pandas](https://pandas.pydata.org/)
 * [PyPi](https://pypi.org/) to publish Python package.
 
 In the next figure, it is shown the flux diagram of the main function: Orr-Sommerfeld
 
 <p align="center">
-  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/Funciones.png" alt="Descripción de la imagen" width="300px">
+  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/Funciones.png" alt="Flux Diagram" width="300px">
 </p>
 
+[Link to flux diagram image on Gitlab repository](https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/Funciones.png)
+
+
 ## Installation
 It is possible to install using pip:
 ```Python
 pip install Orr-Sommerfeld-convmix-CGB
 ```
 ## Examples
 * Importing the package:
@@ -69,23 +74,29 @@
 * Additionally, there is a function that plots the eigenvalues using the matplotlib library. The package also includes an interactive plot of the eigenvalues using pandas
 ```Python
 OS_CM.grafica_autovalores(N,Ra,Pr,Re,alpha,beta)
 ```
 The result is for example:
 
 <p align="center">
-  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/ejautovalores1.png" alt="Descripción de la imagen" width="300px">
+  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/ejautovalores1.png" alt="Eigenvalues example" width="300px">
 </p>
 
+[Link to eigenvalues image on Gitlab repository](https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/ejautovalores1.png)
+
 <p align="center">
-  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/ejemploautovalores.png" alt="Descripción de la imagen" width="600px">
+  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/ejemploautovalores.png" alt="Interactive eigenvalues plot example" width="600px">
 </p>
 
 [Video showing interactive plot](https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/output_video.webm)
 * Eigenvectors can also be plotted using the previously mentioned normalization:
+```Python
 OS_CM.grafica_autofunciones(N,Ra,Pr,Re,alpha,beta)
+```
 
 The result is something like this:
 
 <p align="center">
-  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/autofunciongod.png" alt="Descripción de la imagen" width="300px">
+  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/autofunciongod.png" alt="Eigenvectors plot example" width="300px">
 </p>
+
+[Link to eigenvectors image on Gitlab repository](https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/autofunciongod.png)
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.7/pyproject.toml` & `orr_sommerfeld_convmix_cgb-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "Orr_Sommerfeld_convmix_CGB"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="Pablo Szuban", email="pablo.szuban@ib.edu.ar" },
 ]
 description = "Paquete para cálculo de autovalores y autofunciones."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `orr_sommerfeld_convmix_cgb-0.2.7/PKG-INFO` & `orr_sommerfeld_convmix_cgb-0.2.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orr_Sommerfeld_convmix_CGB
-Version: 0.2.7
+Version: 0.2.8
 Summary: Paquete para cálculo de autovalores y autofunciones.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Project-URL: Source Code, https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb
 Author-email: Pablo Szuban <pablo.szuban@ib.edu.ar>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,16 @@
 # Orr-Sommerfeld-convmix-CGB Package
 It is a python package developed in order to solve the Orr Sommerfeld equations. It is free for the community and allows to calculate disturbances for one flow of interest: Mixed convection in vertical rectangular channels like the following one: 
 
 <p align="center">
   <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/Canal.png" alt="Descripción de la imagen" width="300px">
 </p>
 
+[Link to channel description image on Gitlab repository](https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/Canal.png)
+
 The perturbations can be used to analyze the phenomenon of the laminar-turbulent transition. 
 
 ## Table of contents
 * [General info](#general-info)
 * [Technologies](#technologies)
 * [Installation](#installation)
 * [Examples](#examples)
@@ -42,17 +44,20 @@
 * [Plotly](https://plotly.com/)
 * [Pandas](https://pandas.pydata.org/)
 * [PyPi](https://pypi.org/) to publish Python package.
 
 In the next figure, it is shown the flux diagram of the main function: Orr-Sommerfeld
 
 <p align="center">
-  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/Funciones.png" alt="Descripción de la imagen" width="300px">
+  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/Funciones.png" alt="Flux Diagram" width="300px">
 </p>
 
+[Link to flux diagram image on Gitlab repository](https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/Funciones.png)
+
+
 ## Installation
 It is possible to install using pip:
 ```Python
 pip install Orr-Sommerfeld-convmix-CGB
 ```
 ## Examples
 * Importing the package:
@@ -84,23 +89,29 @@
 * Additionally, there is a function that plots the eigenvalues using the matplotlib library. The package also includes an interactive plot of the eigenvalues using pandas
 ```Python
 OS_CM.grafica_autovalores(N,Ra,Pr,Re,alpha,beta)
 ```
 The result is for example:
 
 <p align="center">
-  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/ejautovalores1.png" alt="Descripción de la imagen" width="300px">
+  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/ejautovalores1.png" alt="Eigenvalues example" width="300px">
 </p>
 
+[Link to eigenvalues image on Gitlab repository](https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/ejautovalores1.png)
+
 <p align="center">
-  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/ejemploautovalores.png" alt="Descripción de la imagen" width="600px">
+  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/ejemploautovalores.png" alt="Interactive eigenvalues plot example" width="600px">
 </p>
 
 [Video showing interactive plot](https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/output_video.webm)
 * Eigenvectors can also be plotted using the previously mentioned normalization:
+```Python
 OS_CM.grafica_autofunciones(N,Ra,Pr,Re,alpha,beta)
+```
 
 The result is something like this:
 
 <p align="center">
-  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/autofunciongod.png" alt="Descripción de la imagen" width="300px">
+  <img src="https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/autofunciongod.png" alt="Eigenvectors plot example" width="300px">
 </p>
+
+[Link to eigenvectors image on Gitlab repository](https://gitlab.com/mecom-cnea-os/orr-sommerfeld-convmix-cgb/-/raw/main/Examples/autofunciongod.png)
```

