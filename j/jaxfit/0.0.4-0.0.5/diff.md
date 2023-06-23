# Comparing `tmp/jaxfit-0.0.4.tar.gz` & `tmp/jaxfit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxfit-0.0.4.tar", last modified: Mon Nov 14 22:56:35 2022, max compression
+gzip compressed data, was "jaxfit-0.0.5.tar", last modified: Fri Jun 23 12:27:30 2023, max compression
```

## Comparing `jaxfit-0.0.4.tar` & `jaxfit-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-11-14 22:56:35.635000 jaxfit-0.0.4/
--rw-rw-rw-   0        0        0     1539 2022-08-08 11:59:22.000000 jaxfit-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      332 2022-11-14 22:56:35.600000 jaxfit-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    10002 2022-08-26 13:49:12.000000 jaxfit-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2022-11-14 22:56:35.435000 jaxfit-0.0.4/jaxfit/
--rw-rw-rw-   0        0        0      173 2022-07-21 12:32:10.000000 jaxfit-0.0.4/jaxfit/__init__.py
--rw-rw-rw-   0        0        0     2577 2022-07-21 12:32:10.000000 jaxfit-0.0.4/jaxfit/_optimize.py
--rw-rw-rw-   0        0        0     5462 2022-11-14 22:40:00.000000 jaxfit-0.0.4/jaxfit/common_jax.py
--rw-rw-rw-   0        0        0    25338 2022-07-21 12:32:10.000000 jaxfit-0.0.4/jaxfit/common_scipy.py
--rw-rw-rw-   0        0        0    49564 2022-07-21 12:32:10.000000 jaxfit-0.0.4/jaxfit/least_squares.py
--rw-rw-rw-   0        0        0    17157 2022-11-14 22:42:12.000000 jaxfit-0.0.4/jaxfit/minpack.py
--rw-rw-rw-   0        0        0    31321 2022-11-14 22:40:00.000000 jaxfit-0.0.4/jaxfit/trf.py
-drwxrwxrwx   0        0        0        0 2022-11-14 22:56:35.587000 jaxfit-0.0.4/jaxfit.egg-info/
--rw-rw-rw-   0        0        0      332 2022-11-14 22:56:34.000000 jaxfit-0.0.4/jaxfit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2022-11-14 22:56:35.000000 jaxfit-0.0.4/jaxfit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-14 22:56:35.000000 jaxfit-0.0.4/jaxfit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2022-11-14 22:56:35.000000 jaxfit-0.0.4/jaxfit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-11-14 22:56:35.000000 jaxfit-0.0.4/jaxfit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       96 2022-03-15 01:19:07.000000 jaxfit-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      470 2022-11-14 22:56:35.627000 jaxfit-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0       69 2022-03-15 01:19:48.000000 jaxfit-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:27:30.029000 jaxfit-0.0.5/
+-rw-rw-rw-   0        0        0     1539 2023-05-12 14:25:03.000000 jaxfit-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      332 2023-06-23 12:27:29.992000 jaxfit-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9879 2023-01-09 17:20:27.000000 jaxfit-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 12:27:29.781000 jaxfit-0.0.5/jaxfit/
+-rw-rw-rw-   0        0        0      336 2023-01-09 13:30:22.000000 jaxfit-0.0.5/jaxfit/__init__.py
+-rw-rw-rw-   0        0        0     2577 2022-07-21 12:32:10.000000 jaxfit-0.0.5/jaxfit/_optimize.py
+-rw-rw-rw-   0        0        0     8909 2023-01-09 15:14:10.000000 jaxfit-0.0.5/jaxfit/common_jax.py
+-rw-rw-rw-   0        0        0    21781 2023-01-09 16:40:35.000000 jaxfit-0.0.5/jaxfit/common_scipy.py
+-rw-rw-rw-   0        0        0    26889 2023-01-09 15:48:53.000000 jaxfit-0.0.5/jaxfit/least_squares.py
+-rw-rw-rw-   0        0        0     5465 2023-01-10 12:16:56.000000 jaxfit-0.0.5/jaxfit/loss_functions.py
+-rw-rw-rw-   0        0        0    22129 2023-06-23 10:14:58.000000 jaxfit-0.0.5/jaxfit/minpack.py
+-rw-rw-rw-   0        0        0    54044 2023-01-09 16:35:38.000000 jaxfit-0.0.5/jaxfit/trf.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:27:29.916000 jaxfit-0.0.5/jaxfit.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-06-23 12:27:29.000000 jaxfit-0.0.5/jaxfit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2023-06-23 12:27:29.000000 jaxfit-0.0.5/jaxfit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 12:27:29.000000 jaxfit-0.0.5/jaxfit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-23 12:27:29.000000 jaxfit-0.0.5/jaxfit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 12:27:29.000000 jaxfit-0.0.5/jaxfit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       96 2022-03-15 01:19:07.000000 jaxfit-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      486 2023-06-23 12:27:30.023000 jaxfit-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       69 2022-03-15 01:19:48.000000 jaxfit-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:27:29.970000 jaxfit-0.0.5/tests/
+-rw-rw-rw-   0        0        0    32298 2022-07-13 13:33:18.000000 jaxfit-0.0.5/tests/test_least_squares.py
+-rw-rw-rw-   0        0        0    31235 2022-07-21 12:45:01.000000 jaxfit-0.0.5/tests/test_minpack.py
```

### Comparing `jaxfit-0.0.4/LICENSE.txt` & `jaxfit-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaxfit-0.0.4/README.md` & `jaxfit-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 <div align="center">
-<img src="https://github.com/Dipolar-Quantum-Gases/jaxfit/blob/main/images/JAXFit_small.jpg" alt="logo"></img>
+<img src="docs/images/JAXFit_small.jpg" alt="logo"></img>
 </div>
 
 # JAXFit: Nonlinear least squares curve fitting for the GPU/TPU
 
 
 [**Quickstart**](#quickstart-colab-in-the-cloud)
 | [**Install guide**](#installation)
 | [**ArXiv Paper**](https://doi.org/10.48550/arXiv.2208.12187)
-
-<!--
-| [**Reference docs**](https://youtu.be/xvFZjo5PgG0)
--->
+| [**Documentation**](https://jaxfit.readthedocs.io/)
 
 ## What is JAXFit?
 
 JAXFit takes well tested and developed SciPy nonlinear least squares (NLSQ) curve fitting algorithms, but runs them on the GPU/TPU using [JAX](https://jax.readthedocs.io/en/latest/notebooks/quickstart.html) for a massive fit speed up. The package is very easy to use as the fit functions are defined only in Python with no CUDA programming needed. An introductory paper detailing the algorithm and performance improvements over SciPy/Gpufit can be found [here](https://doi.org/10.48550/arXiv.2208.12187).
 
 JAXFit also improves on SciPy's algorithm by taking advantage of JAX's in-built [automatic differentiation](https://jax.readthedocs.io/en/latest/notebooks/autodiff_cookbook.html) (autodiff) of Python functions. We use JAX's autodiff to calculate the Jacobians in the NLSQ algorithms rather than requiring the user to give analytic partial derivatives or using numeric approximation techniques.
 
@@ -59,27 +56,26 @@
 * [Citing JAXFit](#citing-jax)
 * [Reference documentation](#reference-documentation)
 
 ## Quickstart: Colab in the Cloud
 The easiest way to test out JAXFit is using a Colab notebook connected to a Google Cloud GPU. JAX comes pre-installed so you'll be able to start fitting right away.
 
 We have a few tutorial notebooks including:
-- [The basics: fitting basic functions with JAXFit](https://colab.research.google.com/github/Dipolar-Quantum-Gases/jaxfit/blob/main/examples/JAXFit%20Quickstart.ipynb)
-- [Fitting 2D images with JAXFit](https://colab.research.google.com/github/Dipolar-Quantum-Gases/jaxfit/blob/main/examples/JAXFit%202D%20Gaussian%20Demo.ipynb)
+- [The basics: fitting basic functions with JAXFit](https://colab.research.google.com/github/Dipolar-Quantum-Gases/jaxfit/blob/main/docs/notebooks/JAXFit_Quickstart.ipynb)
+- [Fitting 2D images with JAXFit](https://colab.research.google.com/github/Dipolar-Quantum-Gases/jaxfit/blob/main/docs/notebooks/JAXFit_2D_Gaussian_Demo.ipynb)
 
 ## Current gotchas
 
 Full disclosure we've copied most of this from the [JAX repo](https://github.com/google/jax#current-gotchas), but JAXFit inherits
 JAX's idiosyncrasies and so the "gotchas" are mostly the same.
 
 ### Double precision required
-First and foremost by default JAX enforces single precision (32-bit, e.g. `float32`), but JAXFit needs double precision (64-bit, e.g. `float64`). [To enable
-   double-precision](https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#double-64bit-precision)
-   (64-bit, e.g. `float64`) one needs to set the `jax_enable_x64` variable at
-   startup (or set the environment variable `JAX_ENABLE_X64=True`). 
+First and foremost by default JAX enforces single precision (32-bit, e.g. `float32`), but JAXFit needs double precision (64-bit, e.g. `float64`). 
+[To enable double-precision](https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#double-64bit-precision)
+(64-bit, e.g. `float64`) one needs to set the `jax_enable_x64` variable at startup (or set the environment variable `JAX_ENABLE_X64=True`). 
    
 JAXFit does this when it is imported, but should you import JAX before JAXFit, then you'll need to set this flag yourself e.g.
 
 ```python
 from jax.config import config
 config.update("jax_enable_x64", True)
 
@@ -89,42 +85,30 @@
 
 ### Other caveats
 Below are some more things to be careful of, but a full list can be found in [JAX's Gotchas
 Notebook](https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html).
 Some standouts:
 
 1. JAX transformations only work on [pure functions](https://en.wikipedia.org/wiki/Pure_function), which don't have side-effects and respect [referential transparency](https://en.wikipedia.org/wiki/Referential_transparency) (i.e. object identity testing with `is` isn't preserved). If you use a JAX transformation on an impure Python function, you might see an error like `Exception: Can't lift Traced...`  or `Exception: Different traces at same level`.
-1. [In-place mutating updates of
-   arrays](https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#in-place-updates), like `x[i] += y`, aren't supported, but [there are functional alternatives](https://jax.readthedocs.io/en/latest/jax.ops.html). Under a `jit`, those functional alternatives will reuse buffers in-place automatically.
-1. Some transformations, like `jit`, [constrain how you can use Python control
-   flow](https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#control-flow).
-   You'll always get loud errors if something goes wrong. You might have to use
-   [`jit`'s `static_argnums`
-   parameter](https://jax.readthedocs.io/en/latest/jax.html#just-in-time-compilation-jit),
-   [structured control flow
-   primitives](https://jax.readthedocs.io/en/latest/jax.lax.html#control-flow-operators)
-   like
-   [`lax.scan`](https://jax.readthedocs.io/en/latest/_autosummary/jax.lax.scan.html#jax.lax.scan).
-1. Some of NumPy's dtype promotion semantics involving a mix of Python scalars
-   and NumPy types aren't preserved, namely `np.add(1, np.array([2],
-   np.float32)).dtype` is `float64` rather than `float32`.
-1. If you're looking for [convolution
-   operators](https://jax.readthedocs.io/en/latest/notebooks/convolutions.html),
-   they're in the `jax.lax` package.
+1. [In-place mutating updates of arrays](https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#in-place-updates), like `x[i] += y`, aren't supported, but [there are functional alternatives](https://jax.readthedocs.io/en/latest/jax.ops.html). Under a `jit`, those functional alternatives will reuse buffers in-place automatically.
+1. Some transformations, like `jit`, [constrain how you can use Python control flow](https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#control-flow). You'll always get loud errors if something goes wrong. You might have to use [jit's static_argnums parameter](https://jax.readthedocs.io/en/latest/jax.html#just-in-time-compilation-jit), [structured control flow primitives](https://jax.readthedocs.io/en/latest/jax.lax.html#control-flow-operators) like [lax.scan](https://jax.readthedocs.io/en/latest/_autosummary/jax.lax.scan.html#jax.lax.scan).
+1. Some of NumPy's dtype promotion semantics involving a mix of Python scalars and NumPy types aren't preserved, namely `np.add(1, np.array([2], np.float32)).dtype` is `float64` rather than `float32`.
+1. If you're looking for [convolution operators](https://jax.readthedocs.io/en/latest/notebooks/convolutions.html), they're in the `jax.lax` package.
 
 
 ## Installation
 
 JAXFit is written in pure Python and is based on the JAX package. JAX therefore needs to be installed before installing JAXFit via pip. JAX installation requires 
 a bit of effort since it is optimized for the computer hardware you'll be using (GPU vs. CPU). 
 
 Installing JAX on Linux is natively supported by the JAX team and instructions
 to do so can be found [here](https://github.com/google/jax#installation). 
 
-For Windows systems, the officially supported method is building directly from the source code (see [Building JAX from source](https://jax.readthedocs.io/en/latest/developer.html#building-from-source)). However, we've found it easier to use pre-built JAX wheels which can be found in [this Github repo](https://github.com/cloudhan/jax-windows-builder) and we've included detailed instructions on this installation process below.
+For Windows systems, the officially supported method is building directly from the source code 
+(see [Building JAX from source](https://jax.readthedocs.io/en/latest/developer.html#building-from-source)). However, we've found it easier to use pre-built JAX wheels which can be found in [this Github repo](https://github.com/cloudhan/jax-windows-builder) and we've included detailed instructions on this installation process below.
 
 After installing JAX, you can now install JAXFit via the following pip command
 
 ```
 pip install jaxfit
 ```
 
@@ -192,8 +176,8 @@
 }
 ```
 
 
 ## Reference documentation
 
 For details about the JAXFit API, see the
-[reference documentation](https://jax.readthedocs.io/).
+[reference documentation](https://jaxfit.readthedocs.io/).
```

### Comparing `jaxfit-0.0.4/jaxfit/_optimize.py` & `jaxfit-0.0.5/jaxfit/_optimize.py`

 * *Files identical despite different names*

### Comparing `jaxfit-0.0.4/jaxfit/common_scipy.py` & `jaxfit-0.0.5/jaxfit/common_scipy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Functions used by least-squares algorithms."""
+"""Functions used by least-squares algorithms. Those functions that involve
+large computations are reimplemented in the common_jax.py file using JAX."""
 from math import copysign
 
 import numpy as np
 from numpy.linalg import norm
 
 from scipy.linalg import cho_factor, cho_solve, LinAlgError
 from scipy.sparse import issparse
@@ -13,22 +14,25 @@
 # Functions related to a trust-region problem.
 
 
 def intersect_trust_region(x, s, Delta):
     """Find the intersection of a line with the boundary of a trust region.
     This function solves the quadratic equation with respect to t
     ||(x + s*t)||**2 = Delta**2.
+
     Returns
     -------
     t_neg, t_pos : tuple of float
         Negative and positive roots.
+        
     Raises
     ------
     ValueError
         If `s` is zero or `x` is not within the trust region.
+
     """
     a = np.dot(s, s)
     if a == 0:
         raise ValueError("`s` is zero.")
 
     b = np.dot(x, s)
 
@@ -48,18 +52,19 @@
     else:
         return t2, t1
     
     
 def solve_lsq_trust_region(n, m, uf, s, V, Delta, initial_alpha=None,
                            rtol=0.01, max_iter=10):
     """Solve a trust-region problem arising in least-squares minimization.
-    This function implements a method described by J. J. More [1]_ and used
+    This function implements a method described by J. J. More [12]_ and used
     in MINPACK, but it relies on a single SVD of Jacobian instead of series
     of Cholesky decompositions. Before running this function, compute:
     ``U, s, VT = svd(J, full_matrices=False)``.
+
     Parameters
     ----------
     n : int
         Number of variables.
     m : int
         Number of residuals.
     uf : ndarray
@@ -74,34 +79,37 @@
         Initial guess for alpha, which might be available from a previous
         iteration. If None, determined automatically.
     rtol : float, optional
         Stopping tolerance for the root-finding procedure. Namely, the
         solution ``p`` will satisfy ``abs(norm(p) - Delta) < rtol * Delta``.
     max_iter : int, optional
         Maximum allowed number of iterations for the root-finding procedure.
+
     Returns
     -------
     p : ndarray, shape (n,)
         Found solution of a trust-region problem.
     alpha : float
         Positive value such that (J.T*J + alpha*I)*p = -J.T*f.
         Sometimes called Levenberg-Marquardt parameter.
     n_iter : int
         Number of iterations made by root-finding procedure. Zero means
         that Gauss-Newton step was selected as the solution.
+
     References
     ----------
-    .. [1] More, J. J., "The Levenberg-Marquardt Algorithm: Implementation
+    .. [12] More, J. J., "The Levenberg-Marquardt Algorithm: Implementation
            and Theory," Numerical Analysis, ed. G. A. Watson, Lecture Notes
            in Mathematics 630, Springer Verlag, pp. 105-116, 1977.
+
     """
     def phi_and_derivative(alpha, suf, s, Delta):
         """Function of which to find zero.
         It is defined as "norm of regularized (by alpha) least-squares
-        solution minus `Delta`". Refer to [1]_.
+        solution minus `Delta`". Refer to [12]_.
         """
         denom = s**2 + alpha
         p_norm = norm(suf / denom)
         phi = p_norm - Delta
         phi_prime = -np.sum(suf ** 2 / denom**3) / p_norm
         return phi, phi_prime
     
@@ -155,142 +163,37 @@
     # this. It is done to prevent p lie outside the trust region (which can
     # cause problems later).
     p *= Delta / norm(p)
 
     return p, alpha, it + 1
 
 
-# def solve_lsq_trust_region(n, m, uf, s, V, Delta, initial_alpha=None,
-#                            rtol=0.01, max_iter=10):
-#     """Solve a trust-region problem arising in least-squares minimization.
-#     This function implements a method described by J. J. More [1]_ and used
-#     in MINPACK, but it relies on a single SVD of Jacobian instead of series
-#     of Cholesky decompositions. Before running this function, compute:
-#     ``U, s, VT = svd(J, full_matrices=False)``.
-#     Parameters
-#     ----------
-#     n : int
-#         Number of variables.
-#     m : int
-#         Number of residuals.
-#     uf : ndarray
-#         Computed as U.T.dot(f).
-#     s : ndarray
-#         Singular values of J.
-#     V : ndarray
-#         Transpose of VT.
-#     Delta : float
-#         Radius of a trust region.
-#     initial_alpha : float, optional
-#         Initial guess for alpha, which might be available from a previous
-#         iteration. If None, determined automatically.
-#     rtol : float, optional
-#         Stopping tolerance for the root-finding procedure. Namely, the
-#         solution ``p`` will satisfy ``abs(norm(p) - Delta) < rtol * Delta``.
-#     max_iter : int, optional
-#         Maximum allowed number of iterations for the root-finding procedure.
-#     Returns
-#     -------
-#     p : ndarray, shape (n,)
-#         Found solution of a trust-region problem.
-#     alpha : float
-#         Positive value such that (J.T*J + alpha*I)*p = -J.T*f.
-#         Sometimes called Levenberg-Marquardt parameter.
-#     n_iter : int
-#         Number of iterations made by root-finding procedure. Zero means
-#         that Gauss-Newton step was selected as the solution.
-#     References
-#     ----------
-#     .. [1] More, J. J., "The Levenberg-Marquardt Algorithm: Implementation
-#            and Theory," Numerical Analysis, ed. G. A. Watson, Lecture Notes
-#            in Mathematics 630, Springer Verlag, pp. 105-116, 1977.
-#     """
-#     def phi_and_derivative(alpha, suf, s, Delta):
-#         """Function of which to find zero.
-#         It is defined as "norm of regularized (by alpha) least-squares
-#         solution minus `Delta`". Refer to [1]_.
-#         """
-#         denom = s**2 + alpha
-#         p_norm = norm(suf / denom)
-#         phi = p_norm - Delta
-#         phi_prime = -np.sum(suf ** 2 / denom**3) / p_norm
-#         return phi, phi_prime
-
-#     suf = s * uf
-
-#     # Check if J has full rank and try Gauss-Newton step.
-#     if m >= n:
-#         threshold = EPS * m * s[0]
-#         full_rank = s[-1] > threshold
-#     else:
-#         full_rank = False
-
-#     if full_rank:
-#         p = -V.dot(uf / s)
-#         if norm(p) <= Delta:
-#             return p, 0.0, 0
-
-#     alpha_upper = norm(suf) / Delta
-
-#     if full_rank:
-#         phi, phi_prime = phi_and_derivative(0.0, suf, s, Delta)
-#         alpha_lower = -phi / phi_prime
-#     else:
-#         alpha_lower = 0.0
-
-#     if initial_alpha is None or not full_rank and initial_alpha == 0:
-#         alpha = max(0.001 * alpha_upper, (alpha_lower * alpha_upper)**0.5)
-#     else:
-#         alpha = initial_alpha
-
-#     for it in range(max_iter):
-#         if alpha < alpha_lower or alpha > alpha_upper:
-#             alpha = max(0.001 * alpha_upper, (alpha_lower * alpha_upper)**0.5)
-
-#         phi, phi_prime = phi_and_derivative(alpha, suf, s, Delta)
-
-#         if phi < 0:
-#             alpha_upper = alpha
-
-#         ratio = phi / phi_prime
-#         alpha_lower = max(alpha_lower, alpha - ratio)
-#         alpha -= (phi + Delta) * ratio / Delta
-
-#         if np.abs(phi) < rtol * Delta:
-#             break
-
-#     p = -V.dot(suf / (s**2 + alpha))
-
-#     # Make the norm of p equal to Delta, p is changed only slightly during
-#     # this. It is done to prevent p lie outside the trust region (which can
-#     # cause problems later).
-#     p *= Delta / norm(p)
-
-#     return p, alpha, it + 1
-
 
 def solve_trust_region_2d(B, g, Delta):
     """Solve a general trust-region problem in 2 dimensions.
     The problem is reformulated as a 4th order algebraic equation,
     the solution of which is found by numpy.roots.
+
     Parameters
     ----------
     B : ndarray, shape (2, 2)
         Symmetric matrix, defines a quadratic term of the function.
     g : ndarray, shape (2,)
         Defines a linear term of the function.
     Delta : float
         Radius of a trust region.
+
     Returns
     -------
     p : ndarray, shape (2,)
         Found solution.
     newton_step : bool
         Whether the returned solution is the Newton step which lies within
         the trust region.
+
     """
     try:
         R, lower = cho_factor(B)
         p = -cho_solve((R, lower), g)
         if np.dot(p, p) <= Delta**2:
             return p, True
     except LinAlgError:
@@ -315,20 +218,22 @@
 
     return p, False
 
 
 def update_tr_radius(Delta, actual_reduction, predicted_reduction,
                      step_norm, bound_hit):
     """Update the radius of a trust region based on the cost reduction.
+
     Returns
     -------
     Delta : float
         New radius.
     ratio : float
         Ratio between actual and predicted reductions.
+
     """
     if predicted_reduction > 0:
         ratio = actual_reduction / predicted_reduction
     elif predicted_reduction == actual_reduction == 0:
         ratio = 1
     else:
         ratio = 0
@@ -340,71 +245,73 @@
 
     return Delta, ratio
 
 
 # Construction and minimization of quadratic functions.
 
 
-def build_quadratic_1d(J, g, s, diag=None, s0=None):
-    """Parameterize a multivariate quadratic function along a line.
-    The resulting univariate quadratic function is given as follows:
-    ::
-        f(t) = 0.5 * (s0 + s*t).T * (J.T*J + diag) * (s0 + s*t) +
-               g.T * (s0 + s*t)
-    Parameters
-    ----------
-    J : ndarray, sparse matrix or LinearOperator shape (m, n)
-        Jacobian matrix, affects the quadratic term.
-    g : ndarray, shape (n,)
-        Gradient, defines the linear term.
-    s : ndarray, shape (n,)
-        Direction vector of a line.
-    diag : None or ndarray with shape (n,), optional
-        Addition diagonal part, affects the quadratic term.
-        If None, assumed to be 0.
-    s0 : None or ndarray with shape (n,), optional
-        Initial point. If None, assumed to be 0.
-    Returns
-    -------
-    a : float
-        Coefficient for t**2.
-    b : float
-        Coefficient for t.
-    c : float
-        Free term. Returned only if `s0` is provided.
-    """
-    v = J.dot(s)
-    a = np.dot(v, v)
-    if diag is not None:
-        a += np.dot(s * diag, s)
-    a *= 0.5
-
-    b = np.dot(g, s)
-
-    if s0 is not None:
-        u = J.dot(s0)
-        b += np.dot(u, v)
-        c = 0.5 * np.dot(u, u) + np.dot(g, s0)
-        if diag is not None:
-            b += np.dot(s0 * diag, s)
-            c += 0.5 * np.dot(s0 * diag, s0)
-        return a, b, c
-    else:
-        return a, b
+# def build_quadratic_1d(J, g, s, diag=None, s0=None):
+#     """Parameterize a multivariate quadratic function along a line.
+#     The resulting univariate quadratic function is given as follows:
+#     ::
+#         f(t) = 0.5 * (s0 + s*t).T * (J.T*J + diag) * (s0 + s*t) +
+#                g.T * (s0 + s*t)
+#     Parameters
+#     ----------
+#     J : ndarray, sparse matrix or LinearOperator shape (m, n)
+#         Jacobian matrix, affects the quadratic term.
+#     g : ndarray, shape (n,)
+#         Gradient, defines the linear term.
+#     s : ndarray, shape (n,)
+#         Direction vector of a line.
+#     diag : None or ndarray with shape (n,), optional
+#         Addition diagonal part, affects the quadratic term.
+#         If None, assumed to be 0.
+#     s0 : None or ndarray with shape (n,), optional
+#         Initial point. If None, assumed to be 0.
+#     Returns
+#     -------
+#     a : float
+#         Coefficient for t**2.
+#     b : float
+#         Coefficient for t.
+#     c : float
+#         Free term. Returned only if `s0` is provided.
+#     """
+#     v = J.dot(s)
+#     a = np.dot(v, v)
+#     if diag is not None:
+#         a += np.dot(s * diag, s)
+#     a *= 0.5
+
+#     b = np.dot(g, s)
+
+#     if s0 is not None:
+#         u = J.dot(s0)
+#         b += np.dot(u, v)
+#         c = 0.5 * np.dot(u, u) + np.dot(g, s0)
+#         if diag is not None:
+#             b += np.dot(s0 * diag, s)
+#             c += 0.5 * np.dot(s0 * diag, s0)
+#         return a, b, c
+#     else:
+#         return a, b
 
 
 def minimize_quadratic_1d(a, b, lb, ub, c=0):
     """Minimize a 1-D quadratic function subject to bounds.
     The free term `c` is 0 by default. Bounds must be finite.
+
     Returns
     -------
     t : float
         Minimum point.
     y : float
         Minimum value.
+
     """
     t = [lb, ub]
     if a != 0:
         extremum = -0.5 * b / a
         if lb < extremum < ub:
             t.append(extremum)
     t = np.asarray(t)
@@ -412,30 +319,33 @@
     min_index = np.argmin(y)
     return t[min_index], y[min_index]
 
 
 def evaluate_quadratic(J, g, s, diag=None):
     """Compute values of a quadratic function arising in least squares.
     The function is 0.5 * s.T * (J.T * J + diag) * s + g.T * s.
+
     Parameters
     ----------
     J : ndarray, sparse matrix or LinearOperator, shape (m, n)
         Jacobian matrix, affects the quadratic term.
     g : ndarray, shape (n,)
         Gradient, defines the linear term.
     s : ndarray, shape (k, n) or (n,)
         Array containing steps as rows.
     diag : ndarray, shape (n,), optional
         Addition diagonal part, affects the quadratic term.
         If None, assumed to be 0.
+
     Returns
     -------
     values : ndarray with shape (k,) or float
         Values of the function. If `s` was 2-D, then ndarray is
         returned, otherwise, float is returned.
+
     """
     if s.ndim == 1:
         Js = J.dot(s)
         q = np.dot(Js, Js)
         if diag is not None:
             q += np.dot(s * diag, s)
     else:
@@ -457,24 +367,27 @@
     return np.all((x >= lb) & (x <= ub))
 
 
 def step_size_to_bound(x, s, lb, ub):
     """Compute a min_step size required to reach a bound.
     The function computes a positive scalar t, such that x + s * t is on
     the bound.
+
     Returns
     -------
     step : float
         Computed step. Non-negative value.
     hits : ndarray of int with shape of x
         Each element indicates whether a corresponding variable reaches the
         bound:
+        
              *  0 - the bound was not hit.
              * -1 - the lower bound was hit.
              *  1 - the upper bound was hit.
+
     """
     non_zero = np.nonzero(s)
     s_non_zero = s[non_zero]
     steps = np.empty_like(x)
     steps.fill(np.inf)
     with np.errstate(over='ignore'):
         steps[non_zero] = np.maximum((lb - x)[non_zero] / s_non_zero,
@@ -483,21 +396,23 @@
     return min_step, np.equal(steps, min_step) * np.sign(s).astype(int)
 
 
 def find_active_constraints(x, lb, ub, rtol=1e-10):
     """Determine which constraints are active in a given point.
     The threshold is computed using `rtol` and the absolute value of the
     closest bound.
+
     Returns
     -------
     active : ndarray of int with shape of x
         Each component shows whether the corresponding constraint is active:
              *  0 - a constraint is not active.
              * -1 - a lower bound is active.
              *  1 - a upper bound is active.
+
     """
     active = np.zeros_like(x, dtype=int)
 
     if rtol == 0:
         active[x <= lb] = -1
         active[x >= ub] = 1
         return active
@@ -543,34 +458,37 @@
     x_new[tight_bounds] = 0.5 * (lb[tight_bounds] + ub[tight_bounds])
     # print('x_new', x_new)
     return x_new
 
 
 def CL_scaling_vector(x, g, lb, ub):
     """Compute Coleman-Li scaling vector and its derivatives.
-    Components of a vector v are defined as follows:
-    ::
+    Components of a vector v are defined as follows::
+
                | ub[i] - x[i], if g[i] < 0 and ub[i] < np.inf
         v[i] = | x[i] - lb[i], if g[i] > 0 and lb[i] > -np.inf
                | 1,           otherwise
+
     According to this definition v[i] >= 0 for all i. It differs from the
-    definition in paper [1]_ (eq. (2.2)), where the absolute value of v is
+    definition in paper [5]_ (eq. (2.2)), where the absolute value of v is
     used. Both definitions are equivalent down the line.
     Derivatives of v with respect to x take value 1, -1 or 0 depending on a
     case.
+
     Returns
     -------
     v : ndarray with shape of x
         Scaling vector.
     dv : ndarray with shape of x
         Derivatives of v[i] with respect to x[i], diagonal elements of v's
         Jacobian.
+
     References
     ----------
-    .. [1] M.A. Branch, T.F. Coleman, and Y. Li, "A Subspace, Interior,
+    .. [5] M.A. Branch, T.F. Coleman, and Y. Li, "A Subspace, Interior,
            and Conjugate Gradient Method for Large-Scale Bound-Constrained
            Minimization Problems," SIAM Journal on Scientific Computing,
            Vol. 21, Number 1, pp 1-23, 1999.
     """
     v = np.ones_like(x)
     dv = np.zeros_like(x)
 
@@ -664,125 +582,125 @@
     print("{0:^15}{1:^15.4e}{2}{3}{4:^15.2e}".format(
         iteration, cost, cost_reduction, step_norm, optimality))
 
 
 # Simple helper functions.
 
 
-def compute_grad(J, f):
-    """Compute gradient of the least-squares cost function."""
-    if isinstance(J, LinearOperator):
-        return J.rmatvec(f)
-    else:
-        print('isdot')
-        return J.T.dot(f)
+# def compute_grad(J, f):
+#     """Compute gradient of the least-squares cost function."""
+#     if isinstance(J, LinearOperator):
+#         return J.rmatvec(f)
+#     else:
+#         print('isdot')
+#         return J.T.dot(f)
 
 
-def compute_jac_scale(J, scale_inv_old=None):
-    """Compute variables scale based on the Jacobian matrix."""
-    if issparse(J):
-        scale_inv = np.asarray(J.power(2).sum(axis=0)).ravel()**0.5
-    else:
-        scale_inv = np.sum(J**2, axis=0)**0.5
+# def compute_jac_scale(J, scale_inv_old=None):
+#     """Compute variables scale based on the Jacobian matrix."""
+#     if issparse(J):
+#         scale_inv = np.asarray(J.power(2).sum(axis=0)).ravel()**0.5
+#     else:
+#         scale_inv = np.sum(J**2, axis=0)**0.5
 
-    if scale_inv_old is None:
-        scale_inv[scale_inv == 0] = 1
-    else:
-        scale_inv = np.maximum(scale_inv, scale_inv_old)
+#     if scale_inv_old is None:
+#         scale_inv[scale_inv == 0] = 1
+#     else:
+#         scale_inv = np.maximum(scale_inv, scale_inv_old)
 
-    return 1 / scale_inv, scale_inv
+#     return 1 / scale_inv, scale_inv
 
 
-def left_multiplied_operator(J, d):
-    """Return diag(d) J as LinearOperator."""
-    J = aslinearoperator(J)
+# def left_multiplied_operator(J, d):
+#     """Return diag(d) J as LinearOperator."""
+#     J = aslinearoperator(J)
 
-    def matvec(x):
-        return d * J.matvec(x)
+#     def matvec(x):
+#         return d * J.matvec(x)
 
-    def matmat(X):
-        return d[:, np.newaxis] * J.matmat(X)
+#     def matmat(X):
+#         return d[:, np.newaxis] * J.matmat(X)
 
-    def rmatvec(x):
-        return J.rmatvec(x.ravel() * d)
+#     def rmatvec(x):
+#         return J.rmatvec(x.ravel() * d)
 
-    return LinearOperator(J.shape, matvec=matvec, matmat=matmat,
-                          rmatvec=rmatvec)
+#     return LinearOperator(J.shape, matvec=matvec, matmat=matmat,
+#                           rmatvec=rmatvec)
 
 
-def right_multiplied_operator(J, d):
-    """Return J diag(d) as LinearOperator."""
-    J = aslinearoperator(J)
+# def right_multiplied_operator(J, d):
+#     """Return J diag(d) as LinearOperator."""
+#     J = aslinearoperator(J)
 
-    def matvec(x):
-        return J.matvec(np.ravel(x) * d)
+#     def matvec(x):
+#         return J.matvec(np.ravel(x) * d)
 
-    def matmat(X):
-        return J.matmat(X * d[:, np.newaxis])
+#     def matmat(X):
+#         return J.matmat(X * d[:, np.newaxis])
 
-    def rmatvec(x):
-        return d * J.rmatvec(x)
+#     def rmatvec(x):
+#         return d * J.rmatvec(x)
 
-    return LinearOperator(J.shape, matvec=matvec, matmat=matmat,
-                          rmatvec=rmatvec)
+#     return LinearOperator(J.shape, matvec=matvec, matmat=matmat,
+#                           rmatvec=rmatvec)
 
 
-def regularized_lsq_operator(J, diag):
-    """Return a matrix arising in regularized least squares as LinearOperator.
-    The matrix is
-        [ J ]
-        [ D ]
-    where D is diagonal matrix with elements from `diag`.
-    """
-    J = aslinearoperator(J)
-    m, n = J.shape
+# def regularized_lsq_operator(J, diag):
+#     """Return a matrix arising in regularized least squares as LinearOperator.
+#     The matrix is
+#         [ J ]
+#         [ D ]
+#     where D is diagonal matrix with elements from `diag`.
+#     """
+#     J = aslinearoperator(J)
+#     m, n = J.shape
 
-    def matvec(x):
-        return np.hstack((J.matvec(x), diag * x))
+#     def matvec(x):
+#         return np.hstack((J.matvec(x), diag * x))
 
-    def rmatvec(x):
-        x1 = x[:m]
-        x2 = x[m:]
-        return J.rmatvec(x1) + diag * x2
+#     def rmatvec(x):
+#         x1 = x[:m]
+#         x2 = x[m:]
+#         return J.rmatvec(x1) + diag * x2
 
-    return LinearOperator((m + n, n), matvec=matvec, rmatvec=rmatvec)
+#     return LinearOperator((m + n, n), matvec=matvec, rmatvec=rmatvec)
 
 
-def right_multiply(J, d, copy=True):
-    """Compute J diag(d).
-    If `copy` is False, `J` is modified in place (unless being LinearOperator).
-    """
-    if copy and not isinstance(J, LinearOperator):
-        J = J.copy()
+# def right_multiply(J, d, copy=True):
+#     """Compute J diag(d).
+#     If `copy` is False, `J` is modified in place (unless being LinearOperator).
+#     """
+#     if copy and not isinstance(J, LinearOperator):
+#         J = J.copy()
 
-    if issparse(J):
-        J.data *= d.take(J.indices, mode='clip')  # scikit-learn recipe.
-    elif isinstance(J, LinearOperator):
-        J = right_multiplied_operator(J, d)
-    else:
-        J *= d
+#     if issparse(J):
+#         J.data *= d.take(J.indices, mode='clip')  # scikit-learn recipe.
+#     elif isinstance(J, LinearOperator):
+#         J = right_multiplied_operator(J, d)
+#     else:
+#         J *= d
 
-    return J
+#     return J
 
 
-def left_multiply(J, d, copy=True):
-    """Compute diag(d) J.
-    If `copy` is False, `J` is modified in place (unless being LinearOperator).
-    """
-    if copy and not isinstance(J, LinearOperator):
-        J = J.copy()
+# def left_multiply(J, d, copy=True):
+#     """Compute diag(d) J.
+#     If `copy` is False, `J` is modified in place (unless being LinearOperator).
+#     """
+#     if copy and not isinstance(J, LinearOperator):
+#         J = J.copy()
 
-    if issparse(J):
-        J.data *= np.repeat(d, np.diff(J.indptr))  # scikit-learn recipe.
-    elif isinstance(J, LinearOperator):
-        J = left_multiplied_operator(J, d)
-    else:
-        J *= d[:, np.newaxis]
+#     if issparse(J):
+#         J.data *= np.repeat(d, np.diff(J.indptr))  # scikit-learn recipe.
+#     elif isinstance(J, LinearOperator):
+#         J = left_multiplied_operator(J, d)
+#     else:
+#         J *= d[:, np.newaxis]
 
-    return J
+#     return J
 
 
 def check_termination(dF, F, dx_norm, x_norm, ratio, ftol, xtol):
     """Check termination condition for nonlinear least squares."""
     ftol_satisfied = dF < ftol * F and ratio > 0.25
     xtol_satisfied = dx_norm < xtol * (xtol + x_norm)
 
@@ -792,18 +710,18 @@
         return 2
     elif xtol_satisfied:
         return 3
     else:
         return None
 
 
-def scale_for_robust_loss_function(J, f, rho):
-    """Scale Jacobian and residuals for a robust loss function.
-    Arrays are modified in place.
-    """
-    J_scale = rho[1] + 2 * rho[2] * f**2
-    J_scale[J_scale < EPS] = EPS
-    J_scale **= 0.5
+# def scale_for_robust_loss_function(J, f, rho):
+#     """Scale Jacobian and residuals for a robust loss function.
+#     Arrays are modified in place.
+#     """
+#     J_scale = rho[1] + 2 * rho[2] * f**2
+#     J_scale[J_scale < EPS] = EPS
+#     J_scale **= 0.5
 
-    f *= rho[1] / J_scale
+#     f *= rho[1] / J_scale
 
-    return left_multiply(J, J_scale, copy=False), f
+#     return left_multiply(J, J_scale, copy=False), f
```

