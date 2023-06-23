# Comparing `tmp/hivae2-0.8.tar.gz` & `tmp/hivae2-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivae2-0.8.tar", last modified: Fri Aug 26 10:21:38 2022, max compression
+gzip compressed data, was "hivae2-0.9.tar", last modified: Fri Aug 26 12:18:46 2022, max compression
```

## Comparing `hivae2-0.8.tar` & `hivae2-0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 karwath    (501) staff       (20)        0 2022-08-26 10:21:38.971078 hivae2-0.8/
--rw-r--r--   0 karwath    (501) staff       (20)     1079 2022-08-24 17:27:27.000000 hivae2-0.8/LICENSE
--rw-r--r--   0 karwath    (501) staff       (20)     2922 2022-08-26 10:21:38.970934 hivae2-0.8/PKG-INFO
--rw-r--r--   0 karwath    (501) staff       (20)     2484 2022-08-24 17:47:31.000000 hivae2-0.8/README.md
-drwxr-xr-x   0 karwath    (501) staff       (20)        0 2022-08-26 10:21:38.969825 hivae2-0.8/hivae/
--rw-r--r--   0 karwath    (501) staff       (20)    23036 2022-08-24 17:22:42.000000 hivae2-0.8/hivae/VAE_functions.py
--rw-r--r--   0 karwath    (501) staff       (20)      224 2022-08-24 17:05:04.000000 hivae2-0.8/hivae/__init__.py
--rw-r--r--   0 karwath    (501) staff       (20)     3180 2022-08-24 17:22:39.000000 hivae2-0.8/hivae/graph_new.py
--rw-r--r--   0 karwath    (501) staff       (20)    26828 2022-08-26 10:21:12.000000 hivae2-0.8/hivae/hivae.py
--rw-r--r--   0 karwath    (501) staff       (20)     6299 2022-08-24 17:26:07.000000 hivae2-0.8/hivae/loglik_models_missing_normalize.py
--rw-r--r--   0 karwath    (501) staff       (20)     4638 2022-08-24 17:26:00.000000 hivae2-0.8/hivae/model_HIVAE_factorized.py
--rw-r--r--   0 karwath    (501) staff       (20)     4582 2022-08-24 17:25:56.000000 hivae2-0.8/hivae/model_HIVAE_inputDropout.py
--rw-r--r--   0 karwath    (501) staff       (20)     2843 2022-08-24 14:04:44.000000 hivae2-0.8/hivae/parser_arguments.py
--rw-r--r--   0 karwath    (501) staff       (20)    20100 2022-08-24 14:04:44.000000 hivae2-0.8/hivae/read_functions.py
--rw-r--r--   0 karwath    (501) staff       (20)      274 2022-08-24 14:04:44.000000 hivae2-0.8/hivae/utils.py
-drwxr-xr-x   0 karwath    (501) staff       (20)        0 2022-08-26 10:21:38.970733 hivae2-0.8/hivae2.egg-info/
--rw-r--r--   0 karwath    (501) staff       (20)     2922 2022-08-26 10:21:38.000000 hivae2-0.8/hivae2.egg-info/PKG-INFO
--rw-r--r--   0 karwath    (501) staff       (20)      451 2022-08-26 10:21:38.000000 hivae2-0.8/hivae2.egg-info/SOURCES.txt
--rw-r--r--   0 karwath    (501) staff       (20)        1 2022-08-26 10:21:38.000000 hivae2-0.8/hivae2.egg-info/dependency_links.txt
--rw-r--r--   0 karwath    (501) staff       (20)        1 2022-08-24 18:19:51.000000 hivae2-0.8/hivae2.egg-info/not-zip-safe
--rw-r--r--   0 karwath    (501) staff       (20)       38 2022-08-26 10:21:38.000000 hivae2-0.8/hivae2.egg-info/requires.txt
--rw-r--r--   0 karwath    (501) staff       (20)        6 2022-08-26 10:21:38.000000 hivae2-0.8/hivae2.egg-info/top_level.txt
--rw-r--r--   0 karwath    (501) staff       (20)       38 2022-08-26 10:21:38.971126 hivae2-0.8/setup.cfg
--rw-r--r--   0 karwath    (501) staff       (20)      931 2022-08-26 10:21:27.000000 hivae2-0.8/setup.py
+drwxr-xr-x   0 karwath    (501) staff       (20)        0 2022-08-26 12:18:46.982671 hivae2-0.9/
+-rw-r--r--   0 karwath    (501) staff       (20)     1079 2022-08-24 17:27:27.000000 hivae2-0.9/LICENSE
+-rw-r--r--   0 karwath    (501) staff       (20)     2922 2022-08-26 12:18:46.982533 hivae2-0.9/PKG-INFO
+-rw-r--r--   0 karwath    (501) staff       (20)     2484 2022-08-24 17:47:31.000000 hivae2-0.9/README.md
+drwxr-xr-x   0 karwath    (501) staff       (20)        0 2022-08-26 12:18:46.981119 hivae2-0.9/hivae/
+-rw-r--r--   0 karwath    (501) staff       (20)    23036 2022-08-24 17:22:42.000000 hivae2-0.9/hivae/VAE_functions.py
+-rw-r--r--   0 karwath    (501) staff       (20)      224 2022-08-24 17:05:04.000000 hivae2-0.9/hivae/__init__.py
+-rw-r--r--   0 karwath    (501) staff       (20)     3435 2022-08-26 12:05:30.000000 hivae2-0.9/hivae/graph_new.py
+-rw-r--r--   0 karwath    (501) staff       (20)    28058 2022-08-26 12:07:53.000000 hivae2-0.9/hivae/hivae.py
+-rw-r--r--   0 karwath    (501) staff       (20)     6299 2022-08-24 17:26:07.000000 hivae2-0.9/hivae/loglik_models_missing_normalize.py
+-rw-r--r--   0 karwath    (501) staff       (20)     4638 2022-08-24 17:26:00.000000 hivae2-0.9/hivae/model_HIVAE_factorized.py
+-rw-r--r--   0 karwath    (501) staff       (20)     4582 2022-08-24 17:25:56.000000 hivae2-0.9/hivae/model_HIVAE_inputDropout.py
+-rw-r--r--   0 karwath    (501) staff       (20)     2843 2022-08-24 14:04:44.000000 hivae2-0.9/hivae/parser_arguments.py
+-rw-r--r--   0 karwath    (501) staff       (20)    20100 2022-08-24 14:04:44.000000 hivae2-0.9/hivae/read_functions.py
+-rw-r--r--   0 karwath    (501) staff       (20)      274 2022-08-24 14:04:44.000000 hivae2-0.9/hivae/utils.py
+drwxr-xr-x   0 karwath    (501) staff       (20)        0 2022-08-26 12:18:46.982277 hivae2-0.9/hivae2.egg-info/
+-rw-r--r--   0 karwath    (501) staff       (20)     2922 2022-08-26 12:18:46.000000 hivae2-0.9/hivae2.egg-info/PKG-INFO
+-rw-r--r--   0 karwath    (501) staff       (20)      451 2022-08-26 12:18:46.000000 hivae2-0.9/hivae2.egg-info/SOURCES.txt
+-rw-r--r--   0 karwath    (501) staff       (20)        1 2022-08-26 12:18:46.000000 hivae2-0.9/hivae2.egg-info/dependency_links.txt
+-rw-r--r--   0 karwath    (501) staff       (20)        1 2022-08-24 18:19:51.000000 hivae2-0.9/hivae2.egg-info/not-zip-safe
+-rw-r--r--   0 karwath    (501) staff       (20)       38 2022-08-26 12:18:46.000000 hivae2-0.9/hivae2.egg-info/requires.txt
+-rw-r--r--   0 karwath    (501) staff       (20)        6 2022-08-26 12:18:46.000000 hivae2-0.9/hivae2.egg-info/top_level.txt
+-rw-r--r--   0 karwath    (501) staff       (20)       38 2022-08-26 12:18:46.982726 hivae2-0.9/setup.cfg
+-rw-r--r--   0 karwath    (501) staff       (20)      931 2022-08-26 10:26:03.000000 hivae2-0.9/setup.py
```

### Comparing `hivae2-0.8/LICENSE` & `hivae2-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hivae2-0.8/PKG-INFO` & `hivae2-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivae2
-Version: 0.8
+Version: 0.9
 Summary: HIVAE (Handling incomplete heterogeneous data using VAEs. - by Nazabal, et al., DOI: 10.1016/j.patcog.2020.107501, 2020) - Extenstion of implementations as easy to use Python library/tf2 version
 Home-page: https://github.com/gkoutos-group/hivae/
 Author: Andreas Karwath
 Author-email: a.karwath@bham.ac.uk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hivae2-0.8/README.md` & `hivae2-0.9/README.md`

 * *Files identical despite different names*

### Comparing `hivae2-0.8/hivae/VAE_functions.py` & `hivae2-0.9/hivae/VAE_functions.py`

 * *Files identical despite different names*

### Comparing `hivae2-0.8/hivae/graph_new.py` & `hivae2-0.9/hivae/graph_new.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,52 +8,54 @@
 @author: anazabal, olmosUC3M, ivaleraM
 @changes: athro
 """
 
 import tensorflow as tf
 import numpy as np
 from hivae import VAE_functions
+import hivae #import hivae as hivae
 
 def HVAE_graph(model_name, types_description, batch_size, learning_rate=1e-3, z_dim=2, y_dim=1, s_dim=2, y_dim_partition=[]):
     
     #We select the model for the VAE
-    print('[*] Importing model: ' + model_name)
+    #print('[*] Importing model: ' + model_name)
+    hivae.hivae.vprint_s(2,'[*] Importing model: ' + model_name)
     # how to import a submoule 101
     model = __import__('hivae.{}'.format(model_name),fromlist=[model_name])
     #model = __import__(model_name)
     
     #Load placeholders
-    print('[*] Defining placeholders')
+    hivae.hivae.vprint_s(2,'[*] Defining placeholders')
     batch_data_list, batch_data_list_observed, miss_list, tau, tau2, types_list = VAE_functions.place_holder_types(types_description, batch_size)
     
     #Batch normalization of the data
     X_list, normalization_params = VAE_functions.batch_normalization(batch_data_list_observed, types_list, miss_list)
     
     #Set dimensionality of Y
     if y_dim_partition:
         y_dim_output = np.sum(y_dim_partition)
     else:
         y_dim_partition = y_dim*np.ones(len(types_list),dtype=int)
         y_dim_output = np.sum(y_dim_partition)
     
     #Encoder definition
-    print('[*] Defining Encoder...')
+    hivae.hivae.vprint_s(2,'[*] Defining Encoder...')
     samples, q_params = model.encoder(X_list, miss_list, batch_size, z_dim, s_dim, tau)
     encoding = samples
-    # print('debug ' * 10)
-    # print(samples)
-    # print('- ' * 10)
-    # print(q_params)
-    # print('debug ' * 10)
+    # hivae.hivae.vprint_s(2,'debug ' * 10)
+    # hivae.hivae.vprint_s(2,samples)
+    # hivae.hivae.vprint_s(2,'- ' * 10)
+    # hivae.hivae.vprint_s(2,q_params)
+    # hivae.hivae.vprint_s(2,'debug ' * 10)
 
     
-    print('[*] Defining Decoder...')
+    hivae.hivae.vprint_s(2,'[*] Defining Decoder...')
     theta, samples, p_params, log_p_x, log_p_x_missing = model.decoder(batch_data_list, miss_list, types_list, samples, q_params, normalization_params, batch_size, z_dim, y_dim_output, y_dim_partition, tau2)
 
-    print('[*] Defining Cost function...')
+    hivae.hivae.vprint_s(2,'[*] Defining Cost function...')
     ELBO, loss_reconstruction, KL_z, KL_s = model.cost_function(log_p_x, p_params, q_params, types_list, z_dim, y_dim_output, s_dim)
     
     optim = tf.compat.v1.train.AdamOptimizer(learning_rate).minimize(-ELBO)
     
     #Generator function for testing purposes
     samples_test, test_params, log_p_x_test, log_p_x_missing_test = model.samples_generator(batch_data_list, X_list, miss_list, types_list, batch_size, z_dim, y_dim_output, y_dim_partition, s_dim, tau, tau2, normalization_params)
```

### Comparing `hivae2-0.8/hivae/hivae.py` & `hivae2-0.9/hivae/hivae.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,16 @@
         self.save             = 1000 # parameter?
         self.save_every_epoch = save_every_epoch    
         self.dim_s            = save_get(network_dict,'dim_s',None) 
         self.dim_z            = save_get(network_dict,'dim_z',None) 
         self.dim_y            = save_get(network_dict,'dim_y',None)
         self.batch_size       = save_get(network_dict,'batch_size',32)
         if verbosity_level!=None:
+            #debug
+            #print('DEBUG setting verbosity_level init')
             self.set_verbosity_level(verbosity_level)
         #self.verbosity_level  = verbosity_level
 
 
         # self.true_miss_file   = true_miss_file
         # self.miss_file        = miss_file
         if not results_path:
@@ -107,36 +109,17 @@
         
         self.full_network_path = full_network_path
         self.full_results_path = full_results_path
 
         self.network_file_name = '{}_ckpt'.format(self.full_network_path) 
         self.log_file_name     = '{}/log_file_{}.txt'.format(self.full_network_path,self.savefile)
 
-        print('self.full_network_path',self.full_network_path)
-        print('self.full_results_path',self.full_results_path)
-        print('self.network_file_name', self.network_file_name)
-
-
-    # use own printing - should be changed to better logging
-    @staticmethod
-    def set_verbosity_level(self,verbosity_level=3):
-        setattr(hivae, 'verbosity_level', int(verbosity_level))
-
-        #self.verbosity_level = verbosity_level
-        
-    @staticmethod
-    def vprint(self,verbosity_level,*args):
-        #if verbosity_level<=self.verbosity_level:
-        if verbosity_level<=int(getattr(hivae, 'verbosity_level')):
-            if verbosity_level==1:
-                print('INFO :\t',*args)
-            elif verbosity_level==2:
-                print('DEBUG:\t',*args)
-            elif verbosity_level==3:
-                print('ERROR:\t',*args)
+        self.vprint(1,'self.full_network_path',self.full_network_path)
+        self.vprint(1,'self.full_results_path',self.full_results_path)
+        self.vprint(1,'self.network_file_name', self.network_file_name)
 
 
             
 
         
     def print_loss(self,epoch, start_time, avg_loss, avg_test_loglik, avg_KL_s, avg_KL_z):
         
@@ -525,11 +508,62 @@
                 
 
                 return (train_data_transformed,data_reconstruction,loglik_mean_reconstructed,
                             z_total[np.argsort(random_perm)],
                             s_total[np.argsort(random_perm)])
 
         
+    # use own printing - should be changed to better logging
+    # classmethods are kept for backwards compatibility
+    @classmethod
+    def set_verbosity_level(cls,verbosity_level=3):
+        #print('DEBUGGER setting verbosity_level method')
+        # try:
+        #     verbosity_level = int(verbosity_level)
+        #     setattr(hivae, 'verbosity_level', int(verbosity_level))
+
+        # except:
+        #     print('HIVAE: VERBOSITY LEVEL NOT SET (not an int <<{}>>)'.format(verbosity_level))
+        #     pass
+        #self.verbosity_level = verbosity_level
+
+        hivae.set_verbosity_level(verbosity_level)
+        
+    def vprint(cls,vl,*args):
+        # #verbosity_level = int(verbosity_level)
+        # global_vl = getattr(hivae, 'verbosity_level')
+        # if global_vl <= vl:  
+        #     if vl==1:
+        #         print('INFO :\t',*args)
+        #     elif vl==2:
+        #         print('DEBUG:\t',*args)
+        #     elif vl==3:
+        #         print('ERROR:\t',*args)
+        hivae.vprint_s(vl,*args)
+        
+    @staticmethod
+    def vprint_s(vl,*args):
+        #verbosity_level = int(verbosity_level)
+        global_vl = getattr(hivae, 'verbosity_level')
+        if global_vl <= vl:  
+            if vl==1:
+                print('INFO :\t',*args)
+            elif vl==2:
+                print('DEBUG:\t',*args)
+            elif vl==3:
+                print('ERROR:\t',*args)
+
+    def set_verbosity_level_s(verbosity_level=3):
+        #print('DEBUGGER setting verbosity_level method')
+        try:
+            verbosity_level = int(verbosity_level)
+            setattr(hivae, 'verbosity_level', int(verbosity_level))
+
+        except:
+            print('HIVAE: VERBOSITY LEVEL NOT SET (not an int <<{}>>)'.format(verbosity_level))
+            pass
+
+
```

### Comparing `hivae2-0.8/hivae/loglik_models_missing_normalize.py` & `hivae2-0.9/hivae/loglik_models_missing_normalize.py`

 * *Files identical despite different names*

### Comparing `hivae2-0.8/hivae/model_HIVAE_factorized.py` & `hivae2-0.9/hivae/model_HIVAE_factorized.py`

 * *Files identical despite different names*

### Comparing `hivae2-0.8/hivae/model_HIVAE_inputDropout.py` & `hivae2-0.9/hivae/model_HIVAE_inputDropout.py`

 * *Files identical despite different names*

### Comparing `hivae2-0.8/hivae/parser_arguments.py` & `hivae2-0.9/hivae/parser_arguments.py`

 * *Files identical despite different names*

### Comparing `hivae2-0.8/hivae/read_functions.py` & `hivae2-0.9/hivae/read_functions.py`

 * *Files identical despite different names*

### Comparing `hivae2-0.8/hivae2.egg-info/PKG-INFO` & `hivae2-0.9/hivae2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivae2
-Version: 0.8
+Version: 0.9
 Summary: HIVAE (Handling incomplete heterogeneous data using VAEs. - by Nazabal, et al., DOI: 10.1016/j.patcog.2020.107501, 2020) - Extenstion of implementations as easy to use Python library/tf2 version
 Home-page: https://github.com/gkoutos-group/hivae/
 Author: Andreas Karwath
 Author-email: a.karwath@bham.ac.uk
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hivae2-0.8/setup.py` & `hivae2-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                 'tensorflow-probability',    
                 'pandas',
                 'sklearn',
                     ]
     
 setuptools.setup(
     name='hivae2',
-    version='0.8',
+    version='0.9',
     url='https://github.com/gkoutos-group/hivae/',
     license='MIT',
     author='Andreas Karwath',
     author_email='a.karwath@bham.ac.uk',
     description='HIVAE (Handling incomplete heterogeneous data using VAEs. - by Nazabal, et al., DOI: 10.1016/j.patcog.2020.107501, 2020) - Extenstion of implementations as easy to use Python library/tf2 version',
     packages=setuptools.find_packages(exclude=['examples']),
     install_requires=requirements,
```

