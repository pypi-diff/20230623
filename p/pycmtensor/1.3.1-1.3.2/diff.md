# Comparing `tmp/pycmtensor-1.3.1.tar.gz` & `tmp/pycmtensor-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycmtensor-1.3.1.tar", max compression
+gzip compressed data, was "pycmtensor-1.3.2.tar", max compression
```

## Comparing `pycmtensor-1.3.1.tar` & `pycmtensor-1.3.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1070 2022-11-17 16:21:59.841938 pycmtensor-1.3.1/LICENSE
--rw-r--r--   0        0        0    10501 2022-11-17 16:21:59.841938 pycmtensor-1.3.1/README.md
--rw-r--r--   0        0        0      362 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/__init__.py
--rw-r--r--   0        0        0     5870 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/config.py
--rw-r--r--   0        0        0    11474 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/data.py
--rw-r--r--   0        0        0    13883 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/expressions.py
--rw-r--r--   0        0        0    11316 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/functions.py
--rw-r--r--   0        0        0     1376 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/logger.py
--rw-r--r--   0        0        0     2514 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/models/MNL.py
--rw-r--r--   0        0        0      189 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/models/ResLogit.py
--rw-r--r--   0        0        0       21 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/models/__init__.py
--rw-r--r--   0        0        0     6890 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/models/layers.py
--rw-r--r--   0        0        0    17876 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/optimizers.py
--rw-r--r--   0        0        0    11520 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/pycmtensor.py
--rw-r--r--   0        0        0     4959 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/results.py
--rw-r--r--   0        0        0     7126 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/scheduler.py
--rw-r--r--   0        0        0     3798 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/statistics.py
--rw-r--r--   0        0        0      420 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pycmtensor/utils.py
--rw-r--r--   0        0        0     2931 2022-11-17 16:21:59.849938 pycmtensor-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    12697 2022-11-17 16:22:12.201770 pycmtensor-1.3.1/setup.py
--rw-r--r--   0        0        0    12636 2022-11-17 16:22:12.202922 pycmtensor-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-23 09:45:45.165672 pycmtensor-1.3.2/LICENSE
+-rw-r--r--   0        0        0    10842 2023-06-23 09:45:45.165672 pycmtensor-1.3.2/README.md
+-rw-r--r--   0        0        0      362 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/__init__.py
+-rw-r--r--   0        0        0     6050 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/config.py
+-rw-r--r--   0        0        0    11593 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/data.py
+-rw-r--r--   0        0        0    13948 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/expressions.py
+-rw-r--r--   0        0        0    11511 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/functions.py
+-rw-r--r--   0        0        0     1366 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/logger.py
+-rw-r--r--   0        0        0     3208 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/models/MNL.py
+-rw-r--r--   0        0        0      189 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/models/ResLogit.py
+-rw-r--r--   0        0        0       21 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/models/__init__.py
+-rw-r--r--   0        0        0     6890 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/models/layers.py
+-rw-r--r--   0        0        0    18014 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/optimizers.py
+-rw-r--r--   0        0        0    11944 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/pycmtensor.py
+-rw-r--r--   0        0        0     4959 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/results.py
+-rw-r--r--   0        0        0     7126 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/scheduler.py
+-rw-r--r--   0        0        0     3798 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/statistics.py
+-rw-r--r--   0        0        0      420 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pycmtensor/utils.py
+-rw-r--r--   0        0        0     2943 2023-06-23 09:45:45.173672 pycmtensor-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    12987 1970-01-01 00:00:00.000000 pycmtensor-1.3.2/PKG-INFO
```

### Comparing `pycmtensor-1.3.1/LICENSE` & `pycmtensor-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.3.1/README.md` & `pycmtensor-1.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,296 +1,305 @@
 # PyCMTensor
 
 ![Licence](https://img.shields.io/badge/Licence-MIT-blue)
 ![](https://img.shields.io/pypi/pyversions/pycmtensor)
 [![PyPI version](https://badge.fury.io/py/pycmtensor.svg)](https://badge.fury.io/py/pycmtensor)
 [![Documentation Status](https://readthedocs.org/projects/pycmtensor/badge/?version=latest)](https://pycmtensor.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/mwong009/pycmtensor/branch/master/graph/badge.svg?token=LFwgggDyjS)](https://codecov.io/gh/mwong009/pycmtensor)
+[![Downloads](https://static.pepy.tech/personalized-badge/pycmtensor?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pycmtensor)
 
 [![Tests](https://github.com/mwong009/pycmtensor/actions/workflows/tests.yml/badge.svg)](https://github.com/mwong009/pycmtensor/actions/workflows/tests.yml)
 [![CodeQL](https://github.com/mwong009/pycmtensor/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/mwong009/pycmtensor/actions/workflows/codeql-analysis.yml)
 [![Publish](https://github.com/mwong009/pycmtensor/actions/workflows/publish.yml/badge.svg)](https://github.com/mwong009/pycmtensor/actions/workflows/publish.yml)
 [![DOI](https://zenodo.org/badge/460802394.svg)](https://zenodo.org/badge/latestdoi/460802394)
 
-A tensor-based discrete choice modelling Python package. 
-
-## Citation
-
-Cite as:
-
-    @software{melvin_wong_2022_7249280,
-      author       = {Melvin Wong},
-      title        = {mwong009/pycmtensor: v1.3.1},
-      year         = 2022,
-      version      = {v1.3.1},
-      doi          = {10.5281/zenodo.7249280},
-      url          = {https://doi.org/10.5281/zenodo.7249280}
-    }
+PyCMTensor is a discrete choice modelling development tool on deep learning libraries, enabling development of complex models using deep neural networks.
+PyCMTensor is build with [Aesara](https://github.com/aesara-devs/aesara) package, similar to ``Tensorflow`` or ``Keras``.
+``Aesara`` is used the backend library because of its hackable, open-source nature.
+Users of [Biogeme](https://biogeme.epfl.ch) would be familiar with the syntax of PyCMTensor.
+PyCMTensor improves on [Biogeme](https://biogeme.epfl.ch) in situations where much more complex models are necessary, for example, integrating neural networks into discrete choice models.
+PyCMTensor also include the ability to estimate models using stochastic gradient descent methods by default, e.g. Nesterov Accelerated Gradient (NAG), Adaptive momentum (ADAM), or RMSProp.
 
 ## Table of contents
 
-
 - [PyCMTensor](#pycmtensor)
-	- [Citation](#citation)
-	- [Table of contents](#table-of-contents)
-	- [About PyCMTensor](#about-pycmtensor)
-	- [Features](#features)
+  - [Table of contents](#table-of-contents)
+  - [Features](#features)
 - [Quick start](#quick-start)
-	- [Installation](#installation)
+  - [Installation](#installation)
 - [Usage](#usage)
-	- [Simple example: Swissmetro dataset](#simple-example-swissmetro-dataset)
-	- [Results](#results)
+  - [Simple example: MNL model using the Swissmetro dataset](#simple-example-mnl-model-using-the-swissmetro-dataset)
+  - [Results](#results)
 - [Development](#development)
-	- [Installing the virtual environment](#installing-the-virtual-environment)
-	- [Install the project and development dependencies](#install-the-project-and-development-dependencies)
-
-## About PyCMTensor
-
-PyCMTensor is a discrete choice modelling development tool on deep learning libraries, enabling development of complex models using deep neural networks.
-PyCMTensor is build on [Aesara](https://github.com/aesara-devs/aesara), a tensor library which uses features commonly found in deep learning packages such as ``Tensorflow`` and ``Keras``.
-``Aesara`` was chosen as the back end mathematical library because of its hackable, open-source nature.
-Users of [Biogeme](https://biogeme.epfl.ch) would be familiar with the syntax of PyCMTensor.
+  - [Installing the virtual environment](#installing-the-virtual-environment)
+  - [Install the project and development dependencies](#install-the-project-and-development-dependencies)
+  - [Citation](#citation)
 
-PyCMTensor improves on [Biogeme](https://biogeme.epfl.ch) in situations where much more complex models are necessary, for example, integrating neural networks into discrete choice models.
-PyCMTensor also include the ability to estimate models using 1st order stochastic gradient descent methods by default, such as Nesterov Accelerated Gradient (NAG), Adaptive momentum (ADAM), or RMSProp.
 
 ## Features
 
-* Estimate complex choice models with neural networks using deep learning algorithms
-* Combines traditional econometric models (e.g. Multinomial Logit) with deep learning models (e.g. ResNets)
-* Shares similar programming syntax with ``Biogeme``, allowing easy transition between models
+* Estimate complex choice models using deep learning methods
+* Combines traditional econometric models (Multinomial Logit) with neural networks
+* Similar programming syntax as ``Biogeme``
 * Uses tensor features found in the ``Aesara`` library
 
 ---
 
 # Quick start
 
 ## Installation
 
 1. Download and install [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
-	Full Anaconda works fine, but Miniconda is recommmended for a minimal installation. Ensure that Conda is using at least **Python 3.9**
+    Full Anaconda works fine, but Miniconda is recommmended for a minimal installation. Ensure that Conda is using at least **Python 3.9**
+
+2. Install conda dependencies:
+   
+    Dependencies are OS specific
 
-	Next, install the required dependencies:
+    **Windows**
 
-	**Windows**
+    ```
+    conda install mkl-service conda-forge::cxx-compiler conda-forge::m2w64-toolchain
+    ```
+    **Linux**
 
-	```
-	conda install mkl-service conda-forge::cxx-compiler conda-forge::m2w64-toolchain
-	```
-	**Linux**
+    ```
+    conda install mkl-service conda-forge::cxx-compiler
+    ```
 
-	```
-	conda install mkl-service conda-forge::cxx-compiler
-	```
+    **Mac OSX**
 
-	**Mac OSX**
+    ```
+    conda install mkl-service Clang
+    ```
 
-	```
-	conda install mkl-service Clang
-	```
+    **\*\*Optional\*\***
 
-2. Install the ``PyCMTensor`` package
+    Alternatively, conda ``environment.yml`` files are provided in the ``environment/`` in respective operating systems, for example in Windows:
 
-	PyCMTensor is available on PyPi https://pypi.org/project/pycmtensor/. It can be installed with ``pip``
+    ```
+    conda env create -f environment/environment_windows.yml
+    conda activate pycmtensor-dev
+    ```
 
-	```
-	pip install -U pycmtensor==1.3.1
-	```
 
-	Alternatively, the latest development version is available via [Github](https://github.com/mwong009/pycmtensor). It can be installed via 
+3. Install the ``PyCMTensor`` package from PyPI via pip
 
-	```
-	pip install -U git+https://github.com/mwong009/pycmtensor.git
-	```
+    ```
+    pip install -U pycmtensor==1.3.2
+    ```
+
+    Alternatively, the latest development version is available via [Github](https://github.com/mwong009/pycmtensor). It can be installed via 
+
+    ```
+    pip install -U git+https://github.com/mwong009/pycmtensor.git
+    ```
 
 For more information about installing, see [Installation](https://pycmtensor.readthedocs.io/en/latest/installation.html).
 
 # Usage
 
 PyCMTensor uses syntax very similar to ``Biogeme``. Users of ``Biogeme`` should be familiar with the syntax.
 Make sure you are using the correct Conda environment and/or the required packages are installed.
 
-## Simple example: Swissmetro dataset
+## Simple example: MNL model using the Swissmetro dataset
 
-1. Start an interactive session (e.g. ``IPython`` or Jupyter Notebook) and import the ``PyCMTensor`` package:
-	```python
-	import pycmtensor as cmt
-	import pandas as pd
-	```
-
-	Several submodules to include:
-	```python
-	from pycmtensor.expressions import Beta # Beta class for model parameters
-	from pycmtensor.models import MNL  # MNL model
-	from pycmtensor.statistics import elasticities  # For calculating elasticities
-	```
+1. Start an interactive session (e.g. ``IPython`` or Jupyter Notebook) and import the ``PyCMTensor`` package and ``pandas``:
+    ```python
+    import pycmtensor as cmt
+    import pandas as pd
+    ```
+
+    Include the additional submodules:
+    ```python
+    from pycmtensor.expressions import Beta # Beta class for model parameters
+    from pycmtensor.models import MNL  # MNL model
+    from pycmtensor.statistics import elasticities  # For calculating elasticities
+    ```
 
-	For a full list of submodules and description, refer to [API Reference](https://pycmtensor.readthedocs.io/en/latest/autoapi/index.html).
-	Using the [swissmetro dataset](https://biogeme.epfl.ch/data.html), we define a simple MNL model. 
+    For a full list of submodules and description, refer to [API Reference](https://pycmtensor.readthedocs.io/en/latest/autoapi/index.html).
+    Using the [swissmetro dataset](https://biogeme.epfl.ch/data.html), we define a simple MNL model. 
 
 
 > :warning: Note: The following is a replication of the results from Biogeme using the ``Adam`` optimization method with constant learning rate.
 
 
 1. Import the dataset and perform some data cleaning
-	```python
-	swissmetro = pd.read_csv("swissmetro.dat", sep="\t")
-	swissmetro.drop(swissmetro[swissmetro["CHOICE"] == 0].index, inplace=True)
-	swissmetro["CHOICE"] -= 1  # set the first choice index to 0
-	db = cmt.Data(df=swissmetro, choice="CHOICE")
-	db.autoscale_data(except_for=["ID", "ORIGIN", "DEST"])  # scales dataset
-	db.split_db(split_frac=0.8)  # split dataset into train/valid sets
-	```
+    ```python
+    swissmetro = pd.read_csv("swissmetro.dat", sep="\t")
+    db = cmt.Data(
+        df=swissmetro,
+        choice="CHOICE",
+        drop=[swissmetro["CHOICE"] == 0],
+        autoscale=True,
+        autoscale_except=["ID", "ORIGIN", "DEST", "CHOICE"],
+        split=0.8,
+    )
+    ```
 
 2. Initialize the model parameters and specify the utility functions and availability conditions
-	```python
-	b_cost = Beta("b_cost", 0.0, None, None, 0)
-	b_time = Beta("b_time", 0.0, None, None, 0)
-	asc_train = Beta("asc_train", 0.0, None, None, 0)
-	asc_car = Beta("asc_car", 0.0, None, None, 0)
-	asc_sm = Beta("asc_sm", 0.0, None, None, 1)
-
-	U_1 = b_cost * db["TRAIN_CO"] + b_time * db["TRAIN_TT"] + asc_train
-	U_2 = b_cost * db["SM_CO"] + b_time * db["SM_TT"] + asc_sm
-	U_3 = b_cost * db["CAR_CO"] + b_time * db["CAR_TT"] + asc_car
-
-	# specify the utility function and the availability conditions
-	U = [U_1, U_2, U_3]  # utility
-	AV = [db["TRAIN_AV"], db["SM_AV"], db["CAR_AV"]]  # availability
-	``` 
+    ```python
+    b_cost = Beta("b_cost", 0.0, None, None, 0)
+    b_time = Beta("b_time", 0.0, None, None, 0)
+    asc_train = Beta("asc_train", 0.0, None, None, 0)
+    asc_car = Beta("asc_car", 0.0, None, None, 0)
+    asc_sm = Beta("asc_sm", 0.0, None, None, 1)
+
+    U_1 = b_cost * db["TRAIN_CO"] + b_time * db["TRAIN_TT"] + asc_train
+    U_2 = b_cost * db["SM_CO"] + b_time * db["SM_TT"] + asc_sm
+    U_3 = b_cost * db["CAR_CO"] + b_time * db["CAR_TT"] + asc_car
+
+    # specify the utility function and the availability conditions
+    U = [U_1, U_2, U_3]  # utility
+    AV = [db["TRAIN_AV"], db["SM_AV"], db["CAR_AV"]]  # availability
+    ``` 
 
 3. Define the Multinomial Logit model
-	```python
-	mymodel = MNL(db, locals(), U, AV, name="MNL")
-	```
+    ```python
+    mymodel = MNL(db, locals(), U, AV)
+    ```
 
 4. Train the model and generate model statistics (Optionally, you can also set the training hyperparameters)
-	```python
-	mymodel.config.set_hyperparameter("max_steps", 200)  # set the max number of train steps
-	mymodel.config.set_hyperparameter("batch_size", 128)  # set the training batch size
-	mymodel.train(db)  # run the model training on the dataset `db`
-	```
+    ```python
+    mymodel.train(db, max_steps=200, batch_size=128)  # run the model training on the dataset `db`
+    ```
 
 ## Results
 The following model functions outputs the statistics, results of the model, and model training
 
 1. **Model estimates**
-	```Python
-	print(mymodel.results.beta_statistics())
-	```
-
-	Output:
-	```
-	              value   std err     t-test   p-value rob. std err rob. t-test rob. p-value
-	asc_car   -0.665638  0.044783 -14.863615       0.0     0.176178    -3.77821     0.000158
-	asc_sm          0.0         -          -         -            -           -            -
-	asc_train -1.646826  0.048099 -34.238218       0.0     0.198978   -8.276443          0.0
-	b_cost     0.024912   0.01943   1.282135  0.199795     0.016413    1.517851     0.129052
-	b_time    -0.313186  0.049708  -6.300485       0.0     0.208239   -1.503979     0.132587
-	```
+    ```Python
+    print(mymodel.results.beta_statistics())
+    ```
+
+    Output:
+    ```
+                  value   std err     t-test   p-value rob. std err rob. t-test rob. p-value
+    asc_car   -0.665638  0.044783 -14.863615       0.0     0.176178    -3.77821     0.000158
+    asc_sm          0.0         -          -         -            -           -            -
+    asc_train -1.646826  0.048099 -34.238218       0.0     0.198978   -8.276443          0.0
+    b_cost     0.024912   0.01943   1.282135  0.199795     0.016413    1.517851     0.129052
+    b_time    -0.313186  0.049708  -6.300485       0.0     0.208239   -1.503979     0.132587
+    ```
 
 2. **Training results**
-	```Python
-	print(mymodel.results.model_statistics())
-	```
-
-	Output:
-	```
-	                                          value
-	Number of training samples used          8575.0
-	Number of validation samples used        2143.0
-	Init. log likelihood               -8874.438875
-	Final log likelihood                -7513.22967
-	Accuracy                                 59.26%
-	Likelihood ratio test                2722.41841
-	Rho square                             0.153385
-	Rho square bar                         0.152822
-	Akaike Information Criterion       15036.459339
-	Bayesian Information Criterion      15071.74237
-	Final gradient norm                    0.007164
-	```
+    ```Python
+    print(mymodel.results.model_statistics())
+    ```
+
+    Output:
+    ```
+                                              value
+    Number of training samples used          8575.0
+    Number of validation samples used        2143.0
+    Init. log likelihood               -8874.438875
+    Final log likelihood                -7513.22967
+    Accuracy                                 59.26%
+    Likelihood ratio test                2722.41841
+    Rho square                             0.153385
+    Rho square bar                         0.152822
+    Akaike Information Criterion       15036.459339
+    Bayesian Information Criterion      15071.74237
+    Final gradient norm                    0.007164
+    ```
 
 3. **Correlation matrix**
-	```Python
-	print(mymodel.results.model_correlation_matrix())
-	```
-
-	Output:
-	```
-	             b_cost    b_time  asc_train   asc_car
-	b_cost     1.000000  0.209979   0.226737 -0.028335
-	b_time     0.209979  1.000000   0.731378  0.796144
-	asc_train  0.226737  0.731378   1.000000  0.664478
-	asc_car   -0.028335  0.796144   0.664478  1.000000
-	```
+    ```Python
+    print(mymodel.results.model_correlation_matrix())
+    ```
+
+    Output:
+    ```
+                 b_cost    b_time  asc_train   asc_car
+    b_cost     1.000000  0.209979   0.226737 -0.028335
+    b_time     0.209979  1.000000   0.731378  0.796144
+    asc_train  0.226737  0.731378   1.000000  0.664478
+    asc_car   -0.028335  0.796144   0.664478  1.000000
+    ```
 
 4. **Elasticities**
-	```Python
-	print(elasticities(mymodel, db, 0, "TRAIN_TT"))  # CHOICE:TRAIN (0) wrt TRAIN_TT
-	```
-
-	Output:
-	```
-	[-0.06813523 -0.01457346 -0.0555597  ... -0.03453162 -0.02809382 -0.02343637]
-	```
+    ```Python
+    print(elasticities(mymodel, db, 0, "TRAIN_TT"))  # CHOICE:TRAIN (0) wrt TRAIN_TT
+    ```
+
+    Output:
+    ```
+    [-0.06813523 -0.01457346 -0.0555597  ... -0.03453162 -0.02809382 -0.02343637]
+    ```
 
 5. **Choice probability predictions**
-	```Python
-	print(mymodel.predict(db, return_choices=False))
-	```
-
-	Output:
-	```
-	[[0.12319342 0.54372904 0.33307754]
-	[0.12267997 0.54499504 0.33232499]
-	[0.12354587 0.54162143 0.3348327 ]
-	...
-	[0.12801816 0.5201341  0.35184774]
-	[0.1271984  0.51681635 0.35598525]
-	[0.12881032 0.51856181 0.35262787]]
-	```
+    ```Python
+    print(mymodel.predict(db, return_choices=False))
+    ```
+
+    Output:
+    ```
+    [[0.12319342 0.54372904 0.33307754]
+    [0.12267997 0.54499504 0.33232499]
+    [0.12354587 0.54162143 0.3348327 ]
+    ...
+    [0.12801816 0.5201341  0.35184774]
+    [0.1271984  0.51681635 0.35598525]
+    [0.12881032 0.51856181 0.35262787]]
+    ```
 
 ---
 
 # Development
 
-(Optional) To develop PyCMTensor development package in a local environment, e.g. to modify, add features etc., you need to set up a virtual (Conda) environment and install the project requirements. Follow the instructions to install Conda (miniconda), then start a new virtual environment with the provided ``environment_<your OS>.yml`` file.
+To develop PyCMTensor development package in a local environment, e.g. to modify, add 
+features etc., you need to set up a virtual (Conda) environment and install the project 
+requirements. Follow the instructions to install Conda (miniconda), then start a new 
+virtual environment with the provided ``environment/environment_<your OS>.yml`` file.
 
 1. Download the git project repository into a local directory
-	```console
-	git clone git://github.com/mwong009/pycmtensor
-	cd pycmtensor
-	```
+    ```console
+    git clone git://github.com/mwong009/pycmtensor
+    cd pycmtensor
+    ```
 
 ## Installing the virtual environment
 
 **Windows**
 
 ```
-conda env create -f environment_windows.yml
+conda env create -f environment/environment_windows.yml
 ```
 
 **Linux**
 
 ```
-conda env create -f environment_linux.yml
+conda env create -f environment/environment_linux.yml
 ```
 
 **Mac OSX**
 
 ```
-conda env create -f environment_macos.yml
+conda env create -f environment/environment_macos.yml
 ```
 
 Next, activate the virtual environment and install ``poetry`` dependency manager via ``pip``
 
 ```
 conda activate pycmtensor-dev
 pip install poetry
 ```
 
 ## Install the project and development dependencies
 
 ```
 poetry install -E dev
 ```
+
+## Citation
+
+Cite this software as:
+
+    @software{melvin_wong_2022_7249280,
+      author       = {Melvin Wong},
+      title        = {mwong009/pycmtensor: v1.3.2},
+      year         = 2022,
+      version      = {v1.3.2},
+      doi          = {10.5281/zenodo.7249280},
+      url          = {https://doi.org/10.5281/zenodo.7249280}
+    }
```

### Comparing `pycmtensor-1.3.1/pycmtensor/config.py` & `pycmtensor-1.3.2/pycmtensor/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import subprocess
 import sys
 
 import numpy as np
 from watermark import watermark
 
-from .logger import log
+from .logger import info, warning
 from .scheduler import *
 
 __all__ = ["Config"]
 
 
 def about():
     return watermark(
@@ -112,19 +112,19 @@
             "patience": 4000,
             "patience_increase": 2,
             "validation_threshold": 1.005,
             "base_learning_rate": 0.01,
             "max_learning_rate": None,
             "batch_size": 250,
             "max_steps": 1000,
-            "clr_cycle_steps": 16,
-            "clr_gamma": None,
             "batch_shuffle": False,
+            "lr_scheduler": ConstantLR(),
+            "clr_gamma": None,
+            "clr_cycle_steps": 16,
         }
-        self.hyperparameters["lr_scheduler"] = ConstantLR(self["base_learning_rate"])
         self.aesara_rc = init_aesara_rc()
         init_environment_variables()
 
     def __print__(self):
         rval = f"\nhyperparameters\n---------------\n"
         for key, val in self.hyperparameters.items():
             rval += f"{key:<24}: {val}\n"
@@ -139,18 +139,23 @@
             self.hyperparameters[name] = val
         else:
             raise NameError(f"hyperparameter {name} is not a valid option")
 
     def __call__(self):
         return self.hyperparameters
 
-    def set_hyperparameter(self, key: str, value):
-        """Helper command to set hyperparameters to ``key: value``"""
-        self.hyperparameters[key] = value
-        log(10, f"set {key}={value}")
+    def set_hyperparameter(self, **kwargs):
+        """function to set hyperparameters"""
+        for key, value in kwargs.items():
+            if key not in self.hyperparameters:
+                warning(f"{key} not a valid training hyperparameter, skipping.")
+            else:
+                self.hyperparameters[key] = value
+                info(f"Hyperparameter set {key}={value}")
+        self.check_values()
 
     def set_lr_scheduler(self, scheduler):
         """Sets the config option ``lr_scheduler`` and ``base_learning rate``"""
         if not isinstance(scheduler, Scheduler):
             raise TypeError(
                 f"{type(scheduler)} is not a {Scheduler} instance, perhaps missing arguments?"
             )
```

### Comparing `pycmtensor-1.3.1/pycmtensor/data.py` & `pycmtensor-1.3.2/pycmtensor/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,14 @@
 
         Args:
             df (pandas.DataFrame): the input Pandas dataframe
             choice (str): column string name of the choice dependent variable
             **kwargs: Keyword arguments, accepted arguments are `drop:pd.Series`,
                 `autoscale:bool`, `autoscale_except:list[str]`, `split:float`
 
-        Attributes:
-            x (list[TensorVariable]): list of tensors corresponding to input features
-            y (list[TensorVariable]): list of the dependent choice variable tensor
-            all (list[TensorVariable]): combined list of x and y variables
-
         Note:
             The following is an example initialization of the swissmetro dataset::
 
                 swissmetro = pd.read_csv(\"../data/swissmetro.dat\", sep=\"\\t\")
                 db = pycmtensor.Data(
                     df=swissmetro,
                     choice=\"CHOICE\",
@@ -85,14 +80,30 @@
     def y(self):
         return self.tensor.y
 
     @property
     def all(self):
         return self.tensor.all
 
+    @property
+    def n_train_samples(self):
+        return len(self.pandas.train_dataset[0])
+
+    @property
+    def n_valid_samples(self):
+        return len(self.pandas.valid_dataset[0])
+
+    @property
+    def train_data(self):
+        return self.pandas.inputs(self.all, split_type="train")
+
+    @property
+    def valid_data(self):
+        return self.pandas.inputs(self.all, split_type="valid")
+
     def __getitem__(self, item: Union[str, list]) -> TensorVariable:
         if isinstance(item, list):
             return [self.tensor[x.name] for x in self.all if x.name in item]
         if item in [x.name for x in self.all]:
             return self.tensor[item]
         else:
             raise ValueError(f"{item} not a valid Variable name")
@@ -106,27 +117,27 @@
         self.split_frac = split_frac
         self.pandas.split_pandas(self.seed, split_frac)
 
     def get_nrows(self) -> int:
         """Returns the lenth of the DataFrame object"""
         return len(self.pandas())
 
-    def get_train_data(self, tensors, index=None, batch_size=None, shift=None, k=0):
+    def get_train_data(self, tensors, index=None, batch_size=None, shift=None):
         """Alias to get train data slice from `self.pandas.inputs()`
 
         See :meth:`PandasDataFrame.inputs()` for details
         """
-        return self.pandas.inputs(tensors, index, batch_size, shift, "train", k)
+        return self.pandas.inputs(tensors, index, batch_size, shift, "train")
 
-    def get_valid_data(self, tensors, index=None, batch_size=None, shift=None, k=0):
+    def get_valid_data(self, tensors, index=None, batch_size=None, shift=None):
         """Alias to get valid data slice from `self.pandas.inputs()`
 
         See :meth:`PandasDataFrame.inputs()` for details
         """
-        return self.pandas.inputs(tensors, index, batch_size, shift, "valid", k)
+        return self.pandas.inputs(tensors, index, batch_size, shift, "valid")
 
     def scale_data(self, **kwargs):
         """Scales data values by data/scale from `key=scale` keyword argument
 
         Args:
             **kwargs: {key: scale} keyword arguments
         """
```

### Comparing `pycmtensor-1.3.1/pycmtensor/expressions.py` & `pycmtensor-1.3.2/pycmtensor/expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from aesara import pprint
 from aesara.tensor.random.utils import RandomStream
 from aesara.tensor.sharedvar import TensorSharedVariable
 from aesara.tensor.var import TensorVariable
 
 from .logger import debug
 
+__all__ = ["FLOATX", "Param", "Beta", "Sigma", "Bias", "Weight"]
 FLOATX = aesara.config.floatX
 
 
 class ExpressionParser:
     """Base class for the ExpressionParser object"""
 
     def __init__(self):
```

### Comparing `pycmtensor-1.3.1/pycmtensor/functions.py` & `pycmtensor-1.3.2/pycmtensor/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,28 @@
 from aesara.tensor.sharedvar import TensorSharedVariable
 from aesara.tensor.var import TensorVariable
 
 from pycmtensor.expressions import Beta, Param
 
 from .logger import error, log
 
+__all__ = [
+    "exp_mov_average",
+    "logit",
+    "loglikelihood",
+    "rmse",
+    "mae",
+    "kl_divergence",
+    "kl_multivar_norm",
+    "errors",
+    "hessians",
+    "bhhh",
+    "gnorm",
+]
+
 
 def exp_mov_average(
     batch_avg: TensorVariable, moving_avg: TensorVariable, alpha: float = 0.1
 ):
     """Calculates the exponential moving average (EMA) of a new minibatch
 
     Args:
```

### Comparing `pycmtensor-1.3.1/pycmtensor/logger.py` & `pycmtensor-1.3.2/pycmtensor/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,17 +49,17 @@
     logger.addHandler(_get_console_handler())
     logger.setLevel(level)
     logger.propagate = False
     return logger
 
 
 default_formatter = logging.Formatter(
-    "[{asctime:s}] {levelname:s}: {message:s}",
+    "{asctime:s} [{levelname:s}] {message:s}",
     style="{",
-    datefmt="%Y-%m-%d %H:%M:%S",
+    datefmt="%H:%M:%S",
 )
 
 main_logger = get_default_logger("pycmtensor", VERBOSITY_DEFAULT)
 log = main_logger.log
 debug = main_logger.debug
 info = main_logger.info
 warning = main_logger.warning
```

### Comparing `pycmtensor-1.3.1/pycmtensor/models/layers.py` & `pycmtensor-1.3.2/pycmtensor/models/layers.py`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.3.1/pycmtensor/optimizers.py` & `pycmtensor-1.3.2/pycmtensor/optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 import aesara
 import aesara.tensor as aet
 from aesara import shared
 from aesara.tensor.sharedvar import TensorSharedVariable
 
 from .data import FLOATX
 
+__all__ = [
+    "Adam",
+    "Nadam",
+    "Adamax",
+    "Adadelta",
+    "RMSProp",
+    "Momentum",
+    "NAG",
+    "Adagrad",
+    "SGD",
+]
+
 
 class Optimizer:
     def __init__(self, name, epsilon=1e-8, **kwargs):
         """Base optimizer class
 
         Args:
             name (str): name of the optimizer
```

### Comparing `pycmtensor-1.3.1/pycmtensor/pycmtensor.py` & `pycmtensor-1.3.2/pycmtensor/pycmtensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 # pycmtensor.py
 """PyCMTensor main module"""
 from collections import OrderedDict
 from time import perf_counter
 from typing import Union
 
+import aesara.tensor as aet
 import dill as pickle
 import numpy as np
 from aesara import function
 from aesara.tensor.var import TensorVariable
 
 from pycmtensor import config, rng
 
 from .expressions import Beta, ExpressionParser, Weight
 from .functions import bhhh, errors, gnorm, hessians
 from .logger import debug, info, warning
+from .optimizers import Adam, Optimizer
 from .results import Results
 from .utils import time_format
 
 
 class PyCMTensorModel:
-    def __init__(self, db):
+    def __init__(self, db, **kwargs):
         """Base model class object"""
         self.name = "PyCMTensorModel"
         self.config = config
         self.params = []  # keep track of all the params
         self.betas = []  # keep track of the Betas
         self.weights = []  # keep track of the Weights
         self.updates = []  # keep track of the updates
         self.inputs = db.all
+        self.learning_rate = aet.scalar("learning_rate")
+        self.optimizer = Adam
         self.results = Results()
 
+        for key, value in kwargs.items():
+            if key == "optimizer" or key == "opt":
+                if not isinstance(value, Optimizer):
+                    raise TypeError(f"invalid optimizer {value}")
+                self.optimizer = value
+
         debug(f"Building model...")
 
     def add_params(self, params: Union[dict, list]):
         """Method to load locally defined variables
 
         Args:
             params (Union[dict, list]): a dict or list of ``TensorSharedVariable``
@@ -67,43 +77,44 @@
             seen.add(p.name)
 
             if isinstance(p, (Beta)):
                 self.betas.append(p)
             else:
                 self.weights.append(p)
 
-        self.n_params = self.get_n_params()
-
     def add_regularizers(self, l_reg: TensorVariable):
         """Adds regularizer to model cost function
 
         Args:
             l_reg (TensorVariable): symbolic variable defining the regularizer term
         """
         if not hasattr(self, "cost"):
             raise ValueError("No valid cost function defined.")
 
         self.cost += l_reg
 
-    def get_n_params(self) -> int:
+    @property
+    def n_params(self):
         """Get the total number of parameters"""
-        return self.get_n_betas() + sum(self.get_n_weights())
+        return self.n_betas + sum(self.n_weights)
 
-    def get_n_betas(self) -> int:
+    @property
+    def n_betas(self):
         """Get the count of Beta parameters"""
         return len(self.betas)
 
+    @property
+    def n_weights(self):
+        """Get the total number of elements of each weight matrix"""
+        return [w.size for w in self.get_weights()]
+
     def get_betas(self) -> dict:
         """Returns the Beta (key, value) pairs as a dict"""
         return {beta.name: beta.get_value() for beta in self.betas}
 
-    def get_n_weights(self) -> list[int]:
-        """Get the total number of elements of each weight matrix"""
-        return [w.size for w in self.get_weights()]
-
     def get_weights(self) -> list[np.ndarray]:
         """Returns the Weights as a list of matrices"""
         return [w.get_value() for w in self.weights]
 
     def reset_values(self):
         """Resets param values to their initial values"""
         for p in self.params:
@@ -171,114 +182,114 @@
         """
         self.gradient_norm = function(
             name="Gradient norm",
             inputs=self.inputs,
             outputs=gnorm(self.cost, self.betas),
         )
 
-    def predict(self, db, return_choices=True, split_type="valid"):
-        """Returns the predicted choice probabilites"""
-        predict_data = db.pandas.inputs(self.inputs, split_type=split_type)
+    def predict(self, db, return_choices: bool = True):
+        """Returns the predicted choice or choice probabilites
+
+        Args:
+            db (pycmtensor.Data): database for prediction
+            return_choices (bool): if `True` then returns discrete choices instead of
+                probabilities
+
+        Returns:
+            numpy.ndarray: the output vector
+        """
         if not return_choices:
-            return self.choice_probabilities(*predict_data)
+            return self.choice_probabilities(*db.valid_data)
         else:
-            return self.choice_predictions(*predict_data)
+            return self.choice_predictions(*db.valid_data)
 
-    def train(self, db, steps=np.inf, k=0):
-        """Function to train the model"""
-        self.config.check_values()  # assert config.hyperparameters
+    def train(self, db, **kwargs):
+        """Function to train the model
+
+        Args:
+            db (pycmtensor.Data): database used to train the model
+            **kwargs: keyword arguments for adjusting training configuration.
+                Possible values are `max_steps:int`, `patience:int`,
+                `lr_scheduler:scheduler.Scheduler`, `batch_size:int`. For more
+                information and other possible options, see
+                :py:data:`hyperparameters <pycmtensor.config.Config.hyperparameters>`
+        """
+        self.config.set_hyperparameter(**kwargs)
 
         # [train-start]
         lr_scheduler = self.config["lr_scheduler"]
         batch_size = self.config["batch_size"]
-        max_steps = min(self.config["max_steps"], steps)
+        max_steps = self.config["max_steps"]
         patience = self.config["patience"]
         patience_increase = self.config["patience_increase"]
         validation_threshold = self.config["validation_threshold"]
 
-        if db.split_frac is not None:
-            n_train_samples = len(db.pandas.train_dataset[k])
-            n_valid_samples = len(db.pandas.valid_dataset[k])
-        else:
-            n_train_samples = db.get_nrows()
-            n_valid_samples = db.get_nrows()
-        n_train_batches = n_train_samples // batch_size
-        validation_frequency = n_train_batches
-        max_iterations = max_steps * n_train_batches
-        debug(
-            f"batch_size={batch_size}, max_steps={max_steps}, n_samples={n_train_samples}"
-        )
+        db.n_train_batches = db.n_train_samples // batch_size
+        validation_frequency = db.n_train_batches
+        max_iterations = max_steps * db.n_train_batches
 
         # initalize results array
         self.results.performance_graph = OrderedDict()
 
-        # set training and validation datasets
-        train_data = db.pandas.inputs(self.inputs, split_type="train")
-        valid_data = db.pandas.inputs(self.inputs, split_type="valid")
-
         # compute the inital results of the model
-        self.results.init_loglikelihood = self.loglikelihood(*train_data)
+        self.results.init_loglikelihood = self.loglikelihood(*db.train_data)
         self.results.best_loglikelihood = self.results.init_loglikelihood
-        self.results.best_valid_error = self.prediction_error(*valid_data)
+        self.results.best_valid_error = self.prediction_error(*db.valid_data)
 
         # loop parameters
         done_looping = False
         step = 0
         iteration = 0
         shift = 0
 
         # set learning rate
         learning_rate = lr_scheduler(step)
 
         # main loop
         start_time = perf_counter()
-        info(f"Start (n={n_train_samples})")
+        info(f"Start (n={db.n_train_samples})")
 
         while (step < max_steps) and (not done_looping):
-
             # loop over batch
             learning_rate = lr_scheduler(step)
-            for index in range(n_train_batches):
+            for index in range(db.n_train_batches):
                 if patience <= iteration:
                     done_looping = True
-                    debug(f"Early stopping... (s={step})")
+                    debug(f"Early stopping... (step={step})")
                     break
 
                 # increment iteration
                 iteration += 1
 
                 # set index and shift slices
                 if self.config["batch_shuffle"]:
-                    index = rng.integers(0, n_train_batches)
+                    index = rng.integers(0, db.n_train_batches)
                     shift = rng.integers(0, batch_size)
 
                 # get data slice from dataset
-                batch_data = db.pandas.inputs(
-                    self.inputs, index, batch_size, shift, split_type="train"
-                )
+                batch_data = db.get_train_data(self.inputs, index, batch_size, shift)
 
                 # model update step
                 self.update_wrt_cost(*batch_data, learning_rate)
 
                 # model validate step
                 if iteration % validation_frequency != 0:
                     continue
 
-                train_ll = self.loglikelihood(*train_data)
-                valid_error = self.prediction_error(*valid_data)
+                train_ll = self.loglikelihood(*db.train_data)
+                valid_error = self.prediction_error(*db.valid_data)
                 self.results.performance_graph[step] = (
                     np.round(train_ll, 2),
                     np.round(valid_error, 4),
                 )
 
                 if valid_error >= self.results.best_valid_error:
                     continue
-                debug(
-                    f"Best validation error = {valid_error*100:.3f}%, (s={step}, i={iteration}, p={patience}, ll={train_ll:.2f})"
-                )
+                msg = f"Best validation error = {valid_error*100:.3f}%, (s={step}, i={iteration}, p={patience}, ll={train_ll:.2f})"
+                debug(msg)
 
                 self.results.best_step = step
                 self.results.best_iteration = iteration
                 self.results.best_loglikelihood = train_ll
                 self.results.best_valid_error = valid_error
 
                 self.results.betas = self.betas
@@ -294,29 +305,30 @@
 
             # increment step
             step += 1
 
         train_time = round(perf_counter() - start_time, 3)
         self.results.train_time = time_format(train_time)
         self.results.iterations_per_sec = round(iteration / train_time, 2)
-        msg = f"End (t={self.results.train_time}, VE={self.results.best_valid_error*100:.3f}%, LL={self.results.best_loglikelihood}, S={self.results.best_step})"
+        msg = f"End (t={self.results.train_time}, VE={self.results.best_valid_error*100:.2f}%, LL={self.results.best_loglikelihood:.2f}, Step={self.results.best_step})"
         info(msg)
 
         self.betas = self.results.betas
         self.weights = self.results.weights
-        self.results.n_train_samples = n_train_samples
-        self.results.n_valid_samples = n_valid_samples
+        self.results.n_train_samples = db.n_train_samples
+        self.results.n_valid_samples = db.n_valid_samples
         self.results.n_params = self.n_params
         self.results.seed = self.config["seed"]
         self.results.lr_history_graph = self.config["lr_scheduler"].history
 
         # statistical analysis step
-        self.results.gnorm = self.gradient_norm(*train_data)
-        self.results.hessian_matrix = self.H(*train_data)
-        self.results.bhhh_matrix = self.BHHH(*train_data)
+        self.results.gnorm = self.gradient_norm(*db.train_data)
+        self.results.hessian_matrix = self.H(*db.train_data)
+        self.results.bhhh_matrix = self.BHHH(*db.train_data)
 
     def export_to_pickle(self, f):
+        """to be removed in 1.4.0"""
         model = self
         pickle.dump(model, f)
 
     def __str__(self):
         return f"{self.name}"
```

### Comparing `pycmtensor-1.3.1/pycmtensor/results.py` & `pycmtensor-1.3.2/pycmtensor/results.py`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.3.1/pycmtensor/scheduler.py` & `pycmtensor-1.3.2/pycmtensor/scheduler.py`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.3.1/pycmtensor/statistics.py` & `pycmtensor-1.3.2/pycmtensor/statistics.py`

 * *Files identical despite different names*

### Comparing `pycmtensor-1.3.1/pyproject.toml` & `pycmtensor-1.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,97 @@
 [tool.poetry]
 name = "pycmtensor"
-version = "1.3.1"
-description = "Python Tensor based package for Deep neural net assisted Discrete Choice Modelling."
+version = "1.3.2"
+description = "Python Tensor based package for discrete choice modelling."
 authors = ["Melvin Wong <m.j.w.wong@tue.nl>"]
 license = "MIT License"
 readme = "README.md"
 
 homepage = ""
 repository = "https://github.com/mwong009/pycmtensor"
 documentation = ""
 
-keywords = ["pycmtensor"]
+keywords = []
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.dependencies]
 # Core
-python = "~3.9.7"
-aesara = "^2.7.4"
-numpy = "^1.19.0"
+python = "~3.11"
+aesara = "~2.9"
+numpy = "^1.21.2"
 scipy = "^1.7.1"
-pandas = "^1.3.5"
+pandas = "^1.4.1"
 pydot = "^1.4.2"
-dill = ">=0.3.4"
+dill = "^0.3.4"
 watermark = "^2.3.1"
 
 # Formatters
-black = { version = "^22.6.0", optional = true } 
-isort = { version = "^5.10.1", optional = true } 
+black = { version = "^23.3.0", optional = true } 
+isort = { version = "^5.9.1", optional = true } 
 
 #Linters
 pydocstyle = { version = "^6.1.1", optional = true } 
-rstcheck = { version = "^3.3.1", optional = true } 
+rstcheck = { version = "^6.1.2", optional = true } 
 
 # Documentation
-Sphinx = { version = "^4.4.0", optional = true } 
-sphinx-book-theme = { version = "^0.2.0", optional = true } 
-sphinx-design = {version = "^0.3.0", optional = true}
-sphinx-autoapi = { version = "^1.8.4", optional = true } 
-myst-parser = {version = "^0.18.0", optional = true}
+Sphinx = { version = "^5.3.0", optional = true } 
+sphinx-book-theme = { version = "^1.0.1", optional = true } 
+sphinx-design = {version = "^0.4.1", optional = true}
+sphinx-autoapi = { version = "^2.1.1", optional = true } 
+myst-nb = {version = "^0.17.2", optional = true}
 
 # Tooling
-pre-commit = { version = "^2.17.0", optional = true } 
-commitizen = { version = "^2.21.0", optional = true } 
+pre-commit = { version = "^3.3.3", optional = true } 
+commitizen = { version = "^3.3.0", optional = true } 
 
 [tool.poetry.dev-dependencies]
 # Testing
 pytest = "^7.0"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.1.0"
 
 [tool.poetry.extras]
 lint = ["black", "isort", "pydocstyle", "rstcheck"]
 commit = ["commitizen", "pre-commit"]
-docs = ["Sphinx", "sphinx-book-theme", "sphinx-autoapi", "myst-parser", "sphinx-design"]
-dev = ["black", "isort", "pydocstyle", "rstcheck", "Sphinx", "sphinx-book-theme", "sphinx-design", "sphinx-autoapi", "myst-parser", "commitizen", "pre-commit"]
+docs = ["Sphinx", "sphinx-book-theme", "sphinx-autoapi", "myst-nb", "sphinx-design"]
+dev = ["black", "isort", "pydocstyle", "rstcheck", "Sphinx", "sphinx-book-theme", "sphinx-design", "sphinx-autoapi", "myst-nb", "commitizen", "pre-commit"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 skip_glob = ".pytest_cache/*"
 
 [tool.black]
 line-length = 88
-target-version = ["py39"]
+target-version = ["py311"]
 quiet = false
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.3.1"
+version = "1.3.2"
 tag_format = "v$version"
 version_files = [
     "pyproject.toml:version",
     "pycmtensor/__init__.py",
     "docs/conf.py",
+    "docs/index.md",
     "README.md"
 ]
 
 [tool.pytest]
 markers = []
 # command: 
 # poetry run pytest .
```

### Comparing `pycmtensor-1.3.1/setup.py` & `pycmtensor-1.3.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,351 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pycmtensor
+Version: 1.3.2
+Summary: Python Tensor based package for discrete choice modelling.
+Home-page: https://github.com/mwong009/pycmtensor
+License: MIT
+Author: Melvin Wong
+Author-email: m.j.w.wong@tue.nl
+Requires-Python: >=3.11,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Provides-Extra: commit
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: lint
+Requires-Dist: Sphinx (>=5.3.0,<6.0.0) ; extra == "docs" or extra == "dev"
+Requires-Dist: aesara (>=2.9,<2.10)
+Requires-Dist: black (>=23.3.0,<24.0.0) ; extra == "lint" or extra == "dev"
+Requires-Dist: commitizen (>=3.3.0,<4.0.0) ; extra == "commit" or extra == "dev"
+Requires-Dist: dill (>=0.3.4,<0.4.0)
+Requires-Dist: isort (>=5.9.1,<6.0.0) ; extra == "lint" or extra == "dev"
+Requires-Dist: myst-nb (>=0.17.2,<0.18.0) ; extra == "docs" or extra == "dev"
+Requires-Dist: numpy (>=1.21.2,<2.0.0)
+Requires-Dist: pandas (>=1.4.1,<2.0.0)
+Requires-Dist: pre-commit (>=3.3.3,<4.0.0) ; extra == "commit" or extra == "dev"
+Requires-Dist: pydocstyle (>=6.1.1,<7.0.0) ; extra == "lint" or extra == "dev"
+Requires-Dist: pydot (>=1.4.2,<2.0.0)
+Requires-Dist: rstcheck (>=6.1.2,<7.0.0) ; extra == "lint" or extra == "dev"
+Requires-Dist: scipy (>=1.7.1,<2.0.0)
+Requires-Dist: sphinx-autoapi (>=2.1.1,<3.0.0) ; extra == "docs" or extra == "dev"
+Requires-Dist: sphinx-book-theme (>=1.0.1,<2.0.0) ; extra == "docs" or extra == "dev"
+Requires-Dist: sphinx-design (>=0.4.1,<0.5.0) ; extra == "docs" or extra == "dev"
+Requires-Dist: watermark (>=2.3.1,<3.0.0)
+Project-URL: Repository, https://github.com/mwong009/pycmtensor
+Description-Content-Type: text/markdown
 
-packages = \
-['pycmtensor', 'pycmtensor.models']
+# PyCMTensor
 
-package_data = \
-{'': ['*']}
+![Licence](https://img.shields.io/badge/Licence-MIT-blue)
+![](https://img.shields.io/pypi/pyversions/pycmtensor)
+[![PyPI version](https://badge.fury.io/py/pycmtensor.svg)](https://badge.fury.io/py/pycmtensor)
+[![Documentation Status](https://readthedocs.org/projects/pycmtensor/badge/?version=latest)](https://pycmtensor.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/gh/mwong009/pycmtensor/branch/master/graph/badge.svg?token=LFwgggDyjS)](https://codecov.io/gh/mwong009/pycmtensor)
+[![Downloads](https://static.pepy.tech/personalized-badge/pycmtensor?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pycmtensor)
 
-install_requires = \
-['aesara>=2.7.4,<3.0.0',
- 'dill>=0.3.4',
- 'numpy>=1.19.0,<2.0.0',
- 'pandas>=1.3.5,<2.0.0',
- 'pydot>=1.4.2,<2.0.0',
- 'scipy>=1.7.1,<2.0.0',
- 'watermark>=2.3.1,<3.0.0']
-
-extras_require = \
-{'commit': ['pre-commit>=2.17.0,<3.0.0', 'commitizen>=2.21.0,<3.0.0'],
- 'dev': ['black>=22.6.0,<23.0.0',
-         'isort>=5.10.1,<6.0.0',
-         'pydocstyle>=6.1.1,<7.0.0',
-         'rstcheck>=3.3.1,<4.0.0',
-         'Sphinx>=4.4.0,<5.0.0',
-         'sphinx-book-theme>=0.2.0,<0.3.0',
-         'sphinx-design>=0.3.0,<0.4.0',
-         'sphinx-autoapi>=1.8.4,<2.0.0',
-         'myst-parser>=0.18.0,<0.19.0',
-         'pre-commit>=2.17.0,<3.0.0',
-         'commitizen>=2.21.0,<3.0.0'],
- 'docs': ['Sphinx>=4.4.0,<5.0.0',
-          'sphinx-book-theme>=0.2.0,<0.3.0',
-          'sphinx-design>=0.3.0,<0.4.0',
-          'sphinx-autoapi>=1.8.4,<2.0.0',
-          'myst-parser>=0.18.0,<0.19.0'],
- 'lint': ['black>=22.6.0,<23.0.0',
-          'isort>=5.10.1,<6.0.0',
-          'pydocstyle>=6.1.1,<7.0.0',
-          'rstcheck>=3.3.1,<4.0.0']}
-
-setup_kwargs = {
-    'name': 'pycmtensor',
-    'version': '1.3.1',
-    'description': 'Python Tensor based package for Deep neural net assisted Discrete Choice Modelling.',
-    'long_description': '# PyCMTensor\n\n![Licence](https://img.shields.io/badge/Licence-MIT-blue)\n![](https://img.shields.io/pypi/pyversions/pycmtensor)\n[![PyPI version](https://badge.fury.io/py/pycmtensor.svg)](https://badge.fury.io/py/pycmtensor)\n[![Documentation Status](https://readthedocs.org/projects/pycmtensor/badge/?version=latest)](https://pycmtensor.readthedocs.io/en/latest/?badge=latest)\n[![codecov](https://codecov.io/gh/mwong009/pycmtensor/branch/master/graph/badge.svg?token=LFwgggDyjS)](https://codecov.io/gh/mwong009/pycmtensor)\n\n[![Tests](https://github.com/mwong009/pycmtensor/actions/workflows/tests.yml/badge.svg)](https://github.com/mwong009/pycmtensor/actions/workflows/tests.yml)\n[![CodeQL](https://github.com/mwong009/pycmtensor/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/mwong009/pycmtensor/actions/workflows/codeql-analysis.yml)\n[![Publish](https://github.com/mwong009/pycmtensor/actions/workflows/publish.yml/badge.svg)](https://github.com/mwong009/pycmtensor/actions/workflows/publish.yml)\n[![DOI](https://zenodo.org/badge/460802394.svg)](https://zenodo.org/badge/latestdoi/460802394)\n\nA tensor-based discrete choice modelling Python package. \n\n## Citation\n\nCite as:\n\n    @software{melvin_wong_2022_7249280,\n      author       = {Melvin Wong},\n      title        = {mwong009/pycmtensor: v1.3.1},\n      year         = 2022,\n      version      = {v1.3.1},\n      doi          = {10.5281/zenodo.7249280},\n      url          = {https://doi.org/10.5281/zenodo.7249280}\n    }\n\n## Table of contents\n\n\n- [PyCMTensor](#pycmtensor)\n\t- [Citation](#citation)\n\t- [Table of contents](#table-of-contents)\n\t- [About PyCMTensor](#about-pycmtensor)\n\t- [Features](#features)\n- [Quick start](#quick-start)\n\t- [Installation](#installation)\n- [Usage](#usage)\n\t- [Simple example: Swissmetro dataset](#simple-example-swissmetro-dataset)\n\t- [Results](#results)\n- [Development](#development)\n\t- [Installing the virtual environment](#installing-the-virtual-environment)\n\t- [Install the project and development dependencies](#install-the-project-and-development-dependencies)\n\n## About PyCMTensor\n\nPyCMTensor is a discrete choice modelling development tool on deep learning libraries, enabling development of complex models using deep neural networks.\nPyCMTensor is build on [Aesara](https://github.com/aesara-devs/aesara), a tensor library which uses features commonly found in deep learning packages such as ``Tensorflow`` and ``Keras``.\n``Aesara`` was chosen as the back end mathematical library because of its hackable, open-source nature.\nUsers of [Biogeme](https://biogeme.epfl.ch) would be familiar with the syntax of PyCMTensor.\n\nPyCMTensor improves on [Biogeme](https://biogeme.epfl.ch) in situations where much more complex models are necessary, for example, integrating neural networks into discrete choice models.\nPyCMTensor also include the ability to estimate models using 1st order stochastic gradient descent methods by default, such as Nesterov Accelerated Gradient (NAG), Adaptive momentum (ADAM), or RMSProp.\n\n## Features\n\n* Estimate complex choice models with neural networks using deep learning algorithms\n* Combines traditional econometric models (e.g. Multinomial Logit) with deep learning models (e.g. ResNets)\n* Shares similar programming syntax with ``Biogeme``, allowing easy transition between models\n* Uses tensor features found in the ``Aesara`` library\n\n---\n\n# Quick start\n\n## Installation\n\n1. Download and install [Miniconda](https://docs.conda.io/en/latest/miniconda.html)\n\n\tFull Anaconda works fine, but Miniconda is recommmended for a minimal installation. Ensure that Conda is using at least **Python 3.9**\n\n\tNext, install the required dependencies:\n\n\t**Windows**\n\n\t```\n\tconda install mkl-service conda-forge::cxx-compiler conda-forge::m2w64-toolchain\n\t```\n\t**Linux**\n\n\t```\n\tconda install mkl-service conda-forge::cxx-compiler\n\t```\n\n\t**Mac OSX**\n\n\t```\n\tconda install mkl-service Clang\n\t```\n\n2. Install the ``PyCMTensor`` package\n\n\tPyCMTensor is available on PyPi https://pypi.org/project/pycmtensor/. It can be installed with ``pip``\n\n\t```\n\tpip install -U pycmtensor==1.3.1\n\t```\n\n\tAlternatively, the latest development version is available via [Github](https://github.com/mwong009/pycmtensor). It can be installed via \n\n\t```\n\tpip install -U git+https://github.com/mwong009/pycmtensor.git\n\t```\n\nFor more information about installing, see [Installation](https://pycmtensor.readthedocs.io/en/latest/installation.html).\n\n# Usage\n\nPyCMTensor uses syntax very similar to ``Biogeme``. Users of ``Biogeme`` should be familiar with the syntax.\nMake sure you are using the correct Conda environment and/or the required packages are installed.\n\n## Simple example: Swissmetro dataset\n\n1. Start an interactive session (e.g. ``IPython`` or Jupyter Notebook) and import the ``PyCMTensor`` package:\n\t```python\n\timport pycmtensor as cmt\n\timport pandas as pd\n\t```\n\n\tSeveral submodules to include:\n\t```python\n\tfrom pycmtensor.expressions import Beta # Beta class for model parameters\n\tfrom pycmtensor.models import MNL  # MNL model\n\tfrom pycmtensor.statistics import elasticities  # For calculating elasticities\n\t```\n\n\tFor a full list of submodules and description, refer to [API Reference](https://pycmtensor.readthedocs.io/en/latest/autoapi/index.html).\n\tUsing the [swissmetro dataset](https://biogeme.epfl.ch/data.html), we define a simple MNL model. \n\n\n> :warning: Note: The following is a replication of the results from Biogeme using the ``Adam`` optimization method with constant learning rate.\n\n\n1. Import the dataset and perform some data cleaning\n\t```python\n\tswissmetro = pd.read_csv("swissmetro.dat", sep="\\t")\n\tswissmetro.drop(swissmetro[swissmetro["CHOICE"] == 0].index, inplace=True)\n\tswissmetro["CHOICE"] -= 1  # set the first choice index to 0\n\tdb = cmt.Data(df=swissmetro, choice="CHOICE")\n\tdb.autoscale_data(except_for=["ID", "ORIGIN", "DEST"])  # scales dataset\n\tdb.split_db(split_frac=0.8)  # split dataset into train/valid sets\n\t```\n\n2. Initialize the model parameters and specify the utility functions and availability conditions\n\t```python\n\tb_cost = Beta("b_cost", 0.0, None, None, 0)\n\tb_time = Beta("b_time", 0.0, None, None, 0)\n\tasc_train = Beta("asc_train", 0.0, None, None, 0)\n\tasc_car = Beta("asc_car", 0.0, None, None, 0)\n\tasc_sm = Beta("asc_sm", 0.0, None, None, 1)\n\n\tU_1 = b_cost * db["TRAIN_CO"] + b_time * db["TRAIN_TT"] + asc_train\n\tU_2 = b_cost * db["SM_CO"] + b_time * db["SM_TT"] + asc_sm\n\tU_3 = b_cost * db["CAR_CO"] + b_time * db["CAR_TT"] + asc_car\n\n\t# specify the utility function and the availability conditions\n\tU = [U_1, U_2, U_3]  # utility\n\tAV = [db["TRAIN_AV"], db["SM_AV"], db["CAR_AV"]]  # availability\n\t``` \n\n3. Define the Multinomial Logit model\n\t```python\n\tmymodel = MNL(db, locals(), U, AV, name="MNL")\n\t```\n\n4. Train the model and generate model statistics (Optionally, you can also set the training hyperparameters)\n\t```python\n\tmymodel.config.set_hyperparameter("max_steps", 200)  # set the max number of train steps\n\tmymodel.config.set_hyperparameter("batch_size", 128)  # set the training batch size\n\tmymodel.train(db)  # run the model training on the dataset `db`\n\t```\n\n## Results\nThe following model functions outputs the statistics, results of the model, and model training\n\n1. **Model estimates**\n\t```Python\n\tprint(mymodel.results.beta_statistics())\n\t```\n\n\tOutput:\n\t```\n\t              value   std err     t-test   p-value rob. std err rob. t-test rob. p-value\n\tasc_car   -0.665638  0.044783 -14.863615       0.0     0.176178    -3.77821     0.000158\n\tasc_sm          0.0         -          -         -            -           -            -\n\tasc_train -1.646826  0.048099 -34.238218       0.0     0.198978   -8.276443          0.0\n\tb_cost     0.024912   0.01943   1.282135  0.199795     0.016413    1.517851     0.129052\n\tb_time    -0.313186  0.049708  -6.300485       0.0     0.208239   -1.503979     0.132587\n\t```\n\n2. **Training results**\n\t```Python\n\tprint(mymodel.results.model_statistics())\n\t```\n\n\tOutput:\n\t```\n\t                                          value\n\tNumber of training samples used          8575.0\n\tNumber of validation samples used        2143.0\n\tInit. log likelihood               -8874.438875\n\tFinal log likelihood                -7513.22967\n\tAccuracy                                 59.26%\n\tLikelihood ratio test                2722.41841\n\tRho square                             0.153385\n\tRho square bar                         0.152822\n\tAkaike Information Criterion       15036.459339\n\tBayesian Information Criterion      15071.74237\n\tFinal gradient norm                    0.007164\n\t```\n\n3. **Correlation matrix**\n\t```Python\n\tprint(mymodel.results.model_correlation_matrix())\n\t```\n\n\tOutput:\n\t```\n\t             b_cost    b_time  asc_train   asc_car\n\tb_cost     1.000000  0.209979   0.226737 -0.028335\n\tb_time     0.209979  1.000000   0.731378  0.796144\n\tasc_train  0.226737  0.731378   1.000000  0.664478\n\tasc_car   -0.028335  0.796144   0.664478  1.000000\n\t```\n\n4. **Elasticities**\n\t```Python\n\tprint(elasticities(mymodel, db, 0, "TRAIN_TT"))  # CHOICE:TRAIN (0) wrt TRAIN_TT\n\t```\n\n\tOutput:\n\t```\n\t[-0.06813523 -0.01457346 -0.0555597  ... -0.03453162 -0.02809382 -0.02343637]\n\t```\n\n5. **Choice probability predictions**\n\t```Python\n\tprint(mymodel.predict(db, return_choices=False))\n\t```\n\n\tOutput:\n\t```\n\t[[0.12319342 0.54372904 0.33307754]\n\t[0.12267997 0.54499504 0.33232499]\n\t[0.12354587 0.54162143 0.3348327 ]\n\t...\n\t[0.12801816 0.5201341  0.35184774]\n\t[0.1271984  0.51681635 0.35598525]\n\t[0.12881032 0.51856181 0.35262787]]\n\t```\n\n---\n\n# Development\n\n(Optional) To develop PyCMTensor development package in a local environment, e.g. to modify, add features etc., you need to set up a virtual (Conda) environment and install the project requirements. Follow the instructions to install Conda (miniconda), then start a new virtual environment with the provided ``environment_<your OS>.yml`` file.\n\n1. Download the git project repository into a local directory\n\t```console\n\tgit clone git://github.com/mwong009/pycmtensor\n\tcd pycmtensor\n\t```\n\n## Installing the virtual environment\n\n**Windows**\n\n```\nconda env create -f environment_windows.yml\n```\n\n**Linux**\n\n```\nconda env create -f environment_linux.yml\n```\n\n**Mac OSX**\n\n```\nconda env create -f environment_macos.yml\n```\n\nNext, activate the virtual environment and install ``poetry`` dependency manager via ``pip``\n\n```\nconda activate pycmtensor-dev\npip install poetry\n```\n\n## Install the project and development dependencies\n\n```\npoetry install -E dev\n```\n',
-    'author': 'Melvin Wong',
-    'author_email': 'm.j.w.wong@tue.nl',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/mwong009/pycmtensor',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.9.7,<3.10.0',
-}
+[![Tests](https://github.com/mwong009/pycmtensor/actions/workflows/tests.yml/badge.svg)](https://github.com/mwong009/pycmtensor/actions/workflows/tests.yml)
+[![CodeQL](https://github.com/mwong009/pycmtensor/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/mwong009/pycmtensor/actions/workflows/codeql-analysis.yml)
+[![Publish](https://github.com/mwong009/pycmtensor/actions/workflows/publish.yml/badge.svg)](https://github.com/mwong009/pycmtensor/actions/workflows/publish.yml)
+[![DOI](https://zenodo.org/badge/460802394.svg)](https://zenodo.org/badge/latestdoi/460802394)
 
+PyCMTensor is a discrete choice modelling development tool on deep learning libraries, enabling development of complex models using deep neural networks.
+PyCMTensor is build with [Aesara](https://github.com/aesara-devs/aesara) package, similar to ``Tensorflow`` or ``Keras``.
+``Aesara`` is used the backend library because of its hackable, open-source nature.
+Users of [Biogeme](https://biogeme.epfl.ch) would be familiar with the syntax of PyCMTensor.
+PyCMTensor improves on [Biogeme](https://biogeme.epfl.ch) in situations where much more complex models are necessary, for example, integrating neural networks into discrete choice models.
+PyCMTensor also include the ability to estimate models using stochastic gradient descent methods by default, e.g. Nesterov Accelerated Gradient (NAG), Adaptive momentum (ADAM), or RMSProp.
+
+## Table of contents
+
+- [PyCMTensor](#pycmtensor)
+  - [Table of contents](#table-of-contents)
+  - [Features](#features)
+- [Quick start](#quick-start)
+  - [Installation](#installation)
+- [Usage](#usage)
+  - [Simple example: MNL model using the Swissmetro dataset](#simple-example-mnl-model-using-the-swissmetro-dataset)
+  - [Results](#results)
+- [Development](#development)
+  - [Installing the virtual environment](#installing-the-virtual-environment)
+  - [Install the project and development dependencies](#install-the-project-and-development-dependencies)
+  - [Citation](#citation)
+
+
+## Features
+
+* Estimate complex choice models using deep learning methods
+* Combines traditional econometric models (Multinomial Logit) with neural networks
+* Similar programming syntax as ``Biogeme``
+* Uses tensor features found in the ``Aesara`` library
+
+---
+
+# Quick start
+
+## Installation
+
+1. Download and install [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
+
+    Full Anaconda works fine, but Miniconda is recommmended for a minimal installation. Ensure that Conda is using at least **Python 3.9**
+
+2. Install conda dependencies:
+   
+    Dependencies are OS specific
+
+    **Windows**
+
+    ```
+    conda install mkl-service conda-forge::cxx-compiler conda-forge::m2w64-toolchain
+    ```
+    **Linux**
+
+    ```
+    conda install mkl-service conda-forge::cxx-compiler
+    ```
+
+    **Mac OSX**
+
+    ```
+    conda install mkl-service Clang
+    ```
+
+    **\*\*Optional\*\***
+
+    Alternatively, conda ``environment.yml`` files are provided in the ``environment/`` in respective operating systems, for example in Windows:
+
+    ```
+    conda env create -f environment/environment_windows.yml
+    conda activate pycmtensor-dev
+    ```
+
+
+3. Install the ``PyCMTensor`` package from PyPI via pip
+
+    ```
+    pip install -U pycmtensor==1.3.2
+    ```
+
+    Alternatively, the latest development version is available via [Github](https://github.com/mwong009/pycmtensor). It can be installed via 
+
+    ```
+    pip install -U git+https://github.com/mwong009/pycmtensor.git
+    ```
+
+For more information about installing, see [Installation](https://pycmtensor.readthedocs.io/en/latest/installation.html).
+
+# Usage
+
+PyCMTensor uses syntax very similar to ``Biogeme``. Users of ``Biogeme`` should be familiar with the syntax.
+Make sure you are using the correct Conda environment and/or the required packages are installed.
+
+## Simple example: MNL model using the Swissmetro dataset
+
+1. Start an interactive session (e.g. ``IPython`` or Jupyter Notebook) and import the ``PyCMTensor`` package and ``pandas``:
+    ```python
+    import pycmtensor as cmt
+    import pandas as pd
+    ```
+
+    Include the additional submodules:
+    ```python
+    from pycmtensor.expressions import Beta # Beta class for model parameters
+    from pycmtensor.models import MNL  # MNL model
+    from pycmtensor.statistics import elasticities  # For calculating elasticities
+    ```
+
+    For a full list of submodules and description, refer to [API Reference](https://pycmtensor.readthedocs.io/en/latest/autoapi/index.html).
+    Using the [swissmetro dataset](https://biogeme.epfl.ch/data.html), we define a simple MNL model. 
+
+
+> :warning: Note: The following is a replication of the results from Biogeme using the ``Adam`` optimization method with constant learning rate.
+
+
+1. Import the dataset and perform some data cleaning
+    ```python
+    swissmetro = pd.read_csv("swissmetro.dat", sep="\t")
+    db = cmt.Data(
+        df=swissmetro,
+        choice="CHOICE",
+        drop=[swissmetro["CHOICE"] == 0],
+        autoscale=True,
+        autoscale_except=["ID", "ORIGIN", "DEST", "CHOICE"],
+        split=0.8,
+    )
+    ```
+
+2. Initialize the model parameters and specify the utility functions and availability conditions
+    ```python
+    b_cost = Beta("b_cost", 0.0, None, None, 0)
+    b_time = Beta("b_time", 0.0, None, None, 0)
+    asc_train = Beta("asc_train", 0.0, None, None, 0)
+    asc_car = Beta("asc_car", 0.0, None, None, 0)
+    asc_sm = Beta("asc_sm", 0.0, None, None, 1)
+
+    U_1 = b_cost * db["TRAIN_CO"] + b_time * db["TRAIN_TT"] + asc_train
+    U_2 = b_cost * db["SM_CO"] + b_time * db["SM_TT"] + asc_sm
+    U_3 = b_cost * db["CAR_CO"] + b_time * db["CAR_TT"] + asc_car
+
+    # specify the utility function and the availability conditions
+    U = [U_1, U_2, U_3]  # utility
+    AV = [db["TRAIN_AV"], db["SM_AV"], db["CAR_AV"]]  # availability
+    ``` 
+
+3. Define the Multinomial Logit model
+    ```python
+    mymodel = MNL(db, locals(), U, AV)
+    ```
+
+4. Train the model and generate model statistics (Optionally, you can also set the training hyperparameters)
+    ```python
+    mymodel.train(db, max_steps=200, batch_size=128)  # run the model training on the dataset `db`
+    ```
+
+## Results
+The following model functions outputs the statistics, results of the model, and model training
+
+1. **Model estimates**
+    ```Python
+    print(mymodel.results.beta_statistics())
+    ```
+
+    Output:
+    ```
+                  value   std err     t-test   p-value rob. std err rob. t-test rob. p-value
+    asc_car   -0.665638  0.044783 -14.863615       0.0     0.176178    -3.77821     0.000158
+    asc_sm          0.0         -          -         -            -           -            -
+    asc_train -1.646826  0.048099 -34.238218       0.0     0.198978   -8.276443          0.0
+    b_cost     0.024912   0.01943   1.282135  0.199795     0.016413    1.517851     0.129052
+    b_time    -0.313186  0.049708  -6.300485       0.0     0.208239   -1.503979     0.132587
+    ```
+
+2. **Training results**
+    ```Python
+    print(mymodel.results.model_statistics())
+    ```
+
+    Output:
+    ```
+                                              value
+    Number of training samples used          8575.0
+    Number of validation samples used        2143.0
+    Init. log likelihood               -8874.438875
+    Final log likelihood                -7513.22967
+    Accuracy                                 59.26%
+    Likelihood ratio test                2722.41841
+    Rho square                             0.153385
+    Rho square bar                         0.152822
+    Akaike Information Criterion       15036.459339
+    Bayesian Information Criterion      15071.74237
+    Final gradient norm                    0.007164
+    ```
+
+3. **Correlation matrix**
+    ```Python
+    print(mymodel.results.model_correlation_matrix())
+    ```
+
+    Output:
+    ```
+                 b_cost    b_time  asc_train   asc_car
+    b_cost     1.000000  0.209979   0.226737 -0.028335
+    b_time     0.209979  1.000000   0.731378  0.796144
+    asc_train  0.226737  0.731378   1.000000  0.664478
+    asc_car   -0.028335  0.796144   0.664478  1.000000
+    ```
+
+4. **Elasticities**
+    ```Python
+    print(elasticities(mymodel, db, 0, "TRAIN_TT"))  # CHOICE:TRAIN (0) wrt TRAIN_TT
+    ```
+
+    Output:
+    ```
+    [-0.06813523 -0.01457346 -0.0555597  ... -0.03453162 -0.02809382 -0.02343637]
+    ```
+
+5. **Choice probability predictions**
+    ```Python
+    print(mymodel.predict(db, return_choices=False))
+    ```
+
+    Output:
+    ```
+    [[0.12319342 0.54372904 0.33307754]
+    [0.12267997 0.54499504 0.33232499]
+    [0.12354587 0.54162143 0.3348327 ]
+    ...
+    [0.12801816 0.5201341  0.35184774]
+    [0.1271984  0.51681635 0.35598525]
+    [0.12881032 0.51856181 0.35262787]]
+    ```
+
+---
+
+# Development
+
+To develop PyCMTensor development package in a local environment, e.g. to modify, add 
+features etc., you need to set up a virtual (Conda) environment and install the project 
+requirements. Follow the instructions to install Conda (miniconda), then start a new 
+virtual environment with the provided ``environment/environment_<your OS>.yml`` file.
+
+1. Download the git project repository into a local directory
+    ```console
+    git clone git://github.com/mwong009/pycmtensor
+    cd pycmtensor
+    ```
+
+## Installing the virtual environment
+
+**Windows**
+
+```
+conda env create -f environment/environment_windows.yml
+```
+
+**Linux**
+
+```
+conda env create -f environment/environment_linux.yml
+```
+
+**Mac OSX**
+
+```
+conda env create -f environment/environment_macos.yml
+```
+
+Next, activate the virtual environment and install ``poetry`` dependency manager via ``pip``
+
+```
+conda activate pycmtensor-dev
+pip install poetry
+```
+
+## Install the project and development dependencies
+
+```
+poetry install -E dev
+```
+
+## Citation
+
+Cite this software as:
+
+    @software{melvin_wong_2022_7249280,
+      author       = {Melvin Wong},
+      title        = {mwong009/pycmtensor: v1.3.2},
+      year         = 2022,
+      version      = {v1.3.2},
+      doi          = {10.5281/zenodo.7249280},
+      url          = {https://doi.org/10.5281/zenodo.7249280}
+    }
 
-setup(**setup_kwargs)
```

