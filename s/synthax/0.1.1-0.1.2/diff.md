# Comparing `tmp/synthax-0.1.1.tar.gz` & `tmp/synthax-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthax-0.1.1.tar", last modified: Tue Jun 20 18:32:37 2023, max compression
+gzip compressed data, was "synthax-0.1.2.tar", last modified: Thu Jun 22 23:10:22 2023, max compression
```

## Comparing `synthax-0.1.1.tar` & `synthax-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:32:37.045415 synthax-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-20 18:32:25.000000 synthax-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-20 18:32:37.045415 synthax-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-20 18:32:25.000000 synthax-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:32:37.045415 synthax-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-20 18:32:25.000000 synthax-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:32:37.045415 synthax-0.1.1/synthax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:32:37.045415 synthax-0.1.1/synthax/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/modules/amplifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/modules/blend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/modules/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/modules/envelopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/modules/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/modules/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/modules/lfos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/modules/mixers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/modules/oscillators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19034 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/synth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-20 18:32:25.000000 synthax-0.1.1/synthax/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:32:37.045415 synthax-0.1.1/synthax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-20 18:32:37.000000 synthax-0.1.1/synthax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 18:32:37.000000 synthax-0.1.1/synthax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:32:37.000000 synthax-0.1.1/synthax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 18:32:37.000000 synthax-0.1.1/synthax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 18:32:37.000000 synthax-0.1.1/synthax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:22.553551 synthax-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-22 23:10:13.000000 synthax-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-22 23:10:22.553551 synthax-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-22 23:10:13.000000 synthax-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 23:10:22.553551 synthax-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-22 23:10:13.000000 synthax-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:22.545551 synthax-0.1.2/synthax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:22.553551 synthax-0.1.2/synthax/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/amplifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/blend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/envelopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/lfos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/mixers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/modules/oscillators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19034 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/synth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-22 23:10:13.000000 synthax-0.1.2/synthax/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:10:22.549551 synthax-0.1.2/synthax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-22 23:10:22.000000 synthax-0.1.2/synthax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-22 23:10:22.000000 synthax-0.1.2/synthax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 23:10:22.000000 synthax-0.1.2/synthax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-22 23:10:22.000000 synthax-0.1.2/synthax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 23:10:22.000000 synthax-0.1.2/synthax.egg-info/top_level.txt
```

### Comparing `synthax-0.1.1/LICENSE` & `synthax-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/PKG-INFO` & `synthax-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthax
-Version: 0.1.1
+Version: 0.1.2
 Summary: SynthAX: A Fast Modular Synthesizer in JAX
 Home-page: https://github.com/PapayaResearch/synthax
 Author: Manuel Cherep, Nikhil Singh
 Author-email: mcherep@mit.edu, nsingh1@mit.edu
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: synthax Version: 0.1.1 Summary: SynthAX: A Fast
+Metadata-Version: 2.1 Name: synthax Version: 0.1.2 Summary: SynthAX: A Fast
 Modular Synthesizer in JAX Home-page: https://github.com/PapayaResearch/synthax
 Author: Manuel Cherep, Nikhil Singh Author-email: mcherep@mit.edu,
 nsingh1@mit.edu Classifier: Programming Language :: Python :: 3.9 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE # SynthAX: A Fast Modular Synthesizer in JAX â¡ï¸ [!
 [Pyversions](https://img.shields.io/pypi/pyversions/synthax.svg?style=flat-
```

### Comparing `synthax-0.1.1/README.md` & `synthax-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/setup.py` & `synthax-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 setup(name="synthax",
-      version="0.1.1",
+      version="0.1.2",
       url="https://github.com/PapayaResearch/synthax",
       author="Manuel Cherep, Nikhil Singh",
       author_email="mcherep@mit.edu, nsingh1@mit.edu",
       description="SynthAX: A Fast Modular Synthesizer in JAX",
       long_description=open("README.md").read(),
       long_description_content_type="text/markdown",
       packages=find_packages(),
```

### Comparing `synthax-0.1.1/synthax/config.py` & `synthax-0.1.2/synthax/config.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/functional.py` & `synthax-0.1.2/synthax/functional.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import jax
+import flax
 import jax.numpy as jnp
 import chex
+from typing import Tuple
 from synthax.types import Signal
 
 
 def midi_to_hz(midi: chex.Array) -> chex.Array:
     """
     Convert from midi (linear pitch) to frequency in Hz.
 
@@ -49,7 +51,25 @@
 
 def normalize(signal: Signal) -> Signal:
     """
     Normalize every individual signal in batch.
     """
     max_sample = jnp.max(jnp.abs(signal), axis=1, keepdims=True)[0]
     return signal / max_sample
+
+def flatten_params(
+        params: flax.core.frozen_dict.FrozenDict
+) -> Tuple[dict, chex.Array]:
+    """
+    Takes flax params and returns flat keys and batch of values
+    """
+    flat_dict = flax.traverse_util.flatten_dict(params)
+    keys = flat_dict.keys()
+    values = jnp.array(list(flat_dict.values()))
+    return keys, values
+
+def unflatten_params(keys: dict, values: chex.Array) -> dict:
+    """
+    Reconstructs the params from keys and values. It can be
+    passed to functions expecting a FrozenDict, but it's not frozen.
+    """
+    return flax.traverse_util.unflatten_dict(dict(zip(keys, values)))
```

### Comparing `synthax-0.1.1/synthax/io.py` & `synthax-0.1.2/synthax/io.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/modules/amplifiers.py` & `synthax-0.1.2/synthax/modules/amplifiers.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/modules/base.py` & `synthax-0.1.2/synthax/modules/base.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/modules/blend.py` & `synthax-0.1.2/synthax/modules/blend.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/modules/control.py` & `synthax-0.1.2/synthax/modules/control.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/modules/envelopes.py` & `synthax-0.1.2/synthax/modules/envelopes.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/modules/filters.py` & `synthax-0.1.2/synthax/modules/filters.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/modules/keyboard.py` & `synthax-0.1.2/synthax/modules/keyboard.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/modules/lfos.py` & `synthax-0.1.2/synthax/modules/lfos.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/modules/mixers.py` & `synthax-0.1.2/synthax/modules/mixers.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/modules/oscillators.py` & `synthax-0.1.2/synthax/modules/oscillators.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/parameter.py` & `synthax-0.1.2/synthax/parameter.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/synth.py` & `synthax-0.1.2/synthax/synth.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax/types.py` & `synthax-0.1.2/synthax/types.py`

 * *Files identical despite different names*

### Comparing `synthax-0.1.1/synthax.egg-info/PKG-INFO` & `synthax-0.1.2/synthax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthax
-Version: 0.1.1
+Version: 0.1.2
 Summary: SynthAX: A Fast Modular Synthesizer in JAX
 Home-page: https://github.com/PapayaResearch/synthax
 Author: Manuel Cherep, Nikhil Singh
 Author-email: mcherep@mit.edu, nsingh1@mit.edu
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: synthax Version: 0.1.1 Summary: SynthAX: A Fast
+Metadata-Version: 2.1 Name: synthax Version: 0.1.2 Summary: SynthAX: A Fast
 Modular Synthesizer in JAX Home-page: https://github.com/PapayaResearch/synthax
 Author: Manuel Cherep, Nikhil Singh Author-email: mcherep@mit.edu,
 nsingh1@mit.edu Classifier: Programming Language :: Python :: 3.9 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE # SynthAX: A Fast Modular Synthesizer in JAX â¡ï¸ [!
 [Pyversions](https://img.shields.io/pypi/pyversions/synthax.svg?style=flat-
```

### Comparing `synthax-0.1.1/synthax.egg-info/SOURCES.txt` & `synthax-0.1.2/synthax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

