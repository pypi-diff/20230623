# Comparing `tmp/factor_pricing_model_risk_model-2023.4.0.tar.gz` & `tmp/factor_pricing_model_risk_model-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factor_pricing_model_risk_model-2023.4.0.tar", max compression
+gzip compressed data, was "factor_pricing_model_risk_model-2023.5.0.tar", max compression
```

## Comparing `factor_pricing_model_risk_model-2023.4.0.tar` & `factor_pricing_model_risk_model-2023.5.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1078 2023-06-05 21:42:22.109424 factor_pricing_model_risk_model-2023.4.0/LICENSE
--rw-r--r--   0        0        0     6687 2023-06-05 21:42:22.109424 factor_pricing_model_risk_model-2023.4.0/README.md
--rw-r--r--   0        0        0     2617 2023-06-05 21:42:27.569488 factor_pricing_model_risk_model-2023.4.0/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-05 21:42:27.525487 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/__init__.py
--rw-r--r--   0        0        0      253 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/accuracy/__init__.py
--rw-r--r--   0        0        0     3060 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/accuracy/bias.py
--rw-r--r--   0        0        0     5199 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/accuracy/value_at_risk.py
--rw-r--r--   0        0        0      113 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/config.py
--rw-r--r--   0        0        0        0 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/dataset/__init__.py
--rw-r--r--   0        0        0     3255 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/dataset/crypto.py
--rw-r--r--   0        0        0       46 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/engine/__init__.py
--rw-r--r--   0        0        0      183 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/engine/numpy.py
--rw-r--r--   0        0        0    11187 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/factor_risk_model.py
--rw-r--r--   0        0        0     7438 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/__init__.py
--rw-r--r--   0        0        0      621 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/portfolio.py
--rw-r--r--   0        0        0      796 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/returns.py
--rw-r--r--   0        0        0        0 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/py.typed
--rw-r--r--   0        0        0       59 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/regressor/__init__.py
--rw-r--r--   0        0        0     1138 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/regressor/ewls.py
--rw-r--r--   0        0        0     2514 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/regressor/wls.py
--rw-r--r--   0        0        0     2835 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/risk_model.py
--rw-r--r--   0        0        0     5537 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/rolling_factor_risk_model.py
--rw-r--r--   0        0        0     5025 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/rolling_risk_model.py
--rw-r--r--   0        0        0       59 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/statistical/__init__.py
--rw-r--r--   0        0        0     3932 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/statistical/apca.py
--rw-r--r--   0        0        0     4728 2023-06-05 21:42:22.205424 factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/statistical/pca.py
--rw-r--r--   0        0        0     8370 1970-01-01 00:00:00.000000 factor_pricing_model_risk_model-2023.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-22 16:01:53.894281 factor_pricing_model_risk_model-2023.5.0/LICENSE
+-rw-r--r--   0        0        0     7067 2023-06-22 16:01:53.894281 factor_pricing_model_risk_model-2023.5.0/README.md
+-rw-r--r--   0        0        0     2642 2023-06-22 16:02:00.050354 factor_pricing_model_risk_model-2023.5.0/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-22 16:02:00.010353 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/__init__.py
+-rw-r--r--   0        0        0      253 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/accuracy/__init__.py
+-rw-r--r--   0        0        0     3410 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/accuracy/bias.py
+-rw-r--r--   0        0        0     5663 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/accuracy/value_at_risk.py
+-rw-r--r--   0        0        0      113 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/config.py
+-rw-r--r--   0        0        0     2638 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/cov_estimator.py
+-rw-r--r--   0        0        0        0 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/dataset/__init__.py
+-rw-r--r--   0        0        0     3255 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/dataset/crypto.py
+-rw-r--r--   0        0        0       46 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/engine/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/engine/numpy.py
+-rw-r--r--   0        0        0    11187 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/factor_risk_model.py
+-rw-r--r--   0        0        0     7438 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/pipeline/__init__.py
+-rw-r--r--   0        0        0      621 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/pipeline/portfolio.py
+-rw-r--r--   0        0        0      796 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/pipeline/returns.py
+-rw-r--r--   0        0        0        0 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/py.typed
+-rw-r--r--   0        0        0       59 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/regressor/__init__.py
+-rw-r--r--   0        0        0     1138 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/regressor/ewls.py
+-rw-r--r--   0        0        0     2514 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/regressor/wls.py
+-rw-r--r--   0        0        0     3251 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/risk_model.py
+-rw-r--r--   0        0        0     5537 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/rolling_factor_risk_model.py
+-rw-r--r--   0        0        0     5025 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/rolling_risk_model.py
+-rw-r--r--   0        0        0       59 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/statistical/__init__.py
+-rw-r--r--   0        0        0     3932 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/statistical/apca.py
+-rw-r--r--   0        0        0     4728 2023-06-22 16:01:54.010282 factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/statistical/pca.py
+-rw-r--r--   0        0        0     8750 1970-01-01 00:00:00.000000 factor_pricing_model_risk_model-2023.5.0/PKG-INFO
```

### Comparing `factor_pricing_model_risk_model-2023.4.0/LICENSE` & `factor_pricing_model_risk_model-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/README.md` & `factor_pricing_model_risk_model-2023.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,20 @@
 
 The project provides frameworks to create multi-factor risk
 model on an "enterprise-like" level.
 
 The target audiences are researchers, developers and fund
 management looking for flexibility in creating risk models.
 
+## Examples
+
+For end-to-end examples, please refer to [examples](https://github.com/factorpricingmodel/factor-pricing-model-risk-model/tree/main/examples) for the below notebooks
+
+- [Cryptocurrency Statistical Risk Model](https://colab.research.google.com/github/factorpricingmodel/factor-pricing-model-risk-model/blob/main/examples/notebook/crypto_statistical_risk_model.ipynb)
+
 ## Features
 
 Basically, there are three major features provided in the library
 
 - Factor risk model creation
 - Covariance estimator
 - Tracking risk model accuracy
```

#### html2text {}

```diff
@@ -7,34 +7,39 @@
 model.readthedocs.io/en/latest/) ## Installation Install this via pip (or your
 favourite package manager): `pip install factor-pricing-model-risk-model` ##
 Usage The library contains the pipelines to build the risk model. You can run
 the pipelines interactively in Jupyter Notebook. ```python import
 fpm_risk_model ``` ## Objective The project provides frameworks to create
 multi-factor risk model on an "enterprise-like" level. The target audiences are
 researchers, developers and fund management looking for flexibility in creating
-risk models. ## Features Basically, there are three major features provided in
-the library - Factor risk model creation - Covariance estimator - Tracking risk
-model accuracy ## Factor risk model The factor risk model is created by fitting
-instrument returns (which could be weekly, daily, or even higher granularity)
-and other related parameters into the model, and its products are factor
-exposures, factor returns, factor covariance, and residual returns
-(idiosyncratic returns). For example, to create a simple statistical PCA risk
-model, ``` from fpm_risk_model.statistics import PCA risk_model = PCA
-(n_components=5) risk_model.fit(X=returns) # Get fitted factor exposures
-risk_model.factor_exposures ``` Then, the risk model can be transformed by the
-returns of a larger homogeneous universe. ``` risk_model.transform
-(y=model_returns) ``` For further details, please refer to the [section](https:
-//factor-pricing-model-risk-model.readthedocs.io/en/latest/risk_model/
-factor_risk_model.html) in the documentation. ## Covariance estimation
-Currently, covariance estimation is supported in factor risk model, and the
-estimation depends on the fitted results. For example, a risk model transformed
-by model universe returns can derive the pairwise covariance and correlation
-for the model universe. ``` risk_model.transform(y=model_returns) cov =
-risk_model.cov() corr = risk_model.corr() ``` The following features will be
-supported in the near future - Covariance shrinkage - Covariance estimation
+risk models. ## Examples For end-to-end examples, please refer to [examples]
+(https://github.com/factorpricingmodel/factor-pricing-model-risk-model/tree/
+main/examples) for the below notebooks - [Cryptocurrency Statistical Risk
+Model](https://colab.research.google.com/github/factorpricingmodel/factor-
+pricing-model-risk-model/blob/main/examples/notebook/
+crypto_statistical_risk_model.ipynb) ## Features Basically, there are three
+major features provided in the library - Factor risk model creation -
+Covariance estimator - Tracking risk model accuracy ## Factor risk model The
+factor risk model is created by fitting instrument returns (which could be
+weekly, daily, or even higher granularity) and other related parameters into
+the model, and its products are factor exposures, factor returns, factor
+covariance, and residual returns (idiosyncratic returns). For example, to
+create a simple statistical PCA risk model, ``` from fpm_risk_model.statistics
+import PCA risk_model = PCA(n_components=5) risk_model.fit(X=returns) # Get
+fitted factor exposures risk_model.factor_exposures ``` Then, the risk model
+can be transformed by the returns of a larger homogeneous universe. ```
+risk_model.transform(y=model_returns) ``` For further details, please refer to
+the [section](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
+risk_model/factor_risk_model.html) in the documentation. ## Covariance
+estimation Currently, covariance estimation is supported in factor risk model,
+and the estimation depends on the fitted results. For example, a risk model
+transformed by model universe returns can derive the pairwise covariance and
+correlation for the model universe. ``` risk_model.transform(y=model_returns)
+cov = risk_model.cov() corr = risk_model.corr() ``` The following features will
+be supported in the near future - Covariance shrinkage - Covariance estimation
 from returns For further details, please refer to the [section](https://factor-
 pricing-model-risk-model.readthedocs.io/en/latest/risk_model/covariance.html)
 in the documentation. ## Tracking risk model accuracy The library also focuses
 on the predictability interpretation of the risk model, and provides a few
 benchmarks to examine the following metrics - [Bias](https://factor-pricing-
 model-risk-model.readthedocs.io/en/latest/accuracy/bias.html) - [Value at Risk
 (VaR)](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
```

### Comparing `factor_pricing_model_risk_model-2023.4.0/pyproject.toml` & `factor_pricing_model_risk_model-2023.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "factor-pricing-model-risk-model"
-version = "2023.4.0"
+version = "2023.5.0"
 description = "Package to build risk models for factor pricing model"
 authors = ["Factor Pricing Model <factor.pricing.model@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/factorpricingmodel/factor-pricing-model-risk-model"
 documentation = "https://factor-pricing-model-risk-model.readthedocs.io"
 classifiers = [
@@ -44,14 +44,15 @@
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 docformatter = "^1.5.0"
+pyarrow = ">=12.0,<13.0"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/fpm_risk_model/__init__.py:__version__"
 build_command = "pip install poetry && poetry build"
```

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/accuracy/bias.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/accuracy/bias.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Optional
+from typing import Any, Dict, Optional, Union
 
 from numpy import nan, sqrt, sum
 from pandas import DataFrame, Series
 
 from ..rolling_factor_risk_model import RollingFactorRiskModel
 
 
 def compute_standardized_returns(
     X: DataFrame,
     weights: DataFrame,
-    rolling_risk_model: Optional[RollingFactorRiskModel] = None,
+    rolling_risk_model: Optional[Union[RollingFactorRiskModel, Dict[Any, Any]]] = None,
     forecast_vols: Optional[Series] = None,
     cov_halflife: Optional[float] = None,
 ) -> Series:
     """
     Compute the standardized returns given the rolling risk model.
 
     Standardized return is defined as
@@ -24,16 +24,17 @@
 
     Parameters
     ----------
     X: ndarray
         The instrument forecast returns.
     weights: ndarray
         Weights of the instruments.
-    rolling_risk_model: RollingFactorRiskModel
-        The rolling risk model.
+    rolling_risk_model: Union[RollingFactorRiskModel, Dict[Any, Any]]
+        A rolling risk model object or dictionary of covariances of
+        which the keys and values are dates and covariances.
     forecast_vols: Series
         The forecast volatility.
     cov_halflife: Optional[float]
         Halflife in computing covariances.
 
     Returns
     -------
@@ -46,31 +47,30 @@
         returns = sum(X.loc[index, instruments] * index_weights)
         if forecast_vols is not None:
             vol = forecast_vols.loc[index]
         else:
             risk_model = rolling_risk_model.get(index)
             if risk_model is None:
                 continue
-            cov = (
-                risk_model.cov(halflife=cov_halflife)
-                .reindex(index=instruments, columns=instruments)
-                .fillna(0.0)
-                .values
-            )
+            elif isinstance(risk_model, DataFrame):
+                cov = risk_model
+            else:
+                cov = risk_model.cov(halflife=cov_halflife)
+            cov = cov.reindex(index=instruments, columns=instruments).fillna(0.0).values
             vol = sqrt((cov @ index_weights) @ index_weights)
         b_t[index] = returns / vol
 
     return b_t
 
 
 def compute_bias_statistics(
     X: DataFrame,
     weights: DataFrame,
     window: int,
-    rolling_risk_model: Optional[RollingFactorRiskModel] = None,
+    rolling_risk_model: Optional[Union[RollingFactorRiskModel, Dict[Any, Any]]] = None,
     forecast_vols: Optional[Series] = None,
     min_periods: Optional[int] = None,
     cov_halflife: Optional[float] = None,
 ) -> Series:
     """
     Compute the bias statistics.
 
@@ -88,16 +88,17 @@
     ----------
     X: ndarray
         The instrument forecast returns.
     weights: ndarray
         Weights of the instruments.
     forecast_vols: Optional[Series]
         The forecast volatility.
-    rolling_risk_model: RollingFactorRiskModel
-        The rolling risk model.
+    rolling_risk_model: Union[RollingFactorRiskModel, Dict[Any, Any]]
+        A rolling risk model object or dictionary of covariances of
+        which the keys and values are dates and covariances.
     cov_halflife: Optional[float]
         Halflife in computing covariances.
 
     Returns
     -------
     Series
         A timeseries of bias statistic.
```

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/accuracy/value_at_risk.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/accuracy/value_at_risk.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Optional
+from typing import Any, Dict, Optional, Union
 
 from numpy import nan, ndarray, sqrt, sum
 from pandas import DataFrame, Series
 from scipy.stats import norm
 
 from ..rolling_factor_risk_model import RollingFactorRiskModel
 
 
 def compute_value_at_risk_threshold(
     weights: DataFrame,
-    rolling_risk_model: Optional[RollingFactorRiskModel] = None,
+    rolling_risk_model: Optional[Union[RollingFactorRiskModel, Dict[Any, Any]]] = None,
     forecast_vols: Optional[Series] = None,
     threshold: Optional[float] = 0.95,
     cov_halflife: Optional[float] = None,
 ) -> Series:
     """
     Compute the VaR threshold for the given weights.
 
@@ -21,16 +21,17 @@
     ----------
     weights : DataFrame
         The portfolio weights for each instrument. The input
         index and columns are the date / time and instruments
         respectively. The weights should be normalized, i.e.
         sum to one for each time frame.
 
-    rolling_risk_model: Optional[RollingFactorRiskModel]
-        The rolling risk model.
+    rolling_risk_model: Union[RollingFactorRiskModel, Dict[Any, Any]]
+        A rolling risk model object or dictionary of covariances of
+        which the keys and values are dates and covariances.
 
     forecast_vols: Optional[Series]
         The forecast volatility of instruments.
 
     threshold: float
         The threshold for the VaR. The value should be between 0
         and 1. Default is 95%.
@@ -44,32 +45,32 @@
     value_at_risk = Series(nan, index=weights.index)
     instruments = weights.columns
     for index, index_weights in weights.iterrows():
         if rolling_risk_model is not None:
             risk_model = rolling_risk_model.get(index)
             if risk_model is None:
                 continue
-            cov = (
-                risk_model.cov(halflife=cov_halflife)
-                .reindex(index=instruments, columns=instruments)
-                .fillna(0.0)
-                .values
-            )
+            elif isinstance(risk_model, DataFrame):
+                cov = risk_model
+            else:
+                cov = risk_model.cov(halflife=cov_halflife)
+
+            cov = cov.reindex(index=instruments, columns=instruments).fillna(0.0).values
             vol = sqrt((cov @ index_weights) @ index_weights)
         else:
             vol = forecast_vols[index]
         value_at_risk[index] = quantile * vol
 
     return value_at_risk
 
 
 def compute_value_at_risk_breach_statistics(
     X: DataFrame,
     weights: DataFrame,
-    rolling_risk_model: Optional[RollingFactorRiskModel] = None,
+    rolling_risk_model: Optional[Union[RollingFactorRiskModel, Dict[Any, Any]]] = None,
     forecast_vols: Optional[Series] = None,
     threshold: Optional[float] = 0.95,
     cov_halflife: Optional[float] = None,
 ) -> Series:
     """
     Compute the VaR breach statistics.
 
@@ -81,16 +82,17 @@
 
     weights : DataFrame
         The portfolio weights for each instrument. The input
         index and columns are the date / time and instruments
         respectively. The weights should be normalized, i.e.
         sum to one for each time frame.
 
-    rolling_risk_model: Optional[RollingFactorRiskModel]
-        The rolling risk model.
+    rolling_risk_model: Union[RollingFactorRiskModel, Dict[Any, Any]]
+        A rolling risk model object or dictionary of covariances of
+        which the keys and values are dates and covariances.
 
     forecast_vols: Optional[Series]
         The forecast volatility of instruments.
 
     threshold: float
         The threshold for the VaR. The value should be between 0
         and 1. Default is 95%.
@@ -109,15 +111,15 @@
     return portfolio_returns.le(-value_at_risk_threshold)
 
 
 def compute_value_at_risk_rolling_breach_statistics(
     X: ndarray,
     weights: ndarray,
     window: int,
-    rolling_risk_model: Optional[RollingFactorRiskModel] = None,
+    rolling_risk_model: Optional[Union[RollingFactorRiskModel, Dict[Any, Any]]] = None,
     forecast_vols: Optional[Series] = None,
     threshold: Optional[float] = 0.95,
     min_periods: Optional[int] = None,
     cov_halflife: Optional[float] = None,
 ) -> Series:
     """
     Compute the VaR breach statistics.
@@ -134,16 +136,17 @@
         respectively. The weights should be normalized, i.e.
         sum to one for each time frame.
 
     window: int
         The number of rolling time frames to compute the percentage
         of returns breaching the specified VaR.
 
-    rolling_risk_model: Optional[RollingFactorRiskModel]
-        The rolling risk model.
+    rolling_risk_model: Union[RollingFactorRiskModel, Dict[Any, Any]]
+        A rolling risk model object or dictionary of covariances of
+        which the keys and values are dates and covariances.
 
     forecast_vols: Optional[Series]
         The forecast volatility of instruments.
 
     threshold: Optional[float]
         The threshold for the VaR. The value should be between 0
         and 1. Default is 95%.
```

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/dataset/crypto.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/dataset/crypto.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/factor_risk_model.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/factor_risk_model.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/__init__.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/portfolio.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/pipeline/portfolio.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/pipeline/returns.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/pipeline/returns.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/regressor/ewls.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/regressor/ewls.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/regressor/wls.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/regressor/wls.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/risk_model.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/risk_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import Any, Union
 
-from numpy import ndarray
+from numpy import diagonal, ndarray, sqrt
 from pandas import DataFrame, Series
 
 from .config import Config
 from .engine import NumpyEngine
 
 
 class RiskModelConfig(Config):
@@ -69,15 +69,30 @@
         Returns
         -------
         numpy.ndarray
             A square pairwise covariance matrix which its
             diagonal entries are the variances.
         """
 
-    def corr(self, **kwargs):
+    def vol(self, **kwargs) -> ndarray:
+        """
+        Get the volatility series.
+
+        Returns
+        -------
+        numpy.ndarray
+            Volatility series derived from covariance matrix.
+        """
+        cov = self.cov(**kwargs)
+        vol = sqrt(diagonal(cov))
+        if isinstance(cov, DataFrame):
+            vol = Series(vol, index=cov.index)
+        return vol
+
+    def corr(self, **kwargs) -> ndarray:
         """
         Get the correlation matrix.
 
         Returns
         -------
         numpy.ndarray
             A square pairwise correlation matrix which its
```

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/rolling_factor_risk_model.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/rolling_factor_risk_model.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/rolling_risk_model.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/rolling_risk_model.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/statistical/apca.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/statistical/apca.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/src/fpm_risk_model/statistical/pca.py` & `factor_pricing_model_risk_model-2023.5.0/src/fpm_risk_model/statistical/pca.py`

 * *Files identical despite different names*

### Comparing `factor_pricing_model_risk_model-2023.4.0/PKG-INFO` & `factor_pricing_model_risk_model-2023.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factor-pricing-model-risk-model
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: Package to build risk models for factor pricing model
 Home-page: https://github.com/factorpricingmodel/factor-pricing-model-risk-model
 License: MIT
 Author: Factor Pricing Model
 Author-email: factor.pricing.model@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -86,14 +86,20 @@
 
 The project provides frameworks to create multi-factor risk
 model on an "enterprise-like" level.
 
 The target audiences are researchers, developers and fund
 management looking for flexibility in creating risk models.
 
+## Examples
+
+For end-to-end examples, please refer to [examples](https://github.com/factorpricingmodel/factor-pricing-model-risk-model/tree/main/examples) for the below notebooks
+
+- [Cryptocurrency Statistical Risk Model](https://colab.research.google.com/github/factorpricingmodel/factor-pricing-model-risk-model/blob/main/examples/notebook/crypto_statistical_risk_model.ipynb)
+
 ## Features
 
 Basically, there are three major features provided in the library
 
 - Factor risk model creation
 - Covariance estimator
 - Tracking risk model accuracy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: factor-pricing-model-risk-model Version: 2023.4.0
+Metadata-Version: 2.1 Name: factor-pricing-model-risk-model Version: 2023.5.0
 Summary: Package to build risk models for factor pricing model Home-page:
 https://github.com/factorpricingmodel/factor-pricing-model-risk-model License:
 MIT Author: Factor Pricing Model Author-email: factor.pricing.model@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
@@ -29,34 +29,39 @@
 model.readthedocs.io/en/latest/) ## Installation Install this via pip (or your
 favourite package manager): `pip install factor-pricing-model-risk-model` ##
 Usage The library contains the pipelines to build the risk model. You can run
 the pipelines interactively in Jupyter Notebook. ```python import
 fpm_risk_model ``` ## Objective The project provides frameworks to create
 multi-factor risk model on an "enterprise-like" level. The target audiences are
 researchers, developers and fund management looking for flexibility in creating
-risk models. ## Features Basically, there are three major features provided in
-the library - Factor risk model creation - Covariance estimator - Tracking risk
-model accuracy ## Factor risk model The factor risk model is created by fitting
-instrument returns (which could be weekly, daily, or even higher granularity)
-and other related parameters into the model, and its products are factor
-exposures, factor returns, factor covariance, and residual returns
-(idiosyncratic returns). For example, to create a simple statistical PCA risk
-model, ``` from fpm_risk_model.statistics import PCA risk_model = PCA
-(n_components=5) risk_model.fit(X=returns) # Get fitted factor exposures
-risk_model.factor_exposures ``` Then, the risk model can be transformed by the
-returns of a larger homogeneous universe. ``` risk_model.transform
-(y=model_returns) ``` For further details, please refer to the [section](https:
-//factor-pricing-model-risk-model.readthedocs.io/en/latest/risk_model/
-factor_risk_model.html) in the documentation. ## Covariance estimation
-Currently, covariance estimation is supported in factor risk model, and the
-estimation depends on the fitted results. For example, a risk model transformed
-by model universe returns can derive the pairwise covariance and correlation
-for the model universe. ``` risk_model.transform(y=model_returns) cov =
-risk_model.cov() corr = risk_model.corr() ``` The following features will be
-supported in the near future - Covariance shrinkage - Covariance estimation
+risk models. ## Examples For end-to-end examples, please refer to [examples]
+(https://github.com/factorpricingmodel/factor-pricing-model-risk-model/tree/
+main/examples) for the below notebooks - [Cryptocurrency Statistical Risk
+Model](https://colab.research.google.com/github/factorpricingmodel/factor-
+pricing-model-risk-model/blob/main/examples/notebook/
+crypto_statistical_risk_model.ipynb) ## Features Basically, there are three
+major features provided in the library - Factor risk model creation -
+Covariance estimator - Tracking risk model accuracy ## Factor risk model The
+factor risk model is created by fitting instrument returns (which could be
+weekly, daily, or even higher granularity) and other related parameters into
+the model, and its products are factor exposures, factor returns, factor
+covariance, and residual returns (idiosyncratic returns). For example, to
+create a simple statistical PCA risk model, ``` from fpm_risk_model.statistics
+import PCA risk_model = PCA(n_components=5) risk_model.fit(X=returns) # Get
+fitted factor exposures risk_model.factor_exposures ``` Then, the risk model
+can be transformed by the returns of a larger homogeneous universe. ```
+risk_model.transform(y=model_returns) ``` For further details, please refer to
+the [section](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
+risk_model/factor_risk_model.html) in the documentation. ## Covariance
+estimation Currently, covariance estimation is supported in factor risk model,
+and the estimation depends on the fitted results. For example, a risk model
+transformed by model universe returns can derive the pairwise covariance and
+correlation for the model universe. ``` risk_model.transform(y=model_returns)
+cov = risk_model.cov() corr = risk_model.corr() ``` The following features will
+be supported in the near future - Covariance shrinkage - Covariance estimation
 from returns For further details, please refer to the [section](https://factor-
 pricing-model-risk-model.readthedocs.io/en/latest/risk_model/covariance.html)
 in the documentation. ## Tracking risk model accuracy The library also focuses
 on the predictability interpretation of the risk model, and provides a few
 benchmarks to examine the following metrics - [Bias](https://factor-pricing-
 model-risk-model.readthedocs.io/en/latest/accuracy/bias.html) - [Value at Risk
 (VaR)](https://factor-pricing-model-risk-model.readthedocs.io/en/latest/
```

