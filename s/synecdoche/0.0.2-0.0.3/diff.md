# Comparing `tmp/synecdoche-0.0.2.tar.gz` & `tmp/synecdoche-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synecdoche-0.0.2.tar", last modified: Fri Jun 23 17:36:19 2023, max compression
+gzip compressed data, was "synecdoche-0.0.3.tar", last modified: Fri Jun 23 20:15:28 2023, max compression
```

## Comparing `synecdoche-0.0.2.tar` & `synecdoche-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 17:36:19.004902 synecdoche-0.0.2/
--rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-23 14:39:41.000000 synecdoche-0.0.2/LICENSE
--rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-23 17:36:19.004902 synecdoche-0.0.2/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      491 2023-06-23 17:14:16.000000 synecdoche-0.0.2/README.md
--rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-23 17:36:19.004902 synecdoche-0.0.2/setup.cfg
--rw-rw-r--   0 legion    (1000) legion    (1000)     1447 2023-06-23 17:33:35.000000 synecdoche-0.0.2/setup.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 17:36:19.004902 synecdoche-0.0.2/synecdoche/
--rw-rw-r--   0 legion    (1000) legion    (1000)      129 2023-06-23 17:33:17.000000 synecdoche-0.0.2/synecdoche/__init__.py
--rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:39.000000 synecdoche-0.0.2/synecdoche/_version.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     1491 2023-06-23 15:04:33.000000 synecdoche-0.0.2/synecdoche/experimental.py
--rw-rw-r--   0 legion    (1000) legion    (1000)     8312 2023-06-23 15:15:36.000000 synecdoche-0.0.2/synecdoche/hyper.py
-drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 17:36:19.004902 synecdoche-0.0.2/synecdoche.egg-info/
--rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-23 17:36:18.000000 synecdoche-0.0.2/synecdoche.egg-info/PKG-INFO
--rw-rw-r--   0 legion    (1000) legion    (1000)      288 2023-06-23 17:36:18.000000 synecdoche-0.0.2/synecdoche.egg-info/SOURCES.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-23 17:36:18.000000 synecdoche-0.0.2/synecdoche.egg-info/dependency_links.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       34 2023-06-23 17:36:18.000000 synecdoche-0.0.2/synecdoche.egg-info/requires.txt
--rw-rw-r--   0 legion    (1000) legion    (1000)       11 2023-06-23 17:36:18.000000 synecdoche-0.0.2/synecdoche.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:15:28.887444 synecdoche-0.0.3/
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1064 2023-06-23 14:39:41.000000 synecdoche-0.0.3/LICENSE
+-rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-23 20:15:28.887444 synecdoche-0.0.3/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      590 2023-06-23 20:10:30.000000 synecdoche-0.0.3/README.md
+-rw-rw-r--   0 legion    (1000) legion    (1000)       38 2023-06-23 20:15:28.887444 synecdoche-0.0.3/setup.cfg
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1447 2023-06-23 20:11:13.000000 synecdoche-0.0.3/setup.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:15:28.887444 synecdoche-0.0.3/synecdoche/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      129 2023-06-23 17:33:17.000000 synecdoche-0.0.3/synecdoche/__init__.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)       21 2023-06-23 17:32:39.000000 synecdoche-0.0.3/synecdoche/_version.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     1740 2023-06-23 20:07:56.000000 synecdoche-0.0.3/synecdoche/experimental.py
+-rw-rw-r--   0 legion    (1000) legion    (1000)     8460 2023-06-23 20:10:09.000000 synecdoche-0.0.3/synecdoche/hyper.py
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:15:28.887444 synecdoche-0.0.3/synecdoche.egg-info/
+-rw-rw-r--   0 legion    (1000) legion    (1000)      834 2023-06-23 20:15:28.000000 synecdoche-0.0.3/synecdoche.egg-info/PKG-INFO
+-rw-rw-r--   0 legion    (1000) legion    (1000)      311 2023-06-23 20:15:28.000000 synecdoche-0.0.3/synecdoche.egg-info/SOURCES.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)        1 2023-06-23 20:15:28.000000 synecdoche-0.0.3/synecdoche.egg-info/dependency_links.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       34 2023-06-23 20:15:28.000000 synecdoche-0.0.3/synecdoche.egg-info/requires.txt
+-rw-rw-r--   0 legion    (1000) legion    (1000)       11 2023-06-23 20:15:28.000000 synecdoche-0.0.3/synecdoche.egg-info/top_level.txt
+drwxrwxr-x   0 legion    (1000) legion    (1000)        0 2023-06-23 20:15:28.887444 synecdoche-0.0.3/tests/
+-rw-rw-r--   0 legion    (1000) legion    (1000)       85 2023-06-23 17:42:50.000000 synecdoche-0.0.3/tests/test_networks.py
```

### Comparing `synecdoche-0.0.2/LICENSE` & `synecdoche-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `synecdoche-0.0.2/PKG-INFO` & `synecdoche-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synecdoche
-Version: 0.0.2
+Version: 0.0.3
 Summary: Synecdoche: Hypernetworks for Haiku in JAX
 Home-page: https://github.com/kmheckel/synecdoche
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `synecdoche-0.0.2/setup.py` & `synecdoche-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "dm-haiku",
     ],
 )
 
 # This call to setup() does all the work
 setup(
     name="synecdoche",
-    version="0.0.2",
+    version="0.0.3",
     description="Synecdoche: Hypernetworks for Haiku in JAX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kmheckel/synecdoche",
     author="Kade Heckel",
     author_email="example@email.com",
     license="MIT",
```

### Comparing `synecdoche-0.0.2/synecdoche/experimental.py` & `synecdoche-0.0.3/synecdoche/experimental.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import jax
 import jax.tree_util as tree
 import jax.numpy as jnp
 import haiku as hk
 
 class DynamicHypernetwork(hk.Module):
+    """
+    Hypernetwork that takes the current batch as inputs, averages the samples, and then uses that average to predict weights for the layer.
+    """
+
     def __init__(self, embedding_dim, latent_dim, network_params):
         super().__init__()
         # PyTree data needed to reconstruct net
         self.tgt_treedef = tree.tree_structure(network_params)
         self.tgt_sizes = tree.tree_map(jnp.size, network_params)
         self.num_tgt_layers = len(tree.tree_leaves(network_params))
         self.target_layer_shapes = tree.tree_map(jnp.shape, network_params)
         
         # hypernetwork dimensions
         self.embedding_dim = embedding_dim
         self.latent_dim = latent_dim
-        self.hyper_out_dim = tree.tree_reduce(max, self.tgt_sizes)
         
     def __call__(self, x):
         avg = jnp.mean(x, axis=0)
         layer_inputs = jnp.repeat(jnp.expand_dims(avg, 0), self.num_tgt_layers, 0)
-        projections = hk.nets.MLP([self.embedding_dim, self.latent_dim, self.hyper_out_dim])(layer_inputs)
+        projections = hk.nets.MLP([self.embedding_dim, self.latent_dim, self.latent_dim])(layer_inputs)
 
         layer_projections = jnp.split(projections, self.num_tgt_layers)
                 
         rebuilt_tree = tree.tree_unflatten(self.tgt_treedef, layer_projections)
-        resized_tree = tree.tree_map(lambda layer, size: layer[1,:size], # the axis=1 is odd.
+        resized_tree = tree.tree_map(lambda layer, size: jnp.pad(layer[1,:size], 
+                                                                 (0,max(0,size-layer.size)), 
+                                                                 mode="wrap"), 
                                      rebuilt_tree, 
                                      self.tgt_sizes
                                     )
         net = tree.tree_map(jnp.reshape, resized_tree, self.target_layer_shapes)
         return net
```

### Comparing `synecdoche-0.0.2/synecdoche/hyper.py` & `synecdoche-0.0.3/synecdoche/hyper.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import jax.tree_util as tree
 import jax.numpy as jnp
 import haiku as hk
 
 
 def param_count(hypernetwork_params):
     """ Count the number of learnable params in a network"""
-    return jnp.sum(tree.tree_map(jnp.size, hypernetwork_params))
+    return sum(tree.tree_leaves(tree.tree_map(jnp.size, hypernetwork_params)))
 
-def hypernetwork_compression_ratio(hypernet_params, target_params):
+def compression_ratio(hypernet_params, target_params):
     """ Compute the savings from using a hypernetwork based approach"""
     return param_count(hypernet_params) / param_count(target_params)
 
 
 class RandomProjection(hk.Module):
     """
     Use random projection to translate a set of optimizable/evovable weights into
@@ -169,24 +169,26 @@
         self.tgt_sizes = tree.tree_map(jnp.size, network_params)
         self.num_tgt_layers = len(tree.tree_leaves(network_params))
         self.target_layer_shapes = tree.tree_map(jnp.shape, network_params)
         
         # hypernetwork dimensions
         self.embedding_dim = embedding_dim
         self.latent_dim = latent_dim
-        self.hyper_out_dim = tree.tree_reduce(max, self.tgt_sizes)
         
     def __call__(self):
         embeddings = hk.get_parameter("w", [self.num_tgt_layers, self.embedding_dim],
                                       init=hk.initializers.TruncatedNormal())
-        projections = hk.nets.MLP([self.latent_dim, self.hyper_out_dim])(embeddings)
+        projections = hk.nets.MLP([self.latent_dim, self.latent_dim])(embeddings)
         # tgt_layers X max_layer_size matrix
         
         layer_projections = jnp.split(projections, self.num_tgt_layers)
                 
         rebuilt_tree = tree.tree_unflatten(self.tgt_treedef, layer_projections)
-        resized_tree = tree.tree_map(lambda layer, size: layer[1,:size], 
+        # this is ugly... sorry...
+        resized_tree = tree.tree_map(lambda layer, size: jnp.pad(layer[1,:size], 
+                                                                 (0,max(0,size-layer.size)), 
+                                                                 mode="wrap"), 
                                      rebuilt_tree, 
                                      self.tgt_sizes
                                     )
         net = tree.tree_map(jnp.reshape, resized_tree, self.target_layer_shapes)
         return net
```

### Comparing `synecdoche-0.0.2/synecdoche.egg-info/PKG-INFO` & `synecdoche-0.0.3/synecdoche.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synecdoche
-Version: 0.0.2
+Version: 0.0.3
 Summary: Synecdoche: Hypernetworks for Haiku in JAX
 Home-page: https://github.com/kmheckel/synecdoche
 Author: Kade Heckel
 Author-email: example@email.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

