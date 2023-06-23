# Comparing `tmp/fast_depends-2.0.3.tar.gz` & `tmp/fast_depends-2.0.4.tar.gz`

## Comparing `fast_depends-2.0.3.tar` & `fast_depends-2.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.3/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.3/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.3/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.0.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/_compat.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/use.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/core/__init__.py
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/core/build.py
--rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/core/model.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/dependencies/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/dependencies/model.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/dependencies/provider.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.3/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.3/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.3/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.3/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.3/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.3/LICENSE
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 fast_depends-2.0.3/README.md
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 fast_depends-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 fast_depends-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.4/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.4/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.4/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.0.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/__init__.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/_compat.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/use.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/core/__init__.py
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/core/build.py
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/core/model.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/dependencies/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/dependencies/model.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/dependencies/provider.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.4/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.4/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.4/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.4/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.4/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.4/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.4/LICENSE
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 fast_depends-2.0.4/README.md
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 fast_depends-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 fast_depends-2.0.4/PKG-INFO
```

### Comparing `fast_depends-2.0.3/CONTRIBUTING.md` & `fast_depends-2.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/.github/workflows/documentation.yml` & `fast_depends-2.0.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/.github/workflows/publish_coverage.yml` & `fast_depends-2.0.4/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/.github/workflows/publish_pypi.yml` & `fast_depends-2.0.4/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/.github/workflows/tests.yml` & `fast_depends-2.0.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/fast_depends/_compat.py` & `fast_depends-2.0.4/fast_depends/_compat.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/fast_depends/use.py` & `fast_depends-2.0.4/fast_depends/use.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/fast_depends/utils.py` & `fast_depends-2.0.4/fast_depends/utils.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/fast_depends/core/build.py` & `fast_depends-2.0.4/fast_depends/core/build.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/fast_depends/core/model.py` & `fast_depends-2.0.4/fast_depends/core/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/fast_depends/dependencies/model.py` & `fast_depends-2.0.4/fast_depends/dependencies/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/fast_depends/library/model.py` & `fast_depends-2.0.4/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/LICENSE` & `fast_depends-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/README.md` & `fast_depends-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.3/pyproject.toml` & `fast_depends-2.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Framework :: Pydantic",
     "Framework :: Pydantic :: 1",
 ]
 
 dependencies = [
-    "pydantic>=1.10",
+    "pydantic>=1.7.4,!=1.8,!=1.8.1,<3.0.0",
     "anyio",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://lancetnik.github.io/FastDepends/"
```

### Comparing `fast_depends-2.0.3/PKG-INFO` & `fast_depends-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 2.0.3
+Version: 2.0.4
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: anyio
-Requires-Dist: pydantic>=1.10
+Requires-Dist: pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4
 Provides-Extra: dev
 Requires-Dist: black>=23.3.0; extra == 'dev'
 Requires-Dist: fast-depends[doc]; extra == 'dev'
 Requires-Dist: fast-depends[test]; extra == 'dev'
 Requires-Dist: isort>=5; extra == 'dev'
 Requires-Dist: mypy>=1.1; extra == 'dev'
 Requires-Dist: ruff>=0.0.260; extra == 'dev'
```

