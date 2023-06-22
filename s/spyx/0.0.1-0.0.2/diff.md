# Comparing `tmp/spyx-0.0.1.tar.gz` & `tmp/spyx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyx-0.0.1.tar", last modified: Thu Jun 22 07:37:14 2023, max compression
+gzip compressed data, was "spyx-0.0.2.tar", last modified: Thu Jun 22 15:03:09 2023, max compression
```

## Comparing `spyx-0.0.1.tar` & `spyx-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 07:37:14.145033 spyx-0.0.1/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.1/LICENSE
--rw-rw-r--   0 legion    (1000) legion    (1000)      759 2023-06-22 07:37:14.145033 spyx-0.0.1/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      800 2023-06-22 07:32:11.000000 spyx-0.0.1/README.md
--rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-22 07:37:14.145033 spyx-0.0.1/setup.cfg
--rw-rw-r--   0 legion    (1000) legion    (1000)     1383 2023-06-22 07:36:55.000000 spyx-0.0.1/setup.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 07:37:14.145033 spyx-0.0.1/spyx/
--rw-rw-r--   0 legion    (1000) legion    (1000)       20 2023-06-21 21:10:32.000000 spyx-0.0.1/spyx/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-21 21:10:32.000000 spyx-0.0.1/spyx/_version.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     8386 2023-06-22 06:52:35.000000 spyx-0.0.1/spyx/actv.py
--rw-rw-r--   0 legion    (1000) legion    (1000)    11574 2023-06-22 06:48:24.000000 spyx-0.0.1/spyx/data.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     2663 2023-06-22 06:44:31.000000 spyx-0.0.1/spyx/loss.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     6586 2023-06-22 07:02:09.000000 spyx-0.0.1/spyx/nn.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 07:37:14.145033 spyx-0.0.1/spyx.egg-info/
--rw-rw-r--   0 legion    (1000) legion    (1000)      759 2023-06-22 07:37:14.000000 spyx-0.0.1/spyx.egg-info/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      272 2023-06-22 07:37:14.000000 spyx-0.0.1/spyx.egg-info/SOURCES.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-22 07:37:14.000000 spyx-0.0.1/spyx.egg-info/dependency_links.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-22 07:37:14.000000 spyx-0.0.1/spyx.egg-info/requires.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-22 07:37:14.000000 spyx-0.0.1/spyx.egg-info/top_level.txt
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 07:37:14.145033 spyx-0.0.1/tests/
--rw-rw-r--   0 legion    (1000) legion    (1000)      302 2023-06-22 07:15:06.000000 spyx-0.0.1/tests/test_networks.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 15:03:09.492961 spyx-0.0.2/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.2/LICENSE
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-22 15:03:09.492961 spyx-0.0.2/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      710 2023-06-22 08:40:57.000000 spyx-0.0.2/README.md
+-rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-22 15:03:09.492961 spyx-0.0.2/setup.cfg
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1384 2023-06-22 14:58:59.000000 spyx-0.0.2/setup.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 15:03:09.492961 spyx-0.0.2/spyx/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      188 2023-06-22 10:53:53.000000 spyx-0.0.2/spyx/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-21 21:10:32.000000 spyx-0.0.2/spyx/_version.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     8427 2023-06-22 11:03:16.000000 spyx-0.0.2/spyx/activation.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)    11549 2023-06-22 11:05:48.000000 spyx-0.0.2/spyx/data.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2663 2023-06-22 06:44:31.000000 spyx-0.0.2/spyx/loss.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     6673 2023-06-22 11:37:32.000000 spyx-0.0.2/spyx/nn.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 15:03:09.492961 spyx-0.0.2/spyx.egg-info/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-22 15:03:09.000000 spyx-0.0.2/spyx.egg-info/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      278 2023-06-22 15:03:09.000000 spyx-0.0.2/spyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-22 15:03:09.000000 spyx-0.0.2/spyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-22 15:03:09.000000 spyx-0.0.2/spyx.egg-info/requires.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-22 15:03:09.000000 spyx-0.0.2/spyx.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 15:03:09.492961 spyx-0.0.2/tests/
+-rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-22 08:36:33.000000 spyx-0.0.2/tests/test_networks.py
```

### Comparing `spyx-0.0.1/LICENSE` & `spyx-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spyx-0.0.1/PKG-INFO` & `spyx-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.1
+Version: 0.0.2
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Spyx is a compact library built on top of DeepMind's Haiku library, enabling easy construction of spiking neural network models.
```

### Comparing `spyx-0.0.1/README.md` & `spyx-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-🏗️🚧 This library is under construction with high probability of breaking changes and major restructuring over the next few months!🚧
+🏗️ 🚧 This library is under construction!🚧
 
 
 Welcome to Spyx, a library for Spiking Neural Networks in JAX!
 
 ![README Art](spyx.png "Title")
 
 Spyx is a compact library built on top of DeepMind's Haiku library, enabling easy construction of spiking neural network models.
```

### Comparing `spyx-0.0.1/setup.py` & `spyx-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
         "numpy",
     ],
 )
 
 # This call to setup() does all the work
 setup(
     name="spyx",
-    version="0.0.1",
+    version="0.0.2",
     description="Spyx: SNNs in JAX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kmheckel/spyx",
     author="Kade Heckel",
     author_email="example@email.com",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
     packages=["spyx"],
     include_package_data=True,
     install_requires=requires
 )
```

### Comparing `spyx-0.0.1/spyx/actv.py` & `spyx-0.0.2/spyx/activation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,57 @@
+import jax
+import jax.numpy as jnp
+import haiku as hk
+
+
 class ActivityRegularization(hk.Module):
     """
     Add state to the SNN to track the average number of spikes emitted per neuron per batch.
     """
 
     def __init__(self, name="ActReg"):
         super().__init__(name=name)
         
     def __call__(self, spikes):
         spike_count = hk.get_state("spike_count", [spikes.shape[-1]], init=jnp.zeros)
         hk.set_state("spike_count", spike_count + jnp.mean(spikes, axis=0))
         return spikes
 
 
-class Heaviside:
+class AdaSpike:
     """
-    This class implements the Heaviside activation function for a spiking neuron.
-    
-    The Heaviside function is a step function that takes a single argument. 
-    It returns 0 if the input is less than 0, and 1 if the input is greater than 0.
-    
-    The Heaviside function is often used in the context of spiking neurons because 
-    it can be used to model the firing of a neuron. When the input to the neuron 
-    (the sum of the weighted inputs) exceeds a certain threshold, the neuron fires, 
-    producing a spike of activity. This can be modeled as the Heaviside function, 
-    where the output is 0 when the input is below the threshold, and 1 when the input 
-    is above the threshold.
-    
-    Attributes:
-        scale_factor: A scaling factor that can be used to adjust the steepness of the 
-                      step function. Default is 25.
+    Simplified version of SuperSpike, dropping the power from the denominator.
+    Features an increasing scale factor with linear schedule, increasing the
+    sharpness of the surrogate gradient over time.
     """
-    
-    
-    
-    def __init__(self, scale_factor=25):
-        self.k = scale_factor
+
+    def __init__(self,  warmup_steps, growth_rate=0.5):
+        self.k = 1
+        self.gr = growth_rate
         
         @jax.custom_vjp
-        def f(U): # primal function
+        def f(U, k): # primal function
             return (U>0).astype(jnp.float16)
         
         # returns value, grad context
-        def f_fwd(U):
-            return f(U), ()
+        def f_fwd(U, k):
+            return f(U), (U, k)
             
-        # Straight Through Estimator
-        def f_bwd(U, grad):
-            return ( grad*U ) 
+        # accepts context, primal val
+        # not sure if k actually changes or it gets jit'ed and stays static..
+        def f_bwd(context, grad):
+            U, k = context
+            return (grad / (1+k*jnp.abs(U)) , )
             
         f.defvjp(f_fwd, f_bwd)
         self.f = f
         
     def __call__(self, U):
-        return self.f(U)
-
+        self.k += self.growth_rate
+        return self.f(U, self.k)
 
 # Surrogate functions
 class Arctan:
     """
     This class implements the Arctangent surrogate gradient activation function for a spiking neuron.
     
     The Arctangent function is a smooth function that approximates the step function. 
@@ -70,37 +64,106 @@
     
     Attributes:
         scale_factor: A scaling factor that can be used to adjust the steepness of the 
                       Arctangent function. Default is 2.
     """
     
 
-
-
     def __init__(self, scale_factor=2):
-        self.a = scale_factor
+        self.k = scale_factor
         
         @jax.custom_vjp
         def f(U): # primal function
             return (U>0).astype(jnp.float16)
         
         # returns value, grad context
         def f_fwd(U):
             return f(U), ()
             
         # Straight Through Estimator
         def f_bwd(U, grad):
-            return ( (1 / (jnp.pi * (1+(jnp.pi*U*a/2)**2))) * grad ) 
+            return ( (1 / (jnp.pi * (1+(jnp.pi*U*self.k/2)**2))) * grad ) 
             
         f.defvjp(f_fwd, f_bwd)
         self.f = f
         
     def __call__(self, U):
         return self.f(U) 
+
+class Boxcar:
+    """
+    Boxcar surrogate gradient activation function. Under construction.
+    """
+
+    def __init__(self, scale_factor=1):
+        self.k = scale_factor
+        
+        @jax.custom_vjp
+        def f(U): # primal function
+            return (U>0).astype(jnp.float16)
+        
+        # returns value, grad context
+        def f_fwd(U):
+            return f(U), U
+            
+        # Needs fixed.
+        def f_bwd(U, grad):
+            if jnp.abs(U) <= 0.5:
+                return ( 0.5 * grad )
+            return ( 0 ) 
+            
+        f.defvjp(f_fwd, f_bwd)
+        self.f = f
+        
+    def __call__(self, U):
+        return self.f(U)
+
+class Heaviside:
+    """
+    This class implements the Heaviside activation function for a spiking neuron.
+    
+    The Heaviside function is a step function that takes a single argument. 
+    It returns 0 if the input is less than 0, and 1 if the input is greater than 0.
     
+    The Heaviside function is often used in the context of spiking neurons because 
+    it can be used to model the firing of a neuron. When the input to the neuron 
+    (the sum of the weighted inputs) exceeds a certain threshold, the neuron fires, 
+    producing a spike of activity. This can be modeled as the Heaviside function, 
+    where the output is 0 when the input is below the threshold, and 1 when the input 
+    is above the threshold.
+    
+    Attributes:
+        scale_factor: A scaling factor that can be used to adjust the steepness of the 
+                      step function. Default is 25.
+    """
+    
+    
+    
+    def __init__(self, scale_factor=25):
+        self.k = scale_factor
+        
+        @jax.custom_vjp
+        def f(U): # primal function
+            return (U>0).astype(jnp.float16)
+        
+        # returns value, grad context
+        def f_fwd(U):
+            return f(U), ()
+            
+        # Straight Through Estimator
+        def f_bwd(U, grad):
+            return ( grad*U ) 
+            
+        f.defvjp(f_fwd, f_bwd)
+        self.f = f
+        
+    def __call__(self, U):
+        return self.f(U)
+
+
 class Sigmoid:
     """
     This class implements the Sigmoid surrogate gradient activation function for a spiking neuron.
     
     The Sigmoid function is a smooth function that approximates the step function. 
     It is used as a surrogate gradient for the step function in the context of spiking neurons. 
     The surrogate gradient is used during the backpropagation process to update the weights of the neuron.
@@ -177,69 +240,8 @@
         def f_bwd(U, grad):
             return (grad / (1+self.k*jnp.abs(U))**2 , )
             
         f.defvjp(f_fwd, f_bwd)
         self.f = f
         
     def __call__(self, U):
-        return self.f(U)
-    
-class AdaSpike:
-    """
-    Simplified version of SuperSpike, dropping the power from the denominator.
-    Features an increasing scale factor with linear schedule, increasing the
-    sharpness of the surrogate gradient over time.
-    """
-
-    def __init__(self,  warmup_steps, growth_rate=0.5):
-        self.k = 1
-        self.gr = growth_rate
-        
-        @jax.custom_vjp
-        def f(U, k): # primal function
-            return (U>0).astype(jnp.float16)
-        
-        # returns value, grad context
-        def f_fwd(U, k):
-            return f(U), (U, k)
-            
-        # accepts context, primal val
-        # not sure if k actually changes or it gets jit'ed and stays static..
-        def f_bwd(context, grad):
-            U, k = context
-            return (grad / (1+k*jnp.abs(U)) , )
-            
-        f.defvjp(f_fwd, f_bwd)
-        self.f = f
-        
-    def __call__(self, U):
-        self.k += self.growth_rate
-        return self.f(U, self.k)
-        
-
-class Boxcar:
-    """
-    Boxcar surrogate gradient activation function. Under construction.
-    """
-
-    def __init__(self, scale_factor=1):
-        self.k = scale_factor
-        
-        @jax.custom_vjp
-        def f(U): # primal function
-            return (U>0).astype(jnp.float16)
-        
-        # returns value, grad context
-        def f_fwd(U):
-            return f(U), U
-            
-        # Needs fixed.
-        def f_bwd(U, grad):
-            if jnp.abs(U) <= 0.5:
-                return ( 0.5 * grad )
-            return ( 0 ) 
-            
-        f.defvjp(f_fwd, f_bwd)
-        self.f = f
-        
-    def __call__(self, U):
-        return self.f(U)
+        return self.f(U)
```

### Comparing `spyx-0.0.1/spyx/data.py` & `spyx-0.0.2/spyx/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,75 +2,67 @@
 from tonic import datasets, transforms
 import torchvision as tv
 from torch.utils.data import DataLoader, Subset
 from sklearn.model_selection import train_test_split
 from collections import namedtuple
 from itertools import cycle
 
+import numpy as np
+import jax
+import jax.numpy as jnp
 
-State = namedtuple("State", "obs labels")
 
+State = namedtuple("State", "obs labels")
 
+# Here we scale the max probability to .8 so that we don't have inputs that are continually spiking.
+# might need to find a home for this in the lib.
+def rate_code(data, steps, key, max_r=0.8):
+    """Unrolls input data along axis 1 and converts to rate encoded spikes."""
 
-class SHD2Raster():
-    """ Tool for rastering SHD samples into frames."""
+    data = jnp.array(data, dtype=jnp.float16)
+    unrolled_data = jnp.repeat(data, steps, axis=1)
+    return jax.random.bernoulli(key, unrolled_data*max_r).astype(jnp.int8)
 
-    def __init__(self, encoding_dim, sample_T = 100):
-        self.encoding_dim = encoding_dim
-        self.sample_T = sample_T
-        
-    def __call__(self, events):
-        # tensor has dimensions (time_steps, encoding_dim)
-        tensor = np.zeros((events["t"].max()+1, self.encoding_dim), dtype=int)
-        np.add.at(tensor, (events["t"], events["x"]), 1)
-        #return tensor[:self.sample_T,:]
-        tensor = tensor[:self.sample_T,:]
-        return np.minimum(tensor, 1)
-    
 
-class shd_loader():
+class MNIST_loader():
     """
-    Dataloading wrapper for the Spiking Heidelberg Dataset.
+    Dataloader for the MNIST dataset, right now it is rate encoded.
+    
     """
 
-
     # Change this to allow a config dictionary of 
-    def __init__(self, batch_size=128, val_size=0.3):        
-        shd_timestep = 1e-6
-        shd_channels = 700
-        net_channels = 128
-        net_dt = 10e-3
-        sample_T = 100
+    def __init__(self, batch_size=32, val_size=0.3, key=0, download_dir='./MNIST'):
            
+        self.key = jax.random.PRNGKey(key)
+        self.sample_T = 64
+        self.spike_rate = 0.7
         self.val_size = val_size
         self.batch_size = batch_size
-        self.obs_shape = tuple([net_channels,])
-        self.act_shape = tuple([20,])
-        
-        transform = transforms.Compose([
-        transforms.Downsample(
-            time_factor=shd_timestep / net_dt,
-            spatial_factor=net_channels / shd_channels
-            ),
-            SHD2Raster(net_channels, sample_T = sample_T)
-        ])
+        self.obs_shape = (28,28)
+        self.act_shape = tuple([10,])
         
-        train_val_dataset = datasets.SHD("./data", train=True, transform=transform)
-        test_dataset = datasets.SHD("./data", train=False, transform=transform)
+        transform = tv.transforms.Compose([
+            tv.transforms.Resize(self.obs_shape),
+            tv.transforms.Grayscale(),
+            tv.transforms.ToTensor(),
+            tv.transforms.Normalize((0,), (1,))])
         
+        # fix this
+        train_val_dataset = tv.datasets.MNIST("./data", train=True, download=True, transform=transform)
+        test_dataset = tv.datasets.MNIST("./data", train=False, download=True, transform=transform)
         # create train/validation split here...
         # generate indices: instead of the actual data we pass in integers instead
         train_indices, val_indices = train_test_split(
-            range(len(train_val_dataset)),
-            test_size=self.val_size,
-            random_state=0,
-            shuffle=True # This really should be set externally!!!!!
+        range(len(train_val_dataset)),
+        test_size=self.val_size,
+        random_state=0,
+        shuffle=True
         )
-        
-        
+    
+    
         train_split = Subset(train_val_dataset, train_indices)
         self.train_len = len(train_indices)
         
         val_split = Subset(train_val_dataset, val_indices)
         self.val_len = len(val_indices)
                         
         self.test_len = len(test_dataset)
@@ -84,79 +76,67 @@
                           collate_fn=tonic.collation.PadTensors(batch_first=True), drop_last=True, shuffle=False)
         self.val_dl = iter(self._val_dl) 
         
         self._test_dl = DataLoader(test_dataset, batch_size=self.batch_size,
                           collate_fn=tonic.collation.PadTensors(batch_first=True), drop_last=True, shuffle=False)
         self.test_dl = iter(self._test_dl)
         
-        
     def train_reset(self):
         self.train_dl = iter(self._train_dl)
         
     def train_step(self):
         batch_data, batch_labels = next(self.train_dl)
-        return State(obs=jnp.array(batch_data, dtype=jnp.int8), # perform cast to jnp.int8 here
+        key, self.key = jax.random.split(self.key)
+        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key), -1)
+        return State(obs=jnp.array(spike_data, dtype=jnp.int8), # perform cast to jnp.int8 here
                      labels=jnp.array(batch_labels))
     
     def val_reset(self):
         self.val_dl = iter(self._val_dl)
         
     def val_step(self):
         batch_data, batch_labels = next(self.val_dl)
-        return State(obs=jnp.array(batch_data, dtype=jnp.int8), # perform cast to jnp.int8 here
+        key, self.key = jax.random.split(self.key)
+        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key), -1)
+        return State(obs=jnp.array(spike_data, dtype=jnp.int8), # perform cast to jnp.int8 here
                      labels=jnp.array(batch_labels))
-    
+        
     def test_reset(self):
         self.test_dl = iter(self._test_dl)
         
     def test_step(self):
         batch_data, batch_labels = next(self.test_dl)
-        return State(obs=jnp.array(batch_data, dtype=jnp.int8), # perform cast to jnp.int8 here
+        key, self.key = jax.random.split(self.key)
+        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key), -1)
+        return State(obs=jnp.array(spike_data, dtype=jnp.int8), # perform cast to jnp.int8 here
                      labels=jnp.array(batch_labels))
-    
-    #########################################################################
 
-    # Here we scale the max probability to .8 so that we don't have inputs that are continually spiking.
-# might need to find a home for this in the lib.
-def rate_code(data, steps, key, max_r=0.8):
-    """Unrolls input data along axis 1 and converts to rate encoded spikes."""
-
-    data = jnp.array(data, dtype=jnp.float16)
-    unrolled_data = jnp.repeat(data, steps, axis=1)
-    return jax.random.bernoulli(key, unrolled_data*max_r).astype(jnp.int8)
 
+###############################################
 
-class MNIST_loader():
+class NMNIST_loader():
     """
-    Dataloader for the MNIST dataset, right now it is rate encoded.
-    
+    Dataloading wrapper for the Neuromorphic MNIST dataset.
     """
 
     # Change this to allow a config dictionary of 
-    def __init__(self, batch_size=32, val_size=0.3, key=0, download_dir='./MNIST'):
+    def __init__(self, batch_size=32, val_size=0.3, download_dir='./NMNIST'):
+        sample_T = 64
            
-        self.key = jax.random.PRNGKey(key)
-        self.sample_T = 64
-        self.spike_rate = 0.7
         self.val_size = val_size
         self.batch_size = batch_size
-        self.obs_shape = (28,28)
+        self.obs_shape = datasets.NMNIST.sensor_size
         self.act_shape = tuple([10,])
         
-        transform = tv.transforms.Compose([
-            tv.transforms.Resize(self.obs_shape),
-            tv.transforms.Grayscale(),
-            tv.transforms.ToTensor(),
-            tv.transforms.Normalize((0,), (1,))])
+        transform = transforms.ToFrame(sensor_size=self.obs_shape, 
+                                       n_time_bins=sample_T)
         
-        # fix this
-        train_val_dataset = tv.datasets.MNIST("./data", train=True, download=True, transform=transform)
-        test_dataset = tv.datasets.MNIST("./data", train=False, download=True, transform=transform)
-        # create train/validation split here...
-        # generate indices: instead of the actual data we pass in integers instead
+
+        train_val_dataset = datasets.NMNIST("./data", first_saccade_only=True, train=True, transform=transform)
+        test_dataset = datasets.NMNIST("./data", first_saccade_only=True, train=False, transform=transform)
         train_indices, val_indices = train_test_split(
         range(len(train_val_dataset)),
         test_size=self.val_size,
         random_state=0,
         shuffle=True
         )
     
@@ -177,77 +157,97 @@
         self._val_dl = DataLoader(val_split, batch_size=self.batch_size,
                           collate_fn=tonic.collation.PadTensors(batch_first=True), drop_last=True, shuffle=False)
         self.val_dl = iter(self._val_dl) 
         
         self._test_dl = DataLoader(test_dataset, batch_size=self.batch_size,
                           collate_fn=tonic.collation.PadTensors(batch_first=True), drop_last=True, shuffle=False)
         self.test_dl = iter(self._test_dl)
-        
+    
     def train_reset(self):
         self.train_dl = iter(self._train_dl)
         
     def train_step(self):
         batch_data, batch_labels = next(self.train_dl)
-        key, self.key = jax.random.split(self.key)
-        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key), -1)
-        return State(obs=jnp.array(spike_data, dtype=jnp.int8), # perform cast to jnp.int8 here
+        return State(obs=jnp.array(batch_data, dtype=jnp.int8), # perform cast to jnp.int8 here
                      labels=jnp.array(batch_labels))
     
     def val_reset(self):
         self.val_dl = iter(self._val_dl)
         
     def val_step(self):
         batch_data, batch_labels = next(self.val_dl)
-        key, self.key = jax.random.split(self.key)
-        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key), -1)
-        return State(obs=jnp.array(spike_data, dtype=jnp.int8), # perform cast to jnp.int8 here
+        return State(obs=jnp.array(batch_data, dtype=jnp.int8), # perform cast to jnp.int8 here
                      labels=jnp.array(batch_labels))
-        
+    
     def test_reset(self):
         self.test_dl = iter(self._test_dl)
         
     def test_step(self):
         batch_data, batch_labels = next(self.test_dl)
-        key, self.key = jax.random.split(self.key)
-        spike_data = jnp.expand_dims(rate_code(batch_data, self.sample_T, key), -1)
-        return State(obs=jnp.array(spike_data, dtype=jnp.int8), # perform cast to jnp.int8 here
+        return State(obs=jnp.array(batch_data, dtype=jnp.int8), # perform cast to jnp.int8 here
                      labels=jnp.array(batch_labels))
 
-                
-#################################################################################
+###########################################################
 
+class SHD2Raster():
+    """ Tool for rastering SHD samples into frames."""
 
-class NMNIST_loader():
+    def __init__(self, encoding_dim, sample_T = 100):
+        self.encoding_dim = encoding_dim
+        self.sample_T = sample_T
+        
+    def __call__(self, events):
+        # tensor has dimensions (time_steps, encoding_dim)
+        tensor = np.zeros((events["t"].max()+1, self.encoding_dim), dtype=int)
+        np.add.at(tensor, (events["t"], events["x"]), 1)
+        #return tensor[:self.sample_T,:]
+        tensor = tensor[:self.sample_T,:]
+        return np.minimum(tensor, 1)
+    
+
+class SHD_loader():
     """
-    Dataloading wrapper for the Neuromorphic MNIST dataset.
+    Dataloading wrapper for the Spiking Heidelberg Dataset.
     """
 
+
     # Change this to allow a config dictionary of 
-    def __init__(self, batch_size=32, val_size=0.3, download_dir='./NMNIST'):
-        sample_T = 64
+    def __init__(self, batch_size=128, val_size=0.3):        
+        shd_timestep = 1e-6
+        shd_channels = 700
+        net_channels = 128
+        net_dt = 10e-3
+        sample_T = 100
            
         self.val_size = val_size
         self.batch_size = batch_size
-        self.obs_shape = datasets.NMNIST.sensor_size
-        self.act_shape = tuple([10,])
+        self.obs_shape = tuple([net_channels,])
+        self.act_shape = tuple([20,])
         
-        transform = transforms.ToFrame(sensor_size=self.obs_shape, 
-                                       n_time_bins=sample_T)
+        transform = transforms.Compose([
+        transforms.Downsample(
+            time_factor=shd_timestep / net_dt,
+            spatial_factor=net_channels / shd_channels
+            ),
+            SHD2Raster(net_channels, sample_T = sample_T)
+        ])
         
-
-        train_val_dataset = datasets.NMNIST("./data", first_saccade_only=True, train=True, transform=transform)
-        test_dataset = datasets.NMNIST("./data", first_saccade_only=True, train=False, transform=transform)
+        train_val_dataset = datasets.SHD("./data", train=True, transform=transform)
+        test_dataset = datasets.SHD("./data", train=False, transform=transform)
+        
+        # create train/validation split here...
+        # generate indices: instead of the actual data we pass in integers instead
         train_indices, val_indices = train_test_split(
-        range(len(train_val_dataset)),
-        test_size=self.val_size,
-        random_state=0,
-        shuffle=True
+            range(len(train_val_dataset)),
+            test_size=self.val_size,
+            random_state=0,
+            shuffle=True # This really should be set externally!!!!!
         )
-    
-    
+        
+        
         train_split = Subset(train_val_dataset, train_indices)
         self.train_len = len(train_indices)
         
         val_split = Subset(train_val_dataset, val_indices)
         self.val_len = len(val_indices)
                         
         self.test_len = len(test_dataset)
@@ -260,15 +260,16 @@
         self._val_dl = DataLoader(val_split, batch_size=self.batch_size,
                           collate_fn=tonic.collation.PadTensors(batch_first=True), drop_last=True, shuffle=False)
         self.val_dl = iter(self._val_dl) 
         
         self._test_dl = DataLoader(test_dataset, batch_size=self.batch_size,
                           collate_fn=tonic.collation.PadTensors(batch_first=True), drop_last=True, shuffle=False)
         self.test_dl = iter(self._test_dl)
-    
+        
+        
     def train_reset(self):
         self.train_dl = iter(self._train_dl)
         
     def train_step(self):
         batch_data, batch_labels = next(self.train_dl)
         return State(obs=jnp.array(batch_data, dtype=jnp.int8), # perform cast to jnp.int8 here
                      labels=jnp.array(batch_labels))
@@ -283,8 +284,8 @@
     
     def test_reset(self):
         self.test_dl = iter(self._test_dl)
         
     def test_step(self):
         batch_data, batch_labels = next(self.test_dl)
         return State(obs=jnp.array(batch_data, dtype=jnp.int8), # perform cast to jnp.int8 here
-                     labels=jnp.array(batch_labels))
+                     labels=jnp.array(batch_labels))
```

### Comparing `spyx-0.0.1/spyx/loss.py` & `spyx-0.0.2/spyx/loss.py`

 * *Files identical despite different names*

### Comparing `spyx-0.0.1/spyx/nn.py` & `spyx-0.0.2/spyx/nn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,13 @@
 import jax
 import jax.numpy as jnp
 import haiku as hk
+from .activation import Heaviside
 
 
-
-class LIF(hk.RNNCore): # bfloat16 covers a wide range of unused values...
-    """
-    Leaky Integrate and Fire neuron model inspired by the implementation in
-    snnTorch:
-
-    https://snntorch.readthedocs.io/en/latest/snn.neurons_leaky.html
-    
-    """
-
-    def __init__(self, hidden_size, beta=None, threshold=1, 
-                 activation = Heaviside(),
-                 name="LIF"):
-        super().__init__(name=name)
-        self.hidden_size = hidden_size
-        self.beta = beta
-        self.threshold = threshold
-        self.act = activation
-    
-    def __call__(self, x, V):
-        
-        # numerical stability gremlin...
-        beta = self.beta
-        if not beta:
-            beta = hk.get_parameter("b", [self.hidden_size], dtype=jnp.float16,
-                                init=hk.initializers.TruncatedNormal(0.25, 0.5))
-            beta = jax.nn.hard_sigmoid(beta)
-        # calculate whether spike is generated, and update membrane potential
-        spikes = self.act(V - self.threshold)
-        V = (beta*V + x - spikes*self.threshold).astype(jnp.float16)
-        
-        return spikes, V
-
-    def initial_state(self, batch_size): # figure out how to make dynamic...
-        return jnp.zeros([batch_size, self.hidden_size], dtype=jnp.float16)
-    
-    
-
 class ALIF(hk.RNNCore): # make alpha and beta learnable with an additional clamp func
     """
     Adaptive LIF Neuron based on the model used in LSNNs:
 
     Bellec, G., Salaj, D., Subramoney, A., Legenstein, R. & Maass, W. 
     Long short- term memory and learning-to-learn in networks of spiking neurons. 
     32nd Conference on Neural Information Processing Systems (2018).
@@ -85,14 +48,72 @@
         
         VT = jnp.concatenate([V,T], axis=-1, dtype=jnp.float16)
         return spikes, VT
     
     def initial_state(self, batch_size):
         return jnp.zeros([batch_size, self.hidden_size*2], dtype=jnp.float16)
     
+
+        
+# allow for population encoding???
+class LI(hk.RNNCore):
+    """
+    Leaky-Integrate (Non-spiking) neuron model.
+    """
+
+    def __init__(self, layer_size, beta=0.8, name="LI"):
+        super().__init__(name=name)
+        self.layer_size = layer_size
+        self.beta = beta
+    
+    def __call__(self, x, Vin):
+        # calculate whether spike is generated, and update membrane potential
+        Vout = self.beta*Vin + x
+        return Vout, Vout
+    
+    def initial_state(self, batch_size):
+        return jnp.zeros([batch_size, self.layer_size], dtype=jnp.float32)
+
+
+
+class LIF(hk.RNNCore): # bfloat16 covers a wide range of unused values...
+    """
+    Leaky Integrate and Fire neuron model inspired by the implementation in
+    snnTorch:
+
+    https://snntorch.readthedocs.io/en/latest/snn.neurons_leaky.html
+    
+    """
+
+    def __init__(self, hidden_size, beta=None, threshold=1, 
+                 activation = Heaviside(),
+                 name="LIF"):
+        super().__init__(name=name)
+        self.hidden_size = hidden_size
+        self.beta = beta
+        self.threshold = threshold
+        self.act = activation
+    
+    def __call__(self, x, V):
+        
+        # numerical stability gremlin...
+        beta = self.beta
+        if not beta:
+            beta = hk.get_parameter("b", [self.hidden_size], dtype=jnp.float16,
+                                init=hk.initializers.TruncatedNormal(0.25, 0.5))
+            beta = jax.nn.hard_sigmoid(beta)
+        # calculate whether spike is generated, and update membrane potential
+        spikes = self.act(V - self.threshold)
+        V = (beta*V + x - spikes*self.threshold).astype(jnp.float16)
+        
+        return spikes, V
+
+    def initial_state(self, batch_size): # figure out how to make dynamic...
+        return jnp.zeros([batch_size, self.hidden_size], dtype=jnp.float16)
+
 class RLIF(hk.RNNCore): # bfloat16 covers a wide range of unused values...
     """
     Recurrent LIF Neuron adapted from snnTorch:
 
     https://snntorch.readthedocs.io/en/latest/snn.neurons_rleaky.html
     """
 
@@ -120,15 +141,15 @@
         
         return spikes, V
 
     def initial_state(self, batch_size):
         return jnp.zeros([batch_size, self.hidden_size], dtype=jnp.float16)
 
 
-    
+
 # Synaptic Conductance a.k.a CoBa
 class SC(hk.RNNCore): 
     """
     Conductance based neuron modeling synaptic conductance.
 
     Adapted from snnTorch:
 
@@ -166,23 +187,7 @@
         
         VI = jnp.concatenate([V,I], axis=-1, dtype=jnp.float16)
         return spikes, VI
     
     def initial_state(self, batch_size):
         return jnp.zeros([batch_size, self.hidden_size*2], dtype=jnp.float16)
     
-
-        
-# allow for population encoding???
-class LI(hk.RNNCore):
-    def __init__(self, layer_size, beta=0.8, name="LI"):
-        super().__init__(name=name)
-        self.layer_size = layer_size
-        self.beta = beta
-    
-    def __call__(self, x, Vin):
-        # calculate whether spike is generated, and update membrane potential
-        Vout = self.beta*Vin + x
-        return Vout, Vout
-    
-    def initial_state(self, batch_size):
-        return jnp.zeros([batch_size, self.layer_size], dtype=jnp.float32)
```

### Comparing `spyx-0.0.1/spyx.egg-info/PKG-INFO` & `spyx-0.0.2/spyx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.1
+Version: 0.0.2
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Spyx is a compact library built on top of DeepMind's Haiku library, enabling easy construction of spiking neural network models.
```

