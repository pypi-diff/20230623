# Comparing `tmp/install-pybci-0.2.4b1.tar.gz` & `tmp/install-pybci-0.2.4b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.2.4b1.tar", last modified: Mon Jun 12 20:20:57 2023, max compression
+gzip compressed data, was "install-pybci-0.2.4b2.tar", last modified: Fri Jun 23 14:39:37 2023, max compression
```

## Comparing `install-pybci-0.2.4b1.tar` & `install-pybci-0.2.4b2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-06-12 20:20:57.000000 install-pybci-0.2.4b1/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-12 20:20:57.000000 install-pybci-0.2.4b1/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:20:57.000000 install-pybci-0.2.4b1/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 20:20:57.000000 install-pybci-0.2.4b1/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 20:20:57.000000 install-pybci-0.2.4b1/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/OptimisedDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Utils/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:20:57.895265 install-pybci-0.2.4b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-12 20:20:28.000000 install-pybci-0.2.4b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-06-23 14:39:37.000000 install-pybci-0.2.4b2/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-23 14:39:37.000000 install-pybci-0.2.4b2/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:39:37.000000 install-pybci-0.2.4b2/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-23 14:39:37.000000 install-pybci-0.2.4b2/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 14:39:37.000000 install-pybci-0.2.4b2/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/OptimisedDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Utils/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:39:37.304489 install-pybci-0.2.4b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-23 14:39:08.000000 install-pybci-0.2.4b2/setup.py
```

### Comparing `install-pybci-0.2.4b1/LICENSE` & `install-pybci-0.2.4b2/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/PKG-INFO` & `install-pybci-0.2.4b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.4b1
-Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
+Version: 0.2.4b2
+Summary: A Python interface to create a BCI with the Lab Streaming Layer, Pytorch, SciKit-Learn and Tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: System :: Networking
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create near-real-time Brain Computer Interfaces (BCI's). with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
@@ -46,15 +52,15 @@
 import time
 from pybci import PyBCI
 bci = PyBCI() # set default epoch timing, looks for first available lsl marker stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
 try:
     while(True): # training based on couple epochs more then min threshold for classifying
-        currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
+        currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent are too close together will be ignored till done processing
         time.sleep(1) # wait for marker updates
         print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
         if len(currentMarkers) > 1:  # check there is more then one marker type received
             if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired:
                 classInfo = bci.CurrentClassifierInfo() # hangs if called too early
                 accuracy = classInfo["accuracy"]
             if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired+1:  
@@ -73,16 +79,16 @@
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
-- Update ReadTheDocs!
-- Finish arduino hand grasp demo and video.
+- ~~Update ReadTheDocs!~~
+- ~~Finish arduino hand grasp demo and video.~~
 - Tst and likely Fix multimodal after new data thread creation
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
 - ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
 - ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
 - ~~Levels of print debug (info, error, none)~~
 - ~~Retrieve feature data~~
```

### Comparing `install-pybci-0.2.4b1/README.md` & `install-pybci-0.2.4b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create near-real-time Brain Computer Interfaces (BCI's). with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
@@ -22,15 +22,15 @@
 import time
 from pybci import PyBCI
 bci = PyBCI() # set default epoch timing, looks for first available lsl marker stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
 try:
     while(True): # training based on couple epochs more then min threshold for classifying
-        currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
+        currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent are too close together will be ignored till done processing
         time.sleep(1) # wait for marker updates
         print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
         if len(currentMarkers) > 1:  # check there is more then one marker type received
             if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired:
                 classInfo = bci.CurrentClassifierInfo() # hangs if called too early
                 accuracy = classInfo["accuracy"]
             if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired+1:  
@@ -49,16 +49,16 @@
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
-- Update ReadTheDocs!
-- Finish arduino hand grasp demo and video.
+- ~~Update ReadTheDocs!~~
+- ~~Finish arduino hand grasp demo and video.~~
 - Tst and likely Fix multimodal after new data thread creation
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
 - ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
 - ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
 - ~~Levels of print debug (info, error, none)~~
 - ~~Retrieve feature data~~
```

### Comparing `install-pybci-0.2.4b1/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.2.4b2/install_pybci.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.4b1
-Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
+Version: 0.2.4b2
+Summary: A Python interface to create a BCI with the Lab Streaming Layer, Pytorch, SciKit-Learn and Tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: System :: Networking
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci) [![PyPI - version](https://img.shields.io/pypi/v/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create near-real-time Brain Computer Interface (BCI)'s. with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create near-real-time Brain Computer Interfaces (BCI's). with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) or [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
 The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
@@ -46,15 +52,15 @@
 import time
 from pybci import PyBCI
 bci = PyBCI() # set default epoch timing, looks for first available lsl marker stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
 try:
     while(True): # training based on couple epochs more then min threshold for classifying
-        currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
+        currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent are too close together will be ignored till done processing
         time.sleep(1) # wait for marker updates
         print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
         if len(currentMarkers) > 1:  # check there is more then one marker type received
             if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired:
                 classInfo = bci.CurrentClassifierInfo() # hangs if called too early
                 accuracy = classInfo["accuracy"]
             if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired+1:  
@@ -73,16 +79,16 @@
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count as more then one marker, example: in training mode a baseline marker may have one marker sent for a 60 second window, whereas target actions may only be ~0.5s long,  when testing the model and data is constantly analysed it would be desirable to standardise the window length, we do this by splitting the 60s window after the received baseline marker in to ~0.5s windows. PyBCI allows optional overlapping of time windows to try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the model will begin to fit. Once fit the classifier info can be queried with CurrentClassifierInfo, this returns the model used and accuracy, is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
-- Update ReadTheDocs!
-- Finish arduino hand grasp demo and video.
+- ~~Update ReadTheDocs!~~
+- ~~Finish arduino hand grasp demo and video.~~
 - Tst and likely Fix multimodal after new data thread creation
 - ~~Combine multiple data streams for multi modal bci!~~
 - ~~Add pytorch compatibility!~~ 
 - ~~run check on pytorch data type (may pass list with [pytorchmodel, pytrochcompilerinfo])~~
 - ~~Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.~~ (Added universal optimised thread to handle all cases)
 - ~~Levels of print debug (info, error, none)~~
 - ~~Retrieve feature data~~
```

### Comparing `install-pybci-0.2.4b1/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.2.4b2/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/Configuration/EpochSettings.py` & `install-pybci-0.2.4b2/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.2.4b2/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.2.4b2/pybci/ThreadClasses/ClassifierThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.2.4b2/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-0.2.4b2/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.2.4b2/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/ThreadClasses/OptimisedDataReceiverThread.py` & `install-pybci-0.2.4b2/pybci/ThreadClasses/OptimisedDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/Utils/Classifier.py` & `install-pybci-0.2.4b2/pybci/Utils/Classifier.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.2.4b2/pybci/Utils/FeatureExtractor.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/Utils/LSLScanner.py` & `install-pybci-0.2.4b2/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/Utils/Logger.py` & `install-pybci-0.2.4b2/pybci/Utils/Logger.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/pybci/pybci.py` & `install-pybci-0.2.4b2/pybci/pybci.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.4b1/setup.py` & `install-pybci-0.2.4b2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 setup(
     name='install-pybci',
 
     version=version['__version__'],
 
-    description='A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages',
+    description='A Python interface to create a BCI with the Lab Streaming Layer, Pytorch, SciKit-Learn and Tensorflow packages',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://github.com/lmbooth/pybci',
 
     # Author details
@@ -65,28 +65,34 @@
         #   4 - Beta
         #   5 - Production/Stable
         'Development Status :: 4 - Beta',
 
         # Indicate who your project is intended for
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
-        'Topic :: System :: Networking',
+        'Intended Audience :: Healthcare Industry',
+        'Topic :: Scientific/Engineering :: Human Machine Interfaces',
+        'Topic :: Scientific/Engineering :: Bio-Informatics',
+        'Topic :: Scientific/Engineering :: Medical Science Apps.',
+        'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering',
 
         # Pick your license as you wish (should match "license" above)
         'License :: OSI Approved :: MIT License',
 
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     python_requires='>=3.9',
     # What does your project relate to?
     keywords='machine learning and data synchronisation on the Lab Streaming Layer',
 
     cmdclass={
         'bdist_wheel': bdist_wheel
@@ -94,15 +100,16 @@
 
     install_requires=[
         "pylsl",
         "scipy",
         "numpy",
         "antropy",
         "tensorflow",
-        "scikit-learn"
+        "scikit-learn",
+        "torch"
     ],
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     packages= find_packages(),#['pybci', 'pybci.examples'],
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
```

