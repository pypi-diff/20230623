# Comparing `tmp/tum_esm_signal-0.2.0.tar.gz` & `tmp/tum_esm_signal-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tum_esm_signal-0.2.0.tar", max compression
+gzip compressed data, was "tum_esm_signal-0.3.0.tar", max compression
```

## Comparing `tum_esm_signal-0.2.0.tar` & `tum_esm_signal-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      895 2023-06-22 13:54:18.385635 tum_esm_signal-0.2.0/README.md
--rw-r--r--   0        0        0      940 2023-06-22 13:52:37.286848 tum_esm_signal-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       85 2023-06-22 10:42:21.174903 tum_esm_signal-0.2.0/tum_esm_signal/__init__.py
--rw-r--r--   0        0        0     2216 2023-06-22 13:51:51.585601 tum_esm_signal-0.2.0/tum_esm_signal/client.py
--rw-r--r--   0        0        0     3872 2023-06-22 11:33:36.395624 tum_esm_signal-0.2.0/tum_esm_signal/pocketbase.py
--rw-r--r--   0        0        0        0 2023-06-22 11:37:33.577931 tum_esm_signal-0.2.0/tum_esm_signal/py.typed
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 tum_esm_signal-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      895 2023-06-22 13:54:18.385635 tum_esm_signal-0.3.0/README.md
+-rw-r--r--   0        0        0      940 2023-06-22 23:00:08.540686 tum_esm_signal-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       85 2023-06-22 10:42:21.174903 tum_esm_signal-0.3.0/tum_esm_signal/__init__.py
+-rw-r--r--   0        0        0     2154 2023-06-22 22:57:26.825569 tum_esm_signal-0.3.0/tum_esm_signal/client.py
+-rw-r--r--   0        0        0     3872 2023-06-22 11:33:36.395624 tum_esm_signal-0.3.0/tum_esm_signal/pocketbase.py
+-rw-r--r--   0        0        0        0 2023-06-22 11:37:33.577931 tum_esm_signal-0.3.0/tum_esm_signal/py.typed
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 tum_esm_signal-0.3.0/PKG-INFO
```

### Comparing `tum_esm_signal-0.2.0/README.md` & `tum_esm_signal-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tum_esm_signal-0.2.0/pyproject.toml` & `tum_esm_signal-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tum_esm_signal"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Moritz Makowski <moritz@dostuffthatmatters.dev>"]
 readme = "README.md"
 packages = [
     {include = "tum_esm_signal"},
     {include = "tum_esm_signal/py.typed"}
 ]
```

### Comparing `tum_esm_signal-0.2.0/tum_esm_signal/client.py` & `tum_esm_signal-0.3.0/tum_esm_signal/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 class TUM_ESM_SignalClient:
     def __init__(
         self,
         cms_identity: str,
         cms_password: str,
         collection_name: str,
         table_name: str,
-        sensor_id: str,
     ) -> None:
         self.pocketbase = tum_esm_signal.PocketBaseInterface(cms_identity, cms_password)
         self.collection_name = collection_name
         self.table_name = table_name
-        self.sensor_id = sensor_id
 
     def connect_column(
         self,
         column_name: str,
         unit: str,
         minimum: float,
         maximum: float,
@@ -61,21 +59,21 @@
             unit,
             description,
             minimum,
             maximum,
             decimal_places,
         )
 
-    def add_datapoint(self, value: float) -> None:
+    def add_datapoint(self, sensor_id: str, value: float) -> None:
         """Add a datapoint to the selected column. The record time
         is set to the current time."""
 
         # looks like "2021-01-01T00:00:00.000Z"
         datetime_str = pendulum.now("UTC").to_iso8601_string()  # type: ignore
         assert isinstance(datetime_str, str)
 
         self.signal_client.pocketbase.create_data_record(
             self.column_id,
-            self.signal_client.sensor_id,
+            sensor_id,
             value,
             datetime_str,
         )
```

### Comparing `tum_esm_signal-0.2.0/tum_esm_signal/pocketbase.py` & `tum_esm_signal-0.3.0/tum_esm_signal/pocketbase.py`

 * *Files identical despite different names*

### Comparing `tum_esm_signal-0.2.0/PKG-INFO` & `tum_esm_signal-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tum-esm-signal
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Home-page: https://github.com/tum-esm/signal
 License: AGPL-3.0-only
 Keywords: python,library,utilities,plotting
 Author: Moritz Makowski
 Author-email: moritz@dostuffthatmatters.dev
 Requires-Python: >=3.9,<4.0
```

