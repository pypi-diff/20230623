# Comparing `tmp/intercode-bench-0.1.3.tar.gz` & `tmp/intercode-bench-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intercode-bench-0.1.3.tar", last modified: Fri Jun 23 21:28:36 2023, max compression
+gzip compressed data, was "intercode-bench-0.1.4.tar", last modified: Fri Jun 23 21:42:26 2023, max compression
```

## Comparing `intercode-bench-0.1.3.tar` & `intercode-bench-0.1.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:28:36.214136 intercode-bench-0.1.3/
--rw-r--r--   0 johnbyang   (502) staff       (20)     1093 2023-06-23 00:41:05.000000 intercode-bench-0.1.3/LICENSE
--rw-r--r--   0 johnbyang   (502) staff       (20)     2969 2023-06-23 21:28:36.214472 intercode-bench-0.1.3/PKG-INFO
--rw-r--r--   0 johnbyang   (502) staff       (20)     1921 2023-06-23 21:25:20.000000 intercode-bench-0.1.3/README.md
--rw-r--r--   0 johnbyang   (502) staff       (20)       84 2023-06-23 00:11:41.000000 intercode-bench-0.1.3/pyproject.toml
--rw-r--r--   0 johnbyang   (502) staff       (20)      112 2023-06-23 21:28:36.215183 intercode-bench-0.1.3/setup.cfg
--rw-r--r--   0 johnbyang   (502) staff       (20)     1500 2023-06-23 21:13:51.000000 intercode-bench-0.1.3/setup.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:28:36.191120 intercode-bench-0.1.3/src/
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:28:36.195223 intercode-bench-0.1.3/src/intercode/
--rw-r--r--   0 johnbyang   (502) staff       (20)      137 2023-06-23 21:28:12.000000 intercode-bench-0.1.3/src/intercode/__init__.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:28:36.196718 intercode-bench-0.1.3/src/intercode/envs/
--rw-r--r--   0 johnbyang   (502) staff       (20)      141 2023-06-23 21:20:36.000000 intercode-bench-0.1.3/src/intercode/envs/__init__.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:28:36.198372 intercode-bench-0.1.3/src/intercode/envs/bash/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:42.000000 intercode-bench-0.1.3/src/intercode/envs/bash/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     7682 2023-06-23 02:47:20.000000 intercode-bench-0.1.3/src/intercode/envs/bash/bash_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:28:36.200090 intercode-bench-0.1.3/src/intercode/envs/game/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:55.000000 intercode-bench-0.1.3/src/intercode/envs/game/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     4552 2023-06-23 02:47:20.000000 intercode-bench-0.1.3/src/intercode/envs/game/ctf_env.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     8569 2023-06-23 02:47:20.000000 intercode-bench-0.1.3/src/intercode/envs/ic_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:28:36.201949 intercode-bench-0.1.3/src/intercode/envs/sql/
--rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:45.000000 intercode-bench-0.1.3/src/intercode/envs/sql/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     5045 2023-06-23 04:27:43.000000 intercode-bench-0.1.3/src/intercode/envs/sql/sql_env.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:28:36.205231 intercode-bench-0.1.3/src/intercode/utils/
--rw-r--r--   0 johnbyang   (502) staff       (20)      148 2023-06-23 00:31:02.000000 intercode-bench-0.1.3/src/intercode/utils/__init__.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     2428 2023-06-23 00:31:02.000000 intercode-bench-0.1.3/src/intercode/utils/data_loader.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1718 2023-06-23 00:31:02.000000 intercode-bench-0.1.3/src/intercode/utils/utils.py
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:28:36.209483 intercode-bench-0.1.3/src/intercode_bench.egg-info/
--rw-r--r--   0 johnbyang   (502) staff       (20)     2969 2023-06-23 21:28:36.000000 intercode-bench-0.1.3/src/intercode_bench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (502) staff       (20)      751 2023-06-23 21:28:36.000000 intercode-bench-0.1.3/src/intercode_bench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)        1 2023-06-23 21:28:36.000000 intercode-bench-0.1.3/src/intercode_bench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)       72 2023-06-23 21:28:36.000000 intercode-bench-0.1.3/src/intercode_bench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (502) staff       (20)       10 2023-06-23 21:28:36.000000 intercode-bench-0.1.3/src/intercode_bench.egg-info/top_level.txt
-drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:28:36.213335 intercode-bench-0.1.3/tests/
--rw-r--r--   0 johnbyang   (502) staff       (20)     1757 2023-06-23 02:47:20.000000 intercode-bench-0.1.3/tests/test_data_loader.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     2498 2023-06-23 02:47:20.000000 intercode-bench-0.1.3/tests/test_env_bash.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1334 2023-06-23 02:47:20.000000 intercode-bench-0.1.3/tests/test_env_ic.py
--rw-r--r--   0 johnbyang   (502) staff       (20)     1683 2023-06-23 02:47:20.000000 intercode-bench-0.1.3/tests/test_env_sql.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:42:26.269443 intercode-bench-0.1.4/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1093 2023-06-23 00:41:05.000000 intercode-bench-0.1.4/LICENSE
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2919 2023-06-23 21:42:26.269645 intercode-bench-0.1.4/PKG-INFO
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1921 2023-06-23 21:38:30.000000 intercode-bench-0.1.4/README.md
+-rw-r--r--   0 johnbyang   (502) staff       (20)       84 2023-06-23 00:11:41.000000 intercode-bench-0.1.4/pyproject.toml
+-rw-r--r--   0 johnbyang   (502) staff       (20)      112 2023-06-23 21:42:26.270320 intercode-bench-0.1.4/setup.cfg
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1451 2023-06-23 21:38:26.000000 intercode-bench-0.1.4/setup.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:42:26.249202 intercode-bench-0.1.4/src/
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:42:26.252614 intercode-bench-0.1.4/src/intercode/
+-rw-r--r--   0 johnbyang   (502) staff       (20)      137 2023-06-23 21:42:01.000000 intercode-bench-0.1.4/src/intercode/__init__.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:42:26.254188 intercode-bench-0.1.4/src/intercode/envs/
+-rw-r--r--   0 johnbyang   (502) staff       (20)      141 2023-06-23 21:20:36.000000 intercode-bench-0.1.4/src/intercode/envs/__init__.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:42:26.255939 intercode-bench-0.1.4/src/intercode/envs/bash/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:42.000000 intercode-bench-0.1.4/src/intercode/envs/bash/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     7682 2023-06-23 02:47:20.000000 intercode-bench-0.1.4/src/intercode/envs/bash/bash_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:42:26.257845 intercode-bench-0.1.4/src/intercode/envs/game/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:55.000000 intercode-bench-0.1.4/src/intercode/envs/game/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     4552 2023-06-23 02:47:20.000000 intercode-bench-0.1.4/src/intercode/envs/game/ctf_env.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     8569 2023-06-23 02:47:20.000000 intercode-bench-0.1.4/src/intercode/envs/ic_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:42:26.259445 intercode-bench-0.1.4/src/intercode/envs/sql/
+-rw-r--r--   0 johnbyang   (502) staff       (20)        0 2023-06-23 02:52:45.000000 intercode-bench-0.1.4/src/intercode/envs/sql/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     5045 2023-06-23 04:27:43.000000 intercode-bench-0.1.4/src/intercode/envs/sql/sql_env.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:42:26.262241 intercode-bench-0.1.4/src/intercode/utils/
+-rw-r--r--   0 johnbyang   (502) staff       (20)      148 2023-06-23 00:31:02.000000 intercode-bench-0.1.4/src/intercode/utils/__init__.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2428 2023-06-23 00:31:02.000000 intercode-bench-0.1.4/src/intercode/utils/data_loader.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1718 2023-06-23 00:31:02.000000 intercode-bench-0.1.4/src/intercode/utils/utils.py
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:42:26.265246 intercode-bench-0.1.4/src/intercode_bench.egg-info/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2919 2023-06-23 21:42:26.000000 intercode-bench-0.1.4/src/intercode_bench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (502) staff       (20)      751 2023-06-23 21:42:26.000000 intercode-bench-0.1.4/src/intercode_bench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)        1 2023-06-23 21:42:26.000000 intercode-bench-0.1.4/src/intercode_bench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)       72 2023-06-23 21:42:26.000000 intercode-bench-0.1.4/src/intercode_bench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (502) staff       (20)       10 2023-06-23 21:42:26.000000 intercode-bench-0.1.4/src/intercode_bench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (502) staff       (20)        0 2023-06-23 21:42:26.268684 intercode-bench-0.1.4/tests/
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1757 2023-06-23 02:47:20.000000 intercode-bench-0.1.4/tests/test_data_loader.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     2498 2023-06-23 02:47:20.000000 intercode-bench-0.1.4/tests/test_env_bash.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1334 2023-06-23 02:47:20.000000 intercode-bench-0.1.4/tests/test_env_ic.py
+-rw-r--r--   0 johnbyang   (502) staff       (20)     1683 2023-06-23 02:47:20.000000 intercode-bench-0.1.4/tests/test_env_sql.py
```

### Comparing `intercode-bench-0.1.3/LICENSE` & `intercode-bench-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.3/PKG-INFO` & `intercode-bench-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: intercode-bench
-Version: 0.1.3
+Version: 0.1.4
 Summary: The official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Bug Reports, https://github.com/intercode-benchmark/intercode-benchmark/issues
 Project-URL: Source Code, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Website, https://intercode-benchmark.github.io/
 Keywords: nlp,benchmark,interaction,code,rl,decision making
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🤖💻 Intercode
 Build interactive code environments for training, testing, and augmenting code and decision making agents
 
 <p>
     <a href="https://badge.fury.io/py/intercode-bench">
         <img src="https://badge.fury.io/py/intercode-bench.svg">
     </a>
     <a href="https://www.python.org/">
-        <img alt="Build" src="https://img.shields.io/badge/Python-3.7+-1f425f.svg?color=purple">
+        <img alt="Build" src="https://img.shields.io/badge/Python-3.8+-1f425f.svg?color=purple">
     </a>
     <a href="https://copyright.princeton.edu/policy">
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
 </p>
 
 ## 👋 Overview
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.3 Summary: The
+Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.4 Summary: The
 official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark Author:
 John Yang Author-email: byjohnyang@gmail.com Project-URL: Documentation, https:
 //github.com/intercode-benchmark/intercode-benchmark Project-URL: Bug Reports,
 https://github.com/intercode-benchmark/intercode-benchmark/issues Project-URL:
 Source Code, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Website, https://intercode-benchmark.github.io/ Keywords:
 nlp,benchmark,interaction,code,rl,decision making Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE # ð¤ð»
-Intercode Build interactive code environments for training, testing, and
-augmenting code and decision making agents
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE # ð¤ð» Intercode Build interactive code environments for training,
+testing, and augmenting code and decision making agents
 [https://badge.fury.io/py/intercode-bench.svg] [Build] [License]
 ## ð Overview InterCode is a **lightweight, flexible, and easy-to-use
 framework** for designing interactive code environments. Following the popular
 [`gym`](https://gymnasium.farama.org/) interface definition, InterCode makes it
 easy to quickly define a code environment and deploy an agent to operate in
 code within the context of the environment. For an overview of InterCode,
 building interactive code tasks with InterCode, and evaluating agents on
```

### Comparing `intercode-bench-0.1.3/README.md` & `intercode-bench-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Build interactive code environments for training, testing, and augmenting code and decision making agents
 
 <p>
     <a href="https://badge.fury.io/py/intercode-bench">
         <img src="https://badge.fury.io/py/intercode-bench.svg">
     </a>
     <a href="https://www.python.org/">
-        <img alt="Build" src="https://img.shields.io/badge/Python-3.7+-1f425f.svg?color=purple">
+        <img alt="Build" src="https://img.shields.io/badge/Python-3.8+-1f425f.svg?color=purple">
     </a>
     <a href="https://copyright.princeton.edu/policy">
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
 </p>
 
 ## 👋 Overview
```

### Comparing `intercode-bench-0.1.3/setup.py` & `intercode-bench-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,22 +17,21 @@
         'Bug Reports': 'https://github.com/intercode-benchmark/intercode-benchmark/issues',
         'Source Code': 'https://github.com/intercode-benchmark/intercode-benchmark',
         'Website': 'https://intercode-benchmark.github.io/',
     },
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3 :: Only',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         'gymnasium',
         'mysql-connector-python',
         'scikit-learn>=1.2.2',
         'pandas',
         'rich',
         'docker'
```

### Comparing `intercode-bench-0.1.3/src/intercode/envs/bash/bash_env.py` & `intercode-bench-0.1.4/src/intercode/envs/bash/bash_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.3/src/intercode/envs/game/ctf_env.py` & `intercode-bench-0.1.4/src/intercode/envs/game/ctf_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.3/src/intercode/envs/ic_env.py` & `intercode-bench-0.1.4/src/intercode/envs/ic_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.3/src/intercode/envs/sql/sql_env.py` & `intercode-bench-0.1.4/src/intercode/envs/sql/sql_env.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.3/src/intercode/utils/data_loader.py` & `intercode-bench-0.1.4/src/intercode/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.3/src/intercode/utils/utils.py` & `intercode-bench-0.1.4/src/intercode/utils/utils.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.3/src/intercode_bench.egg-info/PKG-INFO` & `intercode-bench-0.1.4/src/intercode_bench.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: intercode-bench
-Version: 0.1.3
+Version: 0.1.4
 Summary: The official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Bug Reports, https://github.com/intercode-benchmark/intercode-benchmark/issues
 Project-URL: Source Code, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Website, https://intercode-benchmark.github.io/
 Keywords: nlp,benchmark,interaction,code,rl,decision making
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🤖💻 Intercode
 Build interactive code environments for training, testing, and augmenting code and decision making agents
 
 <p>
     <a href="https://badge.fury.io/py/intercode-bench">
         <img src="https://badge.fury.io/py/intercode-bench.svg">
     </a>
     <a href="https://www.python.org/">
-        <img alt="Build" src="https://img.shields.io/badge/Python-3.7+-1f425f.svg?color=purple">
+        <img alt="Build" src="https://img.shields.io/badge/Python-3.8+-1f425f.svg?color=purple">
     </a>
     <a href="https://copyright.princeton.edu/policy">
         <img alt="License" src="https://img.shields.io/badge/License-MIT-blue">
     </a>
 </p>
 
 ## 👋 Overview
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.3 Summary: The
+Metadata-Version: 2.1 Name: intercode-bench Version: 0.1.4 Summary: The
 official InterCode benchmark package - a framework for interactive code tasks
 Home-page: http://github.com/intercode-benchmark/intercode-benchmark Author:
 John Yang Author-email: byjohnyang@gmail.com Project-URL: Documentation, https:
 //github.com/intercode-benchmark/intercode-benchmark Project-URL: Bug Reports,
 https://github.com/intercode-benchmark/intercode-benchmark/issues Project-URL:
 Source Code, https://github.com/intercode-benchmark/intercode-benchmark
 Project-URL: Website, https://intercode-benchmark.github.io/ Keywords:
 nlp,benchmark,interaction,code,rl,decision making Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE # ð¤ð»
-Intercode Build interactive code environments for training, testing, and
-augmenting code and decision making agents
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE # ð¤ð» Intercode Build interactive code environments for training,
+testing, and augmenting code and decision making agents
 [https://badge.fury.io/py/intercode-bench.svg] [Build] [License]
 ## ð Overview InterCode is a **lightweight, flexible, and easy-to-use
 framework** for designing interactive code environments. Following the popular
 [`gym`](https://gymnasium.farama.org/) interface definition, InterCode makes it
 easy to quickly define a code environment and deploy an agent to operate in
 code within the context of the environment. For an overview of InterCode,
 building interactive code tasks with InterCode, and evaluating agents on
```

### Comparing `intercode-bench-0.1.3/src/intercode_bench.egg-info/SOURCES.txt` & `intercode-bench-0.1.4/src/intercode_bench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.3/tests/test_data_loader.py` & `intercode-bench-0.1.4/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.3/tests/test_env_bash.py` & `intercode-bench-0.1.4/tests/test_env_bash.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.3/tests/test_env_ic.py` & `intercode-bench-0.1.4/tests/test_env_ic.py`

 * *Files identical despite different names*

### Comparing `intercode-bench-0.1.3/tests/test_env_sql.py` & `intercode-bench-0.1.4/tests/test_env_sql.py`

 * *Files identical despite different names*

