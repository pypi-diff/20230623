# Comparing `tmp/swh.perfecthash-0.1.2.tar.gz` & `tmp/swh.perfecthash-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.perfecthash-0.1.2.tar", last modified: Tue Jan 25 15:04:22 2022, max compression
+gzip compressed data, was "swh.perfecthash-1.0.0rc1.tar", last modified: Fri Jun 23 16:27:25 2023, max compression
```

## Comparing `swh.perfecthash-0.1.2.tar` & `swh.perfecthash-1.0.0rc1.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/
--rw-r--r--   0 jenkins    (115) docker     (999)      254 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)     1020 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      147 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1133 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      172 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/README.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      669 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)     3680 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/docs/benchmarks.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      628 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/docs/format.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      356 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      317 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       33 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       66 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        7 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      231 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       93 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2393 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/swh/perfecthash/
--rw-r--r--   0 jenkins    (115) docker     (999)       19 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/swh/perfecthash/.clang-format
--rw-r--r--   0 jenkins    (115) docker     (999)      552 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/swh/perfecthash/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     3583 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/swh/perfecthash/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1441 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/swh/perfecthash/build.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13776 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/swh/perfecthash/hash.c
--rw-r--r--   0 jenkins    (115) docker     (999)     1618 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/swh/perfecthash/hash.h
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/swh/perfecthash/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     5635 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/swh/perfecthash/test_hash.cpp
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/swh/perfecthash/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/swh/perfecthash/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4654 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/swh/perfecthash/tests/test_hash.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/swh.perfecthash.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1133 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/swh.perfecthash.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      885 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/swh.perfecthash.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/swh.perfecthash.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       23 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/swh.perfecthash.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2022-01-25 15:04:22.000000 swh.perfecthash-0.1.2/swh.perfecthash.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1544 2022-01-25 15:04:18.000000 swh.perfecthash-0.1.2/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.581641 swh.perfecthash-1.0.0rc1/
+-rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      279 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      147 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1099 2023-06-23 16:27:25.581641 swh.perfecthash-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      172 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/README.rst
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      350 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/build_cmph.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      733 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)     3696 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/benchmarks.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      628 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/format.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      470 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      317 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      487 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       66 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        7 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      231 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-23 16:27:25.581641 swh.perfecthash-1.0.0rc1/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2393 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/swh/perfecthash/
+-rw-r--r--   0 jenkins    (115) docker     (999)       19 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/.clang-format
+-rw-r--r--   0 jenkins    (115) docker     (999)      552 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     3583 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1751 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/build.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13776 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/hash.c
+-rw-r--r--   0 jenkins    (115) docker     (999)     1618 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/hash.h
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     5635 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/test_hash.cpp
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/swh/perfecthash/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4654 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/swh/perfecthash/tests/test_hash.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 16:27:25.577641 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1099 2023-06-23 16:27:25.000000 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      922 2023-06-23 16:27:25.000000 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-23 16:27:25.000000 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       23 2023-06-23 16:27:25.000000 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-23 16:27:25.000000 swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1623 2023-06-23 16:27:19.000000 swh.perfecthash-1.0.0rc1/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swh.perfecthash-0.1.2/CODE_OF_CONDUCT.md` & `swh.perfecthash-1.0.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-0.1.2/LICENSE` & `swh.perfecthash-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-0.1.2/PKG-INFO` & `swh.perfecthash-1.0.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: swh.perfecthash
-Version: 0.1.2
+Version: 1.0.0rc1
 Summary: Software Heritage Perfect Hash
 Home-page: https://forge.softwareheritage.org/source/swh-perfecthash
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
-License: UNKNOWN
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-perfecthash
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-perfecthash/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -22,9 +20,7 @@
 License-File: LICENSE
 License-File: AUTHORS
 
 Perfect Hash table for Software Heritage Object Storage
 =======================================================
 
 A perfect hash table for software heritage object storage.
-
-
```

### Comparing `swh.perfecthash-0.1.2/conftest.py` & `swh.perfecthash-1.0.0rc1/conftest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 def pytest_addoption(parser):
     parser.addoption(
-        "--shard-size", default=10, type=int, help="Size of the Read Shard file in MB",
+        "--shard-size",
+        default=10,
+        type=int,
+        help="Size of the Read Shard file in MB",
     )
     parser.addoption(
-        "--shard-path", default="/tmp/payload", help="Path of the Read Shard file",
+        "--shard-path",
+        default="/tmp/payload",
+        help="Path of the Read Shard file",
     )
     parser.addoption(
         "--shard-count",
         default=2,
         type=int,
         help="Number of Read Shard files for lookup tests",
     )
     parser.addoption(
         "--object-max-size",
         default=10 * 1024,
         type=int,
         help="Maximum size of an object in bytes",
     )
     parser.addoption(
-        "--lookups", default=10, type=int, help="Number of lookups to perform",
+        "--lookups",
+        default=10,
+        type=int,
+        help="Number of lookups to perform",
     )
```

### Comparing `swh.perfecthash-0.1.2/docs/benchmarks.rst` & `swh.perfecthash-1.0.0rc1/docs/benchmarks.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,41 +23,41 @@
 With a small number of large (<100MB) objects
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The goal is to verify that manipulating up to the largest supported
 object size actually works and does not trigger problems in the
 extreme case that all objects have the maximum size.
 
-* time tox -e py3 -- --basetemp=/mnt/pytest -s --shard-path /mnt/payload --shard-size $((100 * 1024)) --object-max-size $((100 * 1024 * 1024)) -k test_build_speed
+* time tox run -e py3 -- --basetemp=/mnt/pytest -s --shard-path /mnt/payload --shard-size $((100 * 1024)) --object-max-size $((100 * 1024 * 1024)) -k test_build_speed
   number of objects = 2057, total size = 107374116576
   baseline 165.85, write_duration 327.19, build_duration 0.0062, total_duration 327.19
 
 With a large number of small (<4KB) objects
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 It approximates the maximum number of objects a Read Shard can
 contain. The goal is to verify that creating a perfect hash with this
 many items does not require more than a fraction of the time required
 to copy the objects.
 
-* time tox -e py3 -- --basetemp=/mnt/pytest -s --shard-path /mnt/payload --shard-size $((100 * 1024)) --object-max-size $((4 * 1024)) -k test_build_speed
+* time tox run -e py3 -- --basetemp=/mnt/pytest -s --shard-path /mnt/payload --shard-size $((100 * 1024)) --object-max-size $((4 * 1024)) -k test_build_speed
   number of objects = 45973694, total size = 105903024192
   baseline 165.74, write_duration 495.07, build_duration 24.21, total_duration 519.28
 
 
 Object lookup performances
 --------------------------
 
 The machine has 200GB of RAM and can therefore approximately cache the
 content of two Read Shards which can have a significant impact on
 performances. To minimize that effect, four Read Shard are created
 totaling 400GB. All objects are looked up in all shards to verify
 the lookup speed is greater than 5,000 objects per second.
 
-* time tox -e py3 -- --basetemp=/mnt/pytest -s -k test_lookup_speed --lookups $((100 * 1024 * 1024)) --shard-size $((100 * 1024)) --object-max-size $((4 * 1024)) swh/perfecthash/tests/test_hash.py  --shard-path /mnt/payload --shard-count 4
+* time tox run -e py3 -- --basetemp=/mnt/pytest -s -k test_lookup_speed --lookups $((100 * 1024 * 1024)) --shard-size $((100 * 1024)) --object-max-size $((4 * 1024)) swh/perfecthash/tests/test_hash.py  --shard-path /mnt/payload --shard-count 4
   number of objects = 45974390, total size = 105903001920
   key lookups speed = 9769.68/s
 
 
 Setup via Fed4Fire
 ------------------
 
@@ -86,8 +86,8 @@
 * mount /dev/sdc /mnt
 * apt-get install -y python3-venv python3-dev libcmph-dev gcc git emacs-nox
 * git clone -b wip-benchmark https://git.easter-eggs.org/biceps/swh-perfecthash/
 * python3 -m venv bench
 * source bench/bin/activate
 * cd swh-perfecthash
 * pip install -r requirements.txt -r requirements-test.txt tox wheel
-* tox -e py3
+* tox run -e py3
```

### Comparing `swh.perfecthash-0.1.2/docs/format.rst` & `swh.perfecthash-1.0.0rc1/docs/format.rst`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-0.1.2/setup.py` & `swh.perfecthash-1.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-0.1.2/swh/perfecthash/Makefile` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/Makefile`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-0.1.2/swh/perfecthash/__init__.py` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-0.1.2/swh/perfecthash/hash.c` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/hash.c`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-0.1.2/swh/perfecthash/hash.h` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/hash.h`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-0.1.2/swh/perfecthash/test_hash.cpp` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/test_hash.cpp`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-0.1.2/swh/perfecthash/tests/test_hash.py` & `swh.perfecthash-1.0.0rc1/swh/perfecthash/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `swh.perfecthash-0.1.2/swh.perfecthash.egg-info/PKG-INFO` & `swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: swh.perfecthash
-Version: 0.1.2
+Version: 1.0.0rc1
 Summary: Software Heritage Perfect Hash
 Home-page: https://forge.softwareheritage.org/source/swh-perfecthash
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
-License: UNKNOWN
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-perfecthash
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-perfecthash/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -22,9 +20,7 @@
 License-File: LICENSE
 License-File: AUTHORS
 
 Perfect Hash table for Software Heritage Object Storage
 =======================================================
 
 A perfect hash table for software heritage object storage.
-
-
```

### Comparing `swh.perfecthash-0.1.2/swh.perfecthash.egg-info/SOURCES.txt` & `swh.perfecthash-1.0.0rc1/swh.perfecthash.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+.git-blame-ignore-revs
 .gitignore
 .pre-commit-config.yaml
 AUTHORS
 CODE_OF_CONDUCT.md
 CONTRIBUTORS
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
+build_cmph.sh
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 requirements-swh.txt
 requirements-test.txt
 requirements.txt
```

### Comparing `swh.perfecthash-0.1.2/tox.ini` & `swh.perfecthash-1.0.0rc1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 [tox]
+requires =
+  tox>4
 envlist=black,flake8,mypy,py3,c
 
 [testenv]
 extras =
   testing
 deps =
   pytest-cov
@@ -11,69 +13,68 @@
          {envsitepackagesdir}/swh/perfecthash \
          --cov={envsitepackagesdir}/swh/perfecthash \
          --cov-branch {posargs}
 
 [testenv:black]
 skip_install = true
 deps =
-  black==19.10b0
+  black==22.10.0
 commands =
   {envpython} -m black --check swh
 
 [testenv:c]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 commands =
   make -C swh/perfecthash check
 
 [testenv:flake8]
 skip_install = true
 deps =
-  flake8
+  flake8==5.0.4
+  flake8-bugbear==22.9.23
+  pycodestyle==2.9.1
 commands =
   {envpython} -m flake8
 
 [testenv:mypy]
 extras =
   testing
 deps =
-  mypy==0.920
+  mypy==1.0.1
 commands =
   mypy swh
 
 # build documentation outside swh-environment using the current
 # git HEAD of swh-docs, is executed on CI for each diff to prevent
 # breaking doc build
 [testenv:sphinx]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
 deps =
   # fetch and install swh-docs in develop mode
-  -e git+https://forge.softwareheritage.org/source/swh-docs#egg=swh.docs
-
+  -e git+https://gitlab.softwareheritage.org/swh/devel/swh-docs.git\#egg=swh.docs
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx/src/swh-docs/swh/ -C docs
 
-
 # build documentation only inside swh-environment using local state
 # of swh-docs package
 [testenv:sphinx-dev]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
 deps =
   # install swh-docs in develop mode
   -e ../swh-docs
-
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx-dev/src/swh-docs/swh/ -C docs
```

