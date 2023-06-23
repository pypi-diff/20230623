# Comparing `tmp/execution_time_wrapper-1.0.0.tar.gz` & `tmp/execution_time_wrapper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/execution_time_wrapper-1.0.0.tar", last modified: Wed May 25 08:55:41 2022, max compression
+gzip compressed data, was "execution_time_wrapper-1.0.1.tar", last modified: Fri Jun 23 15:10:56 2023, max compression
```

## Comparing `execution_time_wrapper-1.0.0.tar` & `execution_time_wrapper-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 leonardoalchieri   (501) staff       (20)        0 2022-05-25 08:55:41.000000 execution_time_wrapper-1.0.0/
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)     1074 2022-05-25 08:25:15.000000 execution_time_wrapper-1.0.0/LICENSE
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)     2044 2022-05-25 08:55:41.000000 execution_time_wrapper-1.0.0/PKG-INFO
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)     1096 2022-05-25 08:54:56.000000 execution_time_wrapper-1.0.0/README.md
-drwxr-xr-x   0 leonardoalchieri   (501) staff       (20)        0 2022-05-25 08:55:41.000000 execution_time_wrapper-1.0.0/execution_time_wrapper/
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)      130 2022-05-25 08:42:25.000000 execution_time_wrapper-1.0.0/execution_time_wrapper/__init__.py
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)       21 2022-05-25 08:52:13.000000 execution_time_wrapper-1.0.0/execution_time_wrapper/_version.py
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)     1360 2022-05-25 08:30:10.000000 execution_time_wrapper-1.0.0/execution_time_wrapper/log_based.py
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)     1269 2022-05-25 08:38:28.000000 execution_time_wrapper-1.0.0/execution_time_wrapper/print_based.py
-drwxr-xr-x   0 leonardoalchieri   (501) staff       (20)        0 2022-05-25 08:55:41.000000 execution_time_wrapper-1.0.0/execution_time_wrapper.egg-info/
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)     2044 2022-05-25 08:55:41.000000 execution_time_wrapper-1.0.0/execution_time_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)      399 2022-05-25 08:55:41.000000 execution_time_wrapper-1.0.0/execution_time_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)        1 2022-05-25 08:55:41.000000 execution_time_wrapper-1.0.0/execution_time_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)       22 2022-05-25 08:55:41.000000 execution_time_wrapper-1.0.0/execution_time_wrapper.egg-info/requires.txt
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)       23 2022-05-25 08:55:41.000000 execution_time_wrapper-1.0.0/execution_time_wrapper.egg-info/top_level.txt
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)       38 2022-05-25 08:55:41.000000 execution_time_wrapper-1.0.0/setup.cfg
--rw-r--r--   0 leonardoalchieri   (501) staff       (20)     1404 2022-05-25 08:55:32.000000 execution_time_wrapper-1.0.0/setup.py
+drwxr-xr-x   0 leonardoalchieri   (501) staff       (20)        0 2023-06-23 15:10:56.961419 execution_time_wrapper-1.0.1/
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)     1074 2023-06-23 15:08:58.000000 execution_time_wrapper-1.0.1/LICENSE
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)     2590 2023-06-23 15:10:56.961299 execution_time_wrapper-1.0.1/PKG-INFO
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)     1662 2023-06-23 15:09:42.000000 execution_time_wrapper-1.0.1/README.md
+drwxr-xr-x   0 leonardoalchieri   (501) staff       (20)        0 2023-06-23 15:10:56.960286 execution_time_wrapper-1.0.1/execution_time_wrapper/
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)      130 2022-05-25 09:52:14.000000 execution_time_wrapper-1.0.1/execution_time_wrapper/__init__.py
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)       22 2023-06-23 15:08:49.000000 execution_time_wrapper-1.0.1/execution_time_wrapper/_version.py
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)     1360 2022-05-25 09:52:14.000000 execution_time_wrapper-1.0.1/execution_time_wrapper/log_based.py
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)     1269 2022-05-25 09:52:14.000000 execution_time_wrapper-1.0.1/execution_time_wrapper/print_based.py
+drwxr-xr-x   0 leonardoalchieri   (501) staff       (20)        0 2023-06-23 15:10:56.961082 execution_time_wrapper-1.0.1/execution_time_wrapper.egg-info/
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)     2590 2023-06-23 15:10:56.000000 execution_time_wrapper-1.0.1/execution_time_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)      354 2023-06-23 15:10:56.000000 execution_time_wrapper-1.0.1/execution_time_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)        1 2023-06-23 15:10:56.000000 execution_time_wrapper-1.0.1/execution_time_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)       23 2023-06-23 15:10:56.000000 execution_time_wrapper-1.0.1/execution_time_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)       38 2023-06-23 15:10:56.961462 execution_time_wrapper-1.0.1/setup.cfg
+-rw-r--r--   0 leonardoalchieri   (501) staff       (20)     1350 2023-06-23 15:08:39.000000 execution_time_wrapper-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `execution_time_wrapper-1.0.0/LICENSE` & `execution_time_wrapper-1.0.1/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Leonardo Alchieri
+Copyright (c) 2023 Leonardo Alchieri
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `execution_time_wrapper-1.0.0/PKG-INFO` & `execution_time_wrapper-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: execution_time_wrapper
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package with some simple wrapper functions to print the execution time of methods
 Home-page: https://github.com/LeonardoAlchieri/ExecutionTimeWrapper
 Author: Leonardo Alchieri
 Author-email: leonardo@alchieri.eu
 License: MIT
 Keywords: time,wrapper,log,print,execution,speed
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,37 +18,60 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.org/project/execution-time-wrapper/)
-[![PyPI version fury.io](https://badge.fury.io/py/ansicolortags.svg)](https://pypi.org/project/execution-time-wrapper/)
+[![PyPI version](https://badge.fury.io/py/execution-time-wrapper.svg)](https://badge.fury.io/py/execution-time-wrapper)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pybadges.svg)](https://pypi.org/project/execution-time-wrapper/)
-[![Downloads](https://pepy.tech/badge/apple-heartrate-pandas)](https://pepy.tech/project/execution-time-wrapper)
+[![Downloads](https://pepy.tech/badge/execution-time-wrapper)](https://pepy.tech/project/execution-time-wrapper)
 
 # Execution Time Wrapper
 
 A simple package with a few method to get the execution time of methods through wrapping.
 
 ## Usage
 
-Currently, the package contains two methods, one which returns to sdout (print) and one which goes to a logger.
+Currently, the package contains two methods, one which returns to sdout (print) and one which goes to a logger. The method prints the time in a nice way, i.e. milliseconds, seconds, minutes or hours. For example:
 
 ```python
-from execution_time import get_execution_time_log
+from execution_time_wrapper import get_execution_time_print, get_execution_time_log
 
-@get_execution_time_log
+@get_execution_time_print
 def my_fun():
     print("Hello World!")
 ```
-The same for the other method given, i.e. `get_execution_time_print`.
+```python
+my_fun()
+```
+```console
+>> Hello World!
+>> Computation time for my_fun: 0.02 ms
+```
+However, if the function takes more time:
+```python
+from execution_time_wrapper import get_execution_time_print, get_execution_time_log
+from time import sleep
+
+@get_execution_time_print
+def my_fun():
+    sleep(4)
+    print("Hello World!")
+```
+```python
+my_fun()
+```
+```console
+>> Hello World!
+>> Computation time for my_fun: 4.00 s
+```
+
+The same for the other method given, i.e. `get_execution_time_log`.
 
 ## TODOs
 
 [ ] Implement logger level
 
 @2022, Leonardo Alchieri
 
 <sub>People-Centered Computing Lab - [Università della Svizzera italiana, Switzerland](https://www.usi.ch/en)</sub>
-
-
```

### Comparing `execution_time_wrapper-1.0.0/README.md` & `execution_time_wrapper-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,53 @@
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.org/project/execution-time-wrapper/)
-[![PyPI version fury.io](https://badge.fury.io/py/ansicolortags.svg)](https://pypi.org/project/execution-time-wrapper/)
+[![PyPI version](https://badge.fury.io/py/execution-time-wrapper.svg)](https://badge.fury.io/py/execution-time-wrapper)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pybadges.svg)](https://pypi.org/project/execution-time-wrapper/)
-[![Downloads](https://pepy.tech/badge/apple-heartrate-pandas)](https://pepy.tech/project/execution-time-wrapper)
+[![Downloads](https://pepy.tech/badge/execution-time-wrapper)](https://pepy.tech/project/execution-time-wrapper)
 
 # Execution Time Wrapper
 
 A simple package with a few method to get the execution time of methods through wrapping.
 
 ## Usage
 
-Currently, the package contains two methods, one which returns to sdout (print) and one which goes to a logger.
+Currently, the package contains two methods, one which returns to sdout (print) and one which goes to a logger. The method prints the time in a nice way, i.e. milliseconds, seconds, minutes or hours. For example:
 
 ```python
-from execution_time import get_execution_time_log
+from execution_time_wrapper import get_execution_time_print, get_execution_time_log
 
-@get_execution_time_log
+@get_execution_time_print
 def my_fun():
     print("Hello World!")
 ```
-The same for the other method given, i.e. `get_execution_time_print`.
+```python
+my_fun()
+```
+```console
+>> Hello World!
+>> Computation time for my_fun: 0.02 ms
+```
+However, if the function takes more time:
+```python
+from execution_time_wrapper import get_execution_time_print, get_execution_time_log
+from time import sleep
+
+@get_execution_time_print
+def my_fun():
+    sleep(4)
+    print("Hello World!")
+```
+```python
+my_fun()
+```
+```console
+>> Hello World!
+>> Computation time for my_fun: 4.00 s
+```
+
+The same for the other method given, i.e. `get_execution_time_log`.
 
 ## TODOs
 
 [ ] Implement logger level
 
 @2022, Leonardo Alchieri
```

### Comparing `execution_time_wrapper-1.0.0/execution_time_wrapper/log_based.py` & `execution_time_wrapper-1.0.1/execution_time_wrapper/log_based.py`

 * *Files identical despite different names*

### Comparing `execution_time_wrapper-1.0.0/execution_time_wrapper/print_based.py` & `execution_time_wrapper-1.0.1/execution_time_wrapper/print_based.py`

 * *Files identical despite different names*

### Comparing `execution_time_wrapper-1.0.0/execution_time_wrapper.egg-info/PKG-INFO` & `execution_time_wrapper-1.0.1/execution_time_wrapper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: execution-time-wrapper
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package with some simple wrapper functions to print the execution time of methods
 Home-page: https://github.com/LeonardoAlchieri/ExecutionTimeWrapper
 Author: Leonardo Alchieri
 Author-email: leonardo@alchieri.eu
 License: MIT
 Keywords: time,wrapper,log,print,execution,speed
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,37 +18,60 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.org/project/execution-time-wrapper/)
-[![PyPI version fury.io](https://badge.fury.io/py/ansicolortags.svg)](https://pypi.org/project/execution-time-wrapper/)
+[![PyPI version](https://badge.fury.io/py/execution-time-wrapper.svg)](https://badge.fury.io/py/execution-time-wrapper)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/pybadges.svg)](https://pypi.org/project/execution-time-wrapper/)
-[![Downloads](https://pepy.tech/badge/apple-heartrate-pandas)](https://pepy.tech/project/execution-time-wrapper)
+[![Downloads](https://pepy.tech/badge/execution-time-wrapper)](https://pepy.tech/project/execution-time-wrapper)
 
 # Execution Time Wrapper
 
 A simple package with a few method to get the execution time of methods through wrapping.
 
 ## Usage
 
-Currently, the package contains two methods, one which returns to sdout (print) and one which goes to a logger.
+Currently, the package contains two methods, one which returns to sdout (print) and one which goes to a logger. The method prints the time in a nice way, i.e. milliseconds, seconds, minutes or hours. For example:
 
 ```python
-from execution_time import get_execution_time_log
+from execution_time_wrapper import get_execution_time_print, get_execution_time_log
 
-@get_execution_time_log
+@get_execution_time_print
 def my_fun():
     print("Hello World!")
 ```
-The same for the other method given, i.e. `get_execution_time_print`.
+```python
+my_fun()
+```
+```console
+>> Hello World!
+>> Computation time for my_fun: 0.02 ms
+```
+However, if the function takes more time:
+```python
+from execution_time_wrapper import get_execution_time_print, get_execution_time_log
+from time import sleep
+
+@get_execution_time_print
+def my_fun():
+    sleep(4)
+    print("Hello World!")
+```
+```python
+my_fun()
+```
+```console
+>> Hello World!
+>> Computation time for my_fun: 4.00 s
+```
+
+The same for the other method given, i.e. `get_execution_time_log`.
 
 ## TODOs
 
 [ ] Implement logger level
 
 @2022, Leonardo Alchieri
 
 <sub>People-Centered Computing Lab - [Università della Svizzera italiana, Switzerland](https://www.usi.ch/en)</sub>
-
-
```

### Comparing `execution_time_wrapper-1.0.0/setup.py` & `execution_time_wrapper-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from os import path
 with open(path.join(path.abspath(path.dirname(__file__)), "README.md")) as f:
     readme = f.read()
 
 setup(
     name='execution_time_wrapper',
-    version="1.0.0",
+    version="1.0.1",
     license='MIT',
     url='https://github.com/LeonardoAlchieri/ExecutionTimeWrapper',
     author='Leonardo Alchieri',
     author_email='leonardo@alchieri.eu',
     description='A Python package with some simple wrapper functions to print the execution time of methods',
     long_description=readme,
     long_description_content_type="text/markdown",
@@ -27,12 +27,9 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3 :: Only",
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
     ],
-    python_requires=">=3.6",
-    install_requires=[
-    'python_version>="3.6"',
-]
+    python_requires='>=3.6',
 )
```

