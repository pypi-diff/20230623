# Comparing `tmp/mllibs-0.0.1-py2.py3-none-any.whl.zip` & `tmp/mllibs-0.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,32 @@
-Zip file size: 12631 bytes, number of entries: 11
--rw-r--r--  2.0 unx     2897 b- defN 22-Jul-13 22:44 mllibs/bl_regressor.py
--rw-r--r--  2.0 unx     4277 b- defN 22-Jul-13 22:25 mllibs/gmm.py
--rw-r--r--  2.0 unx     5761 b- defN 22-Feb-19 17:54 mllibs/gp_bclassifier.py
--rw-r--r--  2.0 unx     4627 b- defN 22-Feb-19 17:54 mllibs/gp_regressor.py
--rw-r--r--  2.0 unx     6350 b- defN 22-Feb-19 17:54 mllibs/gpr_bclassifier.py
--rw-r--r--  2.0 unx     5170 b- defN 22-Feb-19 17:54 mllibs/kriging_regressor.py
--rw-r--r--  2.0 unx     1091 b- defN 22-Jul-14 00:14 mllibs-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      556 b- defN 22-Jul-14 00:14 mllibs-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Jul-14 00:14 mllibs-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 22-Jul-14 00:14 mllibs-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      855 b- defN 22-Jul-14 00:14 mllibs-0.0.1.dist-info/RECORD
-11 files, 31695 bytes uncompressed, 11199 bytes compressed:  64.7%
+Zip file size: 90519 bytes, number of entries: 30
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-23 08:27 mllibs/__init__.py
+-rw-rw-rw-  2.0 fat     4129 b- defN 23-Jun-23 08:27 mllibs/interface.py
+-rw-rw-rw-  2.0 fat     6567 b- defN 23-Jun-23 08:27 mllibs/mdsplit.py
+-rw-rw-rw-  2.0 fat     9615 b- defN 23-Jun-23 08:27 mllibs/meda_scplot.py
+-rw-rw-rw-  2.0 fat    22334 b- defN 23-Jun-23 08:27 mllibs/meda_splot.py
+-rw-rw-rw-  2.0 fat    31758 b- defN 23-Jun-23 08:27 mllibs/membedding.py
+-rw-rw-rw-  2.0 fat    15320 b- defN 23-Jun-23 08:27 mllibs/mencoder.py
+-rw-rw-rw-  2.0 fat     5312 b- defN 23-Jun-23 08:27 mllibs/mloader.py
+-rw-rw-rw-  2.0 fat     9293 b- defN 23-Jun-23 08:27 mllibs/mnlp_encoder.py
+-rw-rw-rw-  2.0 fat    10978 b- defN 23-Jun-23 08:27 mllibs/moutliers.py
+-rw-rw-rw-  2.0 fat     5409 b- defN 23-Jun-23 08:27 mllibs/mpd_df.py
+-rw-rw-rw-  2.0 fat     7007 b- defN 23-Jun-23 08:27 mllibs/mseda.py
+-rw-rw-rw-  2.0 fat    28065 b- defN 23-Jun-23 08:27 mllibs/msllinear.py
+-rw-rw-rw-  2.0 fat    16859 b- defN 23-Jun-23 08:27 mllibs/mtextnorm.py
+-rw-rw-rw-  2.0 fat    19588 b- defN 23-Jun-23 08:27 mllibs/musldimred.py
+-rw-rw-rw-  2.0 fat    30696 b- defN 23-Jun-23 08:27 mllibs/nlpi.py
+-rw-rw-rw-  2.0 fat    16856 b- defN 23-Jun-23 08:27 mllibs/nlpm.py
+-rw-rw-rw-  2.0 fat    75880 b- defN 23-Jun-23 08:27 mllibs/corpus/wordlist.10000.txt
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-23 08:27 mlmodels/__init__.py
+-rw-rw-rw-  2.0 fat     2994 b- defN 23-Jun-23 08:27 mlmodels/bl_regressor.py
+-rw-rw-rw-  2.0 fat     4402 b- defN 23-Jun-23 08:27 mlmodels/gmm.py
+-rw-rw-rw-  2.0 fat     5761 b- defN 23-Jun-23 08:27 mlmodels/gp_bclassifier.py
+-rw-rw-rw-  2.0 fat     4627 b- defN 23-Jun-23 08:27 mlmodels/gp_regressor.py
+-rw-rw-rw-  2.0 fat     6350 b- defN 23-Jun-23 08:27 mlmodels/gpr_bclassifier.py
+-rw-rw-rw-  2.0 fat     5170 b- defN 23-Jun-23 08:27 mlmodels/kriging_regressor.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-23 08:56 mllibs-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7278 b- defN 23-Jun-23 08:56 mllibs-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-23 08:56 mllibs-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-23 08:56 mllibs-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2316 b- defN 23-Jun-23 08:56 mllibs-0.1.2.dist-info/RECORD
+30 files, 355781 bytes uncompressed, 86899 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,34 +1,91 @@
-Filename: mllibs/bl_regressor.py
+Filename: mllibs/__init__.py
 Comment: 
 
-Filename: mllibs/gmm.py
+Filename: mllibs/interface.py
 Comment: 
 
-Filename: mllibs/gp_bclassifier.py
+Filename: mllibs/mdsplit.py
 Comment: 
 
-Filename: mllibs/gp_regressor.py
+Filename: mllibs/meda_scplot.py
 Comment: 
 
-Filename: mllibs/gpr_bclassifier.py
+Filename: mllibs/meda_splot.py
 Comment: 
 
-Filename: mllibs/kriging_regressor.py
+Filename: mllibs/membedding.py
 Comment: 
 
-Filename: mllibs-0.0.1.dist-info/LICENSE
+Filename: mllibs/mencoder.py
 Comment: 
 
-Filename: mllibs-0.0.1.dist-info/METADATA
+Filename: mllibs/mloader.py
 Comment: 
 
-Filename: mllibs-0.0.1.dist-info/WHEEL
+Filename: mllibs/mnlp_encoder.py
 Comment: 
 
-Filename: mllibs-0.0.1.dist-info/top_level.txt
+Filename: mllibs/moutliers.py
 Comment: 
 
-Filename: mllibs-0.0.1.dist-info/RECORD
+Filename: mllibs/mpd_df.py
+Comment: 
+
+Filename: mllibs/mseda.py
+Comment: 
+
+Filename: mllibs/msllinear.py
+Comment: 
+
+Filename: mllibs/mtextnorm.py
+Comment: 
+
+Filename: mllibs/musldimred.py
+Comment: 
+
+Filename: mllibs/nlpi.py
+Comment: 
+
+Filename: mllibs/nlpm.py
+Comment: 
+
+Filename: mllibs/corpus/wordlist.10000.txt
+Comment: 
+
+Filename: mlmodels/__init__.py
+Comment: 
+
+Filename: mlmodels/bl_regressor.py
+Comment: 
+
+Filename: mlmodels/gmm.py
+Comment: 
+
+Filename: mlmodels/gp_bclassifier.py
+Comment: 
+
+Filename: mlmodels/gp_regressor.py
+Comment: 
+
+Filename: mlmodels/gpr_bclassifier.py
+Comment: 
+
+Filename: mlmodels/kriging_regressor.py
+Comment: 
+
+Filename: mllibs-0.1.2.dist-info/LICENSE
+Comment: 
+
+Filename: mllibs-0.1.2.dist-info/METADATA
+Comment: 
+
+Filename: mllibs-0.1.2.dist-info/WHEEL
+Comment: 
+
+Filename: mllibs-0.1.2.dist-info/top_level.txt
+Comment: 
+
+Filename: mllibs-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mllibs/bl_regressor.py` & `mlmodels/bl_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-
 ''' Bayesian Linear Regression Model '''
 # Two hyperparameter based linear regression model
+# utilised in @https://www.kaggle.com/shtrausslearning/bayesian-regression-house-price-prediction
 
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator,RegressorMixin
 from numpy.linalg import cholesky, det, lstsq, inv, eigvalsh, pinv
 from scipy.optimize import minimize
```

## Comparing `mllibs/gmm.py` & `mlmodels/gmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 ''' GAUSSIAN MIXTURE MODEL CLUSTERING '''
 # Expected minimisation approach GMM for clustering
+#https://github.com/krasserm/bayesian-machine-learning/blob/dev/
+#latent-variable-models/latent_variable_models_part_1.ipynb
 
 import numpy as np
 from scipy.stats import multivariate_normal as mvn
 
 class GMM():
     
     def __init__(self,C=3,max_iter=50,rtol=1e-3,n_restarts=10):
```

## Comparing `mllibs/gp_bclassifier.py` & `mlmodels/gp_bclassifier.py`

 * *Files identical despite different names*

## Comparing `mllibs/gp_regressor.py` & `mlmodels/gp_regressor.py`

 * *Files identical despite different names*

## Comparing `mllibs/gpr_bclassifier.py` & `mlmodels/gpr_bclassifier.py`

 * *Files identical despite different names*

## Comparing `mllibs/kriging_regressor.py` & `mlmodels/kriging_regressor.py`

 * *Files identical despite different names*

## Comparing `mllibs-0.0.1.dist-info/LICENSE` & `mllibs-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

