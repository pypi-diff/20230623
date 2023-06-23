# Comparing `tmp/qps_limit-1.0.0-py3-none-any.whl.zip` & `tmp/qps_limit-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 4673 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       75 b- defN 23-Jun-22 12:21 qps_limit/__init__.py
--rw-rw-r--  2.0 unx     9714 b- defN 23-Jun-22 12:18 qps_limit/limiter.py
--rw-rw-r--  2.0 unx     2515 b- defN 23-Jun-22 12:22 qps_limit-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 12:22 qps_limit-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-22 12:22 qps_limit-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-22 12:22 qps_limit-1.0.0.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      547 b- defN 23-Jun-22 12:22 qps_limit-1.0.0.dist-info/RECORD
-7 files, 12954 bytes uncompressed, 3697 bytes compressed:  71.5%
+Zip file size: 4964 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx      165 b- defN 23-Jun-23 02:21 qps_limit/__init__.py
+-rw-rw-r--  2.0 unx     4665 b- defN 23-Jun-23 02:19 qps_limit/limiter.py
+-rw-rw-r--  2.0 unx     4335 b- defN 23-Jun-23 02:19 qps_limit/run.py
+-rw-rw-r--  2.0 unx     2489 b- defN 23-Jun-23 02:26 qps_limit-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 02:26 qps_limit-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-23 02:26 qps_limit-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-23 02:26 qps_limit-1.0.1.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      621 b- defN 23-Jun-23 02:26 qps_limit-1.0.1.dist-info/RECORD
+8 files, 12378 bytes uncompressed, 3880 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: qps_limit/__init__.py
 Comment: 
 
 Filename: qps_limit/limiter.py
 Comment: 
 
-Filename: qps_limit-1.0.0.dist-info/METADATA
+Filename: qps_limit/run.py
 Comment: 
 
-Filename: qps_limit-1.0.0.dist-info/WHEEL
+Filename: qps_limit-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-1.0.0.dist-info/top_level.txt
+Filename: qps_limit-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-1.0.0.dist-info/zip-safe
+Filename: qps_limit-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-1.0.0.dist-info/RECORD
+Filename: qps_limit-1.0.1.dist-info/zip-safe
+Comment: 
+
+Filename: qps_limit-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,5 +1,10 @@
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
+from .run import batch_run, async_batch_run
 from .limiter import Limiter
 
-__all__ = ['Limiter']
+__all__ = [
+    'batch_run',
+    'async_batch_run',
+    'Limiter'
+]
```

## qps_limit/limiter.py

```diff
@@ -1,216 +1,67 @@
-import asyncio
 import collections
 import itertools
 import math
 import multiprocessing
 import time
-from typing import Any, Callable, Coroutine, Dict, Iterable, Optional, Tuple
+from typing import Any, Callable, Coroutine, Optional
 
-from aiolimiter import AsyncLimiter
 from tqdm import tqdm
 
-
-def get_limiter(max_qps: float):
-    time_period = 0.1
-    max_rate = max_qps * time_period
-    if max_rate < 1:
-        time_period = time_period / max_rate
-        max_rate = 1
-    return AsyncLimiter(max_rate=max_rate, time_period=time_period)
-
-
-async def async_batch_run(
-    func: Callable[..., Coroutine[Any, Any, Any]],
-    idxs: Iterable[int],
-    params: Iterable[Tuple[Tuple, Dict]],
-    max_qps: Optional[float],
-    *,
-    max_workers: int = 128,
-    callback: Callable = None,
-    progress_queue: multiprocessing.Queue = None
-):
-    if max_qps is not None:
-        limiter = get_limiter(max_qps)
-
-        async def limited_func(*args, **kwargs):
-            async with limiter:
-                return await func(*args, **kwargs)
-    else:
-        limited_func = func
-
-    async def callback_func(*args, **kwargs):
-        if callback:
-            return callback(await limited_func(*args, **kwargs))
-        else:
-            return await limited_func(*args, **kwargs)
-
-    result = []
-    queue = asyncio.Queue()
-    jobs_cnt = 0
-
-    for idx, param in zip(idxs, params):
-        await queue.put((idx, param))
-        jobs_cnt += 1
-
-    async def worker():
-        while not queue.empty():
-            _idx, _param = await queue.get()
-            result.append((_idx, await callback_func(*_param[0], **_param[1])))
-            if progress_queue:
-                progress_queue.put_nowait(1)
-
-    await asyncio.gather(*[worker() for _ in range(max_workers)])
-    assert len(result) == jobs_cnt
-    return result
-
-
-def batch_run(
-    func: Callable[..., Coroutine[Any, Any, Any]],
-    idxs: Iterable[int],
-    params: Iterable[Tuple[Tuple, Dict]],
-    max_qps: Optional[float],
-    *,
-    max_workers: int = 128,
-    callback: Callable = None,
-    progress_queue: multiprocessing.Queue = None
-):
-    return asyncio.get_event_loop().run_until_complete(async_batch_run(**locals()))
-
-
-async def async_streaming_batch_run(
-    func: Callable[..., Coroutine[Any, Any, Any]],
-    idxs: Iterable[int],
-    params: Iterable[Tuple[Tuple, Dict]],
-    max_qps: Optional[float],
-    *,
-    max_workers: int = 128,
-    callback: Callable = None,
-    progress_queue: multiprocessing.Queue = None
-):
-    if max_qps is not None:
-        limiter = get_limiter(max_qps)
-
-        async def limited_func(*args, **kwargs):
-            async with limiter:
-                return await func(*args, **kwargs)
-    else:
-        limited_func = func
-
-    async def callback_func(*args, **kwargs):
-        if callback:
-            return callback(await limited_func(*args, **kwargs))
-        else:
-            return await limited_func(*args, **kwargs)
-
-    queue = asyncio.Queue()
-    result = asyncio.Queue()
-    jobs_cnt = 0
-
-    for idx, param in zip(idxs, params):
-        await queue.put((idx, param))
-        jobs_cnt += 1
-
-    async def worker():
-        while not queue.empty():
-            _idx, _param = await queue.get()
-            _res = await callback_func(*_param[0], **_param[1])
-            await result.put((_idx, _res))
-            if progress_queue:
-                progress_queue.put_nowait(1)
-
-    asyncio.gather(*[worker() for _ in range(max_workers)])
-    jobs_consume = 0
-    while jobs_consume < jobs_cnt:
-        yield await result.get()
-        jobs_consume += 1
-    assert jobs_consume == jobs_cnt
-
-
-def streaming_batch_run(
-    func: Callable[..., Coroutine[Any, Any, Any]],
-    idxs: Iterable[int],
-    params: Iterable[Tuple[Tuple, Dict]],
-    max_qps: Optional[float],
-    *,
-    max_workers: int = 128,
-    callback: Callable = None,
-    progress_queue: multiprocessing.Queue = None
-):
-    async_generator = async_streaming_batch_run(**locals())
-
-    def iter_over_async(ait, loop):
-        ait = ait.__aiter__()
-
-        async def get_next():
-            try:
-                return False, await ait.__anext__()
-            except StopAsyncIteration:
-                return True, None
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-    loop = asyncio.get_event_loop()
-    sync_generator = iter_over_async(async_generator, loop)
-    return sync_generator
+from .run import batch_run, streaming_batch_run
 
 
 class Limiter():
 
     def __init__(
         self,
         func: Callable[..., Coroutine[Any, Any, Any]],
         params: Callable,
         num_workers: int = 1,
-        worker_max_qps: float = None,
+        worker_max_qps: Optional[float] = None,
         streaming: bool = False,
-        callback: Callable = None,
+        callback: Optional[Callable] = None,
         progress: bool = True,
         ordered: bool = True,
-        verbose: bool = False
+        verbose: bool = False,
+        max_workers: int = 128,
+        warmup_steps: int = 1
     ) -> Callable:
         self.func = func
         self.params = params
         self.num_workers = num_workers
         self.worker_max_qps = worker_max_qps
         self.streaming = streaming
         self.callback = callback
         self.progress = progress
         self.ordered = ordered
         self.verbose = verbose
 
         self.count_iterator, self.param_iterator = itertools.tee(self.params(), 2)
-        self.count = 0
         counter = itertools.count()
         collections.deque(zip(self.count_iterator, counter), maxlen=0)
         self.count = next(counter)
 
-        self.param_iterator, warmup_param_iterator = itertools.tee(self.param_iterator)
-        warmup_cnt = 1
-        warmup_idx_iterator = (i for i in range(warmup_cnt))
-        warmup_param_iterator = itertools.islice(warmup_param_iterator, warmup_cnt)
+        self.param_iterator, warmup_param_iterator = itertools.tee(self.param_iterator, 2)
+        warmup_param_iterator = itertools.islice(warmup_param_iterator, warmup_steps)
         warmup_start_time = time.time()
         if self.verbose:
-            print("warm up workers with {} data".format(warmup_cnt))
+            print("warm up workers with {} data".format(warmup_steps))
         batch_run(
             func=self.func,
-            idxs=warmup_idx_iterator,
             params=warmup_param_iterator,
             max_qps=None,
             max_workers=1
         )
         warmup_end_time = time.time()
-        avg_worker_time = (warmup_end_time - warmup_start_time) / warmup_cnt
-        max_workers_num = 128
+        avg_worker_time = (warmup_end_time - warmup_start_time) / warmup_steps
         if self.worker_max_qps is None:
-            self.max_workers = max_workers_num
+            self.max_workers = max_workers
         else:
-            self.max_workers = min(max_workers_num, self.worker_max_qps * math.ceil(avg_worker_time))
+            self.max_workers = min(max_workers, self.worker_max_qps * math.ceil(avg_worker_time))
         if self.verbose:
             print("avg worker time: {:.2f}s -> set worker num: {}".format(avg_worker_time, self.max_workers))
 
         if self.ordered:
             self.dict = multiprocessing.Manager().dict()
         else:
             self.queue = multiprocessing.Queue()
@@ -229,55 +80,34 @@
             self.workers.append(multiprocessing.Process(target=_progress_worker, args=()))
         else:
             self.progress_queue = None
 
         for mod in range(self.num_workers):
             self.workers.append(multiprocessing.Process(target=self._worker, args=(mod,)))
 
-    def _worker(self, mod):
-        def make_iterators():
-            def iterator():
-                for idx, (args, kwargs) in enumerate(self.param_iterator):
-                    if idx % self.num_workers == mod:
-                        yield idx, (args, kwargs)
-            a_iter, b_iter = itertools.tee(iterator(), 2)
-            return (a for a, _ in a_iter), (b for _, b in b_iter)
-
-        idx_iterator, param_iterator = make_iterators()
-
-        if not self.streaming:
-            results = batch_run(
-                func=self.func,
-                idxs=idx_iterator,
-                params=param_iterator,
-                max_qps=self.worker_max_qps,
-                max_workers=self.max_workers,
-                callback=self.callback,
-                progress_queue=self.progress_queue
-            )
-            for idx, res in results:
-                if self.ordered:
-                    self.dict[idx] = res
-                else:
-                    self.queue.put((idx, res))
-        else:
-            result_iterator = streaming_batch_run(
-                func=self.func,
-                idxs=idx_iterator,
-                params=param_iterator,
-                max_qps=self.worker_max_qps,
-                max_workers=self.max_workers,
-                callback=self.callback,
-                progress_queue=self.progress_queue
-            )
-            for idx, res in result_iterator:
-                if self.ordered:
-                    self.dict[idx] = res
-                else:
-                    self.queue.put((idx, res))
+    def _worker(self, mod: int):
+        def make_worker_iterator():
+            for idx, (args, kwargs) in enumerate(self.param_iterator):
+                if idx % self.num_workers == mod:
+                    yield args, kwargs
+
+        batch_run_func = batch_run if not self.streaming else streaming_batch_run
+        for idx, res in batch_run_func(
+            func=self.func,
+            params=make_worker_iterator(),
+            max_qps=self.worker_max_qps,
+            max_workers=self.max_workers,
+            callback=self.callback,
+            progress_queue=self.progress_queue
+        ):
+            real_idx = idx * self.num_workers + mod
+            if self.ordered:
+                self.dict[real_idx] = res
+            else:
+                self.queue.put((real_idx, res))
 
     def __call__(self):
         start_time = time.time()
         for worker in self.workers:
             worker.start()
         consume = 0
         while consume < self.count:
```

## Comparing `qps_limit-1.0.0.dist-info/METADATA` & `qps_limit-1.0.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 1.0.0
+Version: 1.0.1
 Summary: Run functions under any limited rate
-Home-page: https://github.com/antct/rate-limit
+Home-page: https://github.com/antct/qps-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -15,38 +15,38 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Requires-Dist: aiolimiter
 
-## Rate Limit
+## QPS Limit
 
 Run functions under any limited rate using `multiprocessing` + `asyncio`
 
 ### Installation
 
 ```bash
 pip install qps-limit
 ```
 
 or install manually via git
 
 ```bash
-git clone git://github.com/antct/rate-limit.git rate-limit
-cd rate-limit
+git clone git://github.com/antct/qps-limit.git qps-limit
+cd qps-limit
 python setup.py install
 ```
 
 ### Usage
 
 ```python
-from qps_limit import MWrapper
+from qps_limit import Limiter
 
-f = MWrapper(
+f = Limiter(
     func="an asynchronous function",
     params="a generator function yields args and kwargs",
     num_workers="number of processes, recommended <= number of CPUs",
     worker_max_qps="maximum qps per process, None means unlimited",
     streaming="stream data processing, useful when the memory is limited",
     callback="a callback function that handles the return values of func",
     progress="display a progress bar",
@@ -85,14 +85,13 @@
     func=func,
     params=params,
     num_workers=10,
     worker_max_qps=10,
     streaming=False,
     callback=callback,
     progress=True,
-    ordered=True,
-    verbose=False
+    ordered=True
 )
 
 for idx, r in f():
     print(idx, r)
 ```
```

