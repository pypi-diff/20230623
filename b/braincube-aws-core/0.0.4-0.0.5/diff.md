# Comparing `tmp/braincube-aws-core-0.0.4.tar.gz` & `tmp/braincube-aws-core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-0.0.4.tar", last modified: Thu Jun 22 15:42:49 2023, max compression
+gzip compressed data, was "braincube-aws-core-0.0.5.tar", last modified: Fri Jun 23 09:50:12 2023, max compression
```

## Comparing `braincube-aws-core-0.0.4.tar` & `braincube-aws-core-0.0.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.717499 braincube-aws-core-0.0.4/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-22 15:42:49.717668 braincube-aws-core-0.0.4/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8009 2023-06-21 20:23:04.000000 braincube-aws-core-0.0.4/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-22 15:42:49.718745 braincube-aws-core-0.0.4/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.698155 braincube-aws-core-0.0.4/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.703203 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-22 15:42:49.000000 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      897 2023-06-22 15:42:49.000000 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-22 15:42:49.000000 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-22 15:42:49.000000 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-22 15:42:49.000000 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.703497 braincube-aws-core-0.0.4/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.707766 braincube-aws-core-0.0.4/src/core/app/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/app/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-0.0.4/src/core/app/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      664 2023-06-21 16:34:05.000000 braincube-aws-core-0.0.4/src/core/app/app_event.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     6203 2023-06-21 20:01:55.000000 braincube-aws-core-0.0.4/src/core/app/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4665 2023-06-22 09:23:59.000000 braincube-aws-core-0.0.4/src/core/app/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      479 2023-06-21 17:15:33.000000 braincube-aws-core-0.0.4/src/core/app/exception_handler.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.711060 braincube-aws-core-0.0.4/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.4/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.4/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.4/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    33246 2023-06-22 15:26:24.000000 braincube-aws-core-0.0.4/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.713222 braincube-aws-core-0.0.4/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.4/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.4/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.715371 braincube-aws-core-0.0.4/src/core/rules_engine/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/rules_engine/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.4/src/core/rules_engine/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.4/src/core/rules_engine/exceptions.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.4/src/core/rules_engine/rule_manager.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.716879 braincube-aws-core-0.0.4/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.4/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.4/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.851637 braincube-aws-core-0.0.5/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-23 09:50:12.851879 braincube-aws-core-0.0.5/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8009 2023-06-21 20:23:04.000000 braincube-aws-core-0.0.5/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-23 09:50:12.853186 braincube-aws-core-0.0.5/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.833845 braincube-aws-core-0.0.5/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.839420 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-23 09:50:12.000000 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      897 2023-06-23 09:50:12.000000 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-23 09:50:12.000000 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-23 09:50:12.000000 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-23 09:50:12.000000 braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.840020 braincube-aws-core-0.0.5/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.843306 braincube-aws-core-0.0.5/src/core/app/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/app/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-0.0.5/src/core/app/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      664 2023-06-21 16:34:05.000000 braincube-aws-core-0.0.5/src/core/app/app_event.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6598 2023-06-23 09:47:26.000000 braincube-aws-core-0.0.5/src/core/app/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4665 2023-06-22 09:23:59.000000 braincube-aws-core-0.0.5/src/core/app/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      479 2023-06-21 17:15:33.000000 braincube-aws-core-0.0.5/src/core/app/exception_handler.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.846017 braincube-aws-core-0.0.5/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.5/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.5/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.5/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    33246 2023-06-22 15:26:24.000000 braincube-aws-core-0.0.5/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.847782 braincube-aws-core-0.0.5/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.5/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.5/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.849763 braincube-aws-core-0.0.5/src/core/rules_engine/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/rules_engine/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.5/src/core/rules_engine/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.5/src/core/rules_engine/exceptions.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.5/src/core/rules_engine/rule_manager.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-23 09:50:12.851263 braincube-aws-core-0.0.5/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.5/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.5/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.5/src/core/utils/data.py
```

### Comparing `braincube-aws-core-0.0.4/LICENSE` & `braincube-aws-core-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/PKG-INFO` & `braincube-aws-core-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-0.0.4/README.md` & `braincube-aws-core-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/setup.cfg` & `braincube-aws-core-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core
-version = 0.0.4
+version = 0.0.5
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/PKG-INFO` & `braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/SOURCES.txt` & `braincube-aws-core-0.0.5/src/braincube_aws_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/app/app_controller.py` & `braincube-aws-core-0.0.5/src/core/app/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/app/app_event.py` & `braincube-aws-core-0.0.5/src/core/app/app_event.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/app/app_module.py` & `braincube-aws-core-0.0.5/src/core/app/app_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -125,14 +125,15 @@
         if not handler:
             raise Exception("Handler not found.")
 
         return await handler(event, context)
 
     async def _serve_cognito(self, event: dict, context) -> dict:
 
+        # TODO: typed
         cognito_key = str(EventType.cognito.value)
         combination_key = f"{cognito_key}::{event['triggerSource']}"
 
         trigger = self._triggers.get(combination_key if combination_key in self._triggers else cognito_key)
         if not trigger:
             raise ValueError(f"unknown event: {cognito_key} source: {event.get('triggerSource')}")
 
@@ -157,16 +158,24 @@
             params = [await provide(cls, name) for cls, name in route.dependencies]
             params.append(http_event_to_request(route.request_type, event, context))
 
             response: HTTPResponse = await route.func(*params)
 
             status_code = response.status
             body = json.dumps(response.body, cls=JSONEncoder) if response.body else response.body
+
             headers = response.headers if response.headers else dict()
-            headers["X-Process-Time"] = int((time.time() - start) * 1000)
+            headers.update({
+                "Access-Control-Allow-Credentials": True,
+                "Access-Control-Allow-Headers":
+                    "Content-Type,Authorization,X-Amz-Date,X-Api-Key,X-Amz-Security-Token,X-Niki-RequestId",
+                "Access-Control-Allow-Methods": "GET,POST,DELETE",
+                "Access-Control-Allow-Origin": "*",
+                "X-Process-Time": int((time.time() - start) * 1000)
+            })
 
         except Exception as error:
             status_code, body, headers = self._exception_handler.handle(error)
 
         return {
             "statusCode": status_code,
             "body": body,
```

### Comparing `braincube-aws-core-0.0.4/src/core/app/data.py` & `braincube-aws-core-0.0.5/src/core/app/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/dal/data.py` & `braincube-aws-core-0.0.5/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/dal/postgres_connection.py` & `braincube-aws-core-0.0.5/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/dal/postgres_repository.py` & `braincube-aws-core-0.0.5/src/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/di/data.py` & `braincube-aws-core-0.0.5/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/di/injector.py` & `braincube-aws-core-0.0.5/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/rules_engine/data.py` & `braincube-aws-core-0.0.5/src/core/rules_engine/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/rules_engine/rule_manager.py` & `braincube-aws-core-0.0.5/src/core/rules_engine/rule_manager.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/utils/convert.py` & `braincube-aws-core-0.0.5/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.4/src/core/utils/data.py` & `braincube-aws-core-0.0.5/src/core/utils/data.py`

 * *Files identical despite different names*

