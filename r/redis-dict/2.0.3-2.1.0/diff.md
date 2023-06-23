# Comparing `tmp/redis dict-2.0.3.tar.gz` & `tmp/redis dict-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis dict-2.0.3.tar", last modified: Sat Apr  1 05:09:06 2023, max compression
+gzip compressed data, was "redis dict-2.1.0.tar", last modified: Fri Jun 23 09:39:48 2023, max compression
```

## Comparing `redis dict-2.0.3.tar` & `redis dict-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 meneer    (1000) meneer    (1000)        0 2023-04-01 05:09:06.370901 redis dict-2.0.3/
--rw-rw-r--   0 meneer    (1000) meneer    (1000)     1070 2021-06-23 18:44:48.000000 redis dict-2.0.3/LICENSE
--rw-rw-r--   0 meneer    (1000) meneer    (1000)     8723 2023-04-01 05:09:06.370901 redis dict-2.0.3/PKG-INFO
--rw-rw-r--   0 meneer    (1000) meneer    (1000)     7756 2023-04-01 05:06:29.000000 redis dict-2.0.3/README.md
-drwxrwxr-x   0 meneer    (1000) meneer    (1000)        0 2023-04-01 05:09:06.370901 redis dict-2.0.3/redis_dict.egg-info/
--rw-rw-r--   0 meneer    (1000) meneer    (1000)     8723 2023-04-01 05:09:06.000000 redis dict-2.0.3/redis_dict.egg-info/PKG-INFO
--rw-rw-r--   0 meneer    (1000) meneer    (1000)      209 2023-04-01 05:09:06.000000 redis dict-2.0.3/redis_dict.egg-info/SOURCES.txt
--rw-rw-r--   0 meneer    (1000) meneer    (1000)        1 2023-04-01 05:09:06.000000 redis dict-2.0.3/redis_dict.egg-info/dependency_links.txt
--rw-rw-r--   0 meneer    (1000) meneer    (1000)        6 2023-04-01 05:09:06.000000 redis dict-2.0.3/redis_dict.egg-info/requires.txt
--rw-rw-r--   0 meneer    (1000) meneer    (1000)       11 2023-04-01 05:09:06.000000 redis dict-2.0.3/redis_dict.egg-info/top_level.txt
--rw-rw-r--   0 meneer    (1000) meneer    (1000)    24074 2023-04-01 04:47:46.000000 redis dict-2.0.3/redis_dict.py
--rw-rw-r--   0 meneer    (1000) meneer    (1000)       38 2023-04-01 05:09:06.370901 redis dict-2.0.3/setup.cfg
--rw-rw-r--   0 meneer    (1000) meneer    (1000)     1304 2023-04-01 04:55:11.000000 redis dict-2.0.3/setup.py
+drwxr-xr-x   0 mbijman    (501) staff       (20)        0 2023-06-23 09:39:48.568845 redis dict-2.1.0/
+-rw-r--r--   0 mbijman    (501) staff       (20)     1070 2023-06-20 10:38:38.000000 redis dict-2.1.0/LICENSE
+-rw-r--r--   0 mbijman    (501) staff       (20)     8624 2023-06-23 09:39:48.568717 redis dict-2.1.0/PKG-INFO
+-rw-r--r--   0 mbijman    (501) staff       (20)     7756 2023-06-20 10:38:38.000000 redis dict-2.1.0/README.md
+drwxr-xr-x   0 mbijman    (501) staff       (20)        0 2023-06-23 09:39:48.568576 redis dict-2.1.0/redis_dict.egg-info/
+-rw-r--r--   0 mbijman    (501) staff       (20)     8624 2023-06-23 09:39:48.000000 redis dict-2.1.0/redis_dict.egg-info/PKG-INFO
+-rw-r--r--   0 mbijman    (501) staff       (20)      209 2023-06-23 09:39:48.000000 redis dict-2.1.0/redis_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 mbijman    (501) staff       (20)        1 2023-06-23 09:39:48.000000 redis dict-2.1.0/redis_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 mbijman    (501) staff       (20)        6 2023-06-23 09:39:48.000000 redis dict-2.1.0/redis_dict.egg-info/requires.txt
+-rw-r--r--   0 mbijman    (501) staff       (20)       11 2023-06-23 09:39:48.000000 redis dict-2.1.0/redis_dict.egg-info/top_level.txt
+-rw-r--r--   0 mbijman    (501) staff       (20)    25221 2023-06-23 09:25:12.000000 redis dict-2.1.0/redis_dict.py
+-rw-r--r--   0 mbijman    (501) staff       (20)       38 2023-06-23 09:39:48.568876 redis dict-2.1.0/setup.cfg
+-rw-r--r--   0 mbijman    (501) staff       (20)     1207 2023-06-22 10:40:15.000000 redis dict-2.1.0/setup.py
```

### Comparing `redis dict-2.0.3/LICENSE` & `redis dict-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redis dict-2.0.3/PKG-INFO` & `redis dict-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: redis dict
-Version: 2.0.3
+Version: 2.1.0
 Summary: Dictionary with Redis as storage backend
 Home-page: https://github.com/Attumm/redisdict
 Author: Melvin Bijman
 Author-email: bijman.m.m@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: System :: Distributed Computing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Redis-dict
 [![Build Status](https://travis-ci.com/Attumm/redis-dict.svg?branch=main)](https://travis-ci.com/Attumm/redis-dict)
 [![Downloads](https://pepy.tech/badge/redis-dict)](https://pepy.tech/project/redis-dict)
```

### Comparing `redis dict-2.0.3/README.md` & `redis dict-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `redis dict-2.0.3/redis_dict.egg-info/PKG-INFO` & `redis dict-2.1.0/redis_dict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: redis-dict
-Version: 2.0.3
+Version: 2.1.0
 Summary: Dictionary with Redis as storage backend
 Home-page: https://github.com/Attumm/redisdict
 Author: Melvin Bijman
 Author-email: bijman.m.m@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: System :: Distributed Computing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Redis-dict
 [![Build Status](https://travis-ci.com/Attumm/redis-dict.svg?branch=main)](https://travis-ci.com/Attumm/redis-dict)
 [![Downloads](https://pepy.tech/badge/redis-dict)](https://pepy.tech/project/redis-dict)
```

### Comparing `redis dict-2.0.3/redis_dict.py` & `redis dict-2.1.0/redis_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 from typing import Any, Callable, Dict, Iterator, Set, List, Tuple, Union, Optional
-
 from redis import StrictRedis
 
 from contextlib import contextmanager
 
 SENTINEL = object()
 
 
@@ -95,14 +94,16 @@
 
     Attributes:
         transform (Dict[str, Callable[[str], Any]]): A dictionary of data type transformation functions for loading data.
         pre_transform (Dict[str, Callable[[Any], str]]): A dictionary of data type transformation functions for storing data.
         namespace (str): A string used as a prefix for Redis keys to separate data in different namespaces.
         expire (Union[int, None]): An optional expiration time for keys, in seconds.
 
+    TODO:
+        Move init to work with types
     """
 
     transform: transform_type = {
         type('').__name__: str,
         type(1).__name__: int,
         type(0.1).__name__: float,
         type(True).__name__: lambda x: x == "True",
@@ -130,14 +131,15 @@
             expire (int, optional): Expiration time for keys in seconds.
             **kwargs: Additional keyword arguments passed to StrictRedis.
         """
         self.temp_redis: Optional[StrictRedis[Any]] = None
 
         self.namespace: str = kwargs.pop('namespace', '')
         self.expire: Union[int, None] = kwargs.pop('expire', None)
+        self.preserve_expiration: bool = kwargs.pop('preserve_expiration', False)
 
         self.redis: StrictRedis[Any] = StrictRedis(decode_responses=True, **kwargs)
         self.get_redis: StrictRedis[Any] = self.redis
         self.iter: Iterator[str] = self.iterkeys()
 
     def _format_key(self, key: str) -> str:
         """
@@ -181,15 +183,20 @@
         store_type, key = type(value).__name__, str(key)
         if not self._valid_input(value, store_type) or not self._valid_input(key, "str"):
             # TODO When needed, make valid_input, pass the reason, or throw a exception.
             raise ValueError("Invalid input value or key size exceeded the maximum limit.")
         value = self.pre_transform.get(store_type, lambda x: x)(value)  # type: ignore
 
         store_value = '{}:{}'.format(store_type, value)
-        self.redis.set(self._format_key(key), store_value, ex=self.expire)
+        formatted_key = self._format_key(key)
+
+        if self.preserve_expiration and self.redis.exists(formatted_key):
+            self.redis.set(formatted_key, store_value, keepttl=True)
+        else:
+            self.redis.set(formatted_key, store_value, ex=self.expire)
 
     def _load(self, key: str) -> Tuple[bool, Any]:
         """
         Load a value from Redis with the given key.
 
         Args:
             key (str): The key to retrieve the value.
@@ -716,7 +723,32 @@
         Returns:
             int: The number of keys deleted.
         """
         keys = list(self._scan_keys(key))
         if len(keys) == 0:
             return 0
         return self.redis.delete(*keys)
+
+    def get_redis_info(self) -> Dict[str, Any]:
+        """
+        Retrieve information and statistics about the Redis server.
+
+        Returns:
+            dict: The information and statistics from the Redis server in a dictionary.
+        """
+        return dict(self.redis.info())
+
+    def get_ttl(self, key: str) -> Optional[int]:
+        """
+        Get the Time To Live (TTL) in seconds for a given key. If the key does not exist or does not have an
+        associated expire, return None.
+
+        Args:
+            key (str): The key for which to get the TTL.
+
+        Returns:
+            Optional[int]: The TTL in seconds if the key exists and has an expire set; otherwise, None.
+        """
+        val = self.redis.ttl(self._format_key(key))
+        if val < 0:
+            return None
+        return val
```

### Comparing `redis dict-2.0.3/setup.py` & `redis dict-2.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     author='Melvin Bijman',
     author_email='bijman.m.m@gmail.com',
 
     description='Dictionary with Redis as storage backend',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
-    version='2.0.3',
+    version='2.1.0',
     py_modules=['redis_dict'],
     install_requires=['redis',],
     license='MIT',
 
     url='https://github.com/Attumm/redisdict',
 
     classifiers=[
@@ -31,18 +31,16 @@
 
         'Topic :: Database',
         'Topic :: System :: Distributed Computing',
 
         'License :: OSI Approved :: MIT License',
 
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

