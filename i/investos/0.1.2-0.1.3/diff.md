# Comparing `tmp/investos-0.1.2.tar.gz` & `tmp/investos-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investos-0.1.2.tar", max compression
+gzip compressed data, was "investos-0.1.3.tar", max compression
```

## Comparing `investos-0.1.2.tar` & `investos-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.2/LICENSE
--rw-r--r--   0        0        0      806 2023-06-23 19:47:27.617845 investos-0.1.2/README.md
--rw-r--r--   0        0        0       48 2023-06-22 23:44:52.403440 investos-0.1.2/investos/__init__.py
--rw-r--r--   0        0        0      237 2023-06-22 23:46:12.605021 investos-0.1.2/investos/portfolio/__init__.py
--rw-r--r--   0        0        0      336 2023-06-22 23:46:19.538745 investos-0.1.2/investos/portfolio/constraint_model/__init__.py
--rw-r--r--   0        0        0      554 2023-06-23 07:08:21.486031 investos-0.1.2/investos/portfolio/constraint_model/base_constraint.py
--rw-r--r--   0        0        0     1377 2023-06-22 23:46:19.540939 investos-0.1.2/investos/portfolio/constraint_model/leverage_constraint.py
--rw-r--r--   0        0        0     2673 2023-06-22 23:46:19.542231 investos-0.1.2/investos/portfolio/constraint_model/long_constraint.py
--rw-r--r--   0        0        0     1366 2023-06-22 23:46:19.542979 investos-0.1.2/investos/portfolio/constraint_model/trade_constraint.py
--rw-r--r--   0        0        0     2400 2023-06-22 23:46:19.543696 investos-0.1.2/investos/portfolio/constraint_model/weight_constraint.py
--rw-r--r--   0        0        0    12997 2023-06-23 17:09:46.339230 investos-0.1.2/investos/portfolio/controller.py
--rw-r--r--   0        0        0      167 2023-06-22 23:46:24.228466 investos-0.1.2/investos/portfolio/cost_model/__init__.py
--rw-r--r--   0        0        0     1866 2023-06-23 07:07:49.043269 investos-0.1.2/investos/portfolio/cost_model/base_cost.py
--rw-r--r--   0        0        0     2151 2023-06-23 06:37:22.698101 investos-0.1.2/investos/portfolio/cost_model/holding_cost.py
--rw-r--r--   0        0        0     4085 2023-06-23 07:07:33.965063 investos-0.1.2/investos/portfolio/cost_model/trading_cost.py
--rw-r--r--   0        0        0       51 2023-06-23 07:06:43.880398 investos-0.1.2/investos/portfolio/result/__init__.py
--rw-r--r--   0        0        0     7515 2023-06-23 17:13:07.013409 investos-0.1.2/investos/portfolio/result/base_result.py
--rw-r--r--   0        0        0      297 2023-06-23 17:05:36.524816 investos-0.1.2/investos/portfolio/result/forecast_result.py
--rw-r--r--   0        0        0      116 2023-06-22 23:46:36.366559 investos-0.1.2/investos/portfolio/risk_model/__init__.py
--rw-r--r--   0        0        0     1314 2023-06-23 07:01:34.207139 investos-0.1.2/investos/portfolio/risk_model/base_risk.py
--rw-r--r--   0        0        0     2648 2023-06-23 07:00:56.552682 investos-0.1.2/investos/portfolio/risk_model/stat_factor_risk.py
--rw-r--r--   0        0        0      159 2023-06-22 23:46:41.515323 investos-0.1.2/investos/portfolio/strategy/__init__.py
--rw-r--r--   0        0        0     1278 2023-06-23 07:02:51.365518 investos-0.1.2/investos/portfolio/strategy/base_strategy.py
--rw-r--r--   0        0        0     3937 2023-06-23 07:03:19.040651 investos-0.1.2/investos/portfolio/strategy/rank_long_short.py
--rw-r--r--   0        0        0     3848 2023-06-23 07:04:39.977541 investos-0.1.2/investos/portfolio/strategy/spo.py
--rw-r--r--   0        0        0     1896 2023-06-22 23:44:52.404096 investos-0.1.2/investos/util.py
--rw-r--r--   0        0        0      726 2023-06-23 21:01:58.006505 investos-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1622 1970-01-01 00:00:00.000000 investos-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.3/LICENSE
+-rw-r--r--   0        0        0      806 2023-06-23 19:47:27.617845 investos-0.1.3/README.md
+-rw-r--r--   0        0        0       48 2023-06-22 23:44:52.403440 investos-0.1.3/investos/__init__.py
+-rw-r--r--   0        0        0      237 2023-06-22 23:46:12.605021 investos-0.1.3/investos/portfolio/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-22 23:46:19.538745 investos-0.1.3/investos/portfolio/constraint_model/__init__.py
+-rw-r--r--   0        0        0      554 2023-06-23 07:08:21.486031 investos-0.1.3/investos/portfolio/constraint_model/base_constraint.py
+-rw-r--r--   0        0        0     1377 2023-06-22 23:46:19.540939 investos-0.1.3/investos/portfolio/constraint_model/leverage_constraint.py
+-rw-r--r--   0        0        0     2673 2023-06-22 23:46:19.542231 investos-0.1.3/investos/portfolio/constraint_model/long_constraint.py
+-rw-r--r--   0        0        0     1366 2023-06-22 23:46:19.542979 investos-0.1.3/investos/portfolio/constraint_model/trade_constraint.py
+-rw-r--r--   0        0        0     2400 2023-06-22 23:46:19.543696 investos-0.1.3/investos/portfolio/constraint_model/weight_constraint.py
+-rw-r--r--   0        0        0    12997 2023-06-23 17:09:46.339230 investos-0.1.3/investos/portfolio/controller.py
+-rw-r--r--   0        0        0      167 2023-06-22 23:46:24.228466 investos-0.1.3/investos/portfolio/cost_model/__init__.py
+-rw-r--r--   0        0        0     1866 2023-06-23 07:07:49.043269 investos-0.1.3/investos/portfolio/cost_model/base_cost.py
+-rw-r--r--   0        0        0     2151 2023-06-23 06:37:22.698101 investos-0.1.3/investos/portfolio/cost_model/holding_cost.py
+-rw-r--r--   0        0        0     4085 2023-06-23 07:07:33.965063 investos-0.1.3/investos/portfolio/cost_model/trading_cost.py
+-rw-r--r--   0        0        0       51 2023-06-23 07:06:43.880398 investos-0.1.3/investos/portfolio/result/__init__.py
+-rw-r--r--   0        0        0     7515 2023-06-23 17:13:07.013409 investos-0.1.3/investos/portfolio/result/base_result.py
+-rw-r--r--   0        0        0      297 2023-06-23 17:05:36.524816 investos-0.1.3/investos/portfolio/result/forecast_result.py
+-rw-r--r--   0        0        0      116 2023-06-22 23:46:36.366559 investos-0.1.3/investos/portfolio/risk_model/__init__.py
+-rw-r--r--   0        0        0     1314 2023-06-23 07:01:34.207139 investos-0.1.3/investos/portfolio/risk_model/base_risk.py
+-rw-r--r--   0        0        0     2648 2023-06-23 07:00:56.552682 investos-0.1.3/investos/portfolio/risk_model/stat_factor_risk.py
+-rw-r--r--   0        0        0      159 2023-06-22 23:46:41.515323 investos-0.1.3/investos/portfolio/strategy/__init__.py
+-rw-r--r--   0        0        0     1278 2023-06-23 07:02:51.365518 investos-0.1.3/investos/portfolio/strategy/base_strategy.py
+-rw-r--r--   0        0        0     3937 2023-06-23 07:03:19.040651 investos-0.1.3/investos/portfolio/strategy/rank_long_short.py
+-rw-r--r--   0        0        0     3848 2023-06-23 07:04:39.977541 investos-0.1.3/investos/portfolio/strategy/spo.py
+-rw-r--r--   0        0        0     1896 2023-06-22 23:44:52.404096 investos-0.1.3/investos/util.py
+-rw-r--r--   0        0        0      726 2023-06-23 21:10:22.552461 investos-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1622 1970-01-01 00:00:00.000000 investos-0.1.3/PKG-INFO
```

### Comparing `investos-0.1.2/LICENSE` & `investos-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/README.md` & `investos-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/constraint_model/base_constraint.py` & `investos-0.1.3/investos/portfolio/constraint_model/base_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/constraint_model/leverage_constraint.py` & `investos-0.1.3/investos/portfolio/constraint_model/leverage_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/constraint_model/long_constraint.py` & `investos-0.1.3/investos/portfolio/constraint_model/long_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/constraint_model/trade_constraint.py` & `investos-0.1.3/investos/portfolio/constraint_model/trade_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/constraint_model/weight_constraint.py` & `investos-0.1.3/investos/portfolio/constraint_model/weight_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/controller.py` & `investos-0.1.3/investos/portfolio/controller.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/cost_model/base_cost.py` & `investos-0.1.3/investos/portfolio/cost_model/base_cost.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/cost_model/holding_cost.py` & `investos-0.1.3/investos/portfolio/cost_model/holding_cost.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/cost_model/trading_cost.py` & `investos-0.1.3/investos/portfolio/cost_model/trading_cost.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/result/base_result.py` & `investos-0.1.3/investos/portfolio/result/base_result.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/risk_model/base_risk.py` & `investos-0.1.3/investos/portfolio/risk_model/base_risk.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/risk_model/stat_factor_risk.py` & `investos-0.1.3/investos/portfolio/risk_model/stat_factor_risk.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/strategy/base_strategy.py` & `investos-0.1.3/investos/portfolio/strategy/base_strategy.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/strategy/rank_long_short.py` & `investos-0.1.3/investos/portfolio/strategy/rank_long_short.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/portfolio/strategy/spo.py` & `investos-0.1.3/investos/portfolio/strategy/spo.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/investos/util.py` & `investos-0.1.3/investos/util.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.2/pyproject.toml` & `investos-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investos"
-version = "0.1.2"
+version = "0.1.3"
 description = "For investors who want to focus on generating alpha"
 authors = ["Charlie Reese"]
 license = "Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-NC-SA)"
 readme = "README.md"
 packages = [{include = "investos"}]
 homepage = "https://investos.io/"
 repository = "https://github.com/charliereese/investos"
```

### Comparing `investos-0.1.2/PKG-INFO` & `investos-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investos
-Version: 0.1.2
+Version: 0.1.3
 Summary: For investors who want to focus on generating alpha
 Home-page: https://investos.io/
 License: Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-NC-SA)
 Author: Charlie Reese
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

