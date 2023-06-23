# Comparing `tmp/kolo-2.9.3.tar.gz` & `tmp/kolo-2.9.4.tar.gz`

## Comparing `kolo-2.9.3.tar` & `kolo-2.9.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 kolo-2.9.3/rust/Cargo.toml
--rw-rw-r--   0     1000     1001       54 2023-05-29 08:14:53.000000 kolo-2.9.3/rust/build.rs
--rw-rw-r--   0     1000     1001    35207 2023-05-29 08:14:53.000000 kolo-2.9.3/rust/src/lib.rs
--rw-rw-r--   0     1000     1001     2176 2023-05-29 08:14:53.000000 kolo-2.9.3/pyproject.toml
--rw-rw-r--   0     1000     1001    11199 2023-05-29 08:15:59.000000 kolo-2.9.3/rust/Cargo.lock
--rw-rw-r--   0     1000     1001     2677 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/django_schema.py
--rw-rw-r--   0     1000     1001     3798 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/serialize.py
--rw-rw-r--   0     1000     1001     3400 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/requests.py
--rw-rw-r--   0     1000     1001      348 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/kolo.py
--rw-rw-r--   0     1000     1001     1322 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/unittest.py
--rw-rw-r--   0     1000     1001     4448 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/exception.py
--rw-rw-r--   0     1000     1001     1457 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/pytest.py
--rw-rw-r--   0     1000     1001     4345 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/sql.py
--rw-rw-r--   0     1000     1001     2262 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/celery.py
--rw-rw-r--   0     1000     1001     3157 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/urllib.py
--rw-rw-r--   0     1000     1001     4141 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/django.py
--rw-rw-r--   0     1000     1001     1778 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/logging.py
--rw-rw-r--   0     1000     1001     5180 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/core.py
--rw-rw-r--   0     1000     1001      809 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/attrs.py
--rw-rw-r--   0     1000     1001     3707 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/urllib3.py
--rw-rw-r--   0     1000     1001      141 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/pypy.py
--rw-rw-r--   0     1000     1001        0 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/__init__.py
--rw-rw-r--   0     1000     1001     2921 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/huey.py
--rw-rw-r--   0     1000     1001     2640 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/middleware.py
--rw-rw-r--   0     1000     1001     1936 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/templates/django_request_test.py.j2
--rw-rw-r--   0     1000     1001    13710 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/profiler.py
--rw-rw-r--   0     1000     1001      169 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/version.py
--rw-rw-r--   0     1000     1001    32582 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/generate_tests.py
--rw-rw-r--   0     1000     1001      360 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/utils.py
--rw-rw-r--   0     1000     1001    11995 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/__main__.py
--rw-rw-r--   0     1000     1001     5542 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/db.py
--rw-rw-r--   0     1000     1001      473 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/git.py
--rw-rw-r--   0     1000     1001      228 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/pytest_plugin.py
--rw-rw-r--   0     1000     1001      108 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/__init__.py
--rw-rw-r--   0     1000     1001     2881 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/config.py
--rw-rw-r--   0     1000     1001      228 2023-05-29 08:14:53.000000 kolo-2.9.3/README.md
--rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 kolo-2.9.3/PKG-INFO
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 kolo-2.9.4/rust/Cargo.toml
+-rw-rw-r--   0     1000     1001       54 2023-05-29 14:34:06.000000 kolo-2.9.4/rust/build.rs
+-rw-rw-r--   0     1000     1001    35207 2023-05-29 14:34:06.000000 kolo-2.9.4/rust/src/lib.rs
+-rw-rw-r--   0     1000     1001     2176 2023-05-29 14:34:06.000000 kolo-2.9.4/pyproject.toml
+-rw-rw-r--   0     1000     1001    11199 2023-05-29 14:35:15.000000 kolo-2.9.4/rust/Cargo.lock
+-rw-rw-r--   0     1000     1001     2677 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/django_schema.py
+-rw-rw-r--   0     1000     1001     3798 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/serialize.py
+-rw-rw-r--   0     1000     1001     3400 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/requests.py
+-rw-rw-r--   0     1000     1001      348 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/kolo.py
+-rw-rw-r--   0     1000     1001     1322 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/unittest.py
+-rw-rw-r--   0     1000     1001     4448 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/exception.py
+-rw-rw-r--   0     1000     1001     1457 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/pytest.py
+-rw-rw-r--   0     1000     1001     4345 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/sql.py
+-rw-rw-r--   0     1000     1001     2262 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/celery.py
+-rw-rw-r--   0     1000     1001     3157 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/urllib.py
+-rw-rw-r--   0     1000     1001     4141 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/django.py
+-rw-rw-r--   0     1000     1001     1778 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/logging.py
+-rw-rw-r--   0     1000     1001     5180 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/core.py
+-rw-rw-r--   0     1000     1001      809 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/attrs.py
+-rw-rw-r--   0     1000     1001     3707 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/urllib3.py
+-rw-rw-r--   0     1000     1001      141 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/pypy.py
+-rw-rw-r--   0     1000     1001        0 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/__init__.py
+-rw-rw-r--   0     1000     1001     2921 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/filters/huey.py
+-rw-rw-r--   0     1000     1001     2640 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/middleware.py
+-rw-rw-r--   0     1000     1001     1936 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/templates/django_request_test.py.j2
+-rw-rw-r--   0     1000     1001    13710 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/profiler.py
+-rw-rw-r--   0     1000     1001      169 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/version.py
+-rw-rw-r--   0     1000     1001    33149 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/generate_tests.py
+-rw-rw-r--   0     1000     1001      360 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/utils.py
+-rw-rw-r--   0     1000     1001    11995 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/__main__.py
+-rw-rw-r--   0     1000     1001     5542 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/db.py
+-rw-rw-r--   0     1000     1001      473 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/git.py
+-rw-rw-r--   0     1000     1001      228 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/pytest_plugin.py
+-rw-rw-r--   0     1000     1001      108 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/__init__.py
+-rw-rw-r--   0     1000     1001     2881 2023-05-29 14:34:06.000000 kolo-2.9.4/src/kolo/config.py
+-rw-rw-r--   0     1000     1001      228 2023-05-29 14:34:06.000000 kolo-2.9.4/README.md
+-rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 kolo-2.9.4/PKG-INFO
```

### Comparing `kolo-2.9.3/rust/src/lib.rs` & `kolo-2.9.4/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/pyproject.toml` & `kolo-2.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "kolo"
-version = "2.9.3"
+version = "2.9.4"
 description = "See everything happening in your running Django app"
 readme = "README.md"
 authors = [
     {name = "Wilhelm Klopp", email = "team@kolo.app"},
     {name = "Lily Foote", email = "lily@kolo.app"},
 ]
 urls.Homepage = "https://kolo.app"
```

### Comparing `kolo-2.9.3/rust/Cargo.lock` & `kolo-2.9.4/rust/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -112,17 +112,17 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
```

### Comparing `kolo-2.9.3/src/kolo/django_schema.py` & `kolo-2.9.4/src/kolo/django_schema.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/serialize.py` & `kolo-2.9.4/src/kolo/serialize.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/requests.py` & `kolo-2.9.4/src/kolo/filters/requests.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/unittest.py` & `kolo-2.9.4/src/kolo/filters/unittest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/exception.py` & `kolo-2.9.4/src/kolo/filters/exception.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/pytest.py` & `kolo-2.9.4/src/kolo/filters/pytest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/sql.py` & `kolo-2.9.4/src/kolo/filters/sql.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/celery.py` & `kolo-2.9.4/src/kolo/filters/celery.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/urllib.py` & `kolo-2.9.4/src/kolo/filters/urllib.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/django.py` & `kolo-2.9.4/src/kolo/filters/django.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/logging.py` & `kolo-2.9.4/src/kolo/filters/logging.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/core.py` & `kolo-2.9.4/src/kolo/filters/core.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/attrs.py` & `kolo-2.9.4/src/kolo/filters/attrs.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/urllib3.py` & `kolo-2.9.4/src/kolo/filters/urllib3.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/filters/huey.py` & `kolo-2.9.4/src/kolo/filters/huey.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/middleware.py` & `kolo-2.9.4/src/kolo/middleware.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/templates/django_request_test.py.j2` & `kolo-2.9.4/src/kolo/templates/django_request_test.py.j2`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/profiler.py` & `kolo-2.9.4/src/kolo/profiler.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/generate_tests.py` & `kolo-2.9.4/src/kolo/generate_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             duration_match = TIMEDELTA_STR_REGEX.match(value)
             if timedelta_match:  # pragma: no branch
                 groups = [int(g) if g else 0 for g in timedelta_match.groups()]
                 value = timedelta(
                     days=groups[0], seconds=groups[1], microseconds=groups[2]
                 )
             elif duration_match:
-                groups = duration_match.groups()
+                groups = duration_match.groups()  # type: ignore
                 value = timedelta(
                     days=int(groups[0]),
                     seconds=int(groups[1]),
                     microseconds=int(groups[2]),
                 )
         else:
             value = timedelta(microseconds=value)
@@ -288,15 +288,15 @@
                     ):
                         continue
             if field.schema["is_relation"]:
                 related_model = field.schema["related_model"]
                 verbose_name = schema[related_model]["verbose_name"]
                 related_pk = field.schema["related_pk"]
                 try:
-                    field.value = names.names[
+                    field.value_repr = field.value = names.names[
                         (verbose_name, related_pk, field.value_repr)
                     ]
                 except KeyError:
                     field.name = field.schema["field_attname"]
             fields.append(field)
         self.values = tuple(fields)
 
@@ -357,15 +357,15 @@
                 continue
 
             if field.schema["is_relation"]:
                 related_model = field.schema["related_model"]
                 verbose_name = schema[related_model]["verbose_name"]
                 related_pk = field.schema["related_pk"]
                 try:
-                    field.value = names.names[
+                    field.value_repr = field.value = names.names[
                         (verbose_name, related_pk, field.value_repr)
                     ]
                 except KeyError:  # pragma: no cover
                     pass
                 else:
                     field.name = field.schema["field_name"]
             fields.append(field)
@@ -416,21 +416,23 @@
     def update_fields(self, names, schema):
         fields = []
         for field in self.fields:
             if field.schema["primary_key"]:
                 continue  # pragma: no cover
             if field.schema["django_field"] == "django.db.models.fields.DateTimeField":
                 continue  # pragma: no cover
+            if field.schema["django_field"] == "django.db.models.fields.json.JSONField":
+                continue  # pragma: no cover
 
             if field.schema["is_relation"]:
                 related_model = field.schema["related_model"]
                 verbose_name = schema[related_model]["verbose_name"]
                 related_pk = field.schema["related_pk"]
                 try:
-                    field.value = names.names[
+                    field.value_repr = field.value = names.names[
                         (verbose_name, related_pk, field.value_repr)
                     ]
                 except KeyError:  # pragma: no cover
                     pass
                 else:
                     field.name = field.schema["field_name"]
             fields.append(field)
@@ -729,15 +731,15 @@
         "HTTP_ACCEPT_LANGUAGE",
         "HTTP_SEC_FETCH_SITE",
         "HTTP_SEC_FETCH_MODE",
         "HTTP_SEC_FETCH_USER",
         "HTTP_SEC_FETCH_DEST",
         "HTTP_SEC_CH_UA_PLATFORM",
         "HTTP_ORIGIN",
-        "HTTP_UPGRADE_INSECURE_REQUESTS"
+        "HTTP_UPGRADE_INSECURE_REQUESTS",
     ]
 
     for request_header in request_headers_to_delete:
         if request_header in request_headers:
             del request_headers[request_header]
 
     if "CONTENT_TYPE" in request_headers:
@@ -816,16 +818,26 @@
             assert current_outbound_request is None
             current_outbound_request = {"request": frame}
         elif frame["type"] == "outbound_http_response":
             if frame["subtype"] == "urllib3":
                 continue
             assert current_outbound_request is not None
             current_outbound_request["response"] = frame
-            if current_outbound_request["response"]["body"] and current_outbound_request["response"]["headers"].get("Content-Type") == "application/json":
-                current_outbound_request["response"]["json_body"] = json.loads(current_outbound_request["response"]["body"])
+
+            content_type = (
+                current_outbound_request["response"]["headers"].get("Content-Type")
+                or current_outbound_request["response"]["headers"].get("content-type")
+                or current_outbound_request["response"]["headers"].get("CONTENT-TYPE")
+            )
+            content_type_is_json = content_type and "application/json" in content_type
+            if current_outbound_request["response"]["body"] and content_type_is_json:
+                current_outbound_request["response"]["json_body"] = json.loads(
+                    current_outbound_request["response"]["body"]
+                )
+
             outbound_request_frames.append(current_outbound_request)
 
             current_outbound_request = None
         elif frame["type"] == "end_sql_query":
             sql_queries.append(frame)
 
     if sql_queries:
```

### Comparing `kolo-2.9.3/src/kolo/__main__.py` & `kolo-2.9.4/src/kolo/__main__.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/db.py` & `kolo-2.9.4/src/kolo/db.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/src/kolo/config.py` & `kolo-2.9.4/src/kolo/config.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.3/PKG-INFO` & `kolo-2.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolo
-Version: 2.9.3
+Version: 2.9.4
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

