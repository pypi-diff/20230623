# Comparing `tmp/catline-0.0.1.tar.gz` & `tmp/catline-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catline-0.0.1.tar", last modified: Fri Jun 23 09:50:13 2023, max compression
+gzip compressed data, was "catline-0.0.2.tar", last modified: Fri Jun 23 10:29:25 2023, max compression
```

## Comparing `catline-0.0.1.tar` & `catline-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 09:50:13.287246 catline-0.0.1/
--rw-rw-rw-   0        0        0     1083 2023-06-23 08:23:30.000000 catline-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      127 2023-06-23 09:50:01.000000 catline-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3654 2023-06-23 09:50:13.287246 catline-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3149 2023-06-23 09:21:36.000000 catline-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 09:50:13.261365 catline-0.0.1/catline/
--rw-rw-rw-   0        0        0       79 2023-06-23 09:47:33.000000 catline-0.0.1/catline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:50:13.280732 catline-0.0.1/catline/__pycache__/
--rw-rw-rw-   0        0        0      346 2023-06-23 09:08:49.000000 catline-0.0.1/catline/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    25368 2023-06-23 09:08:49.000000 catline-0.0.1/catline/__pycache__/_version.cpython-311.pyc
--rw-rw-rw-   0        0        0    11028 2023-06-23 09:12:41.000000 catline-0.0.1/catline/__pycache__/queue.cpython-311.pyc
--rw-rw-rw-   0        0        0      416 2023-06-23 09:08:50.000000 catline-0.0.1/catline/__pycache__/utils.cpython-311.pyc
--rw-rw-rw-   0        0        0    24274 2023-06-23 08:45:38.000000 catline-0.0.1/catline/_version.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:50:13.283239 catline-0.0.1/catline/adapters/
--rw-rw-rw-   0        0        0        0 2023-06-23 08:38:38.000000 catline-0.0.1/catline/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:50:13.286245 catline-0.0.1/catline/adapters/__pycache__/
--rw-rw-rw-   0        0        0      197 2023-06-23 09:08:50.000000 catline-0.0.1/catline/adapters/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     7326 2023-06-23 09:08:50.000000 catline-0.0.1/catline/adapters/__pycache__/json_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0     4367 2023-06-23 09:05:34.000000 catline-0.0.1/catline/adapters/json_adapter.py
--rw-rw-rw-   0        0        0     3212 2023-06-23 08:45:36.000000 catline-0.0.1/catline/adapters/redis_adapter.py
--rw-rw-rw-   0        0        0     7163 2023-06-23 09:12:38.000000 catline-0.0.1/catline/queue.py
--rw-rw-rw-   0        0        0      238 2023-06-23 08:47:13.000000 catline-0.0.1/catline/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:50:13.274726 catline-0.0.1/catline.egg-info/
--rw-rw-rw-   0        0        0     3654 2023-06-23 09:50:13.000000 catline-0.0.1/catline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      704 2023-06-23 09:50:13.000000 catline-0.0.1/catline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 09:50:13.000000 catline-0.0.1/catline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-23 09:50:13.000000 catline-0.0.1/catline.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-23 09:50:13.000000 catline-0.0.1/catline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-06-23 08:30:55.000000 catline-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       12 2023-06-23 08:26:35.000000 catline-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      204 2023-06-23 09:50:13.295374 catline-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1071 2023-06-23 09:49:34.000000 catline-0.0.1/setup.py
--rw-rw-rw-   0        0        0    83607 2023-06-23 08:31:03.000000 catline-0.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:25.830224 catline-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 10:29:11.000000 catline-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 10:29:11.000000 catline-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-23 10:29:25.830224 catline-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-23 10:29:11.000000 catline-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:25.830224 catline-0.0.2/catline/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 10:29:11.000000 catline-0.0.2/catline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-23 10:29:25.830224 catline-0.0.2/catline/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:25.830224 catline-0.0.2/catline/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:11.000000 catline-0.0.2/catline/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-23 10:29:11.000000 catline-0.0.2/catline/adapters/json_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-23 10:29:11.000000 catline-0.0.2/catline/adapters/redis_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-06-23 10:29:11.000000 catline-0.0.2/catline/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-23 10:29:11.000000 catline-0.0.2/catline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:29:25.830224 catline-0.0.2/catline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-23 10:29:25.000000 catline-0.0.2/catline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-23 10:29:25.000000 catline-0.0.2/catline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:29:25.000000 catline-0.0.2/catline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 10:29:25.000000 catline-0.0.2/catline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 10:29:25.000000 catline-0.0.2/catline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 10:29:11.000000 catline-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 10:29:11.000000 catline-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-23 10:29:25.830224 catline-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-23 10:29:11.000000 catline-0.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-23 10:29:11.000000 catline-0.0.2/versioneer.py
```

### Comparing `catline-0.0.1/LICENSE` & `catline-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 yupix
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 yupix
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `catline-0.0.1/PKG-INFO` & `catline-0.0.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,90 +1,73 @@
-Metadata-Version: 2.1
-Name: catline
-Version: 0.0.1
-Summary: Simple job queue
-Home-page: https://github.com/yupix/catline
-Author: yupix
-Author-email: yupi0982@outlook.jp
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Natural Language :: Japanese
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11, <4.0
-Description-Content-Type: text/markdown
-Provides-Extra: redis
-License-File: LICENSE
-
-# CatLine
-
-このプロジェクトは簡易的な非同期 ジョブキューを実装するための物です。
-
-## 注意事項
-
-- `threading` を用いた並列処理はサポート・テストしていません
-- `Queue` クラスは イベントループ作成後にインスタンス化してください。
-- 優先度は 0 ~ 9 であり、 0に近づくほど優先度が高くなります。
-
-## 使い方
-
-以下が例になります。
-このコードの意味をまとめると以下のようになります
-- ジョブが実行された際に引数で渡されたジョブの名前で `meow` と出力する
-- 優先度が0のcatには `VIP` を戦闘につけ、それ以外のcatは `normal` をつける
-- 待機中のジョブが0になった際にループを終了し、キューを停止させる
-
-
-```py
-import asyncio
-import random
-from catline.adapters.json_adapter import QueueStorageJSONAdapter
-from catline.queue import Queue
-
-async def say_meow(cat_name: str):
-    print(f'{cat_name}: meow' + '!' * random.randrange(1,10))
-
-
-async def main():
-    cat_queue = Queue('cat',  QueueStorageJSONAdapter(), say_meow)
-    cat_queue.run()
-    for i in range(random.randrange(1, 20)):
-        priority = random.randrange(0, 9)
-        await cat_queue.add(priority, f'{"VIP" if priority == 0 else "normal"} cat{i}') # type: ignore
-    while True:
-        waiting_cat_number = await cat_queue.count_jobs('waiting')
-        print(f'waiting cat number: {waiting_cat_number}')
-        await asyncio.sleep(1)
-        if waiting_cat_number == 0:
-            break
-    cat_queue.stop()
-    print('finish!!!')
-
-if __name__ == '__main__':
-    asyncio.run(main())
-
-```
-
-## 実装予定の機能
-
-|機能|説明|状態|
-|---|---|---|
-|ジョブの追加|ジョブをキューに追加できる|〇|
-|ジョブの実行|キューにあるジョブをスケジューラーで実行できる|〇|
-|ジョブのリトライ|ジョブが失敗した際に再実行できる|×|
-|ジョブの優先度|ジョブを追加する際優先度を指定できる|〇|
-|スケジューラーの実行間隔|スケジューラーがジョブを実行するまでの間隔を変更できる|〇|
-|キューストレージの変更|キューをredisやjsonに保存する際自分でadapterを作れる|〇|
-|threadingのサポート|並列処理のサポート|×|
-|実行するジョブの上限変更|同時に実行できるジョブの数を変更できる|〇|
-
-## ストレージを自分で作成する方法
-
-このプロジェクトではキューのジョブを保存するためのクラスをアダプターパターンで作成しているため、それに沿ってクラスを作成すれば作成が可能です。
-
-また、デフォルトで `json` 又は `redis` を用いた保存方法がライブラリに同封されているため、特段理由が無い場合はそちらを使うことを推奨します。
-
-### 注意点
-
-1. ジョブを取得する際に優先度順に取得するなどといった処理を自分で作成する必要があります。
-
-
+# CatLine
+
+このプロジェクトは簡易的な非同期 ジョブキューを実装するための物です。
+
+## 注意事項
+
+- `threading` を用いた並列処理はサポート・テストしていません
+- `Queue` クラスは イベントループ作成後にインスタンス化してください。
+- 優先度は 0 ~ 9 であり、 0に近づくほど優先度が高くなります。
+
+## 使い方
+
+以下が例になります。
+このコードの意味をまとめると以下のようになります
+- ジョブが実行された際に引数で渡されたジョブの名前で `meow` と出力する
+- 優先度が0のcatには `VIP` を先頭につけ、それ以外のcatは `normal` をつける
+- 待機中のジョブが0になった際にループを終了し、キューを停止させる
+
+
+```py
+import asyncio
+import random
+from catline.adapters.json_adapter import QueueStorageJSONAdapter
+from catline.queue import Queue
+
+async def say_meow(cat_name: str):
+    print(f'{cat_name}: meow' + '!' * random.randrange(1,10))
+
+
+async def main():
+    cat_queue = Queue('cat',  QueueStorageJSONAdapter(), say_meow)
+    cat_queue.run()
+    for i in range(random.randrange(1, 20)):
+        priority = random.randrange(0, 9)
+        await cat_queue.add(priority, f'{"VIP" if priority == 0 else "normal"} cat{i}') # type: ignore
+    while True:
+        waiting_cat_number = await cat_queue.count_jobs('waiting')
+        print(f'waiting cat number: {waiting_cat_number}')
+        await asyncio.sleep(1)
+        if waiting_cat_number == 0:
+            break
+    cat_queue.stop()
+    print('finish!!!')
+
+if __name__ == '__main__':
+    asyncio.run(main())
+
+```
+
+## 実装予定の機能
+
+|機能|説明|状態|
+|---|---|---|
+|ジョブの追加|ジョブをキューに追加できる|〇|
+|ジョブの実行|キューにあるジョブをスケジューラーで実行できる|〇|
+|ジョブのリトライ|ジョブが失敗した際に再実行できる|×|
+|ジョブの優先度|ジョブを追加する際優先度を指定できる|〇|
+|スケジューラーの実行間隔|スケジューラーがジョブを実行するまでの間隔を変更できる|〇|
+|キューストレージの変更|キューをredisやjsonに保存する際自分でadapterを作れる|〇|
+|threadingのサポート|並列処理のサポート|×|
+|実行するジョブの上限変更|同時に実行できるジョブの数を変更できる|〇|
+
+## ストレージを自分で作成する方法
+
+このプロジェクトではキューのジョブを保存するためのクラスをアダプターパターンで作成しているため、それに沿ってクラスを作成すれば作成が可能です。
+
+また、デフォルトで `json` 又は `redis` を用いた保存方法がライブラリに同封されているため、特段理由が無い場合はそちらを使うことを推奨します。
+
+### 注意点
+
+1. ジョブを取得する際に優先度順に取得するなどといった処理を自分で作成する必要があります。
+
+
```

### Comparing `catline-0.0.1/catline/adapters/redis_adapter.py` & `catline-0.0.2/catline/adapters/redis_adapter.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-import json
-from typing import Any
-from catline.queue import (
-    JOB_PRIORITIES,
-    GetJobsResult,
-    IFQueueStorageAdapter,
-    IJob,
-    JobPriority,
-    QueueKey,
-    QueueStatus,
-)
-
-try:
-    import redis.asyncio  # type: ignore
-except ModuleNotFoundError:
-    HAS_REDIS = False
-else:
-    HAS_REDIS = True
-
-
-class QueueStorageRedisAdapter(IFQueueStorageAdapter):
-    def __init__(self, **kwargs) -> None:
-        if HAS_REDIS is False:
-            raise Exception("Redis has not installed.")
-        self.redis_connection = redis.asyncio.Redis(**kwargs)
-
-    async def add_job(self, key: QueueKey, *args, **kwargs):
-        data: IJob = {
-            "args": args,
-            "identifier": key.identifier,
-            "kwargs": kwargs,
-            "name": key.name,
-            "priority": key.priority,
-            "status": key.status,
-        }  # type: ignore
-        await self.redis_connection.set(key.code, json.dumps(data, ensure_ascii=False))
-
-    async def get_jobs(
-        self, name: str, limit: int, status: QueueStatus
-    ) -> list[GetJobsResult]:
-        result: list[GetJobsResult] = []
-        for priority in JOB_PRIORITIES:
-            if len(result) == limit:
-                break
-            async for _key in self.redis_connection.scan_iter(
-                f"{priority}:{status}:{name}:*"
-            ):
-                key = _key.decode("utf-8")
-                value: str | None = await self.redis_connection.get(key)
-
-                assert value  # 普通あるはず
-
-                _value: IJob = json.loads(value)
-                result.append(
-                    GetJobsResult(
-                        key=key,
-                        args=_value["args"],
-                        kwargs=_value["kwargs"],
-                        status=_value["status"],
-                        identifier=_value["identifier"],
-                        priority=_value["priority"],
-                    )
-                )
-        return result
-
-    async def complete_job(self, name: str, key: QueueKey):
-        ...
-        # await redis_connection.delete(key)
-
-    async def count_jobs(self, name: str, status: QueueStatus) -> int:
-        count = 0
-        keys = []
-        async for key in self.redis_connection.scan_iter(f"*:{status}:{name}:*"):
-            count = count + 1
-            keys.append(key)
-        return count
-
-    async def update_status(
-        self,
-        key: QueueKey,
-        name: str,
-        status: QueueStatus,
-        priority: JobPriority | None = None,
-    ):
-        new_priority = priority if priority else key.priority
-        raw_data = await self.redis_connection.get(key.code)
-        await self.redis_connection.delete(key.code)
-        if raw_data is None:
-            raise Exception(f"指定されたジョブ: {key.code} は存在しません")
-        data: IJob = json.loads(raw_data)
-        data["priority"] = new_priority  # type: ignore
-        data["status"] = status
-        await key.update(status=status, priority=new_priority)  # type: ignore
-        await self.redis_connection.set(key.code, json.dumps(data, ensure_ascii=False))
+import json
+from typing import Any
+from catline.queue import (
+    JOB_PRIORITIES,
+    GetJobsResult,
+    IFQueueStorageAdapter,
+    IJob,
+    JobPriority,
+    QueueKey,
+    QueueStatus,
+)
+
+try:
+    import redis.asyncio  # type: ignore
+except ModuleNotFoundError:
+    HAS_REDIS = False
+else:
+    HAS_REDIS = True
+
+
+class QueueStorageRedisAdapter(IFQueueStorageAdapter):
+    def __init__(self, **kwargs) -> None:
+        if HAS_REDIS is False:
+            raise Exception("Redis has not installed.")
+        self.redis_connection = redis.asyncio.Redis(**kwargs)
+
+    async def add_job(self, key: QueueKey, *args, **kwargs):
+        data: IJob = {
+            "args": args,
+            "identifier": key.identifier,
+            "kwargs": kwargs,
+            "name": key.name,
+            "priority": key.priority,
+            "status": key.status,
+        }  # type: ignore
+        await self.redis_connection.set(key.code, json.dumps(data, ensure_ascii=False))
+
+    async def get_jobs(
+        self, name: str, limit: int, status: QueueStatus
+    ) -> list[GetJobsResult]:
+        result: list[GetJobsResult] = []
+        for priority in JOB_PRIORITIES:
+            if len(result) == limit:
+                break
+            async for _key in self.redis_connection.scan_iter(
+                f"{priority}:{status}:{name}:*"
+            ):
+                key = _key.decode("utf-8")
+                value: str | None = await self.redis_connection.get(key)
+
+                assert value  # 普通あるはず
+
+                _value: IJob = json.loads(value)
+                result.append(
+                    GetJobsResult(
+                        key=key,
+                        args=_value["args"],
+                        kwargs=_value["kwargs"],
+                        status=_value["status"],
+                        identifier=_value["identifier"],
+                        priority=_value["priority"],
+                    )
+                )
+        return result
+
+    async def complete_job(self, name: str, key: QueueKey):
+        ...
+        # await redis_connection.delete(key)
+
+    async def count_jobs(self, name: str, status: QueueStatus) -> int:
+        count = 0
+        keys = []
+        async for key in self.redis_connection.scan_iter(f"*:{status}:{name}:*"):
+            count = count + 1
+            keys.append(key)
+        return count
+
+    async def update_status(
+        self,
+        key: QueueKey,
+        name: str,
+        status: QueueStatus,
+        priority: JobPriority | None = None,
+    ):
+        new_priority = priority if priority else key.priority
+        raw_data = await self.redis_connection.get(key.code)
+        await self.redis_connection.delete(key.code)
+        if raw_data is None:
+            raise Exception(f"指定されたジョブ: {key.code} は存在しません")
+        data: IJob = json.loads(raw_data)
+        data["priority"] = new_priority  # type: ignore
+        data["status"] = status
+        await key.update(status=status, priority=new_priority)  # type: ignore
+        await self.redis_connection.set(key.code, json.dumps(data, ensure_ascii=False))
```

### Comparing `catline-0.0.1/catline.egg-info/PKG-INFO` & `catline-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-Metadata-Version: 2.1
-Name: catline
-Version: 0.0.1
-Summary: Simple job queue
-Home-page: https://github.com/yupix/catline
-Author: yupix
-Author-email: yupi0982@outlook.jp
-License: MIT
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Natural Language :: Japanese
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.11, <4.0
-Description-Content-Type: text/markdown
-Provides-Extra: redis
-License-File: LICENSE
-
-# CatLine
-
-このプロジェクトは簡易的な非同期 ジョブキューを実装するための物です。
-
-## 注意事項
-
-- `threading` を用いた並列処理はサポート・テストしていません
-- `Queue` クラスは イベントループ作成後にインスタンス化してください。
-- 優先度は 0 ~ 9 であり、 0に近づくほど優先度が高くなります。
-
-## 使い方
-
-以下が例になります。
-このコードの意味をまとめると以下のようになります
-- ジョブが実行された際に引数で渡されたジョブの名前で `meow` と出力する
-- 優先度が0のcatには `VIP` を戦闘につけ、それ以外のcatは `normal` をつける
-- 待機中のジョブが0になった際にループを終了し、キューを停止させる
-
-
-```py
-import asyncio
-import random
-from catline.adapters.json_adapter import QueueStorageJSONAdapter
-from catline.queue import Queue
-
-async def say_meow(cat_name: str):
-    print(f'{cat_name}: meow' + '!' * random.randrange(1,10))
-
-
-async def main():
-    cat_queue = Queue('cat',  QueueStorageJSONAdapter(), say_meow)
-    cat_queue.run()
-    for i in range(random.randrange(1, 20)):
-        priority = random.randrange(0, 9)
-        await cat_queue.add(priority, f'{"VIP" if priority == 0 else "normal"} cat{i}') # type: ignore
-    while True:
-        waiting_cat_number = await cat_queue.count_jobs('waiting')
-        print(f'waiting cat number: {waiting_cat_number}')
-        await asyncio.sleep(1)
-        if waiting_cat_number == 0:
-            break
-    cat_queue.stop()
-    print('finish!!!')
-
-if __name__ == '__main__':
-    asyncio.run(main())
-
-```
-
-## 実装予定の機能
-
-|機能|説明|状態|
-|---|---|---|
-|ジョブの追加|ジョブをキューに追加できる|〇|
-|ジョブの実行|キューにあるジョブをスケジューラーで実行できる|〇|
-|ジョブのリトライ|ジョブが失敗した際に再実行できる|×|
-|ジョブの優先度|ジョブを追加する際優先度を指定できる|〇|
-|スケジューラーの実行間隔|スケジューラーがジョブを実行するまでの間隔を変更できる|〇|
-|キューストレージの変更|キューをredisやjsonに保存する際自分でadapterを作れる|〇|
-|threadingのサポート|並列処理のサポート|×|
-|実行するジョブの上限変更|同時に実行できるジョブの数を変更できる|〇|
-
-## ストレージを自分で作成する方法
-
-このプロジェクトではキューのジョブを保存するためのクラスをアダプターパターンで作成しているため、それに沿ってクラスを作成すれば作成が可能です。
-
-また、デフォルトで `json` 又は `redis` を用いた保存方法がライブラリに同封されているため、特段理由が無い場合はそちらを使うことを推奨します。
-
-### 注意点
-
-1. ジョブを取得する際に優先度順に取得するなどといった処理を自分で作成する必要があります。
-
-
+Metadata-Version: 2.1
+Name: catline
+Version: 0.0.2
+Summary: Simple job queue
+Home-page: https://github.com/yupix/catline
+Author: yupix
+Author-email: yupi0982@outlook.jp
+License: MIT
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Natural Language :: Japanese
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.11, <4.0
+Description-Content-Type: text/markdown
+Provides-Extra: redis
+License-File: LICENSE
+
+# CatLine
+
+このプロジェクトは簡易的な非同期 ジョブキューを実装するための物です。
+
+## 注意事項
+
+- `threading` を用いた並列処理はサポート・テストしていません
+- `Queue` クラスは イベントループ作成後にインスタンス化してください。
+- 優先度は 0 ~ 9 であり、 0に近づくほど優先度が高くなります。
+
+## 使い方
+
+以下が例になります。
+このコードの意味をまとめると以下のようになります
+- ジョブが実行された際に引数で渡されたジョブの名前で `meow` と出力する
+- 優先度が0のcatには `VIP` を先頭につけ、それ以外のcatは `normal` をつける
+- 待機中のジョブが0になった際にループを終了し、キューを停止させる
+
+
+```py
+import asyncio
+import random
+from catline.adapters.json_adapter import QueueStorageJSONAdapter
+from catline.queue import Queue
+
+async def say_meow(cat_name: str):
+    print(f'{cat_name}: meow' + '!' * random.randrange(1,10))
+
+
+async def main():
+    cat_queue = Queue('cat',  QueueStorageJSONAdapter(), say_meow)
+    cat_queue.run()
+    for i in range(random.randrange(1, 20)):
+        priority = random.randrange(0, 9)
+        await cat_queue.add(priority, f'{"VIP" if priority == 0 else "normal"} cat{i}') # type: ignore
+    while True:
+        waiting_cat_number = await cat_queue.count_jobs('waiting')
+        print(f'waiting cat number: {waiting_cat_number}')
+        await asyncio.sleep(1)
+        if waiting_cat_number == 0:
+            break
+    cat_queue.stop()
+    print('finish!!!')
+
+if __name__ == '__main__':
+    asyncio.run(main())
+
+```
+
+## 実装予定の機能
+
+|機能|説明|状態|
+|---|---|---|
+|ジョブの追加|ジョブをキューに追加できる|〇|
+|ジョブの実行|キューにあるジョブをスケジューラーで実行できる|〇|
+|ジョブのリトライ|ジョブが失敗した際に再実行できる|×|
+|ジョブの優先度|ジョブを追加する際優先度を指定できる|〇|
+|スケジューラーの実行間隔|スケジューラーがジョブを実行するまでの間隔を変更できる|〇|
+|キューストレージの変更|キューをredisやjsonに保存する際自分でadapterを作れる|〇|
+|threadingのサポート|並列処理のサポート|×|
+|実行するジョブの上限変更|同時に実行できるジョブの数を変更できる|〇|
+
+## ストレージを自分で作成する方法
+
+このプロジェクトではキューのジョブを保存するためのクラスをアダプターパターンで作成しているため、それに沿ってクラスを作成すれば作成が可能です。
+
+また、デフォルトで `json` 又は `redis` を用いた保存方法がライブラリに同封されているため、特段理由が無い場合はそちらを使うことを推奨します。
+
+### 注意点
+
+1. ジョブを取得する際に優先度順に取得するなどといった処理を自分で作成する必要があります。
+
+
```

### Comparing `catline-0.0.1/versioneer.py` & `catline-0.0.2/versioneer.py`

 * *Files identical despite different names*

