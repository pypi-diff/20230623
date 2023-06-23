# Comparing `tmp/hipersim-0.0.7.tar.gz` & `tmp/hipersim-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nkdi\Documents\Programs\HiperSim\release\dist\tmprwccvs3n\hipersim-0.0.7.tar", last modified: Tue Jun 22 12:27:51 2021, max compression
+gzip compressed data, was "C:\Users\nkdi\Documents\Programs\HiperSim\release\dist\tmpwr9yd463\hipersim-0.0.9.tar", last modified: Tue Aug 31 20:32:42 2021, max compression
```

## Comparing `hipersim-0.0.7.tar` & `hipersim-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2021-06-22 12:27:51.620064 hipersim-0.0.7/
--rw-rw-rw-   0        0        0     1086 2021-06-22 12:13:11.000000 hipersim-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1182 2021-06-22 12:27:51.620064 hipersim-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      676 2021-06-22 12:13:11.000000 hipersim-0.0.7/README.md
--rw-rw-rw-   0        0        0      108 2021-06-22 09:04:30.000000 hipersim-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      627 2021-06-22 12:27:51.620064 hipersim-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-06-22 12:27:51.588813 hipersim-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2021-06-22 12:27:51.588813 hipersim-0.0.7/src/hipersim/
--rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.0.7/src/hipersim/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-22 12:27:51.604439 hipersim-0.0.7/src/hipersim/surrogates/
--rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.0.7/src/hipersim/surrogates/__init__.py
--rw-rw-rw-   0        0        0     1021 2019-06-27 09:54:53.000000 hipersim-0.0.7/src/hipersim/surrogates/math_utils.py
--rw-rw-rw-   0        0        0    20937 2021-06-22 12:25:11.000000 hipersim-0.0.7/src/hipersim/surrogates/neuralnets.py
-drwxrwxrwx   0        0        0        0 2021-06-22 12:27:51.620064 hipersim-0.0.7/src/hipersim/turbgen/
--rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.0.7/src/hipersim/turbgen/__init__.py
--rw-rw-rw-   0        0        0    21554 2021-06-22 11:53:52.000000 hipersim-0.0.7/src/hipersim/turbgen/constrain_field.py
--rw-rw-rw-   0        0        0    22981 2021-06-22 11:54:06.000000 hipersim-0.0.7/src/hipersim/turbgen/generate_field.py
--rw-rw-rw-   0        0        0    25078 2021-05-04 20:59:21.000000 hipersim-0.0.7/src/hipersim/turbgen/manntensor.py
--rw-rw-rw-   0        0        0      506 2021-04-24 13:31:48.000000 hipersim-0.0.7/src/hipersim/turbgen/trapezoidal_sum_2d.py
--rw-rw-rw-   0        0        0     4881 2021-06-22 11:53:22.000000 hipersim-0.0.7/src/hipersim/turbgen/turbgen.py
-drwxrwxrwx   0        0        0        0 2021-06-22 12:27:51.604439 hipersim-0.0.7/src/hipersim.egg-info/
--rw-rw-rw-   0        0        0     1182 2021-06-22 12:27:51.000000 hipersim-0.0.7/src/hipersim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2021-06-22 12:27:51.000000 hipersim-0.0.7/src/hipersim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-22 12:27:51.000000 hipersim-0.0.7/src/hipersim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-06-22 12:27:51.000000 hipersim-0.0.7/src/hipersim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.793787 hipersim-0.0.9/
+-rw-rw-rw-   0        0        0     1086 2021-06-22 12:13:11.000000 hipersim-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1338 2021-08-31 20:32:42.794891 hipersim-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2021-08-17 12:41:20.000000 hipersim-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-06-22 09:04:30.000000 hipersim-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      627 2021-08-31 20:32:42.798486 hipersim-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.700692 hipersim-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.726117 hipersim-0.0.9/src/hipersim/
+-rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.0.9/src/hipersim/__init__.py
+drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.755273 hipersim-0.0.9/src/hipersim/surrogates/
+-rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.0.9/src/hipersim/surrogates/__init__.py
+-rw-rw-rw-   0        0        0     1021 2019-06-27 09:54:53.000000 hipersim-0.0.9/src/hipersim/surrogates/math_utils.py
+-rw-rw-rw-   0        0        0    20937 2021-06-22 12:25:11.000000 hipersim-0.0.9/src/hipersim/surrogates/neuralnets.py
+drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.789793 hipersim-0.0.9/src/hipersim/turbgen/
+-rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.0.9/src/hipersim/turbgen/__init__.py
+-rw-rw-rw-   0        0        0    19832 2021-08-30 09:46:31.000000 hipersim-0.0.9/src/hipersim/turbgen/constrain_field.py
+-rw-rw-rw-   0        0        0    17792 2021-08-31 11:49:44.000000 hipersim-0.0.9/src/hipersim/turbgen/constrain_field_1d.py
+-rw-rw-rw-   0        0        0    22981 2021-06-22 11:54:06.000000 hipersim-0.0.9/src/hipersim/turbgen/generate_field.py
+-rw-rw-rw-   0        0        0    25078 2021-05-04 20:59:21.000000 hipersim-0.0.9/src/hipersim/turbgen/manntensor.py
+-rw-rw-rw-   0        0        0      632 2021-08-30 10:02:04.000000 hipersim-0.0.9/src/hipersim/turbgen/trapezoidal_sum_2d.py
+-rw-rw-rw-   0        0        0     6705 2021-08-31 20:27:40.000000 hipersim-0.0.9/src/hipersim/turbgen/turbgen.py
+drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.742720 hipersim-0.0.9/src/hipersim.egg-info/
+-rw-rw-rw-   0        0        0     1338 2021-08-31 20:32:42.000000 hipersim-0.0.9/src/hipersim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2021-08-31 20:32:42.000000 hipersim-0.0.9/src/hipersim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-08-31 20:32:42.000000 hipersim-0.0.9/src/hipersim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2021-08-31 20:32:42.000000 hipersim-0.0.9/src/hipersim.egg-info/top_level.txt
```

### Comparing `hipersim-0.0.7/LICENSE` & `hipersim-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hipersim-0.0.7/PKG-INFO` & `hipersim-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hipersim
-Version: 0.0.7
+Version: 0.0.9
 Summary: A collection of wind energy simulation tools
 Home-page: https://gitlab.windenergy.dtu.dk/HiperSim/hipersim
 Author: Nikolay Dimitrov
 Author-email: nkdi@dtu.dk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,18 @@
 - **turbgen**: 
     - Generation of 3D frozen turbulence fields ("turbulence boxes") with the Mann turbulence spectrum
     - Constrained turbulence field generation and application of constraints on pre-generated turbulence fields
 
 - **surrogates**:
     - A feedforward neural network toolbox, training and evaluation of feedforward neural networks. 
 
+## Installation
+Hipersim is registered as installable Python package in PyPi.org. Installation happens automatically with the following command:
+
+pip install hipersim
+
 ## References
 
 ## License
 Hipersim uses the MIT License.
-## Installation
```

### Comparing `hipersim-0.0.7/README.md` & `hipersim-0.0.9/src/hipersim.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,39 @@
+Metadata-Version: 2.1
+Name: hipersim
+Version: 0.0.9
+Summary: A collection of wind energy simulation tools
+Home-page: https://gitlab.windenergy.dtu.dk/HiperSim/hipersim
+Author: Nikolay Dimitrov
+Author-email: nkdi@dtu.dk
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Hipersim
 
 ## Introduction
 Hipersim is a collection of tools for computationally-efficient simulation of Wind Energy problems using statistical and machine learning methods. Currently, the package contains the following submodules:
 
 - **turbgen**: 
     - Generation of 3D frozen turbulence fields ("turbulence boxes") with the Mann turbulence spectrum
     - Constrained turbulence field generation and application of constraints on pre-generated turbulence fields
 
 - **surrogates**:
     - A feedforward neural network toolbox, training and evaluation of feedforward neural networks. 
 
+## Installation
+Hipersim is registered as installable Python package in PyPi.org. Installation happens automatically with the following command:
+
+pip install hipersim
+
 ## References
 
 ## License
 Hipersim uses the MIT License.
-## Installation
+
+
```

### Comparing `hipersim-0.0.7/setup.cfg` & `hipersim-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 6970 6572 7369 6d0d 0a76 6572   = hipersim..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e37 0d0a 6175  sion = 0.0.7..au
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 6175  sion = 0.0.9..au
 00000030: 7468 6f72 203d 204e 696b 6f6c 6179 2044  thor = Nikolay D
 00000040: 696d 6974 726f 760d 0a61 7574 686f 725f  imitrov..author_
 00000050: 656d 6169 6c20 3d20 6e6b 6469 4064 7475  email = nkdi@dtu
 00000060: 2e64 6b0d 0a64 6573 6372 6970 7469 6f6e  .dk..description
 00000070: 203d 2041 2063 6f6c 6c65 6374 696f 6e20   = A collection 
 00000080: 6f66 2077 696e 6420 656e 6572 6779 2073  of wind energy s
 00000090: 696d 756c 6174 696f 6e20 746f 6f6c 730d  imulation tools.
```

### Comparing `hipersim-0.0.7/src/hipersim/surrogates/math_utils.py` & `hipersim-0.0.9/src/hipersim/surrogates/math_utils.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.0.7/src/hipersim/surrogates/neuralnets.py` & `hipersim-0.0.9/src/hipersim/surrogates/neuralnets.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.0.7/src/hipersim/turbgen/constrain_field.py` & `hipersim-0.0.9/src/hipersim/turbgen/constrain_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 @author: nkdi
 """
 
 def constrain_field(Constraints,u = None,v = None,w = None, BaseName = 'Turb', \
                         alphaepsilon = 1,L = 30,Gamma = 3, Nx = 8192, Ny = 32, Nz = 32, \
                         dx = 1,dy = 1,dz = 1,SaveToFile = 0, UseNormalization = 0, TurbOptions = None):
+
+    import numpy as np
+    import time
+
     '''
     Parse inputs 
     '''
     
     if TurbOptions is None:
         SeedNo = 0
         HighFreqComp = 0
@@ -33,20 +37,23 @@
             '''
             ======================================================================================
             If not given as inputs, load turbulence boxes from files or generate them if necessary
             ======================================================================================'''
             from hipersim.turbgen.generate_field import generate_field 
             u,v,w = generate_field(BaseName,alphaepsilon,L,Gamma,SeedNo,Nx,Ny,Nz,dx,dy,dz, \
                                     HighFreqComp, SaveToFile = 0)
+        else:
             '''
             Load source turbulence boxes 
             '''
+            u = np.fromfile(TurbOptions['Udatafile'],dtype = 'single').reshape((Nx,Ny,Nz))
+            v = np.fromfile(TurbOptions['Udatafile'],dtype = 'single').reshape((Nx,Ny,Nz))
+            w = np.fromfile(TurbOptions['Udatafile'],dtype = 'single').reshape((Nx,Ny,Nz))
+            
 
-    import numpy as np
-    import time
     # from generate_field import generate_field
     # Nx = 1024
     # Ny = 32
     # Nz = 32
     # dx = 2
     # dy = 4
     # dz = 4
@@ -72,60 +79,15 @@
     # Constraints = np.concatenate([np.concatenate([Xconstraints, Xconstraints]), 
     #                               np.concatenate([Yconstraints1, Yconstraints2]),
     #                               np.concatenate([Zconstraints1, Zconstraints2]),
     #                               np.concatenate([Uconstraints, -Uconstraints]),
     #                               np.concatenate([Vconstraints, -Vconstraints]),
     #                               np.concatenate([Wconstraints, -Wconstraints])],axis = 1)
         
-    # % If not given as inputs, load turbulence boxes from files or generate them if necessary
-    
-    # if ~exist('u','var') || ~exist('v','var') || ~exist('w','var')
-    #     if ~isfield(Input,'Udatafile') || ~isfield(Input,'Vdatafile') || ~isfield(Input,'Wdatafile')
-    #         disp('Source turbulence boxes are not specified for all components to be constrained. Generating turbulence boxes instead.');
-    #         [u,v,w] = MannGenerator(Input,Options);
-    #     else
-    #         disp('Loading turbulence boxes..');
-    #         Ufile = fopen(Input.Udatafile);
-    #         Udata = fread(Ufile,'single');
-    #         fclose(Ufile);
-    #         u = zeros(Nx,Ny,Nz);
-    #         for xloc = 1:Nx
-    #             for yloc = 1:Ny
-    #                 dataindex = Ny*Nz*(xloc - 1) + Ny*(yloc-1);
-    #                 UperZ = Udata(dataindex+1:dataindex+Nz);
-    #                 u(xloc,yloc,:) = UperZ;
-    #             end
-    #         end
-    #         clear Udata;     
-    #         Vfile = fopen(Input.Vdatafile);
-    #         Vdata = fread(Vfile,'single');
-    #         fclose(Vfile);
-    #         v = zeros(Nx,Ny,Nz);                  
-    #         for xloc = 1:Nx
-    #             for yloc = 1:Ny
-    #                 dataindex = Ny*Nz*(xloc - 1) + Ny*(yloc-1);
-    #                 VperZ = Vdata(dataindex+1:dataindex+Nz);
-    #                 v(xloc,yloc,:) = VperZ;
-    #             end
-    #         end
-    #         clear Vdata;   
-    #         Wfile = fopen(Wdatafile);
-    #         Wdata = fread(Wfile,'single');
-    #         fclose(Wfile);                   
-    #         w = zeros(Nx,Ny,Nz);
-    #         for xloc = 1:Nx
-    #             for yloc = 1:Ny
-    #                 dataindex = Ny*Nz*(xloc - 1) + Ny*(yloc-1);
-    #                 WperZ = Wdata(dataindex+1:dataindex+Nz);
-    #                 w(xloc,yloc,:) = WperZ;
-    #             end
-    #         end        
-    #         clear Wdata;  
-    #     end
-    # end
+
     
     ''' 
     ===============================================
     APPLY CONSTRAINTS
     ==============================================='''
     
     '''
```

### Comparing `hipersim-0.0.7/src/hipersim/turbgen/generate_field.py` & `hipersim-0.0.9/src/hipersim/turbgen/generate_field.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.0.7/src/hipersim/turbgen/manntensor.py` & `hipersim-0.0.9/src/hipersim/turbgen/manntensor.py`

 * *Files identical despite different names*

### Comparing `hipersim-0.0.7/src/hipersim/turbgen/turbgen.py` & `hipersim-0.0.9/src/hipersim/turbgen/turbgen.py`

 * *Files 20% similar despite different names*

```diff
@@ -79,44 +79,78 @@
         self.u = u
         self.v = v
         self.w = w
         
         
         return u, v, w
     
-    def constrain(self, Constraints = None):
+    def constrain(self, Constraints = None, Component = None, TurbOptions = None):
         if Constraints is None:
             Constraints = self.Constraints
         else:
             self.Constraints = Constraints
+        if TurbOptions is None:
+            TurbOptions = {
+                    'HighFreqComp': self.params['HighFreqComp'],
+                    'SeedNo': self.params['SeedNo']}
+                    
+        if Component is None:
+            from hipersim.turbgen.constrain_field import constrain_field
+
+            
+            if ((hasattr(self,'u')==False) | (hasattr(self,'v') == False) | (hasattr(self,'w') == False)):
+                self.generate()
+            u, v, w = constrain_field(Constraints,
+                                      self.u,
+                                      self.v,
+                                      self.w,
+                                      BaseName = self.params['BaseName'],
+                                      alphaepsilon = self.params['alphaepsilon'],
+                                      L = self.params['L'],
+                                      Gamma = self.params['Gamma'],
+                                      Nx = self.params['Nx'], 
+                                      Ny = self.params['Ny'],
+                                      Nz = self.params['Nz'],
+                                      dx = self.params['dx'],
+                                      dy = self.params['dy'],
+                                      dz = self.params['dz'],
+                                      SaveToFile = self.params['SaveToFile'],
+                                      UseNormalization = 0,
+                                      TurbOptions = TurbOptions)
+            self.u = u
+            self.v = v
+            self.w = w
+            
             
-        from hipersim.turbgen.constrain_field import constrain_field
+            return u, v, w    
+        else:
+            from hipersim.turbgen.constrain_field_1d import constrain_field_1d
 
-        TurbOptions = {
-                        'HighFreqComp': self.params['HighFreqComp'],
-                        'SeedNo': self.params['SeedNo']}
-        
-        if ((hasattr(self,'u')==False) | (hasattr(self,'v') == False) | (hasattr(self,'w') == False)):
-            self.generate()
-        u, v, w = constrain_field(Constraints,
-                                  self.u,
-                                  self.v,
-                                  self.w,
-                                  BaseName = self.params['BaseName'],
-                                  alphaepsilon = self.params['alphaepsilon'],
-                                  L = self.params['L'],
-                                  Gamma = self.params['Gamma'],
-                                  Nx = self.params['Nx'], 
-                                  Ny = self.params['Ny'],
-                                  Nz = self.params['Nz'],
-                                  dx = self.params['dx'],
-                                  dy = self.params['dy'],
-                                  dz = self.params['dz'],
-                                  SaveToFile = self.params['SaveToFile'],
-                                  UseNormalization = 0,
-                                  TurbOptions = TurbOptions)
-        self.u = u
-        self.v = v
-        self.w = w
-        
-        
-        return u, v, w    
+            if (((Component == 'u') & (hasattr(self,'u')==False)) | ((Component == 'v') & (hasattr(self,'v')==False)) | ((Component == 'w') & (hasattr(self,'w')==False))):
+                self.generate()
+            c = constrain_field_1d(Component, 
+                                   Constraints,
+                                   self.u,
+                                   self.v,
+                                   self.w,
+                                   BaseName = self.params['BaseName'],
+                                   alphaepsilon = self.params['alphaepsilon'],
+                                   L = self.params['L'],
+                                   Gamma = self.params['Gamma'],
+                                   Nx = self.params['Nx'], 
+                                   Ny = self.params['Ny'],
+                                   Nz = self.params['Nz'],
+                                   dx = self.params['dx'],
+                                   dy = self.params['dy'],
+                                   dz = self.params['dz'],
+                                   SaveToFile = self.params['SaveToFile'],
+                                   UseNormalization = 0,
+                                   TurbOptions = TurbOptions)
+            
+            if Component == 'u':
+                self.u = c
+            if Component == 'v':
+                self.v = c
+            if Component == 'w':
+                self.w = c
+            
+            return c
```

### Comparing `hipersim-0.0.7/src/hipersim.egg-info/SOURCES.txt` & `hipersim-0.0.9/src/hipersim.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 src/hipersim.egg-info/dependency_links.txt
 src/hipersim.egg-info/top_level.txt
 src/hipersim/surrogates/__init__.py
 src/hipersim/surrogates/math_utils.py
 src/hipersim/surrogates/neuralnets.py
 src/hipersim/turbgen/__init__.py
 src/hipersim/turbgen/constrain_field.py
+src/hipersim/turbgen/constrain_field_1d.py
 src/hipersim/turbgen/generate_field.py
 src/hipersim/turbgen/manntensor.py
 src/hipersim/turbgen/trapezoidal_sum_2d.py
 src/hipersim/turbgen/turbgen.py
```

