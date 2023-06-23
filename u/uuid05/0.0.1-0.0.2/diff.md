# Comparing `tmp/uuid05-0.0.1.tar.gz` & `tmp/uuid05-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uuid05-0.0.1.tar", last modified: Fri Jun 23 17:50:00 2023, max compression
+gzip compressed data, was "uuid05-0.0.2.tar", last modified: Fri Jun 23 18:58:03 2023, max compression
```

## Comparing `uuid05-0.0.1.tar` & `uuid05-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 17:50:00.575182 uuid05-0.0.1/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1097 2023-06-23 16:59:40.000000 uuid05-0.0.1/LICENSE
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4445 2023-06-23 17:50:00.575182 uuid05-0.0.1/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4070 2023-06-23 17:48:17.000000 uuid05-0.0.1/README.md
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 17:50:00.575182 uuid05-0.0.1/cli/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      962 2023-06-23 17:33:16.000000 uuid05-0.0.1/cli/uuid05
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-06-23 17:50:00.575182 uuid05-0.0.1/setup.cfg
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      550 2023-06-23 17:32:38.000000 uuid05-0.0.1/setup.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 17:50:00.575182 uuid05-0.0.1/uuid05/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     3009 2023-06-23 16:58:08.000000 uuid05-0.0.1/uuid05/__init__.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 17:50:00.575182 uuid05-0.0.1/uuid05.egg-info/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4445 2023-06-23 17:50:00.000000 uuid05-0.0.1/uuid05.egg-info/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      176 2023-06-23 17:50:00.000000 uuid05-0.0.1/uuid05.egg-info/SOURCES.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-06-23 17:50:00.000000 uuid05-0.0.1/uuid05.egg-info/dependency_links.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        7 2023-06-23 17:50:00.000000 uuid05-0.0.1/uuid05.egg-info/top_level.txt
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 18:58:03.075288 uuid05-0.0.2/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1097 2023-06-23 18:04:54.000000 uuid05-0.0.2/LICENSE
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4549 2023-06-23 18:58:03.071288 uuid05-0.0.2/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4174 2023-06-23 18:57:50.000000 uuid05-0.0.2/README.md
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 18:58:03.071288 uuid05-0.0.2/cli/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1075 2023-06-23 18:57:50.000000 uuid05-0.0.2/cli/uuid05
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-06-23 18:58:03.075288 uuid05-0.0.2/setup.cfg
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      569 2023-06-23 18:57:50.000000 uuid05-0.0.2/setup.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 18:58:03.071288 uuid05-0.0.2/uuid05/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     3325 2023-06-23 18:57:50.000000 uuid05-0.0.2/uuid05/__init__.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-23 18:58:03.071288 uuid05-0.0.2/uuid05.egg-info/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     4549 2023-06-23 18:58:03.000000 uuid05-0.0.2/uuid05.egg-info/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      176 2023-06-23 18:58:03.000000 uuid05-0.0.2/uuid05.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-06-23 18:58:03.000000 uuid05-0.0.2/uuid05.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        7 2023-06-23 18:58:03.000000 uuid05-0.0.2/uuid05.egg-info/top_level.txt
```

### Comparing `uuid05-0.0.1/LICENSE` & `uuid05-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `uuid05-0.0.1/PKG-INFO` & `uuid05-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: uuid05
-Version: 0.0.1
+Version: 0.0.2
 Summary: Compact human-readable almost unique identifiers for temporary objects in small non-synchronizing distributed systems.
 Home-page: https://github.com/strizhechenko/uuid05
 Author: Oleg Strizhechenko
 Author-email: oleg.strizhechenko@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **UUID05** - compact human-readable almost unique identifiers for temporary objects
 in small non-synchronizing distributed systems.
 
 Well, it's not really unique (that's why 0.5) and collisions are possible
 but probability is low and it's probably acceptable.
 
-The library provides you with just 2 functions: `uuid05() -> int` and `int2b64(int) -> str` and have zero dependencies.
+The library have zero dependencies and provides you with a class: `UUID05` based on `int` with two additional methods:
+
+- `make()` - sort of constructor.
+- `as_b64() -> str` - alternative representation.
 
 **Examples** below explain how it works:
 
 | TTL <br/>(seconds) | Workers | Worker ID | Example value |     Max value | int2b64(max_value) |
 |-------------------:|--------:|----------:|--------------:|--------------:|--------------------|
 |        (hour) 3600 |       2 |         1 |          9589 |        132400 | AgUw               |
 |               3600 |       4 |         2 |         29589 |        332400 | BRJw               |
@@ -39,20 +42,20 @@
 ``` shell
 pip install uuid05
 ```
 
 ## Using
 
 ``` python
-from uuid05 import uuid05, int2b64
+from uuid05 import UUID05
 
 # May be parametrized by workers: int, ttl: int, precision: int
 # defaults are: workers=10, ttl=2 days, precision=1
-uid: int = uuid05()
-suffix: str = int2b64(uid)
+uid = UUID05.make()
+suffix: str = uid.as_b64()
 object_name: str = f'autotest_object_{suffix}'
 ```
 
 It can be also used as an utility from command-line:
 
 ``` shell
 $ uuid05
@@ -63,40 +66,42 @@
 27091
 $ uuid05 -b -t 3600 -w 2
 aZ8
 $ uuid05 -b -w 2
 FvN2
 $ uuid05 -b
 AxHktA
-$ uuid --help
+$ uuid05 -b -a '_-' -w 64
+eB_5Yg
+$ uuid05 --help
 ```
 
-## When UUID05 is suitable
+## Where UUID05 is useful
 
 In E2E/UI-testing. It's slow, and sometimes you need to check a data created by tests _after_ run.
 
 Or, more generally, in staging environments where you aren't sure that your _testing_ system 
 will delete data after runs, but _tested_ system is aware of such a data and deletes it after some time.
 There's also be multiple testing systems instances running simultaneously, and you don't want them to affect each other.
 
 You also may want identifiers to be more or less rememberable for at least 10-15 seconds while you switching tabs.
 
 Oh, and you _don't_ want to synchronize workers via network.
 Otherwise Redis, Memcached or another database with a single INCRementing counter would do the trick.
 
-## When UUID05 isn't suitable
+## When UUID05 is useless
 
 - If your system isn't distributed. Local counter in memory or file will work better.
 - If your objects are persistent - you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid). 
 - If you need to generate multiple UIDs for multiple object really _quick_:
   - generate one and reuse it, using a semantic or loop variable as a suffix;
   - pass **precision** argument to `uuid05()`. It scales automatically with worker count, but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
     - `precision=3` argument will use milliseconds.
     - `precision=6` for microseconds.
   - if `precision=6` is not enough stop trying to make your identifier compact.
-- If you believe that semi-persistent data is a testing antipattern, 
+- If you believe that semi-persistent data is a testing antipattern,
   and it should be cleared by testing system before or after each run.
 
 ## Development
 
 - Tests are doctests and may be run by `pytest`.
 - Documentation - look at code, it's just two files.
```

### Comparing `uuid05-0.0.1/README.md` & `uuid05-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 **UUID05** - compact human-readable almost unique identifiers for temporary objects
 in small non-synchronizing distributed systems.
 
 Well, it's not really unique (that's why 0.5) and collisions are possible
 but probability is low and it's probably acceptable.
 
-The library provides you with just 2 functions: `uuid05() -> int` and `int2b64(int) -> str` and have zero dependencies.
+The library have zero dependencies and provides you with a class: `UUID05` based on `int` with two additional methods:
+
+- `make()` - sort of constructor.
+- `as_b64() -> str` - alternative representation.
 
 **Examples** below explain how it works:
 
 | TTL <br/>(seconds) | Workers | Worker ID | Example value |     Max value | int2b64(max_value) |
 |-------------------:|--------:|----------:|--------------:|--------------:|--------------------|
 |        (hour) 3600 |       2 |         1 |          9589 |        132400 | AgUw               |
 |               3600 |       4 |         2 |         29589 |        332400 | BRJw               |
@@ -28,20 +31,20 @@
 ``` shell
 pip install uuid05
 ```
 
 ## Using
 
 ``` python
-from uuid05 import uuid05, int2b64
+from uuid05 import UUID05
 
 # May be parametrized by workers: int, ttl: int, precision: int
 # defaults are: workers=10, ttl=2 days, precision=1
-uid: int = uuid05()
-suffix: str = int2b64(uid)
+uid = UUID05.make()
+suffix: str = uid.as_b64()
 object_name: str = f'autotest_object_{suffix}'
 ```
 
 It can be also used as an utility from command-line:
 
 ``` shell
 $ uuid05
@@ -52,40 +55,42 @@
 27091
 $ uuid05 -b -t 3600 -w 2
 aZ8
 $ uuid05 -b -w 2
 FvN2
 $ uuid05 -b
 AxHktA
-$ uuid --help
+$ uuid05 -b -a '_-' -w 64
+eB_5Yg
+$ uuid05 --help
 ```
 
-## When UUID05 is suitable
+## Where UUID05 is useful
 
 In E2E/UI-testing. It's slow, and sometimes you need to check a data created by tests _after_ run.
 
 Or, more generally, in staging environments where you aren't sure that your _testing_ system 
 will delete data after runs, but _tested_ system is aware of such a data and deletes it after some time.
 There's also be multiple testing systems instances running simultaneously, and you don't want them to affect each other.
 
 You also may want identifiers to be more or less rememberable for at least 10-15 seconds while you switching tabs.
 
 Oh, and you _don't_ want to synchronize workers via network.
 Otherwise Redis, Memcached or another database with a single INCRementing counter would do the trick.
 
-## When UUID05 isn't suitable
+## When UUID05 is useless
 
 - If your system isn't distributed. Local counter in memory or file will work better.
 - If your objects are persistent - you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid). 
 - If you need to generate multiple UIDs for multiple object really _quick_:
   - generate one and reuse it, using a semantic or loop variable as a suffix;
   - pass **precision** argument to `uuid05()`. It scales automatically with worker count, but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
     - `precision=3` argument will use milliseconds.
     - `precision=6` for microseconds.
   - if `precision=6` is not enough stop trying to make your identifier compact.
-- If you believe that semi-persistent data is a testing antipattern, 
+- If you believe that semi-persistent data is a testing antipattern,
   and it should be cleared by testing system before or after each run.
 
 ## Development
 
 - Tests are doctests and may be run by `pytest`.
 - Documentation - look at code, it's just two files.
```

### Comparing `uuid05-0.0.1/setup.py` & `uuid05-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from pathlib import Path
 from setuptools import setup
 
 setup(
     name='uuid05',
-    version='0.0.1',
+    version='0.0.2',
     packages=['uuid05'],
     url='https://github.com/strizhechenko/uuid05',
     license='MIT',
     author='Oleg Strizhechenko',
     author_email='oleg.strizhechenko@gmail.com',
-    description='Compact human-readable almost unique identifiers for temporary objects in small non-synchronizing distributed systems.',
+    description='Compact human-readable almost unique identifiers for temporary objects in '
+                'small non-synchronizing distributed systems.',
     long_description=Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     scripts=['cli/uuid05'],
 )
```

### Comparing `uuid05-0.0.1/uuid05.egg-info/PKG-INFO` & `uuid05-0.0.2/uuid05.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: uuid05
-Version: 0.0.1
+Version: 0.0.2
 Summary: Compact human-readable almost unique identifiers for temporary objects in small non-synchronizing distributed systems.
 Home-page: https://github.com/strizhechenko/uuid05
 Author: Oleg Strizhechenko
 Author-email: oleg.strizhechenko@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 **UUID05** - compact human-readable almost unique identifiers for temporary objects
 in small non-synchronizing distributed systems.
 
 Well, it's not really unique (that's why 0.5) and collisions are possible
 but probability is low and it's probably acceptable.
 
-The library provides you with just 2 functions: `uuid05() -> int` and `int2b64(int) -> str` and have zero dependencies.
+The library have zero dependencies and provides you with a class: `UUID05` based on `int` with two additional methods:
+
+- `make()` - sort of constructor.
+- `as_b64() -> str` - alternative representation.
 
 **Examples** below explain how it works:
 
 | TTL <br/>(seconds) | Workers | Worker ID | Example value |     Max value | int2b64(max_value) |
 |-------------------:|--------:|----------:|--------------:|--------------:|--------------------|
 |        (hour) 3600 |       2 |         1 |          9589 |        132400 | AgUw               |
 |               3600 |       4 |         2 |         29589 |        332400 | BRJw               |
@@ -39,20 +42,20 @@
 ``` shell
 pip install uuid05
 ```
 
 ## Using
 
 ``` python
-from uuid05 import uuid05, int2b64
+from uuid05 import UUID05
 
 # May be parametrized by workers: int, ttl: int, precision: int
 # defaults are: workers=10, ttl=2 days, precision=1
-uid: int = uuid05()
-suffix: str = int2b64(uid)
+uid = UUID05.make()
+suffix: str = uid.as_b64()
 object_name: str = f'autotest_object_{suffix}'
 ```
 
 It can be also used as an utility from command-line:
 
 ``` shell
 $ uuid05
@@ -63,40 +66,42 @@
 27091
 $ uuid05 -b -t 3600 -w 2
 aZ8
 $ uuid05 -b -w 2
 FvN2
 $ uuid05 -b
 AxHktA
-$ uuid --help
+$ uuid05 -b -a '_-' -w 64
+eB_5Yg
+$ uuid05 --help
 ```
 
-## When UUID05 is suitable
+## Where UUID05 is useful
 
 In E2E/UI-testing. It's slow, and sometimes you need to check a data created by tests _after_ run.
 
 Or, more generally, in staging environments where you aren't sure that your _testing_ system 
 will delete data after runs, but _tested_ system is aware of such a data and deletes it after some time.
 There's also be multiple testing systems instances running simultaneously, and you don't want them to affect each other.
 
 You also may want identifiers to be more or less rememberable for at least 10-15 seconds while you switching tabs.
 
 Oh, and you _don't_ want to synchronize workers via network.
 Otherwise Redis, Memcached or another database with a single INCRementing counter would do the trick.
 
-## When UUID05 isn't suitable
+## When UUID05 is useless
 
 - If your system isn't distributed. Local counter in memory or file will work better.
 - If your objects are persistent - you'd better use [py-nanoid](https://github.com/puyuan/py-nanoid). 
 - If you need to generate multiple UIDs for multiple object really _quick_:
   - generate one and reuse it, using a semantic or loop variable as a suffix;
   - pass **precision** argument to `uuid05()`. It scales automatically with worker count, but if there are less than 16 workers, default is 1 which means 1 uuid per 0.1 second, usually it's enough.
     - `precision=3` argument will use milliseconds.
     - `precision=6` for microseconds.
   - if `precision=6` is not enough stop trying to make your identifier compact.
-- If you believe that semi-persistent data is a testing antipattern, 
+- If you believe that semi-persistent data is a testing antipattern,
   and it should be cleared by testing system before or after each run.
 
 ## Development
 
 - Tests are doctests and may be run by `pytest`.
 - Documentation - look at code, it's just two files.
```

