# Comparing `tmp/metlo-0.1.2.tar.gz` & `tmp/metlo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/akshay/code/metlo-enterprise/ingestors/python/dist/.tmp-62r3kicq/metlo-0.1.2.tar", last modified: Wed Jun 21 18:29:27 2023, max compression
+gzip compressed data, was "/Users/akshay/code/metlo-enterprise/ingestors/python/dist/.tmp-tjmjvnxw/metlo-0.1.3.tar", last modified: Thu Jun 22 22:40:23 2023, max compression
```

## Comparing `metlo-0.1.2.tar` & `metlo-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 18:29:27.000000 metlo-0.1.2/
--rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 18:29:27.000000 metlo-0.1.2/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)     1513 2022-10-31 23:50:46.000000 metlo-0.1.2/README.md
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo/
--rw-r--r--   0 akshay     (501) staff       (20)        0 2022-10-31 23:50:46.000000 metlo-0.1.2/metlo/__init__.py
--rw-r--r--   0 akshay     (501) staff       (20)     7795 2023-06-21 05:25:41.000000 metlo-0.1.2/metlo/django.py
--rw-r--r--   0 akshay     (501) staff       (20)    21704 2023-06-21 18:28:46.000000 metlo-0.1.2/metlo/fastapi.py
--rw-r--r--   0 akshay     (501) staff       (20)     7380 2023-06-21 05:25:41.000000 metlo-0.1.2/metlo/flask.py
--rw-r--r--   0 akshay     (501) staff       (20)      382 2023-06-21 05:25:41.000000 metlo-0.1.2/metlo/utils.py
-drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/
--rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/PKG-INFO
--rw-r--r--   0 akshay     (501) staff       (20)      259 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/SOURCES.txt
--rw-r--r--   0 akshay     (501) staff       (20)        1 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/dependency_links.txt
--rw-r--r--   0 akshay     (501) staff       (20)       42 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/requires.txt
--rw-r--r--   0 akshay     (501) staff       (20)        6 2023-06-21 18:29:27.000000 metlo-0.1.2/metlo.egg-info/top_level.txt
--rw-r--r--   0 akshay     (501) staff       (20)       80 2022-10-31 23:50:46.000000 metlo-0.1.2/pyproject.toml
--rw-r--r--   0 akshay     (501) staff       (20)     1175 2023-06-21 18:29:27.000000 metlo-0.1.2/setup.cfg
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-22 22:40:23.000000 metlo-0.1.3/
+-rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-22 22:40:23.000000 metlo-0.1.3/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)     1513 2022-10-31 23:50:46.000000 metlo-0.1.3/README.md
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo/
+-rw-r--r--   0 akshay     (501) staff       (20)        0 2022-10-31 23:50:46.000000 metlo-0.1.3/metlo/__init__.py
+-rw-r--r--   0 akshay     (501) staff       (20)     7795 2023-06-21 05:25:41.000000 metlo-0.1.3/metlo/django.py
+-rw-r--r--   0 akshay     (501) staff       (20)    22277 2023-06-22 22:39:55.000000 metlo-0.1.3/metlo/fastapi.py
+-rw-r--r--   0 akshay     (501) staff       (20)     7380 2023-06-21 05:25:41.000000 metlo-0.1.3/metlo/flask.py
+-rw-r--r--   0 akshay     (501) staff       (20)      382 2023-06-21 05:25:41.000000 metlo-0.1.3/metlo/utils.py
+drwxr-xr-x   0 akshay     (501) staff       (20)        0 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/
+-rw-r--r--   0 akshay     (501) staff       (20)     2604 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/PKG-INFO
+-rw-r--r--   0 akshay     (501) staff       (20)      259 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/SOURCES.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        1 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/dependency_links.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       42 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/requires.txt
+-rw-r--r--   0 akshay     (501) staff       (20)        6 2023-06-22 22:40:23.000000 metlo-0.1.3/metlo.egg-info/top_level.txt
+-rw-r--r--   0 akshay     (501) staff       (20)       80 2022-10-31 23:50:46.000000 metlo-0.1.3/pyproject.toml
+-rw-r--r--   0 akshay     (501) staff       (20)     1175 2023-06-22 22:40:23.000000 metlo-0.1.3/setup.cfg
```

### Comparing `metlo-0.1.2/PKG-INFO` & `metlo-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metlo
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Python Agent for Metlo
 Home-page: https://www.metlo.com
 License: MIT
 Project-URL: Documentation, https://docs.metlo.com/docs/python
 Project-URL: Source Code, https://github.com/metlo-labs/metlo/
 Project-URL: Issue Tracker, https://github.com/metlo-labs/metlo/issues/
 Project-URL: Twitter, https://mobile.twitter.com/metlohq
```

### Comparing `metlo-0.1.2/README.md` & `metlo-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `metlo-0.1.2/metlo/django.py` & `metlo-0.1.3/metlo/django.py`

 * *Files identical despite different names*

### Comparing `metlo-0.1.2/metlo/fastapi.py` & `metlo-0.1.3/metlo/fastapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,20 +71,35 @@
 def set_value_in_state(key: str, data: typing.Any, scope: Scope):
     scope["state"][get_key(key)] = data
 
 
 class ASGIMiddleware:
     def compile_request(self, scope: Scope):
         user = None
+        req_body = ""
         try:
             user = self.get_user(scope) if self.get_user is not None else None
         except Exception as e:
             self.logger.error("Error obtaining user info from function")
             self.logger.error(e)
             user = None
+        try:
+            req_body = (
+                get_value_from_state("req_body", scope)
+                if (
+                    check_key_in_state("req_body", scope)
+                    and isinstance(get_value_from_state("req_body", scope), bytes)
+                )
+                else b""
+            ).decode()
+        except Exception as e:
+            self.logger.debug("Error decoding request body")
+            self.logger.debug(e)
+            req_body = ""
+
         return {
             "url": {
                 "host": self.api_host
                 if self.api_host is not None
                 else f"{get_dest_ip(scope)}:{get_dest_port(scope)}",
                 "path": scope["path"],
                 "parameters": list(
@@ -108,22 +123,15 @@
                         for x in scope["headers"]
                         if isinstance(x[0], bytes) and isinstance(x[1], bytes)
                     ],
                 )
             )
             if ("headers" in scope and isinstance(scope["headers"], list))
             else [],
-            "body": (
-                get_value_from_state("req_body", scope)
-                if (
-                    check_key_in_state("req_body", scope)
-                    and isinstance(get_value_from_state("req_body", scope), bytes)
-                )
-                else b""
-            ).decode(),
+            "body": req_body,
             "method": scope["method"],
             "user": user,
         }
 
     def compile_meta(self, scope: Scope):
         return {
             "environment": "production",
@@ -132,62 +140,73 @@
             "sourcePort": get_src_port(scope),
             "destination": get_dest_ip(scope),
             "destinationPort": get_dest_port(scope),
             "metloSource": "python/fastapi",
         }
 
     def compile_response(self, scope: Scope):
-        res_body: str = get_value_from_state("res_body", scope, "")
+        res_body: str = ""
+        try:
+            res_body = (
+                get_value_from_state("res_body", scope, "")
+                if check_key_in_state("res_body", scope)
+                and isinstance(get_value_from_state("res_body", scope), bytes)
+                else b""
+            ).decode()
+        except Exception as e:
+            self.logger.debug("Error decoding response body")
+            self.logger.debug(e)
+            res_body = ""
         return {
             "status": get_value_from_state("status", scope, []),
             "headers": list(
                 map(
                     lambda x: {"name": x[0].decode(), "value": x[1].decode()},
                     [
                         x
                         for x in get_value_from_state("res_headers", scope, [])
                         if isinstance(x[0], bytes) and isinstance(x[1], bytes)
                     ],
                 )
             ),
-            "body": get_value_from_state("res_body", scope)
-            if check_key_in_state("res_body", scope)
-            and isinstance(get_value_from_state("res_body", scope), str)
-            else "",
+            "body": res_body,
         }
 
     def check_blocking(self, scope: Scope):
         try:
+            self.logger.debug("Checking for blocking")
             compiledRequest = self.compile_request(scope)
             compiledMeta = self.compile_meta(scope)
             will_reject = metlo_python_agent_bindings_common.block_trace(
                 json.dumps(compiledRequest), json.dumps(compiledMeta)
             )
-            self.logger.debug("Will be rejecting response from Metlo")
+            if will_reject:
+                self.logger.debug("Will be rejecting response from Metlo")
             return will_reject
         except Exception as e:
             self.logger.error(e)
             return False
 
     def process_trace(self, scope):
         try:
             compiledRequest = self.compile_request(scope)
             compiledMeta = self.compile_meta(scope)
             compiledResponse = self.compile_response(scope)
-            will_reject = metlo_python_agent_bindings_common.process_trace(
+            metlo_python_agent_bindings_common.process_trace(
                 json.dumps(
                     {
                         "request": compiledRequest,
                         "response": compiledResponse,
                         "meta": compiledMeta,
                     }
                 )
             )
             self.logger.debug("Sent trace")
         except Exception as e:
+            self.logger.error("Encountered an error while sending trace to Metlo")
             self.logger.error(e)
 
     async def process_rejection(self, scope, receive, send):
         try:
             if self.reject_response is not None:
                 return await self.reject_response(scope)(scope, receive, send)
             else:
@@ -380,15 +399,15 @@
                     # Check if we have stored req_body already
                     if check_key_in_state("req_body", scope):
                         # Get length of current body segment
                         curr_length = len(req["body"])
                         # How much can we store ?
                         remaining_buffer = max(self.max_body - curr_length, 0)
                         # We can store a non-zero amount
-                        if remaining_length > 0:
+                        if remaining_buffer > 0:
                             # How much can we put into the buffer:
                             # - either the full buffer
                             # - or, the remaining length
                             copy_length = min(remaining_buffer, len(req["body"]))
                             # Set the value for length
                             set_value_in_state(
                                 "req_len_stored",
@@ -467,15 +486,15 @@
                                     curr_length + copy_length,
                                     scope,
                                 )
                                 # Add decoded body to buffer
                                 set_value_in_state(
                                     "res_body",
                                     get_value_from_state("res_body", scope)
-                                    + message["body"].decode()[:copy_length],
+                                    + message["body"][:copy_length],
                                     scope,
                                 )
                             else:
                                 # Buffer is full, do nothing
                                 pass
                         # We haven't recorded any part of the body yet.
                         else:
@@ -485,15 +504,15 @@
                                 min(len(message["body"]), self.max_body),
                                 scope,
                             )
 
                             # We want decoded bodies only
                             set_value_in_state(
                                 "res_body",
-                                message["body"].decode()[: self.max_body],
+                                message["body"][: self.max_body],
                                 scope,
                             )
 
                     else:
                         # Somehow body is missing from message of type 'http.response.body'
                         set_value_in_state(
                             "res_len_stored",
```

### Comparing `metlo-0.1.2/metlo/flask.py` & `metlo-0.1.3/metlo/flask.py`

 * *Files identical despite different names*

### Comparing `metlo-0.1.2/metlo.egg-info/PKG-INFO` & `metlo-0.1.3/metlo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metlo
-Version: 0.1.2
+Version: 0.1.3
 Summary: The Python Agent for Metlo
 Home-page: https://www.metlo.com
 License: MIT
 Project-URL: Documentation, https://docs.metlo.com/docs/python
 Project-URL: Source Code, https://github.com/metlo-labs/metlo/
 Project-URL: Issue Tracker, https://github.com/metlo-labs/metlo/issues/
 Project-URL: Twitter, https://mobile.twitter.com/metlohq
```

### Comparing `metlo-0.1.2/setup.cfg` & `metlo-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = metlo
-version = 0.1.2
+version = 0.1.3
 description = The Python Agent for Metlo
 long_description = file: README.md
 long_description_content_type = text/markdown
 repository = https://github.com/metlo-labs/metlo
 url = https://www.metlo.com
 license = MIT
 project_urls =
```

