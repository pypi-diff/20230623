# Comparing `tmp/delicatessen-1.1.tar.gz` & `tmp/delicatessen-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delicatessen-1.1.tar", last modified: Mon Mar 20 17:05:05 2023, max compression
+gzip compressed data, was "delicatessen-1.2.tar", last modified: Fri Jun 23 12:43:20 2023, max compression
```

## Comparing `delicatessen-1.1.tar` & `delicatessen-1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 17:05:05.415763 delicatessen-1.1/
--rw-rw-rw-   0        0        0     1087 2021-10-29 16:28:15.000000 delicatessen-1.1/LICENSE
--rw-rw-rw-   0        0        0     5086 2023-03-20 17:05:05.415763 delicatessen-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3857 2023-01-02 18:15:22.000000 delicatessen-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 17:05:05.292304 delicatessen-1.1/delicatessen/
--rw-rw-rw-   0        0        0      547 2022-01-18 20:28:36.000000 delicatessen-1.1/delicatessen/__init__.py
--rw-rw-rw-   0        0        0     3169 2023-01-12 21:09:35.000000 delicatessen-1.1/delicatessen/data.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:05:05.412018 delicatessen-1.1/delicatessen/estimating_equations/
--rw-rw-rw-   0        0        0      770 2023-03-20 16:34:07.000000 delicatessen-1.1/delicatessen/estimating_equations/__init__.py
--rw-rw-rw-   0        0        0    15451 2023-03-20 16:43:13.000000 delicatessen-1.1/delicatessen/estimating_equations/basic.py
--rw-rw-rw-   0        0        0    29426 2023-03-20 16:52:26.000000 delicatessen-1.1/delicatessen/estimating_equations/causal.py
--rw-rw-rw-   0        0        0    20866 2023-03-20 16:49:59.000000 delicatessen-1.1/delicatessen/estimating_equations/dose_response.py
--rw-rw-rw-   0        0        0      824 2023-01-02 18:05:53.000000 delicatessen-1.1/delicatessen/estimating_equations/processing.py
--rw-rw-rw-   0        0        0    59168 2023-03-20 16:45:53.000000 delicatessen-1.1/delicatessen/estimating_equations/regression.py
--rw-rw-rw-   0        0        0    39223 2023-03-20 16:49:10.000000 delicatessen-1.1/delicatessen/estimating_equations/survival.py
--rw-rw-rw-   0        0        0    31087 2023-03-20 16:41:17.000000 delicatessen-1.1/delicatessen/mestimation.py
--rw-rw-rw-   0        0        0    26621 2023-03-20 17:02:57.000000 delicatessen-1.1/delicatessen/utilities.py
--rw-rw-rw-   0        0        0       21 2023-03-20 16:34:07.000000 delicatessen-1.1/delicatessen/version.py
-drwxrwxrwx   0        0        0        0 2023-03-20 17:05:05.370892 delicatessen-1.1/delicatessen.egg-info/
--rw-rw-rw-   0        0        0     5086 2023-03-20 17:05:04.000000 delicatessen-1.1/delicatessen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2023-03-20 17:05:05.000000 delicatessen-1.1/delicatessen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 17:05:04.000000 delicatessen-1.1/delicatessen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-03-20 17:05:04.000000 delicatessen-1.1/delicatessen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-20 17:05:04.000000 delicatessen-1.1/delicatessen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      112 2023-03-20 17:05:05.421232 delicatessen-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1670 2023-01-02 18:05:53.000000 delicatessen-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:43:20.278180 delicatessen-1.2/
+-rw-rw-rw-   0        0        0     1087 2021-10-29 16:28:15.000000 delicatessen-1.2/LICENSE
+-rw-rw-rw-   0        0        0     5086 2023-06-23 12:43:20.278180 delicatessen-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3857 2023-01-02 18:15:22.000000 delicatessen-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 12:43:20.226587 delicatessen-1.2/delicatessen/
+-rw-rw-rw-   0        0        0      547 2022-01-18 20:28:36.000000 delicatessen-1.2/delicatessen/__init__.py
+-rw-rw-rw-   0        0        0     3169 2023-01-12 21:09:35.000000 delicatessen-1.2/delicatessen/data.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:43:20.276312 delicatessen-1.2/delicatessen/estimating_equations/
+-rw-rw-rw-   0        0        0      770 2023-03-20 16:34:07.000000 delicatessen-1.2/delicatessen/estimating_equations/__init__.py
+-rw-rw-rw-   0        0        0    15451 2023-03-20 16:43:13.000000 delicatessen-1.2/delicatessen/estimating_equations/basic.py
+-rw-rw-rw-   0        0        0    29426 2023-03-20 16:52:26.000000 delicatessen-1.2/delicatessen/estimating_equations/causal.py
+-rw-rw-rw-   0        0        0    20866 2023-03-20 16:49:59.000000 delicatessen-1.2/delicatessen/estimating_equations/dose_response.py
+-rw-rw-rw-   0        0        0      824 2023-01-02 18:05:53.000000 delicatessen-1.2/delicatessen/estimating_equations/processing.py
+-rw-rw-rw-   0        0        0    61504 2023-06-23 12:37:08.000000 delicatessen-1.2/delicatessen/estimating_equations/regression.py
+-rw-rw-rw-   0        0        0    39220 2023-06-23 12:37:08.000000 delicatessen-1.2/delicatessen/estimating_equations/survival.py
+-rw-rw-rw-   0        0        0    31087 2023-03-20 16:41:17.000000 delicatessen-1.2/delicatessen/mestimation.py
+-rw-rw-rw-   0        0        0    27171 2023-06-23 12:37:08.000000 delicatessen-1.2/delicatessen/utilities.py
+-rw-rw-rw-   0        0        0       21 2023-06-23 12:37:08.000000 delicatessen-1.2/delicatessen/version.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:43:20.256378 delicatessen-1.2/delicatessen.egg-info/
+-rw-rw-rw-   0        0        0     5086 2023-06-23 12:43:20.000000 delicatessen-1.2/delicatessen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2023-06-23 12:43:20.000000 delicatessen-1.2/delicatessen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 12:43:20.000000 delicatessen-1.2/delicatessen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-23 12:43:20.000000 delicatessen-1.2/delicatessen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-23 12:43:20.000000 delicatessen-1.2/delicatessen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      112 2023-06-23 12:43:20.278180 delicatessen-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1670 2023-01-02 18:05:53.000000 delicatessen-1.2/setup.py
```

### Comparing `delicatessen-1.1/LICENSE` & `delicatessen-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `delicatessen-1.1/PKG-INFO` & `delicatessen-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delicatessen
-Version: 1.1
+Version: 1.2
 Summary: Generalized M-Estimation
 Home-page: https://github.com/pzivich/Deli
 Author: Paul Zivich
 Author-email: zivich.5@gmail.com
 License: MIT
 Description: ![delicatessen](docs/images/delicatessen_header.png)
```

### Comparing `delicatessen-1.1/README.md` & `delicatessen-1.2/README.md`

 * *Files identical despite different names*

### Comparing `delicatessen-1.1/delicatessen/__init__.py` & `delicatessen-1.2/delicatessen/__init__.py`

 * *Files identical despite different names*

### Comparing `delicatessen-1.1/delicatessen/data.py` & `delicatessen-1.2/delicatessen/data.py`

 * *Files identical despite different names*

### Comparing `delicatessen-1.1/delicatessen/estimating_equations/__init__.py` & `delicatessen-1.2/delicatessen/estimating_equations/__init__.py`

 * *Files identical despite different names*

### Comparing `delicatessen-1.1/delicatessen/estimating_equations/basic.py` & `delicatessen-1.2/delicatessen/estimating_equations/basic.py`

 * *Files identical despite different names*

### Comparing `delicatessen-1.1/delicatessen/estimating_equations/causal.py` & `delicatessen-1.2/delicatessen/estimating_equations/causal.py`

 * *Files identical despite different names*

### Comparing `delicatessen-1.1/delicatessen/estimating_equations/dose_response.py` & `delicatessen-1.2/delicatessen/estimating_equations/dose_response.py`

 * *Files identical despite different names*

### Comparing `delicatessen-1.1/delicatessen/estimating_equations/processing.py` & `delicatessen-1.2/delicatessen/estimating_equations/processing.py`

 * *Files identical despite different names*

### Comparing `delicatessen-1.1/delicatessen/estimating_equations/regression.py` & `delicatessen-1.2/delicatessen/estimating_equations/regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
                                     additive_design_matrix)
 from delicatessen.estimating_equations.processing import generate_weights
 
 #################################################################
 # Basic Regression Estimating Equations
 
 
-def ee_regression(theta, X, y, model, weights=None):
+def ee_regression(theta, X, y, model, weights=None, offset=None):
     r"""Estimating equation for regression. Options include: linear, logistic, and Poisson regression. The general
     estimating equation is
 
     .. math::
 
         \sum_{i=1}^n \left\{ Y_i - g(X_i^T \theta) \right\} X_i = 0
 
@@ -44,14 +44,16 @@
     y : ndarray, list, vector
         1-dimensional vector of n observed values.
     model : str
         Type of regression model to estimate. Options are ``'linear'`` (linear regression), ``'logistic'`` (logistic
         regression), and ``'poisson'`` (Poisson regression).
     weights : ndarray, list, vector, None, optional
         1-dimensional vector of n weights. Default is None, which assigns a weight of 1 to all observations.
+    offset : ndarray, list, vector, None, optional
+        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
 
     Returns
     -------
     array :
         Returns a b-by-n NumPy array evaluated for the input ``theta``
 
     Examples
@@ -114,32 +116,32 @@
 
     References
     ----------
     Boos DD, & Stefanski LA. (2013). M-estimation (estimating equations). In Essential Statistical Inference
     (pp. 297-337). Springer, New York, NY.
     """
     # Preparation of input shapes and object types
-    X, y, beta = _prep_inputs_(X=X, y=y, theta=theta, penalty=None)
+    X, y, beta, offset = _prep_inputs_(X=X, y=y, theta=theta, penalty=None, offset=offset)
 
     # Determining transformation function to use for the regression model
-    transform = _model_transform_(model=model)   # Looking up corresponding transformation
-    pred_y = transform(np.dot(X, beta))          # Generating predicted values via speedy matrix calculation
+    transform = _model_transform_(model=model)    # Looking up corresponding transformation
+    pred_y = transform(np.dot(X, beta) + offset)  # Generating predicted values via speedy matrix calculation
 
     # Allowing for a weighted linear model
     w = generate_weights(weights=weights, n_obs=X.shape[0])
 
     # Output b-by-n matrix
     return w*((y - pred_y) * X).T           # Return weighted regression score function
 
 
 #################################################################
 # Robust Regression Estimating Equations
 
 
-def ee_robust_regression(theta, X, y, model, k, loss='huber', weights=None, upper=None, lower=None):
+def ee_robust_regression(theta, X, y, model, k, loss='huber', weights=None, upper=None, lower=None, offset=None):
     r"""Estimating equations for (unscaled) robust regression. Robust linear regression is robust to outlying
     observations of the outcome variable. Currently, only linear regression is supported by
     ``ee_robust_regression``. The estimating equation is
 
     .. math::
 
         \sum_{i=1}^n f_k(Y_i - X_i^T \theta) X_i = 0
@@ -184,14 +186,16 @@
         1-dimensional vector of n weights. Default is None, which assigns a weight of 1 to all observations.
     lower : int, float, None, optional
         Lower parameter for the 'hampel' loss function. This parameter does not impact the other loss functions.
         Default is ``None``.
     upper : int, float, None, optional
         Upper parameter for the 'hampel' loss function. This parameter does not impact the other loss functions.
         Default is ``None``.
+    offset : ndarray, list, vector, None, optional
+        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
 
     Returns
     -------
     array :
         Returns a b-by-n NumPy array evaluated for the input ``theta``
 
     Examples
@@ -250,23 +254,23 @@
     42(6), 1887-1896.
 
     Huber PJ. (1964). Robust Estimation of a Location Parameter. *The Annals of Mathematical Statistics*, 35(1), 73–101.
 
     Huber PJ, Ronchetti EM. (2009) Robust Statistics 2nd Edition. Wiley. pgs 98-100
     """
     # Preparation of input shapes and object types
-    X, y, beta = _prep_inputs_(X=X, y=y, theta=theta, penalty=None)
+    X, y, beta, offset = _prep_inputs_(X=X, y=y, theta=theta, penalty=None, offset=offset)
 
     # Allowing for a weighted linear model
     w = generate_weights(weights=weights, n_obs=X.shape[0])
 
     # Determining transformation function to use for the regression model
     transform = _model_transform_(model=model,                # Looking up corresponding transformation
                                   assert_linear_model=True)   # ... and make sure it is a linear model
-    pred_y = transform(np.dot(X, beta))                       # Generating predicted values
+    pred_y = transform(np.dot(X, beta) + offset)              # Generating predicted values
 
     # Generating predictions and applying Huber function for robust
     residual = robust_loss_functions(residual=y - pred_y,     # Calculating robust residuals
                                      k=k,                     # ... hyperparameter for loss function
                                      loss=loss,               # ... chosen loss function
                                      a=lower,                 # ... upper limit (Hampel only)
                                      b=upper)                 # ... lower limit (Hampel only)
@@ -275,15 +279,15 @@
     return w*(residual * X).T    # Score function
 
 
 #################################################################
 # Penalized Regression Estimating Equations
 
 
-def ee_ridge_regression(theta, X, y, model, penalty, weights=None, center=0.):
+def ee_ridge_regression(theta, X, y, model, penalty, weights=None, center=0., offset=None):
     r"""Estimating equations for ridge regression. Ridge regression applies an L2-regularization through a squared
     magnitude penalty. The estimating equation for Ridge linear regression is
 
     .. math::
 
         \sum_{i=1}^n \left\{(Y_i - X_i^T \theta) X_i - \lambda \theta \right\} = 0
 
@@ -317,14 +321,16 @@
     weights : ndarray, list, vector, None, optional
         1-dimensional vector of n weights. Default is ``None``, which assigns a weight of 1 to all observations.
     center : int, float, ndarray, list, vector, optional
         Center or reference value to penalized estimated coefficients towards. Default is ``0``, which penalized
         coefficients towards the null. Other center values can be specified for all coefficients (by providing an
         integer or float) or covariate-specific centering values (by providing a vector of values of the same length as
         X).
+    offset : ndarray, list, vector, None, optional
+        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
 
     Returns
     -------
     array :
         Returns a b-by-n NumPy array evaluated for the input ``theta``
 
     Examples
@@ -400,19 +406,22 @@
     Fu WJ. (1998). Penalized regressions: the Bridge versus the LASSO. *Journal of Computational and Graphical
     Statistics*, 7(3), 397-416.
 
     Fu WJ. (2003). Penalized estimating equations. *Biometrics*, 59(1), 126-132.
     """
     # Calling internal bridge penalized regression for implementation
     return ee_bridge_regression(theta=theta,
-                                X=X, y=y, model=model, weights=weights,
-                                penalty=penalty, gamma=2, center=center)
+                                X=X, y=y,
+                                model=model,
+                                weights=weights,
+                                penalty=penalty, gamma=2, center=center,
+                                offset=offset)
 
 
-def ee_lasso_regression(theta, X, y, model, penalty, epsilon=3.e-3, weights=None, center=0.):
+def ee_lasso_regression(theta, X, y, model, penalty, epsilon=3.e-3, weights=None, center=0., offset=None):
     r"""Estimating equation for an approximate LASSO (least absolute shrinkage and selection operator) regressor. LASSO
     regression applies an L1-regularization through a magnitude penalty.
 
     Note
     ----
     As the derivative of the estimating equation for LASSO is not defined, the bread (and sandwich) cannot be used to
     estimate the variance in all settings.
@@ -463,14 +472,16 @@
     weights : ndarray, list, vector, None, optional
         1-dimensional vector of n weights. Default is ``None``, which assigns a weight of 1 to all observations.
     center : int, float, ndarray, list, vector, optional
         Center or reference value to penalized estimated coefficients towards. Default is ``0``, which penalized
         coefficients towards the null. Other center values can be specified for all coefficients (by providing an
         integer or float) or covariate-specific centering values (by providing a vector of values of the same length as
         X).
+    offset : ndarray, list, vector, None, optional
+        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
 
     Returns
     -------
     array :
         Returns a b-by-n NumPy array evaluated for the input ``theta``
 
     Examples
@@ -547,19 +558,22 @@
     Fu WJ. (2003). Penalized estimating equations. *Biometrics*, 59(1), 126-132.
     """
     if epsilon < 0:
         raise ValueError("epsilon must be greater than zero for the approximate LASSO")
 
     # Calling internal bridge penalized regression for implementation
     ee_bridge_regression(theta=theta,
-                         X=X, y=y, model=model, weights=weights,
-                         penalty=penalty, gamma=1+epsilon, center=center)
+                         X=X, y=y,
+                         model=model,
+                         weights=weights,
+                         penalty=penalty, gamma=1+epsilon, center=center,
+                         offset=offset)
 
 
-def ee_elasticnet_regression(theta, X, y, model, penalty, ratio, epsilon=3.e-3, weights=None, center=0.):
+def ee_elasticnet_regression(theta, X, y, model, penalty, ratio, epsilon=3.e-3, weights=None, center=0., offset=None):
     r"""Estimating equations for Elastic-Net regression. Elastic-Net applies both L1- and L2-regularization at a
     pre-specified ratio. Notice that the L1 penalty is based on an approximation. See ``ee_lasso_regression`` for
     further details on the approximation for the L1 penalty.
 
     Note
     ----
     As the derivative of the estimating equation for Elastic-Net is not defined, the bread (and sandwich) cannot be
@@ -609,14 +623,16 @@
     weights : ndarray, list, vector, None, optional
         1-dimensional vector of n weights. Default is ```None``, which assigns a weight of 1 to all observations.
     center : int, float, ndarray, list, vector, optional
         Center or reference value to penalized estimated coefficients towards. Default is ``0``, which penalized
         coefficients towards the null. Other center values can be specified for all coefficients (by providing an
         integer or float) or covariate-specific centering values (by providing a vector of values of the same length as
         X).
+    offset : ndarray, list, vector, None, optional
+        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
 
     Returns
     -------
     array :
         Returns a b-by-n NumPy array evaluated for the input theta and y
 
     Examples
@@ -689,19 +705,21 @@
     ----------
     Fu WJ. (1998). Penalized regressions: the Bridge versus the LASSO. *Journal of Computational and Graphical
     Statistics*, 7(3), 397-416.
 
     Fu WJ. (2003). Penalized estimating equations. *Biometrics*, 59(1), 126-132.
     """
     # Preparation of input shapes and object types
-    X, y, beta, penalty, center = _prep_inputs_(X=X, y=y, theta=theta, penalty=penalty, center=center)
+    X, y, beta, penalty, center, offset = _prep_inputs_(X=X, y=y, theta=theta,
+                                                        penalty=penalty, center=center,
+                                                        offset=offset)
 
     # Determining transformation function to use for the regression model
-    transform = _model_transform_(model=model)  # Looking up corresponding transformation
-    pred_y = transform(np.dot(X, beta))  # Generating predicted values
+    transform = _model_transform_(model=model)    # Looking up corresponding transformation
+    pred_y = transform(np.dot(X, beta) + offset)  # Generating predicted values
 
     # Allowing for a weighted penalized regression model
     w = generate_weights(weights=weights, n_obs=X.shape[0])
 
     # Creating penalty term for ridge regression (bridge with gamma=2 is the special case of ridge)
     if epsilon < 0:
         raise ValueError("epsilon must be greater than zero for the approximate LASSO")
@@ -712,15 +730,15 @@
     penalty_l2 = _bridge_penalty_(theta=theta, n_obs=X.shape[0], penalty=penalty, gamma=2, center=center)
     penalty_terms = ratio*penalty_l1 + (1-ratio)*penalty_l2
 
     # Output b-by-n matrix
     return w * (((y - pred_y) * X).T - penalty_terms[:, None])  # Score function with penalty term subtracted off
 
 
-def ee_bridge_regression(theta, X, y, model, penalty, gamma, weights=None, center=0.):
+def ee_bridge_regression(theta, X, y, model, penalty, gamma, weights=None, center=0., offset=None):
     r"""Estimating equation for bridge penalized regression. The bridge penalty is a generalization of penalized
     regression, that includes L1 and L2-regularization as special cases.
 
     Note
     ----
     While the bridge penalty is defined for :math:`\gamma > 0`, the provided estimating equation only supports
     :math:`\gamma \ge 1`. Additionally, the derivative of the estimating equation is not defined when
@@ -766,14 +784,16 @@
     weights : ndarray, list, vector, None, optional
         1-dimensional vector of n weights. Default is ``None``, which assigns a weight of 1 to all observations.
     center : int, float, ndarray, list, vector, optional
         Center or reference value to penalized estimated coefficients towards. Default is ``0``, which penalized
         coefficients towards the null. Other center values can be specified for all coefficients (by providing an
         integer or float) or covariate-specific centering values (by providing a vector of values of the same length as
         X).
+    offset : ndarray, list, vector, None, optional
+        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
 
     Returns
     -------
     array :
         Returns a b-by-n NumPy array evaluated for the input ``theta``
 
     Examples
@@ -848,19 +868,21 @@
     ----------
     Fu WJ. (1998). Penalized regressions: the Bridge versus the LASSO. *Journal of Computational and Graphical
     Statistics*, 7(3), 397-416.
 
     Fu WJ. (2003). Penalized estimating equations. *Biometrics*, 59(1), 126-132.
     """
     # Preparation of input shapes and object types
-    X, y, beta, penalty, center = _prep_inputs_(X=X, y=y, theta=theta, penalty=penalty, center=center)
+    X, y, beta, penalty, center, offset = _prep_inputs_(X=X, y=y, theta=theta,
+                                                        penalty=penalty, center=center,
+                                                        offset=offset)
 
     # Determining transformation function to use for the regression model
-    transform = _model_transform_(model=model)  # Looking up corresponding transformation
-    pred_y = transform(np.dot(X, beta))  # Generating predicted values
+    transform = _model_transform_(model=model)    # Looking up corresponding transformation
+    pred_y = transform(np.dot(X, beta) + offset)  # Generating predicted values
 
     # Allowing for a weighted penalized regression model
     w = generate_weights(weights=weights, n_obs=X.shape[0])
 
     # Creating penalty term for ridge regression (bridge with gamma=2 is the special case of ridge)
     penalty_terms = _bridge_penalty_(theta=theta, n_obs=X.shape[0], penalty=penalty, gamma=gamma, center=center)
 
@@ -868,15 +890,15 @@
     return w * (((y - pred_y) * X).T - penalty_terms[:, None])  # Score function with penalty term subtracted off
 
 
 #################################################################
 # Flexible Regression Estimating Equations
 
 
-def ee_additive_regression(theta, X, y, specifications, model, weights=None):
+def ee_additive_regression(theta, X, y, specifications, model, weights=None, offset=None):
     r"""Estimating equation for Generalized Additive Models (GAMs). GAMs are an extension of generalized linear models
     that allow for more flexible specifications of relationships of continuous variables. This flexibility is
     accomplished via splines. To further control the flexibility, the spline terms are penalized.
 
     Note
     ----
     The implemented GAM uses L2-penalization. This penalization only applies to the generated spline terms
@@ -934,14 +956,16 @@
         * penalty (float): penalty term (:math:`\lambda`) applied to each corresponding spline basis term. Default is 0,
             which applies no penalty to the spline basis terms.
     model : str
         Type of regression model to estimate. Options are ``'linear'`` (linear regression), ``'logistic'`` (logistic
         regression), and ``'poisson'`` (Poisson regression).
     weights : ndarray, list, vector, None, optional
         1-dimensional vector of n weights. Default is ``None``, which assigns a weight of 1 to all observations.
+    offset : ndarray, list, vector, None, optional
+        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
 
     Returns
     -------
     array :
         Returns a (b+k)-by-n NumPy array evaluated for the input ``theta``
 
     Examples
@@ -1079,21 +1103,22 @@
                                          specifications=specifications,     # ... with the provided specifications
                                          return_penalty=True)               # ... and return corresponding penalties
 
     # Apply spline-penalized regression
     return ee_bridge_regression(theta=theta, y=y, X=Xa,                     # Call bridge reg with additive design
                                 model=model, penalty=penalty,               # ... matrix and processed penalties
                                 gamma=2, weights=weights,                   # ... and set gamma=2 (Ridge reg)
-                                center=0.)                                  # ... with splines ALWAYS penalized to zero
+                                center=0.,                                  # ... with splines ALWAYS penalized to zero
+                                offset=offset)                              # ... and provided offset
 
 
 #################################################################
 # Utility functions for regression equations
 
-def _prep_inputs_(X, y, theta, penalty=None, center=None):
+def _prep_inputs_(X, y, theta, penalty=None, center=None, offset=None):
     """Internal use function to simplify variable transformations for regression. This function is used on the inputs
     to ensure they are the proper shapes
 
     Parameters
     ----------
     X : ndarray
         Dependent variables
@@ -1108,20 +1133,27 @@
     -------
     transformed parameters
     """
     X = np.asarray(X)                       # Convert to NumPy array
     y = np.asarray(y)[:, None]              # Convert to NumPy array and ensure correct shape for matrix algebra
     beta = np.asarray(theta)[:, None]       # Convert to NumPy array and ensure correct shape for matrix algebra
 
+    # Logic to determine the offset variable if requested
+    if offset is None:                           # When offset is None
+        offset = 0                               # ... modify by adding a zero (i.e., no mod)
+    else:                                        # Otherwise
+        offset = np.asarray(offset)[:, None]     # ... ensure that a NumPy array is passed forward
+
+    # What to return if penalty is or is not given
     if penalty is None:                     # Return the transformed objects
-        return X, y, beta
+        return X, y, beta, offset
     else:                                   # Convert penalty term then return all
         penalty = np.asarray(penalty)       # Convert to NumPy array
         center = np.asarray(center)         # Convert to NumPy array
-        return X, y, beta, penalty, center
+        return X, y, beta, penalty, center, offset
 
 
 def _model_transform_(model, assert_linear_model=False):
     """Internal use function to simplify the checking procedure for the model form to use. Takes the input string and
     returns the corresponding function for the variable transformation.
 
     Parameters
```

### Comparing `delicatessen-1.1/delicatessen/estimating_equations/survival.py` & `delicatessen-1.2/delicatessen/estimating_equations/survival.py`

 * *Files 0% similar despite different names*

```diff
@@ -592,21 +592,21 @@
     >>> data['delta'] = np.where(data['T'] < data['C'], 1, 0)
     >>> data['t'] = np.where(data['delta'] == 1, data['T'], data['C'])
     >>> d_obs = data[['X', 'W', 't', 'delta']].copy()
 
     Defining psi, or the stacked estimating equations
 
     >>> def psi(theta):
-    >>>         return ee_aft_weibull(theta=theta, X=d_obs[['C', 'X', 'Z']],
+    >>>         return ee_aft_weibull(theta=theta, X=d_obs[['X', 'W']],
     >>>                               t=d_obs['t'], delta=d_obs['delta'])
 
     Calling the M-estimator (note that `init` has 4 values now, since ``X.shape[1]`` is 2).
 
     >>> estr = MEstimator(stacked_equations=psi, init=[0., 0., 0., 0.])
-    >>> estr.estimate(solver='lm')
+    >>> estr.estimate(solver='hybr')
 
     Inspecting the parameter estimates, variance, and confidence intervals
 
     >>> estr.theta
     >>> estr.variance
     >>> estr.confidence_intervals()
```

### Comparing `delicatessen-1.1/delicatessen/mestimation.py` & `delicatessen-1.2/delicatessen/mestimation.py`

 * *Files identical despite different names*

### Comparing `delicatessen-1.1/delicatessen/utilities.py` & `delicatessen-1.2/delicatessen/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     else:
         raise ValueError("The loss function "+str(loss)+" is not available.")
 
     # Returning the updated values
     return xr
 
 
-def regression_predictions(X, theta, covariance, alpha=0.05):
+def regression_predictions(X, theta, covariance, offset=None, alpha=0.05):
     r"""Generate predicted values of the outcome given a design matrix, point estimates, and covariance matrix.
     This functionality computes :math:`\hat{Y}`, :math:`\hat{Var}\left(\hat{Y}\right)`, and corresponding Wald-type
     :math:`(1 - \alpha) \times` 100% confidence intervals from estimated coefficients and covariance of a regression
     model given a set of specific covariate values.
 
     This function is a helper function to compute the predictions from a regression model for a set of given :math:`X`
     values. Importantly, this method allows for the variance of :math:`\hat{Y}` to be estimated without having to expand
@@ -221,14 +221,16 @@
     X : ndarray, list, vector
         2-dimensional vector of values to generate predicted variances for. The number of columns must match the number
         of coefficients / parameters in ``theta``.
     theta : ndarray
         Estimated coefficients from ``delicatessen.MEstimator.theta``.
     covariance : ndarray
         Estimated covariance matrix from ``delicatessen.MEstimator.variance``.
+    offset : ndarray, None, optional
+        A 1-dimensional offset to be included in the model. Default is None, which applies no offset term.
     alpha : float, optional
         The :math:`\alpha` level for the corresponding confidence intervals. Default is 0.05, which calculate the
         95% confidence intervals. Notice that :math:`0<\alpha<1`.
 
     Returns
     -------
     array :
@@ -289,21 +291,27 @@
     ``delicatessen.utilities.inverse_logit``. For the Poisson model, predictions can easily be transformed using
     ``numpy.exp``.
     """
     # Check valid alpha value is being provided
     if not 0 < alpha < 1:
         raise ValueError("`alpha` must be 0 < a < 1")
 
+    # Process offset term
+    if offset is None:                                 # When offset is None
+        offset = 0                                     # ... modify by adding a zero (i.e., no mod)
+    else:                                              # Otherwise
+        offset = np.asarray(offset)[:, None]           # ... ensure that a NumPy array is passed forward
+
     # Setup inputs for matrix multiplications
     x = np.asarray(X)
     b = np.asarray(theta)
     c = np.asarray(covariance)
 
     # Predicted Y
-    yhat = np.dot(x, b)
+    yhat = np.dot(x, b) + offset
 
     # Predicted Y variance / standard error
     yhat_var = np.sum(np.dot(x, c) * x,
                       axis=1)
 
     # Confidence limit of predictions
     yhat_se = np.sqrt(yhat_var)                        # Taking square root to get SE
```

### Comparing `delicatessen-1.1/delicatessen.egg-info/PKG-INFO` & `delicatessen-1.2/delicatessen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delicatessen
-Version: 1.1
+Version: 1.2
 Summary: Generalized M-Estimation
 Home-page: https://github.com/pzivich/Deli
 Author: Paul Zivich
 Author-email: zivich.5@gmail.com
 License: MIT
 Description: ![delicatessen](docs/images/delicatessen_header.png)
```

### Comparing `delicatessen-1.1/delicatessen.egg-info/SOURCES.txt` & `delicatessen-1.2/delicatessen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delicatessen-1.1/setup.py` & `delicatessen-1.2/setup.py`

 * *Files identical despite different names*

