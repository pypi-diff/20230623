# Comparing `tmp/redis_rate_limiters-0.3.0.tar.gz` & `tmp/redis_rate_limiters-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_rate_limiters-0.3.0.tar", max compression
+gzip compressed data, was "redis_rate_limiters-0.3.1.tar", max compression
```

## Comparing `redis_rate_limiters-0.3.0.tar` & `redis_rate_limiters-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1652 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/LICENSE
--rw-r--r--   0        0        0     5218 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/README.md
--rw-r--r--   0        0        0      294 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/__init__.py
--rw-r--r--   0        0        0     1593 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/base.py
--rw-r--r--   0        0        0      143 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/py.typed
--rw-r--r--   0        0        0     1544 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/semaphore.lua
--rw-r--r--   0        0        0     4465 2023-06-22 13:12:30.712618 redis_rate_limiters-0.3.0/limiters/semaphore.py
--rw-r--r--   0        0        0     2349 2023-06-22 13:12:30.716618 redis_rate_limiters-0.3.0/limiters/token_bucket.lua
--rw-r--r--   0        0        0     3328 2023-06-22 13:12:30.716618 redis_rate_limiters-0.3.0/limiters/token_bucket.py
--rw-r--r--   0        0        0     3155 2023-06-22 13:12:30.716618 redis_rate_limiters-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6474 1970-01-01 00:00:00.000000 redis_rate_limiters-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1652 2023-06-23 13:52:13.060121 redis_rate_limiters-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5218 2023-06-23 13:52:13.060121 redis_rate_limiters-0.3.1/README.md
+-rw-r--r--   0        0        0      294 2023-06-23 13:52:13.060121 redis_rate_limiters-0.3.1/limiters/__init__.py
+-rw-r--r--   0        0        0     1593 2023-06-23 13:52:13.060121 redis_rate_limiters-0.3.1/limiters/base.py
+-rw-r--r--   0        0        0      143 2023-06-23 13:52:13.060121 redis_rate_limiters-0.3.1/limiters/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:52:13.060121 redis_rate_limiters-0.3.1/limiters/py.typed
+-rw-r--r--   0        0        0     1544 2023-06-23 13:52:13.060121 redis_rate_limiters-0.3.1/limiters/semaphore.lua
+-rw-r--r--   0        0        0     4465 2023-06-23 13:52:13.060121 redis_rate_limiters-0.3.1/limiters/semaphore.py
+-rw-r--r--   0        0        0     2349 2023-06-23 13:52:13.060121 redis_rate_limiters-0.3.1/limiters/token_bucket.lua
+-rw-r--r--   0        0        0     3360 2023-06-23 13:52:13.060121 redis_rate_limiters-0.3.1/limiters/token_bucket.py
+-rw-r--r--   0        0        0     3155 2023-06-23 13:52:13.060121 redis_rate_limiters-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6474 1970-01-01 00:00:00.000000 redis_rate_limiters-0.3.1/PKG-INFO
```

### Comparing `redis_rate_limiters-0.3.0/LICENSE` & `redis_rate_limiters-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.3.0/README.md` & `redis_rate_limiters-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.3.0/limiters/base.py` & `redis_rate_limiters-0.3.1/limiters/base.py`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.3.0/limiters/semaphore.lua` & `redis_rate_limiters-0.3.1/limiters/semaphore.lua`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.3.0/limiters/semaphore.py` & `redis_rate_limiters-0.3.1/limiters/semaphore.py`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.3.0/limiters/token_bucket.lua` & `redis_rate_limiters-0.3.1/limiters/token_bucket.lua`

 * *Files identical despite different names*

### Comparing `redis_rate_limiters-0.3.0/limiters/token_bucket.py` & `redis_rate_limiters-0.3.1/limiters/token_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,18 @@
         # Establish how long we should sleep
         sleep_time = (wake_up_time - now).total_seconds()
 
         # Raise an error if we exceed the maximum sleep setting
         if self.max_sleep != 0.0 and sleep_time > self.max_sleep:
             raise MaxSleepExceededError(
                 f'Scheduled to sleep `{sleep_time}` seconds. '
-                f'This exceeds the maximum accepted sleep time of `{self.max_sleep}` seconds.'
+                f'This exceeds the maximum accepted sleep time of `{self.max_sleep}` seconds for {self.name}.'
             )
 
-        logger.info('Sleeping %s seconds', sleep_time)
+        logger.info('Sleeping %s seconds (%s)', sleep_time, self.name)
         return sleep_time
 
     @property
     def key(self) -> str:
         return f'{{limiter}}:token-bucket:{self.name}'
 
     def __str__(self) -> str:
```

### Comparing `redis_rate_limiters-0.3.0/pyproject.toml` & `redis_rate_limiters-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-rate-limiters"
-version = "0.3.0"
+version = "0.3.1"
 description = "Distributed rate limiters"
 license = "BSD-4-Clause"
 authors = ["Sondre Lillebø Gundersen <sondrelg@live.no>"]
 readme = "README.md"
 homepage = "https://github.com/otovo/redis-rate-limiters"
 repository = "https://github.com/otovo/redis-rate-limiters"
 keywords = [
```

### Comparing `redis_rate_limiters-0.3.0/PKG-INFO` & `redis_rate_limiters-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-rate-limiters
-Version: 0.3.0
+Version: 0.3.1
 Summary: Distributed rate limiters
 Home-page: https://github.com/otovo/redis-rate-limiters
 License: BSD-4-Clause
 Keywords: async,sync,rate,limiting,limiters
 Author: Sondre Lillebø Gundersen
 Author-email: sondrelg@live.no
 Requires-Python: >=3.11,<4.0
```

