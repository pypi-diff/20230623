# Comparing `tmp/gopay-2.0.0.tar.gz` & `tmp/gopay-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gopay-2.0.0.tar", max compression
+gzip compressed data, was "gopay-2.0.1.tar", max compression
```

## Comparing `gopay-2.0.0.tar` & `gopay-2.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1075 2023-06-05 14:15:56.541156 gopay-2.0.0/LICENSE
--rw-r--r--   0        0        0     9214 2023-06-07 17:46:47.082495 gopay-2.0.0/README.md
--rw-r--r--   0        0        0     1074 2023-06-07 19:27:48.972875 gopay-2.0.0/gopay/__init__.py
--rw-r--r--   0        0        0     2078 2023-06-07 19:43:18.722194 gopay-2.0.0/gopay/api.py
--rw-r--r--   0        0        0     6017 2023-06-07 15:59:32.469096 gopay-2.0.0/gopay/enums.py
--rw-r--r--   0        0        0     4707 2023-06-07 19:48:11.894502 gopay-2.0.0/gopay/http.py
--rw-r--r--   0        0        0      421 2023-06-07 19:18:42.537102 gopay-2.0.0/gopay/models.py
--rw-r--r--   0        0        0     4797 2023-06-07 19:37:46.464213 gopay-2.0.0/gopay/payments.py
--rw-r--r--   0        0        0     1612 2023-06-07 19:50:57.714267 gopay-2.0.0/gopay/services.py
--rw-r--r--   0        0        0     1145 2023-06-07 19:18:36.705128 gopay-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    10225 1970-01-01 00:00:00.000000 gopay-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-05 14:15:56.541156 gopay-2.0.1/LICENSE
+-rw-r--r--   0        0        0     9214 2023-06-12 15:23:08.929350 gopay-2.0.1/README.md
+-rw-r--r--   0        0        0     1074 2023-06-12 15:23:08.933350 gopay-2.0.1/gopay/__init__.py
+-rw-r--r--   0        0        0     2078 2023-06-12 15:23:08.933350 gopay-2.0.1/gopay/api.py
+-rw-r--r--   0        0        0     6017 2023-06-12 15:23:08.937350 gopay-2.0.1/gopay/enums.py
+-rw-r--r--   0        0        0     4707 2023-06-12 15:23:08.937350 gopay-2.0.1/gopay/http.py
+-rw-r--r--   0        0        0      421 2023-06-12 15:23:08.937350 gopay-2.0.1/gopay/models.py
+-rw-r--r--   0        0        0     4798 2023-06-23 12:26:58.731520 gopay-2.0.1/gopay/payments.py
+-rw-r--r--   0        0        0     1612 2023-06-12 15:23:08.941350 gopay-2.0.1/gopay/services.py
+-rw-r--r--   0        0        0     1145 2023-06-23 12:32:03.847043 gopay-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10225 1970-01-01 00:00:00.000000 gopay-2.0.1/PKG-INFO
```

### Comparing `gopay-2.0.0/LICENSE` & `gopay-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gopay-2.0.0/README.md` & `gopay-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gopay-2.0.0/gopay/__init__.py` & `gopay-2.0.1/gopay/__init__.py`

 * *Files identical despite different names*

### Comparing `gopay-2.0.0/gopay/api.py` & `gopay-2.0.1/gopay/api.py`

 * *Files identical despite different names*

### Comparing `gopay-2.0.0/gopay/enums.py` & `gopay-2.0.1/gopay/enums.py`

 * *Files identical despite different names*

### Comparing `gopay-2.0.0/gopay/http.py` & `gopay-2.0.1/gopay/http.py`

 * *Files identical despite different names*

### Comparing `gopay-2.0.0/gopay/payments.py` & `gopay-2.0.1/gopay/payments.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,8 +138,8 @@
         return self.gopay.call("GET", f"/payments/payment/{payment_id}/eet-receipts")
 
     def find_eet_receipts_by_filter(self, filter: dict) -> Response:
         return self.gopay.call("POST", "/eet-receipts", ContentType.JSON, filter)
 
     @property
     def get_embedjs_url(self) -> str:
-        return self.gopay.base_url[-4] + "/gp-gw/js/embed.js"
+        return self.gopay.base_url[:-4] + "/gp-gw/js/embed.js"
```

### Comparing `gopay-2.0.0/gopay/services.py` & `gopay-2.0.1/gopay/services.py`

 * *Files identical despite different names*

### Comparing `gopay-2.0.0/pyproject.toml` & `gopay-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 homepage = "https://github.com/gopaycommunity/gopay-python-api"
 keywords = ["gopay", "payments", "sdk", "rest", "api"]
 license = "MIT"
 name = "gopay"
 packages = [{include = "gopay"}]
 readme = "README.md"
 repository = "https://github.com/gopaycommunity/gopay-python-api"
-version = "2.0.0"
+version = "2.0.1"
 
 [tool.poetry.dependencies]
 deprecated = "^1.2.14"
 pydantic = "^1.10.8"
 python = "^3.8.1"
 requests = "^2.31.0"
```

### Comparing `gopay-2.0.0/PKG-INFO` & `gopay-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopay
-Version: 2.0.0
+Version: 2.0.1
 Summary: GoPay's Python SDK for Payments REST API
 Home-page: https://github.com/gopaycommunity/gopay-python-api
 License: MIT
 Keywords: gopay,payments,sdk,rest,api
 Author: GoPay
 Author-email: integrace@gopay.cz
 Requires-Python: >=3.8.1,<4.0.0
```

