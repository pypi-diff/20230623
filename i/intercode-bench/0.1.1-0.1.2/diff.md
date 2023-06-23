# Comparing `tmp/intercode-bench-0.1.1.tar.gz` & `tmp/intercode-bench-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intercode-bench-0.1.1.tar", last modified: Fri Jun 23 05:18:19 2023, max compression
+gzip compressed data, was "intercode-bench-0.1.2.tar", last modified: Fri Jun 23 05:32:19 2023, max compression
```

## Comparing `intercode-bench-0.1.1.tar` & `intercode-bench-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:18:19.425312 intercode-bench-0.1.1/
--rw-r--r--   0 johnbyang   (502) staff       (20)     1093 2023-06-23 00:41:05.000000 intercode-bench-0.1.1/LICENSE
--rw-r--r--   0 johnbyang   (502) staff       (20)     1815 2023-06-23 05:18:19.425592 intercode-bench-0.1.1/PKG-INFO
--rw-r--r--   0 johnbyang   (502) staff       (20)      767 2023-06-23 02:54:21.000000 intercode-bench-0.1.1/README.md
--rw-r--r--   0 johnbyang   (502) staff       (20)       84 2023-06-23 00:11:41.000000 intercode-bench-0.1.1/pyproject.toml
--rw-r--r--   0 johnbyang   (502) staff       (20)      112 2023-06-23 05:18:19.426577 intercode-bench-0.1.1/setup.cfg
--rw-r--r--   0 johnbyang   (502) staff       (20)     1459 2023-06-23 04:59:11.000000 intercode-bench-0.1.1/setup.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:18:19.408079 intercode-bench-0.1.1/src/
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:18:19.411318 intercode-bench-0.1.1/src/intercode/
--rw-r--r--   0 johnbyang   (502) staff       (20)      279 2023-06-23 05:17:33.000000 intercode-bench-0.1.1/src/intercode/__init__.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:18:19.412690 intercode-bench-0.1.1/src/intercode/envs/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:22.000000 intercode-bench-0.1.1/src/intercode/envs/__init__.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:18:19.413723 intercode-bench-0.1.1/src/intercode/envs/bash/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:42.000000 intercode-bench-0.1.1/src/intercode/envs/bash/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     7682 2023-06-23 02:47:20.000000 intercode-bench-0.1.1/src/intercode/envs/bash/bash_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:18:19.414648 intercode-bench-0.1.1/src/intercode/envs/game/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:55.000000 intercode-bench-0.1.1/src/intercode/envs/game/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     4552 2023-06-23 02:47:20.000000 intercode-bench-0.1.1/src/intercode/envs/game/ctf_env.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     8569 2023-06-23 02:47:20.000000 intercode-bench-0.1.1/src/intercode/envs/ic_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:18:19.415744 intercode-bench-0.1.1/src/intercode/envs/sql/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:45.000000 intercode-bench-0.1.1/src/intercode/envs/sql/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     5045 2023-06-23 04:27:43.000000 intercode-bench-0.1.1/src/intercode/envs/sql/sql_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:18:19.417624 intercode-bench-0.1.1/src/intercode/utils/
--rw-r--r--   0 johnbyang   (502) staff       (20)      148 2023-06-23 00:31:02.000000 intercode-bench-0.1.1/src/intercode/utils/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     2428 2023-06-23 00:31:02.000000 intercode-bench-0.1.1/src/intercode/utils/data_loader.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1718 2023-06-23 00:31:02.000000 intercode-bench-0.1.1/src/intercode/utils/utils.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:18:19.421636 intercode-bench-0.1.1/src/intercode_bench.egg-info/
--rw-r--r--   0 johnbyang   (502) staff       (20)     1815 2023-06-23 05:18:19.000000 intercode-bench-0.1.1/src/intercode_bench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (502) staff       (20)      751 2023-06-23 05:18:19.000000 intercode-bench-0.1.1/src/intercode_bench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)        1 2023-06-23 05:18:19.000000 intercode-bench-0.1.1/src/intercode_bench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)       53 2023-06-23 05:18:19.000000 intercode-bench-0.1.1/src/intercode_bench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)       10 2023-06-23 05:18:19.000000 intercode-bench-0.1.1/src/intercode_bench.egg-info/top_level.txt
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:18:19.424630 intercode-bench-0.1.1/tests/
--rw-r--r--   0 johnbyang   (502) staff       (20)     1757 2023-06-23 02:47:20.000000 intercode-bench-0.1.1/tests/test_data_loader.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     2498 2023-06-23 02:47:20.000000 intercode-bench-0.1.1/tests/test_env_bash.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1334 2023-06-23 02:47:20.000000 intercode-bench-0.1.1/tests/test_env_ic.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1683 2023-06-23 02:47:20.000000 intercode-bench-0.1.1/tests/test_env_sql.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:32:19.958657 intercode-bench-0.1.2/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1093 2023-06-23 00:41:05.000000 intercode-bench-0.1.2/LICENSE
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1815 2023-06-23 05:32:19.959076 intercode-bench-0.1.2/PKG-INFO
+-rw-r--r--   0 johnbyang   (502) staff       (20)      767 2023-06-23 02:54:21.000000 intercode-bench-0.1.2/README.md
+-rw-r--r--   0 johnbyang   (502) staff       (20)       84 2023-06-23 00:11:41.000000 intercode-bench-0.1.2/pyproject.toml
+-rw-r--r--   0 johnbyang   (502) staff       (20)      112 2023-06-23 05:32:19.959989 intercode-bench-0.1.2/setup.cfg
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1493 2023-06-23 05:20:33.000000 intercode-bench-0.1.2/setup.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:32:19.919801 intercode-bench-0.1.2/src/
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:32:19.924584 intercode-bench-0.1.2/src/intercode/
+-rw-r--r--   0 johnbyang   (502) staff       (20)      279 2023-06-23 05:25:23.000000 intercode-bench-0.1.2/src/intercode/__init__.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:32:19.928824 intercode-bench-0.1.2/src/intercode/envs/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:22.000000 intercode-bench-0.1.2/src/intercode/envs/__init__.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:32:19.933195 intercode-bench-0.1.2/src/intercode/envs/bash/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:42.000000 intercode-bench-0.1.2/src/intercode/envs/bash/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     7682 2023-06-23 02:47:20.000000 intercode-bench-0.1.2/src/intercode/envs/bash/bash_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:32:19.935894 intercode-bench-0.1.2/src/intercode/envs/game/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:55.000000 intercode-bench-0.1.2/src/intercode/envs/game/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     4552 2023-06-23 02:47:20.000000 intercode-bench-0.1.2/src/intercode/envs/game/ctf_env.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     8569 2023-06-23 02:47:20.000000 intercode-bench-0.1.2/src/intercode/envs/ic_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:32:19.939115 intercode-bench-0.1.2/src/intercode/envs/sql/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:45.000000 intercode-bench-0.1.2/src/intercode/envs/sql/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     5045 2023-06-23 04:27:43.000000 intercode-bench-0.1.2/src/intercode/envs/sql/sql_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:32:19.944610 intercode-bench-0.1.2/src/intercode/utils/
+-rw-r--r--   0 johnbyang   (502) staff       (20)      148 2023-06-23 00:31:02.000000 intercode-bench-0.1.2/src/intercode/utils/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2428 2023-06-23 00:31:02.000000 intercode-bench-0.1.2/src/intercode/utils/data_loader.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1718 2023-06-23 00:31:02.000000 intercode-bench-0.1.2/src/intercode/utils/utils.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:32:19.951164 intercode-bench-0.1.2/src/intercode_bench.egg-info/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1815 2023-06-23 05:32:19.000000 intercode-bench-0.1.2/src/intercode_bench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (502) staff       (20)      751 2023-06-23 05:32:19.000000 intercode-bench-0.1.2/src/intercode_bench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)        1 2023-06-23 05:32:19.000000 intercode-bench-0.1.2/src/intercode_bench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)       65 2023-06-23 05:32:19.000000 intercode-bench-0.1.2/src/intercode_bench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)       10 2023-06-23 05:32:19.000000 intercode-bench-0.1.2/src/intercode_bench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 05:32:19.956950 intercode-bench-0.1.2/tests/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1757 2023-06-23 02:47:20.000000 intercode-bench-0.1.2/tests/test_data_loader.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2498 2023-06-23 02:47:20.000000 intercode-bench-0.1.2/tests/test_env_bash.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1334 2023-06-23 02:47:20.000000 intercode-bench-0.1.2/tests/test_env_ic.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1683 2023-06-23 02:47:20.000000 intercode-bench-0.1.2/tests/test_env_sql.py
```

### Comparing `intercode-bench-0.1.1/LICENSE` & `intercode-bench-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/PKG-INFO` & `intercode-bench-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intercode-bench
-Version: 0.1.1
+Version: 0.1.2
 Summary: The official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Bug Reports, https://github.com/intercode-benchmark/intercode-benchmark/issues
 Project-URL: Source Code, https://github.com/intercode-benchmark/intercode-benchmark
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.1 Summary: The
+Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.2 Summary: The
 official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark Author:
 John Yang Author-email: byjohnyang@gmail.com Project-URL: Documentation, https:
 //github.com/intercode-benchmark/intercode-benchmark Project-URL: Bug Reports,
 https://github.com/intercode-benchmark/intercode-benchmark/issues Project-URL:
 Source Code, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Website, https://intercode-benchmark.github.io/ Keywords:
```

### Comparing `intercode-bench-0.1.1/README.md` & `intercode-bench-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/setup.py` & `intercode-bench-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,10 +29,12 @@
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.7',
     install_requires=[
         'gymnasium',
         'mysql-connector-python',
         'scikit-learn',
-        'pandas'
+        'pandas',
+        'rich',
+        'docker'
     ],
 )
```

### Comparing `intercode-bench-0.1.1/src/intercode/envs/bash/bash_env.py` & `intercode-bench-0.1.2/src/intercode/envs/bash/bash_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/src/intercode/envs/game/ctf_env.py` & `intercode-bench-0.1.2/src/intercode/envs/game/ctf_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/src/intercode/envs/ic_env.py` & `intercode-bench-0.1.2/src/intercode/envs/ic_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/src/intercode/envs/sql/sql_env.py` & `intercode-bench-0.1.2/src/intercode/envs/sql/sql_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/src/intercode/utils/data_loader.py` & `intercode-bench-0.1.2/src/intercode/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/src/intercode/utils/utils.py` & `intercode-bench-0.1.2/src/intercode/utils/utils.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/src/intercode_bench.egg-info/PKG-INFO` & `intercode-bench-0.1.2/src/intercode_bench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intercode-bench
-Version: 0.1.1
+Version: 0.1.2
 Summary: The official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Bug Reports, https://github.com/intercode-benchmark/intercode-benchmark/issues
 Project-URL: Source Code, https://github.com/intercode-benchmark/intercode-benchmark
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.1 Summary: The
+Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.2 Summary: The
 official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark Author:
 John Yang Author-email: byjohnyang@gmail.com Project-URL: Documentation, https:
 //github.com/intercode-benchmark/intercode-benchmark Project-URL: Bug Reports,
 https://github.com/intercode-benchmark/intercode-benchmark/issues Project-URL:
 Source Code, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Website, https://intercode-benchmark.github.io/ Keywords:
```

### Comparing `intercode-bench-0.1.1/src/intercode_bench.egg-info/SOURCES.txt` & `intercode-bench-0.1.2/src/intercode_bench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/tests/test_data_loader.py` & `intercode-bench-0.1.2/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/tests/test_env_bash.py` & `intercode-bench-0.1.2/tests/test_env_bash.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/tests/test_env_ic.py` & `intercode-bench-0.1.2/tests/test_env_ic.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.1/tests/test_env_sql.py` & `intercode-bench-0.1.2/tests/test_env_sql.py`

 * *Files identical despite different names*

