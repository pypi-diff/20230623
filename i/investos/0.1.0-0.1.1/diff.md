# Comparing `tmp/investos-0.1.0.tar.gz` & `tmp/investos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investos-0.1.0.tar", max compression
+gzip compressed data, was "investos-0.1.1.tar", max compression
```

## Comparing `investos-0.1.0.tar` & `investos-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,28 @@
--rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.0/LICENSE
--rw-r--r--   0        0        0      741 2023-05-10 23:16:30.261531 investos-0.1.0/README.md
--rw-r--r--   0        0        0       66 2023-06-08 15:11:33.560913 investos-0.1.0/investos/__init__.py
--rw-r--r--   0        0        0      575 2023-06-05 23:07:34.242226 investos-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 investos-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.1/LICENSE
+-rw-r--r--   0        0        0      741 2023-05-10 23:16:30.261531 investos-0.1.1/README.md
+-rw-r--r--   0        0        0       48 2023-06-22 23:44:52.403440 investos-0.1.1/investos/__init__.py
+-rw-r--r--   0        0        0      237 2023-06-22 23:46:12.605021 investos-0.1.1/investos/portfolio/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-22 23:46:19.538745 investos-0.1.1/investos/portfolio/constraint_model/__init__.py
+-rw-r--r--   0        0        0      554 2023-06-23 07:08:21.486031 investos-0.1.1/investos/portfolio/constraint_model/base_constraint.py
+-rw-r--r--   0        0        0     1377 2023-06-22 23:46:19.540939 investos-0.1.1/investos/portfolio/constraint_model/leverage_constraint.py
+-rw-r--r--   0        0        0     2673 2023-06-22 23:46:19.542231 investos-0.1.1/investos/portfolio/constraint_model/long_constraint.py
+-rw-r--r--   0        0        0     1366 2023-06-22 23:46:19.542979 investos-0.1.1/investos/portfolio/constraint_model/trade_constraint.py
+-rw-r--r--   0        0        0     2400 2023-06-22 23:46:19.543696 investos-0.1.1/investos/portfolio/constraint_model/weight_constraint.py
+-rw-r--r--   0        0        0    12997 2023-06-23 17:09:46.339230 investos-0.1.1/investos/portfolio/controller.py
+-rw-r--r--   0        0        0      167 2023-06-22 23:46:24.228466 investos-0.1.1/investos/portfolio/cost_model/__init__.py
+-rw-r--r--   0        0        0     1866 2023-06-23 07:07:49.043269 investos-0.1.1/investos/portfolio/cost_model/base_cost.py
+-rw-r--r--   0        0        0     2151 2023-06-23 06:37:22.698101 investos-0.1.1/investos/portfolio/cost_model/holding_cost.py
+-rw-r--r--   0        0        0     4085 2023-06-23 07:07:33.965063 investos-0.1.1/investos/portfolio/cost_model/trading_cost.py
+-rw-r--r--   0        0        0       51 2023-06-23 07:06:43.880398 investos-0.1.1/investos/portfolio/result/__init__.py
+-rw-r--r--   0        0        0     7515 2023-06-23 17:13:07.013409 investos-0.1.1/investos/portfolio/result/base_result.py
+-rw-r--r--   0        0        0      297 2023-06-23 17:05:36.524816 investos-0.1.1/investos/portfolio/result/forecast_result.py
+-rw-r--r--   0        0        0      116 2023-06-22 23:46:36.366559 investos-0.1.1/investos/portfolio/risk_model/__init__.py
+-rw-r--r--   0        0        0     1314 2023-06-23 07:01:34.207139 investos-0.1.1/investos/portfolio/risk_model/base_risk.py
+-rw-r--r--   0        0        0     2648 2023-06-23 07:00:56.552682 investos-0.1.1/investos/portfolio/risk_model/stat_factor_risk.py
+-rw-r--r--   0        0        0      159 2023-06-22 23:46:41.515323 investos-0.1.1/investos/portfolio/strategy/__init__.py
+-rw-r--r--   0        0        0     1278 2023-06-23 07:02:51.365518 investos-0.1.1/investos/portfolio/strategy/base_strategy.py
+-rw-r--r--   0        0        0     3937 2023-06-23 07:03:19.040651 investos-0.1.1/investos/portfolio/strategy/rank_long_short.py
+-rw-r--r--   0        0        0     3848 2023-06-23 07:04:39.977541 investos-0.1.1/investos/portfolio/strategy/spo.py
+-rw-r--r--   0        0        0     1896 2023-06-22 23:44:52.404096 investos-0.1.1/investos/util.py
+-rw-r--r--   0        0        0      575 2023-06-23 17:17:38.798588 investos-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 investos-0.1.1/PKG-INFO
```

### Comparing `investos-0.1.0/LICENSE` & `investos-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `investos-0.1.0/README.md` & `investos-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `investos-0.1.0/pyproject.toml` & `investos-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investos"
-version = "0.1.0"
+version = "0.1.1"
 description = "For investors who want to focus on generating alpha"
 authors = ["Charlie Reese"]
 license = "Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-NC-SA)"
 readme = "README.md"
 packages = [{include = "investos"}]
 
 [tool.poetry.dependencies]
```

### Comparing `investos-0.1.0/PKG-INFO` & `investos-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investos
-Version: 0.1.0
+Version: 0.1.1
 Summary: For investors who want to focus on generating alpha
 License: Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-NC-SA)
 Author: Charlie Reese
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

