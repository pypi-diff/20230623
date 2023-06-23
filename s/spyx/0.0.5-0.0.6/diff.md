# Comparing `tmp/spyx-0.0.5.tar.gz` & `tmp/spyx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyx-0.0.5.tar", last modified: Thu Jun 22 22:56:57 2023, max compression
+gzip compressed data, was "spyx-0.0.6.tar", last modified: Fri Jun 23 20:13:50 2023, max compression
```

## Comparing `spyx-0.0.5.tar` & `spyx-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:56:57.470841 spyx-0.0.5/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.5/LICENSE
--rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-22 22:56:57.470841 spyx-0.0.5/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)     1374 2023-06-22 22:36:29.000000 spyx-0.0.5/README.md
--rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-22 22:56:57.470841 spyx-0.0.5/setup.cfg
--rw-rw-r--   0 legion    (1000) legion    (1000)     1384 2023-06-22 22:55:57.000000 spyx-0.0.5/setup.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:56:57.470841 spyx-0.0.5/spyx/
--rw-rw-r--   0 legion    (1000) legion    (1000)      188 2023-06-22 10:53:53.000000 spyx-0.0.5/spyx/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-21 21:10:32.000000 spyx-0.0.5/spyx/_version.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     8521 2023-06-22 19:23:00.000000 spyx-0.0.5/spyx/activation.py
--rw-rw-r--   0 legion    (1000) legion    (1000)    12319 2023-06-22 22:55:28.000000 spyx-0.0.5/spyx/data.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     2663 2023-06-22 06:44:31.000000 spyx-0.0.5/spyx/loss.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     6673 2023-06-22 11:37:32.000000 spyx-0.0.5/spyx/nn.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:56:57.470841 spyx-0.0.5/spyx.egg-info/
--rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-22 22:56:57.000000 spyx-0.0.5/spyx.egg-info/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      278 2023-06-22 22:56:57.000000 spyx-0.0.5/spyx.egg-info/SOURCES.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-22 22:56:57.000000 spyx-0.0.5/spyx.egg-info/dependency_links.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-22 22:56:57.000000 spyx-0.0.5/spyx.egg-info/requires.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-22 22:56:57.000000 spyx-0.0.5/spyx.egg-info/top_level.txt
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-22 22:56:57.470841 spyx-0.0.5/tests/
--rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-22 08:36:33.000000 spyx-0.0.5/tests/test_networks.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:13:50.394219 spyx-0.0.6/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-21 21:10:32.000000 spyx-0.0.6/LICENSE
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-23 20:13:50.394219 spyx-0.0.6/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1374 2023-06-22 22:36:29.000000 spyx-0.0.6/README.md
+-rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-23 20:13:50.394219 spyx-0.0.6/setup.cfg
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1384 2023-06-23 20:11:52.000000 spyx-0.0.6/setup.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:13:50.394219 spyx-0.0.6/spyx/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      188 2023-06-22 10:53:53.000000 spyx-0.0.6/spyx/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:35.000000 spyx-0.0.6/spyx/_version.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     8952 2023-06-23 07:55:56.000000 spyx-0.0.6/spyx/activation.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)    12319 2023-06-22 22:55:28.000000 spyx-0.0.6/spyx/data.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     2695 2023-06-23 06:49:08.000000 spyx-0.0.6/spyx/loss.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     7303 2023-06-23 19:28:10.000000 spyx-0.0.6/spyx/nn.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:13:50.394219 spyx-0.0.6/spyx.egg-info/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      760 2023-06-23 20:13:50.000000 spyx-0.0.6/spyx.egg-info/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      278 2023-06-23 20:13:50.000000 spyx-0.0.6/spyx.egg-info/SOURCES.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-23 20:13:50.000000 spyx-0.0.6/spyx.egg-info/dependency_links.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       40 2023-06-23 20:13:50.000000 spyx-0.0.6/spyx.egg-info/requires.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        5 2023-06-23 20:13:50.000000 spyx-0.0.6/spyx.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:13:50.394219 spyx-0.0.6/tests/
+-rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-22 08:36:33.000000 spyx-0.0.6/tests/test_networks.py
```

### Comparing `spyx-0.0.5/LICENSE` & `spyx-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spyx-0.0.5/PKG-INFO` & `spyx-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.5
+Version: 0.0.6
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `spyx-0.0.5/README.md` & `spyx-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `spyx-0.0.5/setup.py` & `spyx-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         "numpy",
     ],
 )
 
 # This call to setup() does all the work
 setup(
     name="spyx",
-    version="0.0.5",
+    version="0.0.6",
     description="Spyx: SNNs in JAX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kmheckel/spyx",
     author="Kade Heckel",
     author_email="example@email.com",
     license="MIT",
```

### Comparing `spyx-0.0.5/spyx/activation.py` & `spyx-0.0.6/spyx/activation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import jax
 import jax.numpy as jnp
 import haiku as hk
 
 # eventually, it would be good to make an abstract class that all activations below extend...
 
+# should this be added to nn?
 class ActivityRegularization(hk.Module):
     """
     Add state to the SNN to track the average number of spikes emitted per neuron per batch.
+
+    Adding this to a network requires using the Haiku transform_with_state transform, which will also return an initial regularization state vector.
+    This blank initial vector can be reused and is provided as the second arg to the SNN's apply function. 
     """
 
     def __init__(self, name="ActReg"):
         super().__init__(name=name)
         
     def __call__(self, spikes):
         spike_count = hk.get_state("spike_count", [spikes.shape[-1]], init=jnp.zeros)
@@ -19,17 +23,22 @@
 
 
 class AdaSpike:
     """
     Simplified version of SuperSpike, dropping the power from the denominator.
     Features an increasing scale factor with linear schedule, increasing the
     sharpness of the surrogate gradient over time.
+
+    $$\frac{\delta S}{\delta U} = \frac{1}{1+k|U|}$$
+
+    Attributes:
+        growth_rate: The amount the scale factor k is incremented by after each batch.
     """
 
-    def __init__(self,  warmup_steps, growth_rate=0.5):
+    def __init__(self, growth_rate=0.5):
         self.k = 1
         self.gr = growth_rate
         
         @jax.custom_vjp
         def f(U, k): # primal function
             return (U>0).astype(jnp.float16)
```

### Comparing `spyx-0.0.5/spyx/data.py` & `spyx-0.0.6/spyx/data.py`

 * *Files identical despite different names*

### Comparing `spyx-0.0.5/spyx/loss.py` & `spyx-0.0.6/spyx/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import jax
 import jax.numpy as jnp
 import optax
 
+# need to make these consistent...
+
 @jax.jit
 def SRR_MSE(avg_spike_counts, target_count):
     """Spike rate regularization based on mean squared error from target rate."""
 
     flat = jnp.concatenate(jax.tree_util.tree_flatten(avg_spike_counts)[0])
     return jnp.sum(optax.l2_loss(flat, jnp.array([target_count]*flat.shape[0])))
 
@@ -30,15 +32,15 @@
 
     """
 
     preds = jnp.argmax(jnp.sum(traces, axis=-2), axis=-1)
     return jnp.sum(preds == targets) / traces.shape[0], preds
 
 @jax.jit
-def integral_crossentropy(traces, targets):
+def integral_xentropy(traces, targets):
     """
     Calculate the crossentropy between the integral of membrane potentials.
     right now has a fixed value for label smoothing to discourage silencing 
     the other neurons in the readout layer.
     """
 
     logits = jnp.sum(traces, axis=-2) # time axis.
```

### Comparing `spyx-0.0.5/spyx/nn.py` & `spyx-0.0.6/spyx/nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,19 @@
     
 
         
 # allow for population encoding???
 class LI(hk.RNNCore):
     """
     Leaky-Integrate (Non-spiking) neuron model.
+
+    Attributes:
+        layer_size: Number of output neurons from the previous linear layer.
+
+        beta: Decay rate on membrane potential (voltage). Set uniformly across the layer.
     """
 
     def __init__(self, layer_size, beta=0.8, name="LI"):
         super().__init__(name=name)
         self.layer_size = layer_size
         self.beta = beta
     
@@ -78,14 +83,21 @@
 class LIF(hk.RNNCore): # bfloat16 covers a wide range of unused values...
     """
     Leaky Integrate and Fire neuron model inspired by the implementation in
     snnTorch:
 
     https://snntorch.readthedocs.io/en/latest/snn.neurons_leaky.html
     
+
+    Attributes:
+        hidden_size: Size of preceding layer's outputs
+        beta: decay rate. Set to float in range (0,1] for uniform decay across layer, otherwise it will be a normal
+            distribution centered on 0.5 with stddev of 0.25
+        threshold: threshold for reset. Defaults to 1.
+        activation: spyx.activation function, default is Heaviside with Straight-Through-Estimation.
     """
 
     def __init__(self, hidden_size, beta=None, threshold=1, 
                  activation = Heaviside(),
                  name="LIF"):
         super().__init__(name=name)
         self.hidden_size = hidden_size
@@ -124,15 +136,15 @@
         self.hidden_size = hidden_size
         self.beta = beta
         self.threshold = threshold
         self.act = activation
     
     def __call__(self, x, V):
         # calculate whether spike is generated, and update membrane potential
-        recurrent = hk.get_parameter("w", [self.hidden_size])
+        recurrent = hk.get_parameter("w", [self.hidden_size], init=hk.initializers.TruncatedNormal())
         
         beta = self.beta
         if not beta:
             beta = hk.get_parameter("b", [self.hidden_size], 
                                 init=hk.initializers.TruncatedNormal(0.25, 0.5))
             beta = jax.nn.hard_sigmoid(beta)
```

### Comparing `spyx-0.0.5/spyx.egg-info/PKG-INFO` & `spyx-0.0.6/spyx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyx
-Version: 0.0.5
+Version: 0.0.6
 Summary: Spyx: SNNs in JAX
 Home-page: https://github.com/kmheckel/spyx
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

