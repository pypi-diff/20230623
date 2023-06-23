# Comparing `tmp/pytorch-pipline-0.2.3.tar.gz` & `tmp/pytorch-pipline-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-pipline-0.2.3.tar", last modified: Tue Jun 20 08:22:27 2023, max compression
+gzip compressed data, was "pytorch-pipline-0.2.4.tar", last modified: Fri Jun 23 06:43:46 2023, max compression
```

## Comparing `pytorch-pipline-0.2.3.tar` & `pytorch-pipline-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:22:27.823863 pytorch-pipline-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-20 08:22:27.823863 pytorch-pipline-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 08:22:18.000000 pytorch-pipline-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:22:27.823863 pytorch-pipline-0.2.3/pytorchPipline/
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-20 08:22:18.000000 pytorch-pipline-0.2.3/pytorchPipline/BenchMark.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-20 08:22:18.000000 pytorch-pipline-0.2.3/pytorchPipline/Pipline.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 08:22:18.000000 pytorch-pipline-0.2.3/pytorchPipline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:22:27.823863 pytorch-pipline-0.2.3/pytorch_pipline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-20 08:22:27.000000 pytorch-pipline-0.2.3/pytorch_pipline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-20 08:22:27.000000 pytorch-pipline-0.2.3/pytorch_pipline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:22:27.000000 pytorch-pipline-0.2.3/pytorch_pipline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 08:22:27.000000 pytorch-pipline-0.2.3/pytorch_pipline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 08:22:27.000000 pytorch-pipline-0.2.3/pytorch_pipline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:22:27.823863 pytorch-pipline-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-20 08:22:18.000000 pytorch-pipline-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:43:46.725211 pytorch-pipline-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-23 06:43:46.725211 pytorch-pipline-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 06:43:34.000000 pytorch-pipline-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:43:46.725211 pytorch-pipline-0.2.4/pytorchPipline/
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-23 06:43:34.000000 pytorch-pipline-0.2.4/pytorchPipline/BenchMark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-23 06:43:34.000000 pytorch-pipline-0.2.4/pytorchPipline/Pipline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-23 06:43:34.000000 pytorch-pipline-0.2.4/pytorchPipline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:43:46.725211 pytorch-pipline-0.2.4/pytorch_pipline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-23 06:43:46.000000 pytorch-pipline-0.2.4/pytorch_pipline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-23 06:43:46.000000 pytorch-pipline-0.2.4/pytorch_pipline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:43:46.000000 pytorch-pipline-0.2.4/pytorch_pipline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 06:43:46.000000 pytorch-pipline-0.2.4/pytorch_pipline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 06:43:46.000000 pytorch-pipline-0.2.4/pytorch_pipline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 06:43:46.725211 pytorch-pipline-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-23 06:43:34.000000 pytorch-pipline-0.2.4/setup.py
```

### Comparing `pytorch-pipline-0.2.3/PKG-INFO` & `pytorch-pipline-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-pipline
-Version: 0.2.3
+Version: 0.2.4
 Summary: Making pytorch training easier
 Author: Charlie Huang
 Author-email: <charliehuang09@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytorch-pipline-0.2.3/pytorchPipline/BenchMark.py` & `pytorch-pipline-0.2.4/pytorchPipline/BenchMark.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import torch.optim as optim
 from torchvision import transforms
 import numpy as np
 from tqdm import trange
 from pytorchPipline.Pipline import TrainModel, TestModel, FitModel
 from timeit import default_timer as timer
 
-def BenchMark(epoch=10, batch_size = 256, progressBar=True, num_workers=0):
+def BenchMark(epoch=10, batch_size = 256, progressBar=True, num_workers=0, device=torch.device('cpu')):
     
     start = timer()
     trainLoader = datasets.MNIST(
         root="./",
         train=True,
         download=True,
         transform=transforms.ToTensor()
@@ -24,16 +24,14 @@
         download=True,
         transform=transforms.ToTensor()
         )
     
     trainLoader = DataLoader(trainLoader, batch_size=batch_size, num_workers=num_workers)
     testLoader = DataLoader(testLoader, batch_size=batch_size, num_workers=num_workers)
     
-    device = torch.device('mps')
-    
     class mainConvModel(nn.Module):
     
         def __init__(self):
             super(mainConvModel, self).__init__()
             self.to64conv = nn.Sequential(
                 nn.Conv2d(1, 4, (3, 3)),
                 nn.ReLU(),
```

### Comparing `pytorch-pipline-0.2.3/pytorchPipline/Pipline.py` & `pytorch-pipline-0.2.4/pytorchPipline/Pipline.py`

 * *Files identical despite different names*

### Comparing `pytorch-pipline-0.2.3/pytorch_pipline.egg-info/PKG-INFO` & `pytorch-pipline-0.2.4/pytorch_pipline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-pipline
-Version: 0.2.3
+Version: 0.2.4
 Summary: Making pytorch training easier
 Author: Charlie Huang
 Author-email: <charliehuang09@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytorch-pipline-0.2.3/setup.py` & `pytorch-pipline-0.2.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.3'
+VERSION = '0.2.4'
 DESCRIPTION = 'Making pytorch training easier'
 LONG_DESCRIPTION = 'A package that has functions making the training loop faster to write'
 
 # Setting up
 setup(
     name="pytorch-pipline",
     version=VERSION,
```

