# Comparing `tmp/framework-reproducibility-0.4.0.tar.gz` & `tmp/framework-reproducibility-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/framework-reproducibility-0.4.0.tar", last modified: Tue Feb 28 01:05:58 2023, max compression
+gzip compressed data, was "dist/framework-reproducibility-0.5.0.tar", last modified: Thu Jun 22 22:45:43 2023, max compression
```

## Comparing `framework-reproducibility-0.4.0.tar` & `framework-reproducibility-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1378 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/PKG-INFO
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     3509 2023-02-28 01:03:54.000000 framework-reproducibility-0.4.0/setup.py
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/fwr13y/
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/fwr13y/seeder/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1646 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/seeder/seed_gen.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2014 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/seeder/pyt.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2185 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/seeder/tf.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2009 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/seeder/paddle.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      777 2023-02-27 23:45:40.000000 framework-reproducibility-0.4.0/fwr13y/seeder/__init__.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      701 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/version.py
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/fwr13y/d9m/
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2687 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/patch_segment_sum.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     3080 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/patch_unsorted_segment_sum.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2923 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/patch_bias_add.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2904 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/enable_determinism.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     3260 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/patch.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      955 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/__init__.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     3752 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/d9m/utils.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      777 2023-02-27 23:45:54.000000 framework-reproducibility-0.4.0/fwr13y/d9m/__init__.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      811 2023-02-27 20:42:41.000000 framework-reproducibility-0.4.0/fwr13y/__init__.py
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/framework_reproducibility.egg-info/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1378 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/framework_reproducibility.egg-info/PKG-INFO
--rw-rw-r--   0 duncan    (1000) duncan    (1000)        7 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/framework_reproducibility.egg-info/top_level.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)        1 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/framework_reproducibility.egg-info/dependency_links.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      667 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/framework_reproducibility.egg-info/SOURCES.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       67 2023-02-28 01:05:58.000000 framework-reproducibility-0.4.0/setup.cfg
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       18 2023-02-28 01:05:21.000000 framework-reproducibility-0.4.0/MANIFEST.in
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     1378 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/PKG-INFO
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2846 2023-04-27 19:27:49.000000 framework-reproducibility-0.5.0/setup.py
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/fwr13y/
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/fwr13y/seeder/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2007 2023-06-22 22:44:48.000000 framework-reproducibility-0.5.0/fwr13y/seeder/seed_gen.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2965 2023-06-22 22:44:48.000000 framework-reproducibility-0.5.0/fwr13y/seeder/pyt.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     3135 2023-06-22 22:44:48.000000 framework-reproducibility-0.5.0/fwr13y/seeder/tf.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2960 2023-06-22 22:44:48.000000 framework-reproducibility-0.5.0/fwr13y/seeder/paddle.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      777 2023-02-28 05:04:37.000000 framework-reproducibility-0.5.0/fwr13y/seeder/__init__.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      701 2023-06-22 22:44:48.000000 framework-reproducibility-0.5.0/fwr13y/version.py
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/fwr13y/d9m/
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2687 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_segment_sum.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     3080 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_unsorted_segment_sum.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2923 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_bias_add.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2904 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/enable_determinism.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     3260 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      955 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/__init__.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     3752 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/utils.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      789 2023-04-27 19:27:49.000000 framework-reproducibility-0.5.0/fwr13y/d9m/__init__.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      823 2023-04-27 19:27:49.000000 framework-reproducibility-0.5.0/fwr13y/__init__.py
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/framework_reproducibility.egg-info/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     1378 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/framework_reproducibility.egg-info/PKG-INFO
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)        7 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/framework_reproducibility.egg-info/top_level.txt
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)        1 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/framework_reproducibility.egg-info/dependency_links.txt
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      667 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/framework_reproducibility.egg-info/SOURCES.txt
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)       67 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/setup.cfg
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)       18 2023-02-28 05:04:37.000000 framework-reproducibility-0.5.0/MANIFEST.in
```

### Comparing `framework-reproducibility-0.4.0/PKG-INFO` & `framework-reproducibility-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framework-reproducibility
-Version: 0.4.0
+Version: 0.5.0
 Summary: Providing reproducibility in deep learning frameworks
 Home-page: https://github.com/NVIDIA/framework-reproducibility
 Author: NVIDIA
 Author-email: duncan@nvidia.com
 License: Apache 2.0
 Description: This package provides patches and tools related to determinism
         (bit-accurate, run-to-run reproducibility) in deep learning frameworks, with a
```

### Comparing `framework-reproducibility-0.4.0/setup.py` & `framework-reproducibility-0.5.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,30 +13,25 @@
 # limitations under the License.
 # ========================================================================
 
 from setuptools import setup, find_packages
 import os
 
 distribution_name = 'framework-reproducibility'
-# package_name = 'fwrepro' + '_reserve'
 package_name = 'fwr13y'
 
 # This file needs to be executed during installation. It's not possible to
 # import the full package during installation because it will fail to import if
 # all the supported frameworks have not been installed. By temporarility
 # appending to sys.path, it's possible to just import from the version module.
 import sys
 sys.path.append(package_name)
 from version import __version__ as version
-# from warning import message as warning_message
 sys.path.remove(package_name)
 
-# if warning_message:
-#   long_description = warning_message
-# else:
 readme = os.path.join(os.path.dirname(os.path.realpath(__file__)),
                       "pypi_description.md")
 with open(readme, "r") as fp:
   long_description = fp.read()
 
 description = ("Providing reproducibility in deep learning frameworks")
 url = "https://github.com/NVIDIA/%s" % distribution_name
@@ -51,26 +46,18 @@
 ]
 
 keywords = ("framework tensorflow gpu deep-learning determinism "
             "reproducibility pytorch seed seeder noise noise-reduction "
             "variance-reduction atomics ngc gpu-determinism deterministic-ops "
             "frameworks gpu-support d9m r13y fwr13y")
 
-# `find_packages(exclude=['fwd9m_reserve'])` is used instead of adding
-# `exclude fwd9m_reserve/*` to `MANIFEST.in` because even though `MANIFEST.in`
-# is attended to in the creation of the source distribution, it is ignored in
-# the creation of the wheel. Folks generally seem to think that
-# `include_package_data=True` is needed to make the exclusions from the contents
-# of the wheel match those of the source distribution, but it doesn't seem to
-# make any difference.
-
 setup(
   name                          = distribution_name,
   version                       = version,
-  packages                      = find_packages(exclude=['fwd9m_reserve']),
+  packages                      = ['fwr13y'],
   url                           = url,
   license                       = 'Apache 2.0',
   author                        = 'NVIDIA',
   author_email                  = 'duncan@nvidia.com',
   description                   = description,
   long_description              = long_description,
   long_description_content_type = 'text/markdown',
```

### Comparing `framework-reproducibility-0.4.0/fwr13y/seeder/seed_gen.py` & `framework-reproducibility-0.5.0/fwr13y/seeder/seed_gen.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,18 +25,27 @@
         self.master_seed = master_seed
         self.ngpus = ngpus
         self.local_rank = local_rank
         self.ntasks = 2
         self._used_seeds = set()
         self._rng = random.Random(0)
 
-    def __call__(self, task, epoch):
-        seed = (
-            self.master_seed + (epoch * self.ngpus + self.local_rank)
-        ) * self.ntasks + task
+    def __call__(self, task, epoch, shared_seed=False):
+        if shared_seed:
+            # Use the same seed for every rank
+            # Constant at the beginning so that the values do not repeat with not shared seeds
+            seed = 2 * (
+                self.master_seed + epoch
+            ) * self.ntasks + task
+        else:
+            # Use different seed for every rank
+            seed = (
+                self.master_seed + (epoch * self.ngpus + self.local_rank)
+            ) * self.ntasks + task
+
         if seed in self._used_seeds:
             print(
                 "Warning!!! seed has been generated more than once!!!", file=sys.stderr
             )
         self._used_seeds.add(seed)
         self._rng.seed(seed)
         return self._rng.randint(0, _MAX_INT32)
```

### Comparing `framework-reproducibility-0.4.0/fwr13y/seeder/pyt.py` & `framework-reproducibility-0.5.0/fwr13y/seeder/pyt.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,35 +18,55 @@
 import numpy as np
 from .seed_gen import SeedGen, generate_master_seed_randomly
 
 
 class Seeder:
     def __init__(self, master_seed, ngpus, local_rank):
 
-        self.master_seed = (
-            master_seed if master_seed is not None else generate_master_seed_randomly()
-        )
+        self.master_seed_was_none = master_seed is None
+        if master_seed is None and local_rank == 0:
+            print('INFO: master_seed is None in seeder.init, random '
+                  'master_seed will be generated (different one for '
+                  'each worker).')
+
+        self.master_seed = (master_seed if master_seed is not None
+                            else generate_master_seed_randomly())
         self.seed_gen = SeedGen(self.master_seed, ngpus, local_rank)
         self._ext_generators = []
+        self._ext_generators_shared = []
 
-    def register_generator(self, gen):
-        self._ext_generators.append(gen)
+    def register_generator(self, gen, shared=False):
+        if shared:
+            if self.master_seed_was_none:
+                raise Exception('master_seed was None during seeder.init, '
+                                'seeds shared among workers cannot be used.')
+            self._ext_generators_shared.append(gen)
+        else:
+            self._ext_generators.append(gen)
 
     def unregister_generator(self, gen):
-        self._ext_generators.remove(gen)
+        try:
+            self._ext_generators.remove(gen)
+        except ValueError:
+            self._ext_generators_shared.remove(gen)
 
     def reseed(self, task, epoch):
         seed = self.seed_gen(task, epoch)
         torch.manual_seed(seed)
         np.random.seed(seed)
         random.seed(seed)
 
         for generator in self._ext_generators:
             generator(seed)
 
+        if self._ext_generators_shared:
+            shared_seed = self.seed_gen(task, epoch, shared_seed=True)
+            for generator in self._ext_generators_shared:
+                generator(shared_seed)
+
 
 _seeder_run = None
 
 
 def init(master_seed, ngpus, local_rank):
     global _seeder_run
     _seeder_run = Seeder(master_seed, ngpus, local_rank)
@@ -58,15 +78,15 @@
 
 
 def get_master_seed():
     global _seeder_run
     return _seeder_run.master_seed
 
 
-def register_generator(gen):
+def register_generator(gen, shared=False):
     global _seeder_run
-    _seeder_run._ext_generators.append(gen)
+    _seeder_run.register_generator(gen, shared)
 
 
 def unregister_generator(gen):
     global _seeder_run
-    _seeder_run._ext_generators.remove(gen)
+    _seeder_run.unregister_generator(gen)
```

### Comparing `framework-reproducibility-0.4.0/fwr13y/seeder/tf.py` & `framework-reproducibility-0.5.0/fwr13y/seeder/paddle.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,43 +10,63 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ========================================================================
 
 import random
-import tensorflow as tf
+import paddle
 import numpy as np
 from .seed_gen import SeedGen, generate_master_seed_randomly
 
 
 class Seeder:
     def __init__(self, master_seed, ngpus, local_rank):
 
-        self.master_seed = (
-            master_seed if master_seed is not None else generate_master_seed_randomly()
-        )
+        self.master_seed_was_none = master_seed is None
+        if master_seed is None and local_rank == 0:
+            print('INFO: master_seed is None in seeder.init, random '
+                  'master_seed will be generated (different one for '
+                  'each worker).')
+
+        self.master_seed = (master_seed if master_seed is not None
+                            else generate_master_seed_randomly())
         self.seed_gen = SeedGen(self.master_seed, ngpus, local_rank)
         self._ext_generators = []
+        self._ext_generators_shared = []
 
-    def register_generator(self, gen):
-        self._ext_generators.append(gen)
+    def register_generator(self, gen, shared=False):
+        if shared:
+            if self.master_seed_was_none:
+                raise Exception('master_seed was None during seeder.init, '
+                                'seeds shared among workers cannot be used.')
+            self._ext_generators_shared.append(gen)
+        else:
+            self._ext_generators.append(gen)
 
     def unregister_generator(self, gen):
-        self._ext_generators.remove(gen)
+        try:
+            self._ext_generators.remove(gen)
+        except ValueError:
+            self._ext_generators_shared.remove(gen)
 
     def reseed(self, task, epoch):
         seed = self.seed_gen(task, epoch)
-        tf.random.set_seed(seed)
+        paddle.seed(seed)
         np.random.seed(seed)
         random.seed(seed)
 
         for generator in self._ext_generators:
             generator(seed)
 
+        if self._ext_generators_shared:
+            shared_seed = self.seed_gen(task, epoch, shared_seed=True)
+            for generator in self._ext_generators_shared:
+                generator(shared_seed)
+
 
 _seeder_run = None
 
 
 def init(master_seed, ngpus, local_rank):
     global _seeder_run
     _seeder_run = Seeder(master_seed, ngpus, local_rank)
@@ -58,21 +78,15 @@
 
 
 def get_master_seed():
     global _seeder_run
     return _seeder_run.master_seed
 
 
-def register_generator(gen):
+def register_generator(gen, shared=False):
     global _seeder_run
-    _seeder_run._ext_generators.append(gen)
+    _seeder_run.register_generator(gen, shared)
 
 
 def unregister_generator(gen):
     global _seeder_run
-    _seeder_run._ext_generators.remove(gen)
-
-
-class SeederCB(tf.keras.callbacks.Callback):
-    def on_epoch_begin(self, epoch, logs=None):
-        global _seeder_run
-        _seeder_run.reseed(1, epoch)
+    _seeder_run.unregister_generator(gen)
```

### Comparing `framework-reproducibility-0.4.0/fwr13y/seeder/paddle.py` & `framework-reproducibility-0.5.0/fwr13y/seeder/tf.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,43 +10,63 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ========================================================================
 
 import random
-import paddle
+import tensorflow as tf
 import numpy as np
 from .seed_gen import SeedGen, generate_master_seed_randomly
 
 
 class Seeder:
     def __init__(self, master_seed, ngpus, local_rank):
 
-        self.master_seed = (
-            master_seed if master_seed is not None else generate_master_seed_randomly()
-        )
+        self.master_seed_was_none = master_seed is None
+        if master_seed is None and local_rank == 0:
+            print('INFO: master_seed is None in seeder.init, random '
+                  'master_seed will be generated (different one for each '
+                  'worker).')
+
+        self.master_seed = (master_seed if master_seed is not None
+                            else generate_master_seed_randomly())
         self.seed_gen = SeedGen(self.master_seed, ngpus, local_rank)
         self._ext_generators = []
+        self._ext_generators_shared = []
 
-    def register_generator(self, gen):
-        self._ext_generators.append(gen)
+    def register_generator(self, gen, shared=False):
+        if shared:
+            if self.master_seed_was_none:
+                raise Exception('master_seed was None during seeder.init, '
+                                'seeds shared among workers cannot be used.')
+            self._ext_generators_shared.append(gen)
+        else:
+            self._ext_generators.append(gen)
 
     def unregister_generator(self, gen):
-        self._ext_generators.remove(gen)
+        try:
+            self._ext_generators.remove(gen)
+        except ValueError:
+            self._ext_generators_shared.remove(gen)
 
     def reseed(self, task, epoch):
         seed = self.seed_gen(task, epoch)
-        paddle.seed(seed)
+        tf.random.set_seed(seed)
         np.random.seed(seed)
         random.seed(seed)
 
         for generator in self._ext_generators:
             generator(seed)
 
+        if self._ext_generators_shared:
+            shared_seed = self.seed_gen(task, epoch, shared_seed=True)
+            for generator in self._ext_generators_shared:
+                generator(shared_seed)
+
 
 _seeder_run = None
 
 
 def init(master_seed, ngpus, local_rank):
     global _seeder_run
     _seeder_run = Seeder(master_seed, ngpus, local_rank)
@@ -58,15 +78,20 @@
 
 
 def get_master_seed():
     global _seeder_run
     return _seeder_run.master_seed
 
 
-def register_generator(gen):
+def register_generator(gen, shared=False):
     global _seeder_run
-    _seeder_run._ext_generators.append(gen)
+    _seeder_run.register_generator(gen, shared)
 
 
 def unregister_generator(gen):
     global _seeder_run
-    _seeder_run._ext_generators.remove(gen)
+    _seeder_run.unregister_generator(gen)
+
+class SeederCB(tf.keras.callbacks.Callback):
+    def on_epoch_begin(self, epoch, logs=None):
+        global _seeder_run
+        _seeder_run.reseed(1, epoch)
```

### Comparing `framework-reproducibility-0.4.0/fwr13y/seeder/__init__.py` & `framework-reproducibility-0.5.0/fwr13y/seeder/__init__.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.4.0/fwr13y/version.py` & `framework-reproducibility-0.5.0/fwr13y/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ========================================================================
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
```

### Comparing `framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/patch_segment_sum.py` & `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_segment_sum.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/patch_unsorted_segment_sum.py` & `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_unsorted_segment_sum.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/patch_bias_add.py` & `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_bias_add.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/enable_determinism.py` & `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/enable_determinism.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/patch.py` & `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.4.0/fwr13y/d9m/tensorflow/__init__.py` & `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.4.0/fwr13y/d9m/utils.py` & `framework-reproducibility-0.5.0/fwr13y/d9m/utils.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.4.0/fwr13y/d9m/__init__.py` & `framework-reproducibility-0.5.0/fwr13y/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 NVIDIA. All Rights Reserved.
+# Copyright 2020 NVIDIA Corporation. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,7 +12,9 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ========================================================================
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
+
+from .version import __version__
```

### Comparing `framework-reproducibility-0.4.0/fwr13y/__init__.py` & `framework-reproducibility-0.5.0/fwr13y/d9m/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2020 NVIDIA. All Rights Reserved.
+# Copyright 2022 NVIDIA Corporation. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,9 +12,7 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ========================================================================
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
-
-from .version import __version__
```

### Comparing `framework-reproducibility-0.4.0/framework_reproducibility.egg-info/PKG-INFO` & `framework-reproducibility-0.5.0/framework_reproducibility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framework-reproducibility
-Version: 0.4.0
+Version: 0.5.0
 Summary: Providing reproducibility in deep learning frameworks
 Home-page: https://github.com/NVIDIA/framework-reproducibility
 Author: NVIDIA
 Author-email: duncan@nvidia.com
 License: Apache 2.0
 Description: This package provides patches and tools related to determinism
         (bit-accurate, run-to-run reproducibility) in deep learning frameworks, with a
```

### Comparing `framework-reproducibility-0.4.0/framework_reproducibility.egg-info/SOURCES.txt` & `framework-reproducibility-0.5.0/framework_reproducibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

