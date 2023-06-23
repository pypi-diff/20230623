# Comparing `tmp/asyncio-oss-1.0.1.tar.gz` & `tmp/asyncio-oss-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncio-oss-1.0.1.tar", last modified: Tue May 30 16:47:52 2023, max compression
+gzip compressed data, was "asyncio-oss-1.0.2.tar", last modified: Fri Jun 23 18:24:18 2023, max compression
```

## Comparing `asyncio-oss-1.0.1.tar` & `asyncio-oss-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-05-30 16:47:52.546381 asyncio-oss-1.0.1/
--rw-r--r--   0 longyao    (501) staff       (20)     1064 2023-05-24 15:02:54.000000 asyncio-oss-1.0.1/LICENSE
--rw-r--r--   0 longyao    (501) staff       (20)     2166 2023-05-30 16:47:52.546225 asyncio-oss-1.0.1/PKG-INFO
--rw-r--r--   0 longyao    (501) staff       (20)     1820 2023-05-30 15:52:33.000000 asyncio-oss-1.0.1/README.md
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-05-30 16:47:52.545251 asyncio-oss-1.0.1/asyncio_oss/
--rw-r--r--   0 longyao    (501) staff       (20)      435 2023-05-29 15:33:32.000000 asyncio-oss-1.0.1/asyncio_oss/__init__.py
--rw-r--r--   0 longyao    (501) staff       (20)   134447 2023-05-24 15:02:54.000000 asyncio-oss-1.0.1/asyncio_oss/api.py
--rw-r--r--   0 longyao    (501) staff       (20)     9063 2023-05-24 15:02:54.000000 asyncio-oss-1.0.1/asyncio_oss/exceptions.py
--rw-r--r--   0 longyao    (501) staff       (20)     6530 2023-05-30 16:32:26.000000 asyncio-oss-1.0.1/asyncio_oss/http.py
--rw-r--r--   0 longyao    (501) staff       (20)    13020 2023-05-24 15:02:54.000000 asyncio-oss-1.0.1/asyncio_oss/iterators.py
--rw-r--r--   0 longyao    (501) staff       (20)    80193 2023-05-24 15:02:54.000000 asyncio-oss-1.0.1/asyncio_oss/models.py
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-05-30 16:47:52.546014 asyncio-oss-1.0.1/asyncio_oss/test/
--rw-r--r--   0 longyao    (501) staff       (20)      554 2023-05-29 13:59:36.000000 asyncio-oss-1.0.1/asyncio_oss/test/__init__.py
--rw-r--r--   0 longyao    (501) staff       (20)     2550 2023-05-30 16:32:26.000000 asyncio-oss-1.0.1/asyncio_oss/test/object_test.py
--rw-r--r--   0 longyao    (501) staff       (20)    26065 2023-05-24 15:02:54.000000 asyncio-oss-1.0.1/asyncio_oss/utils.py
-drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-05-30 16:47:52.545793 asyncio-oss-1.0.1/asyncio_oss.egg-info/
--rw-r--r--   0 longyao    (501) staff       (20)     2166 2023-05-30 16:47:52.000000 asyncio-oss-1.0.1/asyncio_oss.egg-info/PKG-INFO
--rw-r--r--   0 longyao    (501) staff       (20)      418 2023-05-30 16:47:52.000000 asyncio-oss-1.0.1/asyncio_oss.egg-info/SOURCES.txt
--rw-r--r--   0 longyao    (501) staff       (20)        1 2023-05-30 16:47:52.000000 asyncio-oss-1.0.1/asyncio_oss.egg-info/dependency_links.txt
--rw-r--r--   0 longyao    (501) staff       (20)       13 2023-05-30 16:47:52.000000 asyncio-oss-1.0.1/asyncio_oss.egg-info/requires.txt
--rw-r--r--   0 longyao    (501) staff       (20)       12 2023-05-30 16:47:52.000000 asyncio-oss-1.0.1/asyncio_oss.egg-info/top_level.txt
--rw-r--r--   0 longyao    (501) staff       (20)       38 2023-05-30 16:47:52.546436 asyncio-oss-1.0.1/setup.cfg
--rw-r--r--   0 longyao    (501) staff       (20)      679 2023-05-30 16:46:45.000000 asyncio-oss-1.0.1/setup.py
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-23 18:24:18.933663 asyncio-oss-1.0.2/
+-rw-r--r--   0 longyao    (501) staff       (20)     1064 2023-05-24 15:02:54.000000 asyncio-oss-1.0.2/LICENSE
+-rw-r--r--   0 longyao    (501) staff       (20)     2533 2023-06-23 18:24:18.933573 asyncio-oss-1.0.2/PKG-INFO
+-rw-r--r--   0 longyao    (501) staff       (20)     2187 2023-06-23 18:21:23.000000 asyncio-oss-1.0.2/README.md
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-23 18:24:18.932575 asyncio-oss-1.0.2/asyncio_oss/
+-rw-r--r--   0 longyao    (501) staff       (20)      435 2023-05-29 15:33:32.000000 asyncio-oss-1.0.2/asyncio_oss/__init__.py
+-rw-r--r--   0 longyao    (501) staff       (20)   134427 2023-06-05 16:55:09.000000 asyncio-oss-1.0.2/asyncio_oss/api.py
+-rw-r--r--   0 longyao    (501) staff       (20)     9063 2023-05-24 15:02:54.000000 asyncio-oss-1.0.2/asyncio_oss/exceptions.py
+-rw-r--r--   0 longyao    (501) staff       (20)     6431 2023-06-05 16:55:09.000000 asyncio-oss-1.0.2/asyncio_oss/http.py
+-rw-r--r--   0 longyao    (501) staff       (20)    13014 2023-06-23 18:07:43.000000 asyncio-oss-1.0.2/asyncio_oss/iterators.py
+-rw-r--r--   0 longyao    (501) staff       (20)    80193 2023-05-24 15:02:54.000000 asyncio-oss-1.0.2/asyncio_oss/models.py
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-23 18:24:18.933421 asyncio-oss-1.0.2/asyncio_oss/test/
+-rw-r--r--   0 longyao    (501) staff       (20)      554 2023-05-29 13:59:36.000000 asyncio-oss-1.0.2/asyncio_oss/test/__init__.py
+-rw-r--r--   0 longyao    (501) staff       (20)     2550 2023-06-05 16:35:18.000000 asyncio-oss-1.0.2/asyncio_oss/test/object_test.py
+-rw-r--r--   0 longyao    (501) staff       (20)      499 2023-06-23 17:51:40.000000 asyncio-oss-1.0.2/asyncio_oss/test/service_test.py
+-rw-r--r--   0 longyao    (501) staff       (20)    26065 2023-05-24 15:02:54.000000 asyncio-oss-1.0.2/asyncio_oss/utils.py
+drwxr-xr-x   0 longyao    (501) staff       (20)        0 2023-06-23 18:24:18.933119 asyncio-oss-1.0.2/asyncio_oss.egg-info/
+-rw-r--r--   0 longyao    (501) staff       (20)     2533 2023-06-23 18:24:18.000000 asyncio-oss-1.0.2/asyncio_oss.egg-info/PKG-INFO
+-rw-r--r--   0 longyao    (501) staff       (20)      451 2023-06-23 18:24:18.000000 asyncio-oss-1.0.2/asyncio_oss.egg-info/SOURCES.txt
+-rw-r--r--   0 longyao    (501) staff       (20)        1 2023-06-23 18:24:18.000000 asyncio-oss-1.0.2/asyncio_oss.egg-info/dependency_links.txt
+-rw-r--r--   0 longyao    (501) staff       (20)       13 2023-06-23 18:24:18.000000 asyncio-oss-1.0.2/asyncio_oss.egg-info/requires.txt
+-rw-r--r--   0 longyao    (501) staff       (20)       12 2023-06-23 18:24:18.000000 asyncio-oss-1.0.2/asyncio_oss.egg-info/top_level.txt
+-rw-r--r--   0 longyao    (501) staff       (20)       38 2023-06-23 18:24:18.933698 asyncio-oss-1.0.2/setup.cfg
+-rw-r--r--   0 longyao    (501) staff       (20)      679 2023-06-23 18:21:23.000000 asyncio-oss-1.0.2/setup.py
```

### Comparing `asyncio-oss-1.0.1/LICENSE` & `asyncio-oss-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.0.1/PKG-INFO` & `asyncio-oss-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio-oss
-Version: 1.0.1
+Version: 1.0.2
 Summary: An asynchronous python client SDK for OSS(Aliyun Object Storage Service).
 Home-page: https://github.com/Yaocool/async-oss
 Author: Ozzy
 Author-email: ozzycharon@gmail.com
 License: MIT
 Keywords: asyncio-oss,async-oss,oss
 Description-Content-Type: text/markdown
@@ -63,14 +63,21 @@
 
 if __name__ == '__main__':
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
 # ChangeLogs
-* init 1.0.0
-* [Jul 29, 2022] fix `http.py/do_request` method stream read bug
-* [May 29, 2023] add test cases and supported `asyncio-oss` package in PyPI
-
+* [Jul 29, 2022 - 1.0.0]
+  * fix `http.py/do_request` method stream read bug
+* [May 29, 2023]
+  * add test cases and supported `asyncio-oss` package in PyPI
+* [May 30, 2023 - 1.0.1]
+  * bump version to 1.0.1 for PyPI package description updating
+* [June 24, 2023 - 1.0.2]
+  * remove unused fields add params in `asyncio_oss/http.py api.py` files
+  * fix `asyncio_oss/iterators.py/_BaseIterator/__aiter__` method bug
+  * add `list_buckets` test case in `tests/service_test.py` for `Service` class
+  * bump version to 1.0.2
 
 # Discussions
 Any questions can be raised in Discussions, I will answer them from time to time~
```

### Comparing `asyncio-oss-1.0.1/README.md` & `asyncio-oss-1.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -51,14 +51,21 @@
 
 if __name__ == '__main__':
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
 # ChangeLogs
-* init 1.0.0
-* [Jul 29, 2022] fix `http.py/do_request` method stream read bug
-* [May 29, 2023] add test cases and supported `asyncio-oss` package in PyPI
-
+* [Jul 29, 2022 - 1.0.0]
+  * fix `http.py/do_request` method stream read bug
+* [May 29, 2023]
+  * add test cases and supported `asyncio-oss` package in PyPI
+* [May 30, 2023 - 1.0.1]
+  * bump version to 1.0.1 for PyPI package description updating
+* [June 24, 2023 - 1.0.2]
+  * remove unused fields add params in `asyncio_oss/http.py api.py` files
+  * fix `asyncio_oss/iterators.py/_BaseIterator/__aiter__` method bug
+  * add `list_buckets` test case in `tests/service_test.py` for `Service` class
+  * bump version to 1.0.2
 
 # Discussions
 Any questions can be raised in Discussions, I will answer them from time to time~
```

### Comparing `asyncio-oss-1.0.1/asyncio_oss/api.py` & `asyncio-oss-1.0.2/asyncio_oss/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,20 +196,20 @@
 from .models import GetObjectResult as AsyncGetObjectResult
 
 logger = logging.getLogger(__name__)
 
 
 class _Base(object):
     def __init__(self, auth, endpoint, is_cname, session, connect_timeout,
-                 app_name='', enable_crc=True, proxy=None, loop=None):
+                 app_name='', enable_crc=True, proxy=None):
         self.auth = auth
         self.endpoint = _normalize_endpoint(endpoint.strip())
         if utils.is_valid_endpoint(self.endpoint) is not True:
             raise ClientError('The endpoint you has specified is not valid, endpoint: {0}'.format(endpoint))
-        self.session = session or http.Session(loop=loop)
+        self.session = session or http.Session()
         self.timeout = defaults.get(connect_timeout, defaults.connect_timeout)
         self.app_name = app_name
         self.enable_crc = enable_crc
         self.proxy = proxy
 
         self._make_url = _UrlMaker(self.endpoint, is_cname)
```

### Comparing `asyncio-oss-1.0.1/asyncio_oss/exceptions.py` & `asyncio-oss-1.0.2/asyncio_oss/exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.0.1/asyncio_oss/http.py` & `asyncio-oss-1.0.2/asyncio_oss/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 oss2.http
 ~~~~~~~~
 
 这个模块包含了HTTP Adapters。尽管OSS Python SDK内部使用requests库进行HTTP通信，但是对使用者是透明的。
 该模块中的 `Session` 、 `Request` 、`Response` 对requests的对应的类做了简单的封装。
 """
-import asyncio
 import logging
 import platform
 
 import aiohttp
 from requests.structures import CaseInsensitiveDict
 
 from oss2 import __version__, defaults
@@ -24,62 +23,62 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Session(object):
     """属于同一个Session的请求共享一组连接池，如有可能也会重用HTTP连接。"""
 
-    def __init__(self, loop=None):
-        self._loop = loop or asyncio.get_event_loop()
+    def __init__(self):
         self.resp = None
+        self._aio_session = None
 
-        psize = defaults.connection_pool_size
-        connector = aiohttp.TCPConnector(limit=psize, loop=self._loop)
-        self.aio_session = aiohttp.ClientSession(
-            connector=connector,
-            loop=self._loop,
-            skip_auto_headers=['User-Agent', 'Content-Type'])
+    async def _create_session(self):
+        if self._aio_session is None:
+            pool_size = defaults.connection_pool_size
+            connector = aiohttp.TCPConnector(limit=pool_size)
+            self._aio_session = aiohttp.ClientSession(connector=connector)
 
     async def do_request(self, req, timeout):
         try:
             logger.debug(
                 "Send request, method: {0}, url: {1}, params: {2}, headers: {3}, timeout: {4}, proxy: {5}".format(
                     req.method, req.url, req.params, req.headers, timeout, req.proxy))
 
-            # 1. 当设置 progress_callback 或开启 crc 校验时，data 类型会经 oss make_progress_adapter / make_crc_adapter 转换
-            # 成对应的 adapter object，并且在 read 时进行 process_callback 与 crc 校验计算
-            # 2. requests 支持 file-like-object 的读取，而 aiohttp 不支持，因此需要提前将 data 读取出来
+            await self._create_session()
+            # 1. When setting progress_callback or enabling crc verification, the data type will be converted to the
+            # corresponding adapter object by oss make_progress_adapter / make_crc_adapter, and the process_callback
+            # and crc verification calculation will be performed when read
+            # 2. requests supports the reading of file-like-objects, while aiohttp does not, so you need to read the
+            # data in advance
             req_data = req.data.read() if hasattr(req.data, 'read') else req.data
-            resp = await self.aio_session.request(req.method, req.url,
-                                                  data=req_data,
-                                                  params=req.params,
-                                                  headers=req.headers,
-                                                  timeout=timeout,
-                                                  proxy=req.proxy)
+            resp = await self._aio_session.request(
+                req.method,
+                req.url,
+                data=req_data,
+                params=req.params,
+                headers=req.headers,
+                timeout=timeout,
+                proxy=req.proxy
+            )
             self.resp = resp
             return Response(resp)
         except IOError as e:
+            # catch read IO error
             raise RequestError(e)
+        except aiohttp.ClientError:
+            # catch all aiohttp client errors
+            await self._aio_session.close()
 
     async def __aenter__(self):
-        await self.aio_session.__aenter__()
+        await self._create_session()
+        await self._aio_session.__aenter__()
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
-        self._release_resp()
-        await self.aio_session.__aexit__(exc_type, exc_val, exc_tb)
-
-    async def close(self):
-        self._release_resp()
-        await self.aio_session.close()
-
-    def _release_resp(self):
-        if self.resp:
-            self.resp.release()
-            self.resp.close()
+        await self._aio_session.__aexit__(exc_type, exc_val, exc_tb)
 
 
 class Request(object):
     def __init__(self, method, url,
                  data=None,
                  params=None,
                  headers=None,
@@ -150,18 +149,18 @@
         else:
             return await self.response.content.read(amt)
 
     def __aiter__(self):
         return self.response.content
 
 
-# requests对于具有fileno()方法的file object，会用fileno()的返回值作为Content-Length。
-# 这对于已经读取了部分内容，或执行了seek()的file object是不正确的。
+# requests 对于具有 fileno() 方法的 file object，会用 fileno() 的返回值作为 Content-Length。
+# 这对于已经读取了部分内容，或执行了seek() 的 file object是不正确的。
 #
-# _convert_request_body()对于支持seek()和tell() file object，确保是从
+# _convert_request_body() 对于支持 seek() 和 tell() file object，确保是从
 # 当前位置读取，且只读取当前位置到文件结束的内容。
 def _convert_request_body(data):
     data = to_bytes(data)
 
     if hasattr(data, '__len__'):
         return data
```

### Comparing `asyncio-oss-1.0.1/asyncio_oss/iterators.py` & `asyncio-oss-1.0.2/asyncio_oss/iterators.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.max_retries = max_retries if max_retries > 0 else 1
 
         self.entries = []
 
     def _fetch(self):
         raise NotImplemented  # pragma: no cover
 
-    async def __aiter__(self):
+    def __aiter__(self):
         return self
 
     async def __anext__(self):
         while True:
             if self.entries:
                 return self.entries.pop(0)
```

### Comparing `asyncio-oss-1.0.1/asyncio_oss/models.py` & `asyncio-oss-1.0.2/asyncio_oss/models.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.0.1/asyncio_oss/test/__init__.py` & `asyncio-oss-1.0.2/asyncio_oss/test/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.0.1/asyncio_oss/test/object_test.py` & `asyncio-oss-1.0.2/asyncio_oss/test/object_test.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.0.1/asyncio_oss/utils.py` & `asyncio-oss-1.0.2/asyncio_oss/utils.py`

 * *Files identical despite different names*

### Comparing `asyncio-oss-1.0.1/asyncio_oss.egg-info/PKG-INFO` & `asyncio-oss-1.0.2/asyncio_oss.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncio-oss
-Version: 1.0.1
+Version: 1.0.2
 Summary: An asynchronous python client SDK for OSS(Aliyun Object Storage Service).
 Home-page: https://github.com/Yaocool/async-oss
 Author: Ozzy
 Author-email: ozzycharon@gmail.com
 License: MIT
 Keywords: asyncio-oss,async-oss,oss
 Description-Content-Type: text/markdown
@@ -63,14 +63,21 @@
 
 if __name__ == '__main__':
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
 ```
 
 # ChangeLogs
-* init 1.0.0
-* [Jul 29, 2022] fix `http.py/do_request` method stream read bug
-* [May 29, 2023] add test cases and supported `asyncio-oss` package in PyPI
-
+* [Jul 29, 2022 - 1.0.0]
+  * fix `http.py/do_request` method stream read bug
+* [May 29, 2023]
+  * add test cases and supported `asyncio-oss` package in PyPI
+* [May 30, 2023 - 1.0.1]
+  * bump version to 1.0.1 for PyPI package description updating
+* [June 24, 2023 - 1.0.2]
+  * remove unused fields add params in `asyncio_oss/http.py api.py` files
+  * fix `asyncio_oss/iterators.py/_BaseIterator/__aiter__` method bug
+  * add `list_buckets` test case in `tests/service_test.py` for `Service` class
+  * bump version to 1.0.2
 
 # Discussions
 Any questions can be raised in Discussions, I will answer them from time to time~
```

### Comparing `asyncio-oss-1.0.1/setup.py` & `asyncio-oss-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='asyncio-oss',
-    version='1.0.1',
+    version='1.0.2',
     description='An asynchronous python client SDK for OSS(Aliyun Object Storage Service).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Yaocool/async-oss",
     keywords="asyncio-oss, async-oss, oss",
     author='Ozzy',
     author_email='ozzycharon@gmail.com',
```

