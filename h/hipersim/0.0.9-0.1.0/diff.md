# Comparing `tmp/hipersim-0.0.9.tar.gz` & `tmp/hipersim-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nkdi\Documents\Programs\HiperSim\release\dist\tmpwr9yd463\hipersim-0.0.9.tar", last modified: Tue Aug 31 20:32:42 2021, max compression
+gzip compressed data, was "hipersim-0.1.0.tar", last modified: Fri Jun 23 14:39:35 2023, max compression
```

## Comparing `hipersim-0.0.9.tar` & `hipersim-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,39 @@
-drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.793787 hipersim-0.0.9/
--rw-rw-rw-   0        0        0     1086 2021-06-22 12:13:11.000000 hipersim-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1338 2021-08-31 20:32:42.794891 hipersim-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      832 2021-08-17 12:41:20.000000 hipersim-0.0.9/README.md
--rw-rw-rw-   0        0        0      108 2021-06-22 09:04:30.000000 hipersim-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0      627 2021-08-31 20:32:42.798486 hipersim-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.700692 hipersim-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.726117 hipersim-0.0.9/src/hipersim/
--rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.0.9/src/hipersim/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.755273 hipersim-0.0.9/src/hipersim/surrogates/
--rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.0.9/src/hipersim/surrogates/__init__.py
--rw-rw-rw-   0        0        0     1021 2019-06-27 09:54:53.000000 hipersim-0.0.9/src/hipersim/surrogates/math_utils.py
--rw-rw-rw-   0        0        0    20937 2021-06-22 12:25:11.000000 hipersim-0.0.9/src/hipersim/surrogates/neuralnets.py
-drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.789793 hipersim-0.0.9/src/hipersim/turbgen/
--rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.0.9/src/hipersim/turbgen/__init__.py
--rw-rw-rw-   0        0        0    19832 2021-08-30 09:46:31.000000 hipersim-0.0.9/src/hipersim/turbgen/constrain_field.py
--rw-rw-rw-   0        0        0    17792 2021-08-31 11:49:44.000000 hipersim-0.0.9/src/hipersim/turbgen/constrain_field_1d.py
--rw-rw-rw-   0        0        0    22981 2021-06-22 11:54:06.000000 hipersim-0.0.9/src/hipersim/turbgen/generate_field.py
--rw-rw-rw-   0        0        0    25078 2021-05-04 20:59:21.000000 hipersim-0.0.9/src/hipersim/turbgen/manntensor.py
--rw-rw-rw-   0        0        0      632 2021-08-30 10:02:04.000000 hipersim-0.0.9/src/hipersim/turbgen/trapezoidal_sum_2d.py
--rw-rw-rw-   0        0        0     6705 2021-08-31 20:27:40.000000 hipersim-0.0.9/src/hipersim/turbgen/turbgen.py
-drwxrwxrwx   0        0        0        0 2021-08-31 20:32:42.742720 hipersim-0.0.9/src/hipersim.egg-info/
--rw-rw-rw-   0        0        0     1338 2021-08-31 20:32:42.000000 hipersim-0.0.9/src/hipersim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      588 2021-08-31 20:32:42.000000 hipersim-0.0.9/src/hipersim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-31 20:32:42.000000 hipersim-0.0.9/src/hipersim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-08-31 20:32:42.000000 hipersim-0.0.9/src/hipersim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 14:39:34.981090 hipersim-0.1.0/
+-rw-rw-rw-   0        0        0     1086 2021-06-22 12:13:11.000000 hipersim-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       47 2021-10-01 12:38:50.000000 hipersim-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1348 2023-06-23 14:39:34.982602 hipersim-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      907 2021-09-27 21:27:22.000000 hipersim-0.1.0/README.md
+-rw-rw-rw-   0        0        0      108 2021-06-22 09:04:30.000000 hipersim-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      678 2023-06-23 14:39:34.997015 hipersim-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 14:39:33.603843 hipersim-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 14:39:33.673322 hipersim-0.1.0/src/hipersim/
+-rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.1.0/src/hipersim/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:39:34.201674 hipersim-0.1.0/src/hipersim/surrogates/
+-rw-rw-rw-   0        0        0    33135 2021-09-30 23:02:13.000000 hipersim-0.1.0/src/hipersim/surrogates/AutoencoderModel_20Farms_10outputs.sav
+-rw-rw-rw-   0        0        0    31911 2021-10-01 05:42:56.000000 hipersim-0.1.0/src/hipersim/surrogates/PyWake_Surrogate_10Farms_Power_Autoencoder.sav
+-rw-rw-rw-   0        0        0    41997 2021-09-30 20:57:49.000000 hipersim-0.1.0/src/hipersim/surrogates/PyWake_Surrogate_10Farms_Power_RelativeLocation.sav
+-rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.1.0/src/hipersim/surrogates/__init__.py
+-rw-rw-rw-   0        0        0     8179 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/surrogates/farm_utils.py
+-rw-rw-rw-   0        0        0     2006 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/surrogates/math_utils.py
+-rw-rw-rw-   0        0        0    21250 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/surrogates/neuralnets.py
+-rw-rw-rw-   0        0        0      604 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/surrogates/os_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:39:34.828119 hipersim-0.1.0/src/hipersim/turbgen/
+-rw-rw-rw-   0        0        0        0 2019-03-21 12:56:57.000000 hipersim-0.1.0/src/hipersim/turbgen/__init__.py
+-rw-rw-rw-   0        0        0    19408 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/turbgen/constrain_field.py
+-rw-rw-rw-   0        0        0    17771 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/turbgen/constrain_field_1d.py
+-rw-rw-rw-   0        0        0    31003 2023-06-23 14:34:21.000000 hipersim-0.1.0/src/hipersim/turbgen/generate_field.py
+-rw-rw-rw-   0        0        0   457165 2023-06-23 13:55:19.000000 hipersim-0.1.0/src/hipersim/turbgen/mannspectrum.py
+-rw-rw-rw-   0        0        0    26539 2023-03-28 12:05:04.000000 hipersim-0.1.0/src/hipersim/turbgen/manntensor.py
+-rw-rw-rw-   0        0        0      490 2023-06-23 13:55:19.000000 hipersim-0.1.0/src/hipersim/turbgen/trapezoidal_sum_2d.py
+-rw-rw-rw-   0        0        0     8810 2023-06-23 13:55:19.000000 hipersim-0.1.0/src/hipersim/turbgen/turb_utils.py
+-rw-rw-rw-   0        0        0     8042 2023-06-23 13:55:19.000000 hipersim-0.1.0/src/hipersim/turbgen/turbgen.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:39:33.790183 hipersim-0.1.0/src/hipersim.egg-info/
+-rw-rw-rw-   0        0        0     1348 2023-06-23 14:39:33.000000 hipersim-0.1.0/src/hipersim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1061 2023-06-23 14:39:33.000000 hipersim-0.1.0/src/hipersim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 14:39:33.000000 hipersim-0.1.0/src/hipersim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-23 14:39:33.000000 hipersim-0.1.0/src/hipersim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 14:39:33.000000 hipersim-0.1.0/src/hipersim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 14:39:34.973166 hipersim-0.1.0/tests/
+-rw-rw-rw-   0        0        0     1454 2023-06-23 13:55:19.000000 hipersim-0.1.0/tests/test_manntensor.py
+-rw-rw-rw-   0        0        0     9278 2023-06-23 14:34:22.000000 hipersim-0.1.0/tests/test_spectra.py
+-rw-rw-rw-   0        0        0     6278 2023-06-23 14:34:22.000000 hipersim-0.1.0/tests/test_turb_gen.py
```

### Comparing `hipersim-0.0.9/LICENSE` & `hipersim-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hipersim-0.0.9/PKG-INFO` & `hipersim-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 Metadata-Version: 2.1
 Name: hipersim
-Version: 0.0.9
+Version: 0.1.0
 Summary: A collection of wind energy simulation tools
 Home-page: https://gitlab.windenergy.dtu.dk/HiperSim/hipersim
 Author: Nikolay Dimitrov
 Author-email: nkdi@dtu.dk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hipersim
 
 ## Introduction
 Hipersim is a collection of tools for computationally-efficient simulation of Wind Energy problems using statistical and machine learning methods. Currently, the package contains the following submodules:
 
 - **turbgen**: 
     - Generation of 3D frozen turbulence fields ("turbulence boxes") with the Mann turbulence spectrum
     - Constrained turbulence field generation and application of constraints on pre-generated turbulence fields
 
 - **surrogates**:
     - A feedforward neural network toolbox, training and evaluation of feedforward neural networks. 
+	- A set of tools for surrogate-based modeling and analysis of wind farms
 
 ## Installation
 Hipersim is registered as installable Python package in PyPi.org. Installation happens automatically with the following command:
 
 pip install hipersim
 
 ## References
 
 ## License
 Hipersim uses the MIT License.
-
-
```

### Comparing `hipersim-0.0.9/src/hipersim/surrogates/neuralnets.py` & `hipersim-0.1.0/src/hipersim/surrogates/neuralnets.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,504 +1,519 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Aug 24 12:47:19 2018
 
 @author: nkdi
 """
 import numpy as np
-#from w2l import activation_functions
+# from w2l import activation_functions
+# from surrogates import math_utils
 from hipersim.surrogates import math_utils
 
+
 class ann:
-    def __init__(self,**kwargs):
-        #print(kwargs)
+    def __init__(self, **kwargs):
+        # print(kwargs)
         if 'layersizes' in kwargs:
             self.layersizes = kwargs['layersizes']
         else:
             self.layersizes = [1, 10, 1]
-            
-        self.nlayers = len(self.layersizes) - 1 # Input layer is not counted
-        
+
+        self.nlayers = len(self.layersizes) - 1  # Input layer is not counted
+
         if 'neurontypes' in kwargs:
             self.neurontypes = kwargs['neurontypes']
         else:
-            self.neurontypes = ['Linear']*self.nlayers
-            
+            self.neurontypes = ['Linear'] * self.nlayers
+
         if 'activation' in kwargs:
             self.activation = kwargs['activation']
         else:
-            self.activation = ['Relu']*(self.nlayers-1) + ['Linear']
-            
+            self.activation = ['Relu'] * (self.nlayers - 1) + ['Linear']
+
         if 'testratios' in kwargs:
             self.testratios = kwargs['testratios']
         else:
             self.testratios = [0.7, 0.2, 0.1]
-            
+
         if 'output_style' in kwargs:
             self.output_style = kwargs['output_style']
         else:
             self.output_style = 'None'
-            
+
         if 'params' in kwargs:
             self.params = kwargs['params']
         else:
-            self.params = {'weightinit': [0.01]*self.nlayers, 
-                           'regularization': 0.1, 
-                           'learningrate': 0.1, 
-                           'costfunction': 'Lsq', 
-                           'minibatchsize': 0, 
-                           'maxiter': 1500, 
-                           'RMSprop': 0.999, 
-                           'Momentum': 0.9, 
-                           'Xscaling': True, 
+            self.params = {'weightinit': [0.01] * self.nlayers,
+                           'regularization': 0.1,
+                           'learningrate': 0.1,
+                           'costfunction': 'Lsq',
+                           'minibatchsize': 0,
+                           'maxiter': 1500,
+                           'RMSprop': 0.999,
+                           'Momentum': 0.9,
+                           'Xscaling': True,
                            'Yscaling': True}
         # Parse parameters that may have not been given in the input
-        if not 'weightinit' in self.params:
-            self.params['weightinit'] = [0.01]*self.nlayers
-        if not 'regularization' in self.params:
+        if 'weightinit' not in self.params:
+            self.params['weightinit'] = [0.01] * self.nlayers
+        if 'regularization' not in self.params:
             self.params['regularization'] = 0.1
-        if not 'learningrate' in self.params:           
+        if 'learningrate' not in self.params:
             self.params['learningrate'] = 0.1
-        if not 'costfunction' in self.params:
+        if 'costfunction' not in self.params:
             self.params['costfunction'] = 'Lsq'
-        if not 'minibatchsize' in self.params:
+        if 'minibatchsize' not in self.params:
             self.params['minibatchsize'] = 0
-        if not 'maxiter' in self.params:
-            self.params['maxiter'] = 1500 # Same as nepochs
-        if not 'RMSprop' in self.params:
+        if 'maxiter' not in self.params:
+            self.params['maxiter'] = 1500  # Same as nepochs
+        if 'RMSprop' not in self.params:
             self.params['RMSprop'] = 0.999
-        if not 'Momentum' in self.params:
+        if 'Momentum' not in self.params:
             self.params['Momentum'] = 0.9
-        if not 'nepochs' in self.params:
+        if 'nepochs' not in self.params:
             self.params['nepochs'] = self.params['maxiter']
-        if not 'Xscaling' in self.params:
+        if 'Xscaling' not in self.params:
             self.params['Xscaling'] = True
-        if not 'Yscaling' in self.params:
+        if 'Yscaling' not in self.params:
             self.params['Yscaling'] = True
 
-
     def initialize_weights(self):
         W = []
         b = []
-        #np.random.seed(1) # Used only in case we need to maintan consisteny with Matlab
+        # np.random.seed(1) # Used only in case we need to maintan consisteny with Matlab
         for i in range(self.nlayers):
             if self.neurontypes[i] == 'Linear':
-                #Wi = np.random.randn(self.layersizes[i],self.layersizes[i+1])*self.params['weightinit'][i] # Regular way of initializing weights
-                Wi = math_utils.NormalDist(2,np.random.rand(self.layersizes[i],self.layersizes[i+1]),0,1)*self.params['weightinit'][i] # For consistency with Matlab
-                bi = np.zeros([1,self.layersizes[i+1]])
+                # Wi =
+                # np.random.randn(self.layersizes[i],self.layersizes[i+1])*self.params['weightinit'][i]
+                # # Regular way of initializing weights
+                Wi = math_utils.NormalDist(2,
+                                           np.random.rand(self.layersizes[i],
+                                                          self.layersizes[i + 1]),
+                                           0,
+                                           1) * self.params['weightinit'][i]  # For consistency with Matlab
+                bi = np.zeros([1, self.layersizes[i + 1]])
             elif self.neurontypes[i] == 'LinearPretrained':
                 Wi = self.weights['W'][i]
                 bi = self.weights['bias'][i]
             elif self.neurontypes[i] == 'LinearNonTrainable':
                 Wi = self.weights['W'][i]
-                bi = self.weights['bias'][i]                
+                bi = self.weights['bias'][i]
             W.append(Wi)
             b.append(bi)
-            
+
         if hasattr(self, 'weights'):
-            self.weights['W'] = W    
+            self.weights['W'] = W
             self.weights['bias'] = b
         else:
-            self.weights = {'W':W, 'bias':b}
-                        
-        return W,b
-    
-    def forward_propagation(self,X):
+            self.weights = {'W': W, 'bias': b}
+
+        return W, b
+
+    def forward_propagation(self, X):
         A = []
         Z = []
         A.append(X)
         Ai = X
         for i in range(self.nlayers):
-            if self.neurontypes[i]=='Linear':
-                Zi = np.dot(Ai,self.weights['W'][i]) + self.weights['bias'][i]
-            elif self.neurontypes[i]=='LinearPretrained':
-                Zi = np.dot(Ai,self.weights['W'][i]) + self.weights['bias'][i]
-            elif self.neurontypes[i]=='LinearNonTrainable':
-                Zi = np.dot(Ai,self.weights['W'][i]) + self.weights['bias'][i]
+            if self.neurontypes[i] == 'Linear':
+                Zi = np.dot(Ai, self.weights['W'][i]) + self.weights['bias'][i]
+            elif self.neurontypes[i] == 'LinearPretrained':
+                Zi = np.dot(Ai, self.weights['W'][i]) + self.weights['bias'][i]
+            elif self.neurontypes[i] == 'LinearNonTrainable':
+                Zi = np.dot(Ai, self.weights['W'][i]) + self.weights['bias'][i]
             else:
                 raise ValueError('Unknown or unspecified neuron type')
 
             if self.activation[i] == 'Relu':
                 Ai = math_utils.relu(Zi)
             elif self.activation[i] == 'Linear':
                 Ai = Zi
             elif self.activation[i] == 'Tanh':
                 Ai = math_utils.hyperbolic_tangent(Zi)
             elif self.activation[i] == 'Softplus':
                 Ai = math_utils.softplus(Zi)
             else:
                 raise ValueError('Unknown or unspecified activation function')
-            
+
             A.append(Ai)
             Z.append(Zi)
-            
+
         Ypredict = Ai
-        ANNcache = (A,Z)
+        ANNcache = (A, Z)
         return Ypredict, ANNcache
-    
-    def backward_propagation(self,X,Y,Ypredict,ANNcache):
+
+    def backward_propagation(self, X, Y, Ypredict, ANNcache):
         if self.params['costfunction'] == 'Log':
-            dJdAprev = -Y/Ypredict + (1 - Y)/(1 - Ypredict)
+            dJdAprev = -Y / Ypredict + (1 - Y) / (1 - Ypredict)
         elif self.params['costfunction'] == 'Lsq':
-            dJdAprev = (Ypredict -Y)
+            dJdAprev = (Ypredict - Y)
         else:
             raise ValueError('Unknown cost function type')
-        
-        dJdA = [None]*self.nlayers
-        dAdZ = [None]*self.nlayers
-        dJdW = [None]*self.nlayers
-        dJdb = [None]*self.nlayers 
-        dJdZ = [None]*self.nlayers
-        A,Z = ANNcache
-        
-        for i in range(self.nlayers-1, -1,-1):
+
+        dJdA = [None] * self.nlayers
+        dAdZ = [None] * self.nlayers
+        dJdW = [None] * self.nlayers
+        dJdb = [None] * self.nlayers
+        dJdZ = [None] * self.nlayers
+        A, Z = ANNcache
+
+        for i in range(self.nlayers - 1, -1, -1):
             dJdA[i] = dJdAprev
             if self.activation[i] == 'Linear':
                 dAdZ[i] = np.ones(Z[i].shape)
             elif self.activation[i] == 'Relu':
-                dAdZ[i] = np.ones(Z[i].shape)*(Z[i] > 0)
+                dAdZ[i] = np.ones(Z[i].shape) * (Z[i] > 0)
             elif self.activation[i] == 'Softplus':
                 dAdZ[i] = math_utils.logistic(Z[i])
             elif self.activation[i] == 'Tanh':
                 dAdZ[i] = 1 - math_utils.hyperbolic_tangent(Z[i])**2
             elif self.activation[i] == 'Logistic':
-                dAdZ[i] = math_utils.logistic(Z[i])*(1 - math_utils.logistic(Z[i]))
+                dAdZ[i] = math_utils.logistic(Z[i]) * (1 - math_utils.logistic(Z[i]))
             else:
                 raise ValueError('Unknown activation function')
-            
-            dJdZ[i] = dAdZ[i]*dJdA[i]
+
+            dJdZ[i] = dAdZ[i] * dJdA[i]
             mlength = X.shape[0]
             if self.neurontypes[i] == 'Linear':
-                dJdW[i] = (1/mlength)*np.dot(A[i].T,dJdZ[i])
-                dJdb[i] = (1/mlength)*np.sum(dJdZ[i],0,keepdims = True)
+                dJdW[i] = (1 / mlength) * np.dot(A[i].T, dJdZ[i])
+                dJdb[i] = (1 / mlength) * np.sum(dJdZ[i], 0, keepdims=True)
             elif self.neurontypes[i] == 'LinearPretrained':
-                dJdW[i] = (1/mlength)*np.dot(A[i].T,dJdZ[i])
-                dJdb[i] = (1/mlength)*np.sum(dJdZ[i],0,keepdims = True)
+                dJdW[i] = (1 / mlength) * np.dot(A[i].T, dJdZ[i])
+                dJdb[i] = (1 / mlength) * np.sum(dJdZ[i], 0, keepdims=True)
             elif self.neurontypes[i] == 'LinearNonTrainable':
                 dJdW[i] = np.zeros(Z[i].shape)
-                dJdb[i] = np.zeros((1,Z[i].shape[1]))
+                dJdb[i] = np.zeros((1, Z[i].shape[1]))
             else:
                 raise ValueError('Unknown neuron type')
 
-            dJdAprev = np.dot(dJdZ[i],self.weights['W'][i].T)            
-        
+            dJdAprev = np.dot(dJdZ[i], self.weights['W'][i].T)
+
         return dJdW, dJdb
 
-    def backward_propagation_dy(self,X):
+    def backward_propagation_dy(self, X):
         if self.params['Xscaling']:
-            X = (X - self.Xbias)/self.Xscale # Lots of broadcasting taking place here
-            
+            X = (X - self.Xbias) / self.Xscale  # Lots of broadcasting taking place here
+
         Y, ANNcache = self.forward_propagation(X)
         if self.params['Yscaling']:
-            Y = Y*self.Yscale + self.Ybias
-        
-        A,Z = ANNcache
+            Y = Y * self.Yscale + self.Ybias
+
+        A, Z = ANNcache
         noutputs = Y.shape[1]
-                
-        dY = [None]*noutputs
-        
+
+        dY = [None] * noutputs
+
         for iY in range(noutputs):
-        
-            for i in range(self.nlayers-1, -1,-1):
-                
+
+            for i in range(self.nlayers - 1, -1, -1):
+
                 if i == self.nlayers - 1:
-                    Zi = Z[i][:,iY]
-                    Zi = Zi.reshape(Zi.shape[0],1)
-                    Wi = self.weights['W'][i][:,iY]
-                    Wi = Wi.reshape(Wi.shape[0],1)
+                    Zi = Z[i][:, iY]
+                    Zi = Zi.reshape(Zi.shape[0], 1)
+                    Wi = self.weights['W'][i][:, iY]
+                    Wi = Wi.reshape(Wi.shape[0], 1)
                 else:
                     Zi = Z[i]
                     Wi = self.weights['W'][i]
-                    
+
                 if self.activation[i] == 'Linear':
                     dAdZ = np.ones(Zi.shape)
                 elif self.activation[i] == 'Relu':
-                    dAdZ = np.ones(Zi.shape)*(Zi > 0)
+                    dAdZ = np.ones(Zi.shape) * (Zi > 0)
                 elif self.activation[i] == 'Softplus':
                     dAdZ = math_utils.logistic(Zi)
                 elif self.activation[i] == 'Tanh':
                     dAdZ = 1 - math_utils.hyperbolic_tangent(Zi)**2
                 elif self.activation[i] == 'Logistic':
-                    dAdZ = math_utils.logistic(Zi)*(1 - math_utils.logistic(Zi))
+                    dAdZ = math_utils.logistic(Zi) * (1 - math_utils.logistic(Zi))
                 else:
                     raise ValueError('Unknown activation function')
-                
-                if i == self.nlayers-1:
-                    dYi = np.dot(dAdZ,Wi.T)
+
+                if i == self.nlayers - 1:
+                    dYi = np.dot(dAdZ, Wi.T)
                 else:
-                    dYi = np.dot((dAdZ*dYi),Wi.T)
+                    dYi = np.dot((dAdZ * dYi), Wi.T)
 
             if self.params['Yscaling']:
-                dYi = dYi*self.Yscale[0,iY]
+                dYi = dYi * self.Yscale[0, iY]
             if self.params['Xscaling']:
-                dYi = dYi/self.Xscale
-            
+                dYi = dYi / self.Xscale
+
             dY[iY] = dYi
-                        
+
         return Y, dY
-    
-    def check_gradients(self,X):
-        if not hasattr(self,'weights'):
+
+    def check_gradients(self, X):
+        if not hasattr(self, 'weights'):
             self.initialize_weights()
-            
-            
-    def check_gradients_dxdy(self,X):
-        Yout,dYout = self.backward_propagation_dy(X)
-    
-    def compute_cost(self,X,Y):
-        #Computes the cost using log-functions
+
+    def check_gradients_dxdy(self, X):
+        Yout, dYout = self.backward_propagation_dy(X)
+
+    def compute_cost(self, X, Y):
+        # Computes the cost using log-functions
         mtrain = X.shape[0]
         noutputs = Y.shape[1]
-        Ypredict,ANNcache = self.forward_propagation(X)
+        Ypredict, ANNcache = self.forward_propagation(X)
         if self.params['costfunction'] == 'Log':
-            Loss = - (np.multiply(Y,np.log(Ypredict)) + np.multiply((1 - Y), np.log(1 - Ypredict)))
+            Loss = - (np.multiply(Y, np.log(Ypredict)) + np.multiply((1 - Y), np.log(1 - Ypredict)))
         elif self.params['costfunction'] == 'Lsq':
-            Loss = 0.5*np.multiply((Ypredict - Y),(Ypredict - Y))
+            Loss = 0.5 * np.multiply((Ypredict - Y), (Ypredict - Y))
         else:
             print('Unknown loss function type!')
 
         if self.params["regularization"] == 0:
-            J = (1/mtrain)*np.sum(Loss)*(1/noutputs)
+            J = (1 / mtrain) * np.sum(Loss) * (1 / noutputs)
         else:
             v = cell_to_vector(self.weights['W'], self.weights['bias'])
-            J = (1/mtrain)*np.sum(Loss)*(1/noutputs) + (self.params['regularization']/(2*mtrain))*(np.dot(v.T,v))
+            J = (1 / mtrain) * np.sum(Loss) * (1 / noutputs) + \
+                (self.params['regularization'] / (2 * mtrain)) * (np.dot(v.T, v))
 
         return J, Ypredict, ANNcache
 
-    
-    def train(self,X,Y):
+    def train(self, X, Y):
         """
         Uses input-output data pair (X,Y) to train the weights of a neural-net object
-        """        
+        """
         # Parse hyperparameters
         beta2 = self.params['RMSprop']
         if beta2 == 0:
             epsroundoff = 0
         else:
             epsroundoff = 1e-8
-        beta1 = self.params['Momentum']                    
+        beta1 = self.params['Momentum']
         minibatchsize = self.params['minibatchsize']
         nepochs = self.params['nepochs']
-                    
-        self.Xbias = np.mean(X,axis=0, keepdims = True) # Keepdims = True needed to allow broadcasting
-        self.Ybias = np.mean(Y,axis=0, keepdims = True)
-        self.Xscale = np.std(X,axis=0, ddof = 1, keepdims = True)
-        self.Yscale = np.std(Y,axis=0, ddof = 1, keepdims = True)
-        
+
+        self.Xbias = np.mean(X, axis=0, keepdims=True)  # Keepdims = True needed to allow broadcasting
+        self.Ybias = np.mean(Y, axis=0, keepdims=True)
+        self.Xscale = np.std(X, axis=0, ddof=1, keepdims=True)
+        self.Yscale = np.std(Y, axis=0, ddof=1, keepdims=True)
+
         if self.params['Xscaling']:
-            X = (X - self.Xbias)/self.Xscale
+            X = (X - self.Xbias) / self.Xscale
         if self.params['Yscaling']:
-            Y = (Y - self.Ybias)/self.Yscale
+            Y = (Y - self.Ybias) / self.Yscale
 
-        # Split data into training, validation and test sets            
+        # Split data into training, validation and test sets
         Ntotal = X.shape[0]
-        Ntrain = int(np.floor(Ntotal*self.testratios[0]))
-        Ndev = int(np.floor(Ntotal*self.testratios[1]))
-        Xtrain = X[:Ntrain,:]
-        Ytrain = Y[:Ntrain,:]
-        Xdev = X[Ntrain:Ntrain+Ndev,:]
-        Ydev = Y[Ntrain:Ntrain+Ndev,:]
-        Xtest = X[Ntrain+Ndev:,:]
-        Ytest = Y[Ntrain+Ndev:,:]
+        Ntrain = int(np.floor(Ntotal * self.testratios[0]))
+        Ndev = int(np.floor(Ntotal * self.testratios[1]))
+        Xtrain = X[:Ntrain, :]
+        Ytrain = Y[:Ntrain, :]
+        Xdev = X[Ntrain:Ntrain + Ndev, :]
+        Ydev = Y[Ntrain:Ntrain + Ndev, :]
+        Xtest = X[Ntrain + Ndev:, :]
+        Ytest = Y[Ntrain + Ndev:, :]
 
         # Determine iteration scheme
-        if minibatchsize == 0: # Minibatch functionality off
-            minibatchsize = Ntrain # Each iteration is on the entire train set            
+        if minibatchsize == 0:  # Minibatch functionality off
+            minibatchsize = Ntrain  # Each iteration is on the entire train set
             Nbatches = 1
             Niter = self.params['nepochs']
         else:
-            Nbatches = int(np.ceil(Ntrain/minibatchsize))
-            Niter = nepochs*Nbatches
-                        
+            Nbatches = int(np.ceil(Ntrain / minibatchsize))
+            Niter = nepochs * Nbatches
+
         # Initialize variables and weights
         noutputs = Y.shape[1]
-        Jhist = np.zeros([Niter,1])
-        Jgradnorm = np.zeros([Niter,1])
-        Jdevhist = np.zeros([Niter,1])
-        Rsqhist = np.zeros([Niter,noutputs])
-        Rsqdevhist = np.zeros([Niter,noutputs])
-        
+        Jhist = np.zeros([Niter, 1])
+        Jgradnorm = np.zeros([Niter, 1])
+        Jdevhist = np.zeros([Niter, 1])
+        Rsqhist = np.zeros([Niter, noutputs])
+        Rsqdevhist = np.zeros([Niter, noutputs])
+
         self.initialize_weights()
         ntotal = 0
         for i in range(self.nlayers):
-            ntotal+= self.weights['W'][i].shape[0]*self.weights['W'][i].shape[1] + self.weights['bias'][i].shape[0]*self.weights['bias'][i].shape[1] 
-        
+            ntotal += self.weights['W'][i].shape[0] * self.weights['W'][i].shape[1] + \
+                self.weights['bias'][i].shape[0] * self.weights['bias'][i].shape[1]
+
         # Initialize interactive plot/inline-output functionalities
         if self.output_style == 'Verbose':
             print('Verbose output')
         elif self.output_style == 'Plot':
+            import tkinter
+            import matplotlib
             import matplotlib.pyplot as plt
             plt.ion()
-            fig, axs = plt.subplots(1,2,figsize = (8,4))
-            plt00 = axs[0].plot(0,0,'-k')[0]
-            plt01 = axs[0].plot(0,0,'-r')[0]
+            matplotlib.use('TkAgg')
+            fig, axs = plt.subplots(1, 2, figsize=(8, 4))
+            plt00 = axs[0].plot(0, 0, '-k')[0]
+            plt01 = axs[0].plot(0, 0, '-r')[0]
             axs[0].set_xlabel('Number of iterations')
             axs[0].set_ylabel('Cost function value J')
-            plt10 = axs[1].plot(0,0,'-k')[0]
-            plt11 = axs[1].plot(0,0,'-r')[0]
-            plt12 = axs[1].plot(0,0,'--k')[0]
-            plt13 = axs[1].plot(0,0,'--r')[0]
-            
+            plt10 = axs[1].plot(0, 0, '-k')[0]
+            plt11 = axs[1].plot(0, 0, '-r')[0]
+            plt12 = axs[1].plot(0, 0, '--k')[0]
+            plt13 = axs[1].plot(0, 0, '--r')[0]
+
             axs[1].set_xlabel('Number of iterations')
             axs[1].set_ylabel('R-squared')
-            axs[1].set_ylim([0,1])
+            axs[1].set_ylim([0, 1])
             fig.tight_layout()
             fig.show()
             fig.canvas.draw()
-            
-        elif self.output_style == 'None': 
+
+        elif self.output_style == 'None':
             print('Training neural net model:')
-            
-            
+
         # Begin iterations
         go = 1
         i = 0
         ibatch = 0
         iepoch = 0
-        Vd = np.zeros([ntotal,1])
-        Sd = np.zeros([ntotal,1])
+        Vd = np.zeros([ntotal, 1])
+        Sd = np.zeros([ntotal, 1])
         while go == 1:
             # Look at the dev(validation) set and compute cost function and R-square
-            Jdev,Ypredictdev, _ = self.compute_cost(Xdev,Ydev)
+            Jdev, Ypredictdev, _ = self.compute_cost(Xdev, Ydev)
             Jdevhist[i] = Jdev
-            Rsqdevhist[i,:] = math_utils.pairwise_correlation(Ypredictdev,Ydev)**2
-            
+            Rsqdevhist[i, :] = math_utils.pairwise_correlation(Ypredictdev, Ydev)**2
+
             # Pick a single minibatch of training data samples
             if ibatch == Nbatches:
-                Xtraini = Xtrain[ibatch*minibatchsize:,:]
-                Ytraini = Ytrain[ibatch*minibatchsize:,:]
+                Xtraini = Xtrain[ibatch * minibatchsize:, :]
+                Ytraini = Ytrain[ibatch * minibatchsize:, :]
             else:
-                Xtraini = Xtrain[ibatch*minibatchsize:(ibatch+1)*minibatchsize,:]
-                Ytraini = Ytrain[ibatch*minibatchsize:(ibatch+1)*minibatchsize,:]
-                
+                Xtraini = Xtrain[ibatch * minibatchsize:(ibatch + 1) * minibatchsize, :]
+                Ytraini = Ytrain[ibatch * minibatchsize:(ibatch + 1) * minibatchsize, :]
+
             # Compute cost function, cost function gradients, and R-square on one minibatch
-            J,Ypredict,ANNcache = self.compute_cost(Xtraini,Ytraini) # Cost function
-            [dJdW,dJdb] = self.backward_propagation(Xtraini,Ytraini,Ypredict,ANNcache) # Cost function gradients
-            dvecti = cell_to_vector(dJdW,dJdb)
+            J, Ypredict, ANNcache = self.compute_cost(Xtraini, Ytraini)  # Cost function
+            [dJdW, dJdb] = self.backward_propagation(Xtraini, Ytraini, Ypredict, ANNcache)  # Cost function gradients
+            dvecti = cell_to_vector(dJdW, dJdb)
             Jhist[i] = J
-            Jgradnorm[i] = (1/minibatchsize)*np.sqrt(np.dot(dvecti.T,dvecti)) # Gradient norm for monitoring purposes
-            Rsqhist[i,:] = math_utils.pairwise_correlation(Ypredict,Ytraini)**2 # R-square
-            
+            # Gradient norm for monitoring purposes
+            Jgradnorm[i] = (1 / minibatchsize) * np.sqrt(np.dot(dvecti.T, dvecti))
+            Rsqhist[i, :] = math_utils.pairwise_correlation(Ypredict, Ytraini)**2  # R-square
+
             # Update weights based on gradient descent
-            if (beta1 != 0) & (beta2 != 0): # Adam algorithm
-                Vd = beta1*Vd + (1 - beta1)*dvecti
-                Sd = beta2*Sd + (1 - beta2)*(dvecti**2)
-                Vcorr = Vd/(1 - beta1**(i+1))
-                Scorr = Sd/(1 - beta2**(i+1))
-                vupd = cell_to_vector(self.weights['W'], self.weights['bias']) - self.params['learningrate']*(Vcorr/(np.sqrt(Scorr) + epsroundoff)  + cell_to_vector(self.weights['W'], self.weights['bias'])*self.params['regularization']/Xtraini.shape[0])
-            elif beta1 > 0 & beta2 == 0: # Only momentum, no RMSprop, optional regularization
-                Vd = beta1*Vd + (1 - beta1)*dvecti
-                Vcorr = Vd/(1 - beta1**(i+1))
-                vupd = cell_to_vector(self.weights['W'], self.weights['bias']) - self.params['learningrate']*(Vcorr + cell_to_vector(self.weights['W'], self.weights['bias'])*self.params['regularization']/Xtraini.shape[0])
+            if (beta1 != 0) & (beta2 != 0):  # Adam algorithm
+                Vd = beta1 * Vd + (1 - beta1) * dvecti
+                Sd = beta2 * Sd + (1 - beta2) * (dvecti**2)
+                Vcorr = Vd / (1 - beta1**(i + 1))
+                Scorr = Sd / (1 - beta2**(i + 1))
+                vupd = cell_to_vector(self.weights['W'], self.weights['bias']) - self.params['learningrate'] * (Vcorr / (np.sqrt(
+                    Scorr) + epsroundoff) + cell_to_vector(self.weights['W'], self.weights['bias']) * self.params['regularization'] / Xtraini.shape[0])
+            elif beta1 > 0 & beta2 == 0:  # Only momentum, no RMSprop, optional regularization
+                Vd = beta1 * Vd + (1 - beta1) * dvecti
+                Vcorr = Vd / (1 - beta1**(i + 1))
+                vupd = cell_to_vector(self.weights['W'], self.weights['bias']) - self.params['learningrate'] * (
+                    Vcorr + cell_to_vector(self.weights['W'], self.weights['bias']) * self.params['regularization'] / Xtraini.shape[0])
             else:
                 # Simple gradient descent with optional regularization
-                vupd = cell_to_vector(self.weights['W'], self.weights['bias']) - self.params['learningrate']*(cell_to_vector(dJdW,dJdb) + cell_to_vector(self.weights['W'], self.weights['bias'])*self.params['regularization']/Xtraini.shape[0])
+                vupd = cell_to_vector(self.weights['W'],
+                                      self.weights['bias']) - self.params['learningrate'] * (cell_to_vector(dJdW,
+                                                                                                            dJdb) + cell_to_vector(self.weights['W'],
+                                                                                                                                   self.weights['bias']) * self.params['regularization'] / Xtraini.shape[0])
+
+            self.weights['W'], self.weights['bias'] = vector_to_cell(vupd, self.weights['W'], self.weights['bias'])
 
-            self.weights['W'], self.weights['bias'] = vector_to_cell(vupd,self.weights['W'], self.weights['bias'])
-            
             # Print/plot iteration outputs
             if self.output_style == 'Verbose':
                 print('Epoch #' + str(iepoch) + ', batch #' + str(ibatch) + ', cost function value = ' + str(J[0]))
-            elif (self.output_style == 'Plot') & (i >=1):
-                
+            elif (self.output_style == 'Plot') & (i >= 1):
+
                 # Update plot with results from current iteration
                 xplot = np.arange(i)
-                plt00.set_data(xplot,Jhist[:i])
-                plt01.set_data(xplot,Jdevhist[:i])
+                plt00.set_data(xplot, Jhist[:i])
+                plt01.set_data(xplot, Jdevhist[:i])
                 axs[0].relim()
-                axs[0].autoscale_view(True,True,True) #Autoscale                
-                plt10.set_data(xplot,np.min(Rsqhist[:i,:],1))
-                plt11.set_data(xplot,np.min(Rsqdevhist[:i,:],1))
-                plt12.set_data(xplot,np.max(Rsqhist[:i,:],1))
-                plt13.set_data(xplot,np.max(Rsqdevhist[:i,:],1))
-                
+                axs[0].autoscale_view(True, True, True)  # Autoscale
+                plt10.set_data(xplot, np.min(Rsqhist[:i, :], 1))
+                plt11.set_data(xplot, np.min(Rsqdevhist[:i, :], 1))
+                plt12.set_data(xplot, np.max(Rsqhist[:i, :], 1))
+                plt13.set_data(xplot, np.max(Rsqdevhist[:i, :], 1))
+
                 axs[1].relim()
-                axs[1].autoscale_view(True,True,True) #Autoscale                
-                
+                axs[1].autoscale_view(True, True, True)  # Autoscale
+
                 plt.pause(0.001)
                 fig.canvas.draw()
                 plt.show()
 
-            
-            i+=1
-            ibatch+=1
+            i += 1
+            ibatch += 1
             if i >= Niter:
                 go = 0
             if ibatch >= Nbatches:
                 if iepoch >= nepochs:
                     go = 0
                 else:
-                    ibatch=0
-                    iepoch+=1
-                    
-        Jout,Yout, _ = self.compute_cost(Xtest,Ytest)    
-        Rsqout = math_utils.pairwise_correlation(Yout,Ytest)**2
-        
+                    ibatch = 0
+                    iepoch += 1
+
+        Jout, Yout, _ = self.compute_cost(Xtest, Ytest)
+        Rsqout = math_utils.pairwise_correlation(Yout, Ytest)**2
+
         if self.params['Yscaling']:
-            Testbias = (np.mean(Yout,0) - np.mean(Ytest,0))*self.Yscale
+            Testbias = (np.mean(Yout, 0) - np.mean(Ytest, 0)) * self.Yscale
         else:
-            Testbias = np.mean(Yout,0) - np.mean(Ytest,0)
-        
-        self.metrics = {'RsqTest':Rsqout, 'RsqDev':Rsqdevhist[i-1,:],'RsqTrain':Rsqhist[i-1,:],'Testbias':Testbias}
-        
-        self.neurontypes = ['LinearPretrained' if ni == 'Linear' else ni for ni in self.neurontypes] # Start from previous trained state in case a new training command is issued
-                    
-        Outdata = {'Jhist':Jhist, 'Yout':Yout, 'Jout':Jout}
-        
-                
+            Testbias = np.mean(Yout, 0) - np.mean(Ytest, 0)
+
+        self.metrics = {'RsqTest': Rsqout, 'RsqDev': Rsqdevhist[i -
+                                                                1, :], 'RsqTrain': Rsqhist[i - 1, :], 'Testbias': Testbias}
+
+        # Start from previous trained state in case a new training command is issued
+        self.neurontypes = ['LinearPretrained' if ni == 'Linear' else ni for ni in self.neurontypes]
+
+        Outdata = {'Jhist': Jhist, 'Yout': Yout, 'Jout': Jout}
+
         return Outdata
-    
-    def predict(self,X):
+
+    def predict(self, X):
         """
         Run a model prediction (forward propagation + scaling)
-        """        
+        """
         if self.params['Xscaling']:
-            X = (X - self.Xbias)/self.Xscale # Lots of broadcasting taking place here
-        
+            X = (X - self.Xbias) / self.Xscale  # Lots of broadcasting taking place here
+
         Y, _ = self.forward_propagation(X)
         if self.params['Yscaling']:
-            Y = Y*self.Yscale + self.Ybias # Lots of broadcasting also taking place here
-        
+            Y = Y * self.Yscale + self.Ybias  # Lots of broadcasting also taking place here
+
         return Y
-        
-def cell_to_vector(W,b):
+
+
+def cell_to_vector(W, b):
     """
     Reshapes an array from dictionary-type structure to vector
     """
     nlayers = len(W)
     ntotal = 0
-    for i in range (nlayers):
-        ntotal+= W[i].shape[0]*W[i].shape[1] + b[i].shape[0]*b[i].shape[1]        
-    v = np.zeros([ntotal,1])
+    for i in range(nlayers):
+        ntotal += W[i].shape[0] * W[i].shape[1] + b[i].shape[0] * b[i].shape[1]
+    v = np.zeros([ntotal, 1])
     vcount = 0
     for i in range(nlayers):
-        vinc = W[i].shape[0]*W[i].shape[1]
-        v[vcount:vcount+vinc] = np.reshape(W[i],(vinc,1))
-        vcount+= vinc
+        vinc = W[i].shape[0] * W[i].shape[1]
+        v[vcount:vcount + vinc] = np.reshape(W[i], (vinc, 1))
+        vcount += vinc
     for i in range(nlayers):
-        vinc = b[i].shape[0]*b[i].shape[1]
-        v[vcount:vcount+vinc] = np.reshape(b[i],(vinc,1))
-        vcount+= vinc
-        
+        vinc = b[i].shape[0] * b[i].shape[1]
+        v[vcount:vcount + vinc] = np.reshape(b[i], (vinc, 1))
+        vcount += vinc
+
     return v
-        
-def vector_to_cell(v,W,b):
+
+
+def vector_to_cell(v, W, b):
     """
     Reshapes an array from a 1-D vector to a dictionary-type structure
     """
 
     nlayers = len(W)
     vcount = 0
-    
-    for i in range(nlayers):
-        vinc = W[i].shape[0]*W[i].shape[1]
-        W[i] = np.reshape(v[vcount:vcount+vinc],(W[i].shape[0],W[i].shape[1]))
-        vcount+= vinc
-    
+
     for i in range(nlayers):
-        vinc = b[i].shape[0]*b[i].shape[1]
-        b[i] = np.reshape(v[vcount:vcount+vinc],(b[i].shape[0],b[i].shape[1]))
-        vcount+= vinc
-    
-    return W, b   
+        vinc = W[i].shape[0] * W[i].shape[1]
+        W[i] = np.reshape(v[vcount:vcount + vinc], (W[i].shape[0], W[i].shape[1]))
+        vcount += vinc
 
+    for i in range(nlayers):
+        vinc = b[i].shape[0] * b[i].shape[1]
+        b[i] = np.reshape(v[vcount:vcount + vinc], (b[i].shape[0], b[i].shape[1]))
+        vcount += vinc
 
+    return W, b
```

### Comparing `hipersim-0.0.9/src/hipersim/turbgen/constrain_field.py` & `hipersim-0.1.0/src/hipersim/turbgen/constrain_field_1d.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,453 +1,418 @@
 # -*- coding: utf-8 -*-
 """
 Created on Mon May  3 11:39:55 2021
 
 @author: nkdi
 """
 
-def constrain_field(Constraints,u = None,v = None,w = None, BaseName = 'Turb', \
-                        alphaepsilon = 1,L = 30,Gamma = 3, Nx = 8192, Ny = 32, Nz = 32, \
-                        dx = 1,dy = 1,dz = 1,SaveToFile = 0, UseNormalization = 0, TurbOptions = None):
 
+def constrain_field_1d(Constraints, Component=None, c=None, BaseName='Turb',
+                       alphaepsilon=1, L=30, Gamma=3, Nx=8192, Ny=32, Nz=32,
+                       dx=1, dy=1, dz=1, SaveToFile=0, UseNormalization=0, TurbOptions=None):
     import numpy as np
     import time
 
     '''
-    Parse inputs 
+    Parse inputs
     '''
-    
+    if Component is None:
+        Component = 'u'
+        print('Warning: the turbulence component to be constrained was not specified.')
+        print('Assuming u-component.')
+
     if TurbOptions is None:
         SeedNo = 0
         HighFreqComp = 0
     else:
         if 'SeedNo' not in TurbOptions:
             SeedNo = 0
         else:
             SeedNo = TurbOptions['SeedNo']
-            
+
         if 'HighFreqComp' not in TurbOptions:
             HighFreqComp = 0
         else:
             HighFreqComp = TurbOptions['HighFreqComp']
-    
-    if ((u is None) | (v is None) | (w is None)):
-        if 'Udatafile' not in TurbOptions:
-            print('Source turbulence boxes for constrained simulation do not exist.')
-            print('Generating turbulence boxes:')
-            '''
-            ======================================================================================
-            If not given as inputs, load turbulence boxes from files or generate them if necessary
-            ======================================================================================'''
-            from hipersim.turbgen.generate_field import generate_field 
-            u,v,w = generate_field(BaseName,alphaepsilon,L,Gamma,SeedNo,Nx,Ny,Nz,dx,dy,dz, \
-                                    HighFreqComp, SaveToFile = 0)
-        else:
-            '''
-            Load source turbulence boxes 
-            '''
-            u = np.fromfile(TurbOptions['Udatafile'],dtype = 'single').reshape((Nx,Ny,Nz))
-            v = np.fromfile(TurbOptions['Udatafile'],dtype = 'single').reshape((Nx,Ny,Nz))
-            w = np.fromfile(TurbOptions['Udatafile'],dtype = 'single').reshape((Nx,Ny,Nz))
-            
-
-    # from generate_field import generate_field
-    # Nx = 1024
-    # Ny = 32
-    # Nz = 32
-    # dx = 2
-    # dy = 4
-    # dz = 4
-    # L = 30
-    # Gamma = 3
-    # alphaepsilon = 1
-    # SeedNo = 10
-    # HighFreqComp = 1
-    # SaveToFile = 1
-    # BaseName = 'Turb'
-    # HighFreqCompCheat = 1
-    # UseNormalization = 0
-    # u,v,w = generate_field(BaseName,alphaepsilon,L,Gamma,SeedNo,Nx,Ny,Nz,dx,dy,dz, \
-    #                         HighFreqComp, SaveToFile = 0)
-    # Xconstraints = np.atleast_2d(np.arange(1,2000,4)).T
-    # Yconstraints1 = 60*np.ones(Xconstraints.shape)
-    # Zconstraints1 = 10*np.ones(Xconstraints.shape)
-    # Yconstraints2 = 10*np.ones(Xconstraints.shape)
-    # Zconstraints2 = 60*np.ones(Xconstraints.shape)
-    # Uconstraints = 10*np.exp(-0.5*( (Xconstraints - 1000)/200)**2)
-    # Vconstraints = -5*np.exp(-0.5*( (Xconstraints - 1000)/200)**2)
-    # Wconstraints = -2*np.exp(-0.5*( (Xconstraints - 1000)/200)**2)
-    # Constraints = np.concatenate([np.concatenate([Xconstraints, Xconstraints]), 
-    #                               np.concatenate([Yconstraints1, Yconstraints2]),
-    #                               np.concatenate([Zconstraints1, Zconstraints2]),
-    #                               np.concatenate([Uconstraints, -Uconstraints]),
-    #                               np.concatenate([Vconstraints, -Vconstraints]),
-    #                               np.concatenate([Wconstraints, -Wconstraints])],axis = 1)
-        
 
-    
-    ''' 
+    if (c is None):
+        if Component == 'u':
+            if 'Udatafile' not in TurbOptions:
+                print('Source turbulence boxes for constrained simulation do not exist.')
+                print('Generating turbulence boxes:')
+                '''
+                ======================================================================================
+                If not given as inputs, load turbulence boxes from files or generate them if necessary
+                ======================================================================================'''
+                from hipersim.turbgen.generate_field import generate_field
+                # from . generate_field import generate_field
+                # from generate_field import generate_field
+                u, v, w = generate_field(BaseName, alphaepsilon, L, Gamma, SeedNo, Nx, Ny, Nz, dx, dy, dz,
+                                         HighFreqComp, SaveToFile=0)
+                c = u
+            else:
+                '''
+                Load source turbulence boxes
+                '''
+                c = np.fromfile(TurbOptions['Udatafile'], dtype='single').reshape((Nx, Ny, Nz))
+        if Component == 'v':
+            if 'Vdatafile' not in TurbOptions:
+                print('Source turbulence boxes for constrained simulation do not exist.')
+                print('Generating turbulence boxes:')
+                '''
+                ======================================================================================
+                If not given as inputs, load turbulence boxes from files or generate them if necessary
+                ======================================================================================'''
+                from hipersim.turbgen.generate_field import generate_field
+                # from . generate_field import generate_field
+                # from generate_field import generate_field
+                u, v, w = generate_field(BaseName, alphaepsilon, L, Gamma, SeedNo, Nx, Ny, Nz, dx, dy, dz,
+                                         HighFreqComp, SaveToFile=0)
+                c = v
+            else:
+                '''
+                Load source turbulence boxes
+                '''
+                c = np.fromfile(TurbOptions['Vdatafile'], dtype='single').reshape((Nx, Ny, Nz))
+        if Component == 'w':
+            if 'Wdatafile' not in TurbOptions:
+                print('Source turbulence boxes for constrained simulation do not exist.')
+                print('Generating turbulence boxes:')
+                '''
+                ======================================================================================
+                If not given as inputs, load turbulence boxes from files or generate them if necessary
+                ======================================================================================'''
+                from hipersim.turbgen.generate_field import generate_field
+                # from . generate_field import generate_field
+                # from generate_field import generate_field
+                u, v, w = generate_field(BaseName, alphaepsilon, L, Gamma, SeedNo, Nx, Ny, Nz, dx, dy, dz,
+                                         HighFreqComp, SaveToFile=0)
+                c = w
+            else:
+                '''
+                Load source turbulence boxes
+                '''
+                c = np.fromfile(TurbOptions['Wdatafile'], dtype='single').reshape((Nx, Ny, Nz))
+
+    '''
     ===============================================
     APPLY CONSTRAINTS
     ==============================================='''
-    
+
     '''
     ====================================================================
      COMPUTE MANN TENSOR VALUES, THEN IFFT TO GET CORRELATIONS
     ===================================================================='''
     print('Computing Mann tensor / correlation arrays for constrained simulation:')
-    
+
     from hipersim.turbgen.manntensor import manntensorcomponents
+    # from . manntensor import manntensorcomponents
     tstart = time.time()
-    R0uu = np.zeros((Nx,2*Ny,2*Nz), dtype = 'cfloat')
-    R0vv = np.zeros((Nx,2*Ny,2*Nz), dtype = 'cfloat')
-    R0ww = np.zeros((Nx,2*Ny,2*Nz), dtype = 'cfloat')
-    R0uw = np.zeros((Nx,2*Ny,2*Nz), dtype = 'cfloat')
-    
+    R0 = np.zeros((Nx, 2 * Ny, 2 * Nz), dtype='cfloat')
+
     '''
     The u-v, and v-w components are not considered because Rho_uv and Rho_vw
     are zero in the Mann turbulence model
     '''
     pi = np.pi
-    k1sim = np.concatenate([np.arange(0,Nx),np.arange(-Nx,0)])*(pi/(Nx*dx))
-    k2sim = np.concatenate([np.arange(0,Ny),np.arange(-Ny,0)])*(pi/(Ny*dy))
-    k3sim = np.concatenate([np.arange(0,Nz),np.arange(-Nz,0)])*(pi/(Nz*dz))
-    
-    k2simgrid,k3simgrid = np.meshgrid(k2sim,k3sim)
+    k1sim = np.concatenate([np.arange(0, Nx), np.arange(-Nx, 0)]) * (pi / (Nx * dx))
+    k2sim = np.concatenate([np.arange(0, Ny), np.arange(-Ny, 0)]) * (pi / (Ny * dy))
+    k3sim = np.concatenate([np.arange(0, Nz), np.arange(-Nz, 0)]) * (pi / (Nz * dz))
+
+    k2simgrid, k3simgrid = np.meshgrid(k2sim, k3sim)
     '''
     Only half of the wave numbers are considered, it is considered that
-    the correlation will be symmetric about k1 = 0 
+    the correlation will be symmetric about k1 = 0
     '''
-    for ik1 in range(Nx):    
-        Phi11ij, Phi22ij, Phi33ij, __, Phi13ij, __ = manntensorcomponents(k1sim[ik1]*np.ones(k2simgrid.shape),k2simgrid,k3simgrid,Gamma,L,alphaepsilon,2)
-        R0uu[ik1,:,:] = np.fft.ifft2(Phi11ij,axes = (0,1))
-        R0vv[ik1,:,:] = np.fft.ifft2(Phi22ij,axes = (0,1))
-        R0ww[ik1,:,:] = np.fft.ifft2(Phi33ij,axes = (0,1))
-        R0uw[ik1,:,:] = np.fft.ifft2(Phi13ij,axes = (0,1))
-                   
-    Ruu = np.zeros((2*Nx,Ny,Nz))
-    Rvv = np.zeros((2*Nx,Ny,Nz))
-    Rww = np.zeros((2*Nx,Ny,Nz))
-    Ruw = np.zeros((2*Nx,Ny,Nz))
+    if Component == 'u':
+        for ik1 in range(Nx):
+            Phi11ij, __, __, __, __, __ = manntensorcomponents(
+                k1sim[ik1] * np.ones(k2simgrid.shape), k2simgrid, k3simgrid, Gamma, L, alphaepsilon, 2)
+            R0[ik1, :, :] = np.fft.ifft2(Phi11ij, axes=(0, 1))
+    if Component == 'v':
+        for ik1 in range(Nx):
+            __, Phi22ij, __, __, __, __ = manntensorcomponents(
+                k1sim[ik1] * np.ones(k2simgrid.shape), k2simgrid, k3simgrid, Gamma, L, alphaepsilon, 2)
+            R0[ik1, :, :] = np.fft.ifft2(Phi22ij, axes=(0, 1))
+    if Component == 'w':
+        for ik1 in range(Nx):
+            __, __, Phi33ij, __, __, __ = manntensorcomponents(
+                k1sim[ik1] * np.ones(k2simgrid.shape), k2simgrid, k3simgrid, Gamma, L, alphaepsilon, 2)
+            R0[ik1, :, :] = np.fft.ifft2(Phi33ij, axes=(0, 1))
+
+    R = np.zeros((2 * Nx, Ny, Nz))
     for ik2 in range(Ny):
         for ik3 in range(Nz):
-            ''' 
+            '''
             !!! Needs to be checked !!!
-            Changing the choice of where we apply the complex conjugate ends up with 
+            Changing the choice of where we apply the complex conjugate ends up with
             somewhat different constrained fields '''
-            Ruu[:,ik2,ik3] = np.real(np.fft.ifft(np.concatenate([np.conj(R0uu[:,ik2,ik3]), np.flip((R0uu[:,ik2,ik3]))])))
-            Rvv[:,ik2,ik3] = np.real(np.fft.ifft(np.concatenate([np.conj(R0vv[:,ik2,ik3]), np.flip((R0vv[:,ik2,ik3]))])))
-            Rww[:,ik2,ik3] = np.real(np.fft.ifft(np.concatenate([np.conj(R0ww[:,ik2,ik3]), np.flip((R0ww[:,ik2,ik3]))])))
-            Ruw[:,ik2,ik3] = np.real(np.fft.ifft(np.concatenate([np.conj(R0uw[:,ik2,ik3]), np.flip((R0uw[:,ik2,ik3]))])))
-    
-    Ruu = Ruu[:Nx,:Ny,:Nz]
-    Rvv = Rvv[:Nx,:Ny,:Nz]
-    Rww = Rww[:Nx,:Ny,:Nz]
-    Ruw = Ruw[:Nx,:Ny,:Nz]
-    
-    Ruw = Ruw/( np.sqrt(Ruu[0,0,0]*Rww[0,0,0]) )
-    Ruu = Ruu/Ruu[0,0,0]
-    Rvv = Rvv/Rvv[0,0,0]
-    Rww = Rww/Rww[0,0,0]
-    
-    del R0uu, R0vv, R0ww, R0uw # Clear memory from unnecessary variables        
-            
+            R[:, ik2, ik3] = np.real(np.fft.ifft(np.concatenate(
+                [np.conj(R0[:, ik2, ik3]), np.flip((R0[:, ik2, ik3]))])))
+
+    R = R[:Nx, :Ny, :Nz]
+    R = R / R[0, 0, 0]
+
+    del R0  # Clear memory from unnecessary variables
+
     t1 = time.time()
     print('Correlation computations complete')
-    print('Time elapsed is ' + str(t1-tstart))
-    
+    print('Time elapsed is ' + str(t1 - tstart))
+
     '''
     ================================================================
      Compute distances, normalize wind fields and constraint fields
     ================================================================'''
-    
-    
+
     if UseNormalization == 1:
-        varUdata = np.var(u)
-        muUdata = np.mean(u)
+        varUdata = np.var(c)
+        muUdata = np.mean(c)
         stdUdata = np.sqrt(varUdata)
-        Unorm = (u - muUdata)/varUdata
-        varVdata = np.var(v)
-        muVdata = np.mean(v)
-        stdVdata = np.sqrt(varVdata)
-        Vnorm = (v - muVdata)/varVdata
-        varWdata = np.var(w)
-        muWdata = np.mean(w)
-        stdWdata = np.sqrt(varWdata)
-        Wnorm = (w - muWdata)/varWdata    
-        ConstraintValuesUNorm = (Constraints[:,3] - muUdata)/stdUdata
-        ConstraintValuesVNorm = (Constraints[:,4] - muVdata)/stdVdata
-        ConstraintValuesWNorm = (Constraints[:,5] - muWdata)/stdWdata
+        Unorm = (c - muUdata) / varUdata
+        ConstraintValuesUNorm = (Constraints[:, 3] - muUdata) / stdUdata
     else:
-        ConstraintValuesUNorm = Constraints[:,3]
-        ConstraintValuesVNorm = Constraints[:,4]
-        ConstraintValuesWNorm = Constraints[:,5]
-        Unorm = u
-        Vnorm = v
-        Wnorm = w
-    
-    #del u, v, w
-    
+        ConstraintValuesUNorm = Constraints[:, 3]
+        Unorm = c
+
+    # del u, v, w
+
     '''
     ==========================================
      ASSEMBLE CONSTRAINT COVARIANCE MATRIX
     =========================================='''
     print('Populating covariance matrix for the constraints:')
-    Clocx = np.rint(Constraints[:,0]/dx)
-    Clocy = np.rint(Constraints[:,1]/dy)
-    Clocz = np.rint(Constraints[:,2]/dz)
+    Clocx = np.rint(Constraints[:, 0] / dx)
+    Clocy = np.rint(Constraints[:, 1] / dy)
+    Clocz = np.rint(Constraints[:, 2] / dz)
     '''
     ---------------------------------
      Eliminate overlapping constraints
     ---------------------------------'''
     ClocA = np.concatenate([np.atleast_2d(Clocx), np.atleast_2d(Clocy), np.atleast_2d(Clocz)]).T
-    __,ClocIndex = np.unique(ClocA,axis=0,return_index = True)
-    Constraints = Constraints[ClocIndex,:]
+    __, ClocIndex = np.unique(ClocA, axis=0, return_index=True)
+    Constraints = Constraints[ClocIndex, :]
     Clocx = Clocx[ClocIndex]
     Clocy = Clocy[ClocIndex]
     Clocz = Clocz[ClocIndex]
     ConstraintValuesUNorm = ConstraintValuesUNorm[ClocIndex]
-    ConstraintValuesVNorm = ConstraintValuesVNorm[ClocIndex]
-    ConstraintValuesWNorm = ConstraintValuesWNorm[ClocIndex]
     Nconstraints = Constraints.shape[0]
-    
+
     '''
     ---------------------------------------------
      Eliminate constraints too close to each other
     ---------------------------------------------'''
-    Xdist = np.dot(np.atleast_2d(Constraints[:,0]).T,np.ones([1,Nconstraints])) - np.dot(np.ones([Nconstraints,1]),np.atleast_2d(Constraints[:,0]))
-    Ydist = np.dot(np.atleast_2d(Constraints[:,1]).T,np.ones([1,Nconstraints])) - np.dot(np.ones([Nconstraints,1]),np.atleast_2d(Constraints[:,1]))
-    Zdist = np.dot(np.atleast_2d(Constraints[:,2]).T,np.ones([1,Nconstraints])) - np.dot(np.ones([Nconstraints,1]),np.atleast_2d(Constraints[:,2]))
-    
+    Xdist = np.dot(np.atleast_2d(Constraints[:, 0]).T, np.ones([1, Nconstraints])) - \
+        np.dot(np.ones([Nconstraints, 1]), np.atleast_2d(Constraints[:, 0]))
+    Ydist = np.dot(np.atleast_2d(Constraints[:, 1]).T, np.ones([1, Nconstraints])) - \
+        np.dot(np.ones([Nconstraints, 1]), np.atleast_2d(Constraints[:, 1]))
+    Zdist = np.dot(np.atleast_2d(Constraints[:, 2]).T, np.ones([1, Nconstraints])) - \
+        np.dot(np.ones([Nconstraints, 1]), np.atleast_2d(Constraints[:, 2]))
+
     Rdist = np.sqrt(Xdist**2 + Ydist**2 + Zdist**2)
-    Rlimit = max( [L/10, min([dx, dy, dz])])
+    Rlimit = max([L / 10, min([dx, dy, dz])])
     Rexceed = (Rdist > 0) & (Rdist < Rlimit)
-    ValidDistIndex = np.full((Rdist.shape[0]),True,dtype = 'Bool')
+    ValidDistIndex = np.full((Rdist.shape[0]), True, dtype='bool')
     for i in range(Nconstraints):
-        if np.any(Rexceed[i,:i]):
-            Rexceed[i,:] = 0
-            Rexceed[:,i] = 0
+        if np.any(Rexceed[i, :i]):
+            Rexceed[i, :] = 0
+            Rexceed[:, i] = 0
             ValidDistIndex[i] = False
-    Constraints = Constraints[ValidDistIndex,:]
+    Constraints = Constraints[ValidDistIndex, :]
     Clocx = Clocx[ValidDistIndex].astype('int')
     Clocy = Clocy[ValidDistIndex].astype('int')
     Clocz = Clocz[ValidDistIndex].astype('int')
     ConstraintValuesUNorm = ConstraintValuesUNorm[ValidDistIndex]
-    ConstraintValuesVNorm = ConstraintValuesVNorm[ValidDistIndex]
-    ConstraintValuesWNorm = ConstraintValuesWNorm[ValidDistIndex]
     Nconstraints = Constraints.shape[0]
-    
+
     del Rdist, Rexceed, ValidDistIndex
-    
-    
+
     '''
     -----------------------------
      Assemble u-v-w-correlation matrix
     -----------------------------'''
-    CorrCMannUVW = np.zeros((3*Nconstraints,3*Nconstraints))
-    
+    CorrCMannU = np.zeros((Nconstraints, Nconstraints))
+
     for iC in range(Nconstraints):
         xloci = Clocx[iC]
         yloci = Clocy[iC]
         zloci = Clocz[iC]
-        xlocCij = np.abs(xloci-Clocx).astype('int')
-        ylocCij = np.abs(yloci-Clocy).astype('int')
-        zlocCij = np.abs(zloci-Clocz).astype('int')
-        
-        CorrUUij = Ruu[xlocCij,ylocCij,zlocCij]
-        CorrVVij = Rvv[xlocCij,ylocCij,zlocCij]
-        CorrWWij = Rww[xlocCij,ylocCij,zlocCij]
-        CorrUWij = Ruw[xlocCij,ylocCij,zlocCij]
-    
+        xlocCij = np.abs(xloci - Clocx).astype('int')
+        ylocCij = np.abs(yloci - Clocy).astype('int')
+        zlocCij = np.abs(zloci - Clocz).astype('int')
+
+        CorrUUij = R[xlocCij, ylocCij, zlocCij]
+
         # CorrUUij = np.zeros(Nconstraints)
         # CorrVVij = np.zeros(Nconstraints)
         # CorrWWij = np.zeros(Nconstraints)
         # CorrUWij = np.zeros(Nconstraints)
         # for jC in range(Nconstraints):
         #     CorrUUij[jC] = Ruu[xlocCij[jC],ylocCij[jC],zlocCij[jC]]
         #     CorrVVij[jC] = Rvv[xlocCij[jC],ylocCij[jC],zlocCij[jC]]
         #     CorrWWij[jC] = Rww[xlocCij[jC],ylocCij[jC],zlocCij[jC]]
         #     CorrUWij[jC] = Ruw[xlocCij[jC],ylocCij[jC],zlocCij[jC]]
-    
-        CorrCMannUVW[:Nconstraints,iC] = CorrUUij
-        CorrCMannUVW[iC,:Nconstraints] = CorrUUij
-        CorrCMannUVW[Nconstraints:2*Nconstraints,Nconstraints + iC] = CorrVVij
-        CorrCMannUVW[Nconstraints + iC,Nconstraints:2*Nconstraints] = CorrVVij    
-        CorrCMannUVW[2*Nconstraints:,2*Nconstraints + iC] = CorrWWij
-        CorrCMannUVW[2*Nconstraints + iC,2*Nconstraints:] = CorrWWij    
-        CorrCMannUVW[2*Nconstraints:,iC] = CorrUWij
-        CorrCMannUVW[iC,2*Nconstraints:] = CorrUWij    
-           
-        
+
+        CorrCMannU[:Nconstraints, iC] = CorrUUij
+        CorrCMannU[iC, :Nconstraints] = CorrUUij
+
     t2 = time.time()
     print('Constraint-constraint covariance matrix has been assembled')
-    print('Time elapsed is ' + str(t2-t1))
-    
+    print('Time elapsed is ' + str(t2 - t1))
+
     '''
     =========================================================
      APPLY CONSTRAINT EQUATIONS TO COMPUTE THE RESIDUAL FIELD
     =========================================================
-     Using eq.(2) from Dimitrov & Natarajan (2016) to compute 
+     Using eq.(2) from Dimitrov & Natarajan (2016) to compute
      the residual field which is to be added to the unconstrained
      field in order to obtain the constrained result.
-    
+
      Due to memory limitations, eq. (2) is evaluated in batches intended
      to avoid the need of fully assembling the first term in the equation,
      which is a matrix with size (Nx*Ny*Nz)x(Nconstraints).
-     First, the product of the second and third term is evaluated, 
-     then it is multiplied piecewise to a subset of the rows of the 
+     First, the product of the second and third term is evaluated,
+     then it is multiplied piecewise to a subset of the rows of the
      first term.
     '''
     print('Applying constraints...')
-    ConstraintValuesUVWNorm = np.concatenate([ConstraintValuesUNorm, ConstraintValuesVNorm, ConstraintValuesWNorm])
-    UVWcontemporaneous = np.zeros((3*Nconstraints))
-    UVWcontemporaneous[:Nconstraints] = Unorm[Clocx,Clocy,Clocz]
-    UVWcontemporaneous[Nconstraints:2*Nconstraints] = Vnorm[Clocx,Clocy,Clocz]
-    UVWcontemporaneous[2*Nconstraints:] = Wnorm[Clocx,Clocy,Clocz]
-    
+    Ucontemporaneous = Unorm[Clocx, Clocy, Clocz]
+
     '''
-     Computing the product of the second and third terms in eq.(2) in 
+     Computing the product of the second and third terms in eq.(2) in
      Dimitrov & Natarajan (2016)
     '''
-    
-    CConstUVW = np.linalg.solve(CorrCMannUVW, (ConstraintValuesUVWNorm - UVWcontemporaneous))
+
+    CConstU = np.linalg.solve(CorrCMannU, (ConstraintValuesUNorm - Ucontemporaneous))
     # CConstUVW = np.dot(np.linalg.inv(CorrCMannUVW), ConstraintValuesUVWNorm - UVWcontemporaneous)
-    
-    CConstU = np.atleast_2d(CConstUVW[:Nconstraints]).T
-    CConstV = np.atleast_2d(CConstUVW[Nconstraints:2*Nconstraints]).T
-    CConstW = np.atleast_2d(CConstUVW[2*Nconstraints:]).T
-    del CorrCMannUVW
-    
-    Ruu = Ruu.reshape(Nx*Ny*Nz)
-    Rvv = Rvv.reshape(Nx*Ny*Nz)
-    Rww = Rww.reshape(Nx*Ny*Nz)
-    Ruw = Ruw.reshape(Nx*Ny*Nz)
-    
-    ygrid, xgrid, zgrid = np.meshgrid(np.arange(Ny),np.arange(Nx),np.arange(Nz))
-    xvect = xgrid.reshape(Nx*Ny*Nz)
-    yvect = ygrid.reshape(Nx*Ny*Nz)
-    zvect = zgrid.reshape(Nx*Ny*Nz)
-    
+
+    CConstU = np.atleast_2d(CConstU[:Nconstraints]).T
+    del CorrCMannU
+
+    R = R.reshape(Nx * Ny * Nz)
+
+    ygrid, xgrid, zgrid = np.meshgrid(np.arange(Ny), np.arange(Nx), np.arange(Nz))
+    xvect = xgrid.reshape(Nx * Ny * Nz)
+    yvect = ygrid.reshape(Nx * Ny * Nz)
+    zvect = zgrid.reshape(Nx * Ny * Nz)
+
     del xgrid, ygrid, zgrid
-    
-    ures = np.zeros(Nx*Ny*Nz)
-    vres = np.zeros(Nx*Ny*Nz)
-    wres = np.zeros(Nx*Ny*Nz)
-    
+
+    ures = np.zeros(Nx * Ny * Nz)
+
     # Npoints = Nx*Ny*Nz
-    
+
     for iC in range(Nconstraints):
         # dxCov = np.abs(xvect - Clocx[iC])
         # dyCov = np.abs(yvect - Clocy[iC])
         # dzCov = np.abs(zvect - Clocz[iC])
-        dlinear = np.abs(xvect - Clocx[iC])*(Ny*Nz) + np.abs(yvect - Clocy[iC])*Ny + np.abs(zvect - Clocz[iC])
-        CorrUUi = Ruu[dlinear]
-        CorrVVi = Rvv[dlinear]
-        CorrWWi = Rww[dlinear]
-        CorrUWi = Ruw[dlinear]
-        ures+= CorrUUi*CConstU[iC] + CorrUWi*CConstW[iC]
-        vres+= CorrVVi*CConstV[iC]
-        wres+= CorrUWi*CConstU[iC] + CorrWWi*CConstW[iC]
-        
-    Uconstrained = Unorm + np.reshape(ures,(Nx,Ny,Nz))
-    Vconstrained = Vnorm + np.reshape(vres,(Nx,Ny,Nz))
-    Wconstrained = Wnorm + np.reshape(wres,(Nx,Ny,Nz))
-    
-    
+        dlinear = np.abs(xvect - Clocx[iC]) * (Ny * Nz) + np.abs(yvect - Clocy[iC]) * Ny + np.abs(zvect - Clocz[iC])
+        CorrUUi = R[dlinear]
+        ures += CorrUUi * CConstU[iC]
+
+    Uconstrained = Unorm + np.reshape(ures, (Nx, Ny, Nz))
+
     '''
     OLDER IMPLEMENTATION - SIGNIFICANTLY FASTER IN MATLAB BUT SLOW IN PYTHON
     DUE TO ARRAY INDEXING SPEED '''
-    
+
     # Uconstrained = np.zeros((Nx,Ny,Nz))
     # Vconstrained = np.zeros((Nx,Ny,Nz))
-    # Wconstrained = np.zeros((Nx,Ny,Nz))   
-    
+    # Wconstrained = np.zeros((Nx,Ny,Nz))
+
     # CorrUUxyz = np.zeros((Nx,Nconstraints))
     # CorrVVxyz = np.zeros((Nx,Nconstraints))
     # CorrUVxyz = np.zeros((Nx,Nconstraints))
     # CorrVWxyz = np.zeros((Nx,Nconstraints))
     # CorrUWxyz = np.zeros((Nx,Nconstraints))
-    # CorrWWxyz = np.zeros((Nx,Nconstraints)) 
-    
+    # CorrWWxyz = np.zeros((Nx,Nconstraints))
+
     # for yloc in range(Ny):
     #     for zloc in range(Nz):
     #         xloc = np.arange(Nx)
     #         dyCov = np.abs(yloc - Clocy).astype('int')
     #         dzCov = np.abs(zloc - Clocz).astype('int')
     #         '''
     #         !!! This loop needs optimization !!!
     #         '''
     #         for iC in range(Nconstraints):
     #             dxCov = np.abs(xloc - Clocx[iC])
     #             CorrUUxyz[:,iC] = Ruu[dxCov,dyCov[iC],dzCov[iC]]
     #             CorrVVxyz[:,iC] = Rvv[dxCov,dyCov[iC],dzCov[iC]]
     #             CorrUWxyz[:,iC] = Ruw[dxCov,dyCov[iC],dzCov[iC]]
     #             CorrWWxyz[:,iC] = Rww[dxCov,dyCov[iC],dzCov[iC]]
-    
+
     #         '''
     #           Computing the product of the first term in eq. (2) with the
     #           second and third terms - for one point in the y-z plane at a
     #           time.
-    #         '''        
+    #         '''
     #         CtermUYZ = np.dot(CorrUUxyz,CConstU) + np.dot(CorrUVxyz,CConstV) + np.dot(CorrUWxyz,CConstW) # Residual field term - u
     #         CtermVYZ = np.dot(CorrUVxyz,CConstU) + np.dot(CorrVVxyz,CConstV) + np.dot(CorrVWxyz,CConstW) # Residual field term - v
-    #         CtermWYZ = np.dot(CorrUWxyz,CConstU) + np.dot(CorrVWxyz,CConstV) + np.dot(CorrWWxyz,CConstW) # Residual field term - w
-    
+    # CtermWYZ = np.dot(CorrUWxyz,CConstU) + np.dot(CorrVWxyz,CConstV) +
+    # np.dot(CorrWWxyz,CConstW) # Residual field term - w
+
     #         Uconstrained[:,yloc,zloc] = Unorm[:,yloc,zloc] + np.squeeze(CtermUYZ)
     #         Vconstrained[:,yloc,zloc] = Vnorm[:,yloc,zloc] + np.squeeze(CtermVYZ)
     #         Wconstrained[:,yloc,zloc] = Wnorm[:,yloc,zloc] + np.squeeze(CtermWYZ)
-    
+
     # if Options.UseNormalization == 1
     #     Uconstrained = Uconstrained.*stdUdata + muUdata;
     #     Vconstrained = Vconstrained.*stdVdata + muVdata;
     #     Wconstrained = Wconstrained.*stdWdata + muWdata;
     # end
-    
+
     t3 = time.time()
     print('Constraint application complete')
     print('Time elapsed is ' + str(t3 - t2))
-    
+
     if SaveToFile == 1:
-        Uconstrained.reshape(Nx*Ny*Nz).astype('single').tofile(BaseName + '_' + str(SeedNo) + '_c_u' + '_py.bin',sep = '')
-        Vconstrained.reshape(Nx*Ny*Nz).astype('single').tofile(BaseName + '_' + str(SeedNo) + '_c_v' + '_py.bin',sep = '')
-        Wconstrained.reshape(Nx*Ny*Nz).astype('single').tofile(BaseName + '_' + str(SeedNo) + '_c_w' + '_py.bin',sep = '')
-    
-    
+        Uconstrained.reshape(
+            Nx *
+            Ny *
+            Nz).astype('single').tofile(
+            BaseName +
+            '_' +
+            str(SeedNo) +
+            '_c_' +
+            Component +
+            '_py.bin',
+            sep='')
+
     # if nargout > 0
     #     u = Uconstrained;
     #     v = Vconstrained;
     #     w = Wconstrained;
     # end
-    
+
     # if Options.SaveToFile == 1
     #     disp('Saving resulting turbulence boxes:')
     #     clear Unorm Vnorm Wnorm CorrUUxyz CorrVVxyz CorrWWxyz CorrUVxyz CorrUWxyz CorrVWxyz
     #     Uvect = zeros(Nx*Ny*Nz,1);
     #     Vvect = zeros(Nx*Ny*Nz,1);
     #     Wvect = zeros(Nx*Ny*Nz,1);
     #     for xloc = 1:Nx
     #         for yloc = 1:Ny
     #             dataindex = Ny*Nz*(xloc - 1) + Ny*(yloc-1);
     #             UperZ = Uconstrained(xloc,yloc,:);
     #             VperZ = Vconstrained(xloc,yloc,:);
     #             WperZ = Wconstrained(xloc,yloc,:);
-    #             Uvect(dataindex+1:dataindex+Nz) = UperZ;                        
-    #             Vvect(dataindex+1:dataindex+Nz) = VperZ;                        
-    #             Wvect(dataindex+1:dataindex+Nz) = WperZ;                        
+    #             Uvect(dataindex+1:dataindex+Nz) = UperZ;
+    #             Vvect(dataindex+1:dataindex+Nz) = VperZ;
+    #             Wvect(dataindex+1:dataindex+Nz) = WperZ;
     #         end
-    #     end    
+    #     end
     #     OutputFileU = fopen([Input.BaseName '_' num2str(SeedNo) '_c_u.bin'],'w');
-    #     fwrite(OutputFileU,Uvect,'single');    
+    #     fwrite(OutputFileU,Uvect,'single');
     #     fclose(OutputFileU);
-    #     OutputFileV = fopen([Input.BaseName '_' num2str(SeedNo)  '_c_v.bin'],'w');    
-    #     fwrite(OutputFileV,Vvect,'single');    
+    #     OutputFileV = fopen([Input.BaseName '_' num2str(SeedNo)  '_c_v.bin'],'w');
+    #     fwrite(OutputFileV,Vvect,'single');
     #     fclose(OutputFileV);
     #     OutputFileW = fopen([Input.BaseName '_' num2str(SeedNo)  '_c_w.bin'],'w');
-    #     fwrite(OutputFileW,Wvect,'single');    
+    #     fwrite(OutputFileW,Wvect,'single');
     #     fclose(OutputFileW);
     #     disp('DONE!');
     # end
     tend = time.time()
     print('Constrained simulation complete')
-    print('Total time elapsed is ' + str(tend-tstart))
+    print('Total time elapsed is ' + str(tend - tstart))
 
-    return Uconstrained, Vconstrained, Wconstrained
+    return Uconstrained
```

### Comparing `hipersim-0.0.9/src/hipersim.egg-info/PKG-INFO` & `hipersim-0.1.0/src/hipersim.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 Metadata-Version: 2.1
 Name: hipersim
-Version: 0.0.9
+Version: 0.1.0
 Summary: A collection of wind energy simulation tools
 Home-page: https://gitlab.windenergy.dtu.dk/HiperSim/hipersim
 Author: Nikolay Dimitrov
 Author-email: nkdi@dtu.dk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hipersim
 
 ## Introduction
 Hipersim is a collection of tools for computationally-efficient simulation of Wind Energy problems using statistical and machine learning methods. Currently, the package contains the following submodules:
 
 - **turbgen**: 
     - Generation of 3D frozen turbulence fields ("turbulence boxes") with the Mann turbulence spectrum
     - Constrained turbulence field generation and application of constraints on pre-generated turbulence fields
 
 - **surrogates**:
     - A feedforward neural network toolbox, training and evaluation of feedforward neural networks. 
+	- A set of tools for surrogate-based modeling and analysis of wind farms
 
 ## Installation
 Hipersim is registered as installable Python package in PyPi.org. Installation happens automatically with the following command:
 
 pip install hipersim
 
 ## References
 
 ## License
 Hipersim uses the MIT License.
-
-
```

