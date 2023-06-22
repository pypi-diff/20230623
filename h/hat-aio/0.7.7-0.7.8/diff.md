# Comparing `tmp/hat_aio-0.7.7-cp38.cp39.cp310.cp311-none-any.whl.zip` & `tmp/hat_aio-0.7.8-cp310.cp311-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 14779 bytes, number of entries: 12
+Zip file size: 14841 bytes, number of entries: 12
 -rw-r--r--  2.0 unx     1225 b- defN 23-Mar-23 19:16 hat/aio/__init__.py
--rw-r--r--  2.0 unx     2761 b- defN 23-Mar-23 19:15 hat/aio/executor.py
--rw-r--r--  2.0 unx     6903 b- defN 23-Apr-09 18:24 hat/aio/group.py
--rw-r--r--  2.0 unx     9360 b- defN 23-Apr-09 18:39 hat/aio/misc.py
--rw-r--r--  2.0 unx     6172 b- defN 23-Apr-09 19:06 hat/aio/queue.py
--rw-r--r--  2.0 unx     1836 b- defN 23-Apr-09 18:48 hat/aio/wait.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     1794 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/METADATA
--rw-r--r--  2.0 unx      152 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/zip-safe
--rw-rw-r--  2.0 unx      915 b- defN 23-Apr-09 19:09 hat_aio-0.7.7.dist-info/RECORD
-12 files, 42481 bytes uncompressed, 13263 bytes compressed:  68.8%
+-rw-r--r--  2.0 unx     2781 b- defN 23-Jun-22 22:49 hat/aio/executor.py
+-rw-r--r--  2.0 unx     6887 b- defN 23-Jun-22 22:51 hat/aio/group.py
+-rw-r--r--  2.0 unx     8928 b- defN 23-Jun-22 23:01 hat/aio/misc.py
+-rw-r--r--  2.0 unx     6139 b- defN 23-Jun-22 23:02 hat/aio/queue.py
+-rw-r--r--  2.0 unx     1788 b- defN 23-Jun-22 23:04 hat/aio/wait.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2214 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/METADATA
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      915 b- defN 23-Jun-22 23:08 hat_aio-0.7.8.dist-info/RECORD
+12 files, 42354 bytes uncompressed, 13325 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: hat/aio/queue.py
 Comment: 
 
 Filename: hat/aio/wait.py
 Comment: 
 
-Filename: hat_aio-0.7.7.dist-info/LICENSE
+Filename: hat_aio-0.7.8.dist-info/LICENSE
 Comment: 
 
-Filename: hat_aio-0.7.7.dist-info/METADATA
+Filename: hat_aio-0.7.8.dist-info/METADATA
 Comment: 
 
-Filename: hat_aio-0.7.7.dist-info/WHEEL
+Filename: hat_aio-0.7.8.dist-info/WHEEL
 Comment: 
 
-Filename: hat_aio-0.7.7.dist-info/top_level.txt
+Filename: hat_aio-0.7.8.dist-info/top_level.txt
 Comment: 
 
-Filename: hat_aio-0.7.7.dist-info/zip-safe
+Filename: hat_aio-0.7.8.dist-info/zip-safe
 Comment: 
 
-Filename: hat_aio-0.7.7.dist-info/RECORD
+Filename: hat_aio-0.7.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/aio/executor.py

```diff
@@ -1,11 +1,11 @@
+from typing import Awaitable, Callable, Type
 import asyncio
 import concurrent.futures
 import functools
-import typing
 
 from hat.aio.group import Resource, Group
 from hat.aio.misc import uncancellable
 
 
 class Executor(Resource):
     """Executor wrapping `asyncio.loop.run_in_executor`.
@@ -26,42 +26,42 @@
         tid1 = await executor1.spawn(threading.get_ident)
         tid2 = await executor2.spawn(threading.get_ident)
         assert tid1 != tid2
 
     """
 
     def __init__(self,
-                 *args: typing.Any,
-                 executor_cls: typing.Type = concurrent.futures.ThreadPoolExecutor,  # NOQA
+                 *args,
+                 executor_cls: Type[concurrent.futures.Executor] = concurrent.futures.ThreadPoolExecutor,  # NOQA
                  log_exceptions: bool = True):
         self._executor = executor_cls(*args)
         self._async_group = Group(log_exceptions)
 
     @property
     def async_group(self):
         """Async group"""
         return self._async_group
 
     def spawn(self,
-              fn: typing.Callable,
+              fn: Callable,
               *args, **kwargs
               ) -> asyncio.Task:
         """Spawn new task"""
         return self.async_group.spawn(self._spawn, fn, *args, **kwargs)
 
     async def _spawn(self, fn, *args, **kwargs):
         loop = asyncio.get_running_loop()
         func = functools.partial(fn, *args, **kwargs)
         return await uncancellable(loop.run_in_executor(self._executor, func))
 
 
-def create_executor(*args: typing.Any,
-                    executor_cls: typing.Type = concurrent.futures.ThreadPoolExecutor,  # NOQA
-                    loop: typing.Optional[asyncio.AbstractEventLoop] = None
-                    ) -> typing.Callable[..., typing.Awaitable]:
+def create_executor(*args,
+                    executor_cls: Type[concurrent.futures.Executor] = concurrent.futures.ThreadPoolExecutor,  # NOQA
+                    loop: asyncio.AbstractEventLoop | None = None
+                    ) -> Callable[..., Awaitable]:
     """Create `asyncio.loop.run_in_executor` wrapper.
 
     Wrapped executor is created from `executor_cls` with provided `args`.
 
     This function returns coroutine that takes a function and its arguments,
     executes the function in executor and returns the result.
```

## hat/aio/group.py

```diff
@@ -1,11 +1,11 @@
+from typing import Awaitable, Callable
 import abc
 import asyncio
 import logging
-import typing
 import warnings
 
 
 mlog: logging.Logger = logging.getLogger(__name__)
 """Module logger"""
 
 
@@ -75,15 +75,15 @@
     logged with level ERROR.
 
     """
 
     def __init__(self,
                  log_exceptions: bool = True,
                  *,
-                 loop: typing.Optional[asyncio.AbstractEventLoop] = None):
+                 loop: asyncio.AbstractEventLoop | None = None):
         self._log_exceptions = log_exceptions
         self._loop = loop or asyncio.get_running_loop()
         self._closing = self._loop.create_future()
         self._closed = self._loop.create_future()
         self._tasks = set()
         self._parent = None
         self._children = set()
@@ -113,15 +113,15 @@
         await asyncio.shield(self._closing)
 
     async def wait_closed(self):
         """Wait until closed is ``True``."""
         await asyncio.shield(self._closed)
 
     def create_subgroup(self,
-                        log_exceptions: typing.Optional[bool] = None
+                        log_exceptions: bool | None = None
                         ) -> 'Group':
         """Create new Group as a child of this Group. Return the new Group.
 
         When a parent Group gets closed, all of its children are closed.
         Closing of a subgroup has no effect on the parent Group.
 
         If `log_exceptions` is ``None``, subgroup inherits `log_exceptions`
@@ -136,15 +136,15 @@
                             else log_exceptions),
             loop=self._loop)
         child._parent = self
         self._children.add(child)
         return child
 
     def wrap(self,
-             obj: typing.Awaitable
+             obj: Awaitable
              ) -> asyncio.Task:
         """Wrap the awaitable object into a Task and schedule its execution.
         Return the Task object.
 
         Resulting task is shielded and can be canceled only with
         `Group.async_close`.
 
@@ -160,15 +160,15 @@
 
         self._tasks.add(task)
         task.add_done_callback(self._on_task_done)
 
         return asyncio.shield(task)
 
     def spawn(self,
-              fn: typing.Callable[..., typing.Awaitable],
+              fn: Callable[..., Awaitable],
               *args, **kwargs
               ) -> asyncio.Task:
         """Wrap the result of a `fn` into a Task and schedule its execution.
         Return the Task object.
 
         Function `fn` is called with provided `args` and `kwargs`.
         Resulting Task is shielded and can be canceled only with
```

## hat/aio/misc.py

```diff
@@ -1,24 +1,24 @@
+from typing import Any, AsyncIterable, Awaitable, Callable, TypeVar
 import asyncio
 import collections
 import collections.abc
 import contextlib
 import inspect
 import signal
 import sys
-import typing
 
 
-T = typing.TypeVar('T')
+T = TypeVar('T')
 
 
-async def first(xs: typing.AsyncIterable[T],
-                fn: typing.Callable[[T], typing.Any] = lambda _: True,
-                default: typing.Optional[T] = None
-                ) -> typing.Optional[T]:
+async def first(xs: AsyncIterable[T],
+                fn: Callable[[T], Any] = lambda _: True,
+                default: T | None = None
+                ) -> T | None:
     """Return the first element from async iterable that satisfies
     predicate `fn`, or `default` if no such element exists.
 
     Result of predicate `fn` can be of any type. Predicate is satisfied if it's
     return value is truthy.
 
     Args:
@@ -42,17 +42,17 @@
     async for i in xs:
         if fn(i):
             return i
 
     return default
 
 
-async def uncancellable(obj: typing.Awaitable,
+async def uncancellable(obj: Awaitable,
                         raise_cancel: bool = True
-                        ) -> typing.Any:
+                        ) -> Any:
     """Uncancellable execution of a awaitable object.
 
     Object is scheduled as task, shielded and its execution cannot be
     interrupted.
 
     If `raise_cancel` is `True` and the object gets canceled,
     `asyncio.CancelledError` is reraised after the Future finishes.
@@ -93,38 +93,32 @@
     if exception:
         raise exception
 
     return task.result()
 
 
 # TODO: AsyncCallable rewrite needed
-class _AsyncCallableType(type(typing.Callable), _root=True):
+class _AsyncCallableType(type(Callable), _root=True):
 
     def __init__(self):
-        if sys.version_info[:2] == (3, 8):
-            kwargs = {'origin': collections.abc.Callable,
-                      'params': (..., typing.Optional[typing.Awaitable]),
-                      'special': True}
-        else:
-            kwargs = {'origin': collections.abc.Callable,
-                      'nparams': (..., typing.Optional[typing.Awaitable])}
-        super().__init__(**kwargs)
+        super().__init__(origin=collections.abc.Callable,
+                         nparams=(..., Awaitable | None))
 
     def __getitem__(self, params):
         if len(params) == 2:
-            params = (params[0], typing.Union[params[1],
-                                              typing.Awaitable[params[1]]])
+            params = params[0], params[1] | Awaitable[params[1]]
+
         return super().__getitem__(params)
 
 
 AsyncCallable = _AsyncCallableType()
 """Async callable"""
 
 
-async def call(fn: AsyncCallable, *args, **kwargs) -> typing.Any:
+async def call(fn: AsyncCallable, *args, **kwargs) -> Any:
     """Call a function or a coroutine (or other callable object).
 
     Call the `fn` with `args` and `kwargs`. If result of this call is
     awaitable, it is awaited and returned. Otherwise, result is immediately
     returned.
 
     Args:
@@ -157,15 +151,15 @@
 
     if inspect.isawaitable(result):
         result = await result
 
     return result
 
 
-async def call_on_cancel(fn: AsyncCallable, *args, **kwargs) -> typing.Any:
+async def call_on_cancel(fn: AsyncCallable, *args, **kwargs) -> Any:
     """Call a function or a coroutine when canceled.
 
     When canceled, `fn` is called with `args` and `kwargs` by using
     `call` coroutine.
 
     Args:
         fn: function or coroutine
@@ -187,18 +181,18 @@
     """
     with contextlib.suppress(asyncio.CancelledError):
         await asyncio.get_running_loop().create_future()
 
     return await call(fn, *args, *kwargs)
 
 
-async def call_on_done(f: typing.Awaitable,
+async def call_on_done(f: Awaitable,
                        fn: AsyncCallable,
                        *args, **kwargs
-                       ) -> typing.Any:
+                       ) -> Any:
     """Call a function or a coroutine when awaitable is done.
 
     When `f` is done, `fn` is called with `args` and `kwargs` by using
     `call` coroutine.
 
     If this coroutine is canceled before `f` is done, `f` is canceled and `fn`
     is not called.
@@ -227,15 +221,15 @@
     """
     with contextlib.suppress(Exception):
         await f
 
     return await call(fn, *args, *kwargs)
 
 
-def init_asyncio(policy: typing.Optional[asyncio.AbstractEventLoopPolicy] = None):  # NOQA
+def init_asyncio(policy: asyncio.AbstractEventLoopPolicy | None = None):
     """Initialize asyncio.
 
     Sets event loop policy (if ``None``, instance of
     `asyncio.DefaultEventLoopPolicy` is used).
 
     On Windows, `asyncio.WindowsProactorEventLoopPolicy` is used as default
     policy.
@@ -252,18 +246,18 @@
         #     return uvloop.EventLoopPolicy()
 
         return asyncio.DefaultEventLoopPolicy()
 
     asyncio.set_event_loop_policy(policy or get_default_policy())
 
 
-def run_asyncio(future: typing.Awaitable, *,
+def run_asyncio(future: Awaitable, *,
                 handle_signals: bool = True,
-                loop: typing.Optional[asyncio.AbstractEventLoop] = None
-                ) -> typing.Any:
+                loop: asyncio.AbstractEventLoop | None = None
+                ) -> Any:
     """Run asyncio loop until the `future` is completed and return the result.
 
     If `handle_signals` is ``True``, SIGINT and SIGTERM handlers are
     temporarily overridden. Instead of raising ``KeyboardInterrupt`` on every
     signal reception, Future is canceled only once. Additional signals are
     ignored. On Windows, SIGBREAK (CTRL_BREAK_EVENT) handler is also
     overridden.
```

## hat/aio/queue.py

```diff
@@ -1,11 +1,11 @@
+from typing import Any
 import asyncio
 import collections
 import contextlib
-import typing
 
 
 class QueueClosedError(Exception):
     """Raised when trying to use a closed queue."""
 
 
 class QueueEmptyError(Exception):
@@ -103,30 +103,30 @@
         if self._closed:
             return
 
         self._closed = True
         self._wakeup_all(self._putters)
         self._wakeup_next(self._getters)
 
-    def get_nowait(self) -> typing.Any:
+    def get_nowait(self) -> Any:
         """Return an item if one is immediately available, else raise
         `QueueEmptyError`.
 
         Raises:
             QueueEmptyError
 
         """
         if self.empty():
             raise QueueEmptyError()
 
         item = self._queue.popleft()
         self._wakeup_next(self._putters)
         return item
 
-    def put_nowait(self, item: typing.Any):
+    def put_nowait(self, item: Any):
         """Put an item into the queue without blocking.
 
         If no free slot is immediately available, raise `QueueFullError`.
 
         Raises:
             QueueFullError
 
@@ -136,15 +136,15 @@
 
         if self.full():
             raise QueueFullError()
 
         self._queue.append(item)
         self._wakeup_next(self._getters)
 
-    async def get(self) -> typing.Any:
+    async def get(self) -> Any:
         """Remove and return an item from the queue.
 
         If queue is empty, wait until an item is available.
 
         Raises:
             QueueClosedError
 
@@ -172,15 +172,15 @@
                     if not self.empty() or self._closed:
                         self._wakeup_next(self._getters)
 
                 raise
 
         return self.get_nowait()
 
-    async def put(self, item: typing.Any):
+    async def put(self, item: Any):
         """Put an item into the queue.
 
         If the queue is full, wait until a free slot is available before adding
         the item.
 
         Raises:
             QueueClosedError
@@ -204,15 +204,15 @@
                 if not self.full() and not putter.cancelled():
                     self._wakeup_next(self._putters)
 
                 raise
 
         return self.put_nowait(item)
 
-    async def get_until_empty(self) -> typing.Any:
+    async def get_until_empty(self) -> Any:
         """Empty the queue and return the last item.
 
         If queue is empty, wait until at least one item is available.
 
         Raises:
             QueueClosedError
 
@@ -220,15 +220,15 @@
         item = await self.get()
 
         while not self.empty():
             item = self.get_nowait()
 
         return item
 
-    def get_nowait_until_empty(self) -> typing.Any:
+    def get_nowait_until_empty(self) -> Any:
         """Empty the queue and return the last item if at least one
         item is immediately available, else raise `QueueEmptyError`.
 
         Raises:
             QueueEmptyError
 
         """
```

## hat/aio/wait.py

```diff
@@ -1,37 +1,37 @@
+from typing import Any, Awaitable
 import asyncio
-import typing
 
 from hat.aio.group import Group
 from hat.aio.misc import call_on_done, uncancellable
 
 
 class CancelledWithResultError(asyncio.CancelledError):
     """CancelledError with associated result or exception"""
 
     def __init__(self,
-                 result: typing.Optional[typing.Any],
-                 exception: typing.Optional[BaseException]):
+                 result: Any | None,
+                 exception: BaseException | None):
         super().__init__()
         self.__result = result
         self.__exception = exception
 
     @property
-    def result(self) -> typing.Optional[typing.Any]:
+    def result(self) -> Any | None:
         """Result"""
         return self.__result
 
     @property
-    def exception(self) -> typing.Optional[BaseException]:
+    def exception(self) -> BaseException | None:
         return self.__exception
 
 
-async def wait_for(obj: typing.Awaitable,
+async def wait_for(obj: Awaitable,
                    timeout: float
-                   ) -> typing.Any:
+                   ) -> Any:
     """"Wait for the awaitable object to complete, with timeout.
 
     Implementation `asyncio.wait_for` that ensure propagation of
     CancelledError.
 
     If task is cancelled with objects's result available, instead of
     returning result, this implementation raises `CancelledWithResultError`.
```

## Comparing `hat_aio-0.7.7.dist-info/LICENSE` & `hat_aio-0.7.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_aio-0.7.7.dist-info/METADATA` & `hat_aio-0.7.8.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,85 @@
 Metadata-Version: 2.1
 Name: hat-aio
-Version: 0.7.7
+Version: 0.7.8
 Summary: Hat async utility library
 Home-page: https://github.com/hat-open/hat-aio
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-hat-aio - Python async utility library
-======================================
+.. _online documentation: https://hat-aio.hat-open.com
+.. _git repository: https://github.com/hat-open/hat-aio.git
+.. _PyPI project: https://pypi.org/project/hat-aio
+.. _pydoit: https://pydoit.org
+.. _Hat Open: https://hat-open.com
+.. _Končar Digital: https://www.koncar.hr/en
 
-This library is part of Hat Open project - open-source framework of tools and
-libraries for developing applications used for remote monitoring, control and
-management of intelligent electronic devices such as IoT devices, PLCs,
-industrial automation or home automation systems.
 
-Development of Hat Open and associated repositories is sponsored by
-`Končar Digital <https://www.koncar.hr>`_.
+hat-aio - Python async utility library
+======================================
 
 For more information see:
 
-    * hat-aio documentation - `<https://hat-aio.hat-open.com>`_
-    * hat-aio git repository - `<https://github.com/hat-open/hat-aio.git>`_
-    * Hat Open homepage - `<https://hat-open.com>`_
+* `online documentation`_
+* `git repository`_
 
-.. warning::
 
-    This project is currently in state of active development. Features,
-    functionality and API are unstable.
+Runtime requirements
+--------------------
+
+* python >=3.10
 
 
 Install
 -------
 
-::
+`hat-aio` is available as `PyPI project`_::
 
     $ pip install hat-aio
 
 
+Build
+-----
+
+Build tool used for `hat-aio` is `pydoit`_. It can be installed together
+with other python dependencies by running::
+
+    $ pip install -r requirements.pip.dev.txt
+
+For listing available doit tasks, use::
+
+    $ doit list
+
+Default task::
+
+    $ doit
+
+creates wheel package inside `build` directory.
+
+
+Hat Open
+--------
+
+`hat-aio` is part of `Hat Open`_ project - open-source framework of tools
+and libraries for developing applications used for remote monitoring, control
+and management of intelligent electronic devices such as IoT devices, PLCs,
+industrial automation or home automation systems.
+
+Development of Hat Open and associated repositories is sponsored by
+`Končar Digital`_.
+
+
 License
 -------
 
-Copyright 2020-2022 Hat Open AUTHORS
+Copyright 2020-2023 Hat Open AUTHORS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

## Comparing `hat_aio-0.7.7.dist-info/RECORD` & `hat_aio-0.7.8.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 hat/aio/__init__.py,sha256=Z3B9BTS_iZs2sFBp5fACdyukMdoyWxHVF0FtaDaa1A4,1225
-hat/aio/executor.py,sha256=HS_CrkYfLs_s0iDtbeQ09ei_hmkkhWuynVYQ95kh1Jc,2761
-hat/aio/group.py,sha256=Lmmm_pjyrO2pwJStv7N-IZFPVMWbMYXImRWneJm1N4U,6903
-hat/aio/misc.py,sha256=Ej9MVuClHxeq7kEayqksXEs7x7Awll_wtG7mdbz1iIY,9360
-hat/aio/queue.py,sha256=lzY5vC9sPRaybScAzE2TEufU7LiksDcYYnR4tP_wQq0,6172
-hat/aio/wait.py,sha256=wfGKo_xN7AxAgMTsfzNZsopMWkfa6jGZLA3D4ODXvnc,1836
-hat_aio-0.7.7.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-hat_aio-0.7.7.dist-info/METADATA,sha256=tWVfSI6QI3U777YkQo-qOg7pJbXccwXCOue9ho_Bq0E,1794
-hat_aio-0.7.7.dist-info/WHEEL,sha256=zKyos-pqBEVcQ-3nRq9bZ7oUehzVzNUDkBNCZQtNcQ8,152
-hat_aio-0.7.7.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
-hat_aio-0.7.7.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-hat_aio-0.7.7.dist-info/RECORD,,
+hat/aio/executor.py,sha256=3eTTEansyggm6y64bR624OCD7_Q3WUmbPGVXOSkmZ60,2781
+hat/aio/group.py,sha256=a339T1_xowqAB16UWEHejmYVmzPRVUKVN0oXLwoZk-k,6887
+hat/aio/misc.py,sha256=yjBhM1rW16g8qwlFDX9A6wL1mLVbPqftgASqc8a1S8g,8928
+hat/aio/queue.py,sha256=_VHvzVG2zKI1vSiSsNkKwCjrD-6rkR7USUi2qBDIhVc,6139
+hat/aio/wait.py,sha256=ucMjyjyoyZKYBauZXcOfYOLpQItPCbSaj3HmmlpW9hs,1788
+hat_aio-0.7.8.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+hat_aio-0.7.8.dist-info/METADATA,sha256=rDdFxbIKe92290exfLYlLsc1YxUFTYH997iq-I-417A,2214
+hat_aio-0.7.8.dist-info/WHEEL,sha256=md_Sk-cFyicIH6eY_0BVqmsgC0wAFfbS1oq2bLoZiOk,114
+hat_aio-0.7.8.dist-info/top_level.txt,sha256=3RuRoRsaXQZNKwr3T2RE9XepBRTk4YpnXUbMiH5nes8,4
+hat_aio-0.7.8.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+hat_aio-0.7.8.dist-info/RECORD,,
```

