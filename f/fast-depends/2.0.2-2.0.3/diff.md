# Comparing `tmp/fast_depends-2.0.2.tar.gz` & `tmp/fast_depends-2.0.3.tar.gz`

## Comparing `fast_depends-2.0.2.tar` & `fast_depends-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.2/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.2/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fast_depends-2.0.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/__init__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/_compat.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/use.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/core/__init__.py
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/core/build.py
--rw-r--r--   0        0        0     8822 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/core/model.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/dependencies/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/dependencies/model.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/dependencies/provider.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.2/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.2/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.2/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.2/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.2/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.2/LICENSE
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 fast_depends-2.0.2/README.md
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 fast_depends-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     6762 2020-02-02 00:00:00.000000 fast_depends-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.0.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.0.3/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.0.3/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.0.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/__init__.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/_compat.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/use.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/core/__init__.py
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/core/build.py
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/core/model.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/dependencies/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/dependencies/model.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/dependencies/provider.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.0.3/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.0.3/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.0.3/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.0.3/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.0.3/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.0.3/LICENSE
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 fast_depends-2.0.3/README.md
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 fast_depends-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 fast_depends-2.0.3/PKG-INFO
```

### Comparing `fast_depends-2.0.2/CONTRIBUTING.md` & `fast_depends-2.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.2/.github/workflows/documentation.yml` & `fast_depends-2.0.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.2/.github/workflows/publish_coverage.yml` & `fast_depends-2.0.3/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.2/.github/workflows/publish_pypi.yml` & `fast_depends-2.0.3/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.2/.github/workflows/tests.yml` & `fast_depends-2.0.3/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        pydantic-version: ["pydantic-v1", "pydantic-v2"]
       fail-fast: false
     
     services:
       redis:
         image: rabbitmq
         ports:
           - 5672:5672
@@ -31,14 +32,20 @@
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test-v03
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install -e .[test]
+      - name: Install Pydantic v1
+        if: matrix.pydantic-version == 'pydantic-v1'
+        run: pip install "pydantic>=1.10.0,<2.0.0"
+      - name: Install Pydantic v2
+        if: matrix.pydantic-version == 'pydantic-v2'
+        run: pip install --pre "pydantic>=2.0.0b2,<3.0.0"
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh
         env:
           COVERAGE_FILE: coverage/.coverage.${{ runner.os }}-py${{ matrix.python-version }}
           CONTEXT: ${{ runner.os }}-py${{ matrix.python-version }}
       - name: Store coverage files
```

### Comparing `fast_depends-2.0.2/fast_depends/_compat.py` & `fast_depends-2.0.3/fast_depends/_compat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from pydantic import BaseModel, create_model
 from pydantic.version import VERSION as PYDANTIC_VERSION
 
 PYDANTIC_V2 = PYDANTIC_VERSION.startswith("2.")
 
 if PYDANTIC_V2:
     from pydantic._internal._typing_extra import (
-        eval_type_lenient as evaluate_forwardref,  # type: ignore
+        eval_type_lenient as evaluate_forwardref,
     )
-    from pydantic.fields import FieldInfo  # type: ignore
+    from pydantic.fields import FieldInfo
 else:
-    from pydantic.fields import ModelField as FieldInfo  # type: ignore
+    from pydantic.fields import ModelField as FieldInfo  # type: ignore[no-redef]
     from pydantic.typing import evaluate_forwardref  # type: ignore[no-redef]
 
 
 __all__ = (
     "BaseModel",
     "FieldInfo",
     "create_model",
```

### Comparing `fast_depends-2.0.2/fast_depends/use.py` & `fast_depends-2.0.3/fast_depends/use.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.2/fast_depends/utils.py` & `fast_depends-2.0.3/fast_depends/utils.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.2/fast_depends/core/build.py` & `fast_depends-2.0.3/fast_depends/core/build.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.2/fast_depends/core/model.py` & `fast_depends-2.0.3/fast_depends/core/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,28 @@
     use_cache: bool
     cast: bool
 
     @property
     def call_name(self) -> str:
         return getattr(self.call, "__name__", type(self.call).__name__)
 
+    @property
+    def real_params(self) -> Dict[str, FieldInfo]:
+        params = self.params.copy()
+        for name in self.custom_fields.keys():
+            params.pop(name, None)
+        return params
+
+    @property
+    def flat_params(self) -> Dict[str, FieldInfo]:
+        params = self.real_params
+        for d in self.dependencies.values():
+            params.update(d.flat_params)
+        return params
+
     def __init__(
         self,
         call: Union[
             Callable[P, T],
             Callable[P, Awaitable[T]],
         ],
         model: Type[BaseModel],
@@ -85,19 +99,16 @@
         self.dependencies = dependencies or {}
         self.extra_dependencies = extra_dependencies or []
         self.custom_fields = custom_fields or {}
 
         self.alias_arguments = [f.alias or name for name, f in fields.items()]
 
         self.params = fields.copy()
-        self.flat_params = {}
-        for name, d in self.dependencies.items():
+        for name in self.dependencies.keys():
             self.params.pop(name, None)
-            self.flat_params.update(d.flat_params)
-        self.flat_params.update(self.params)
 
         self.use_cache = use_cache
         self.cast = cast
         self.is_async = is_async or is_coroutine_callable(call)
         self.is_generator = is_gen_callable(self.call) or is_async_gen_callable(
             self.call
         )
```

### Comparing `fast_depends-2.0.2/fast_depends/dependencies/model.py` & `fast_depends-2.0.3/fast_depends/dependencies/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.2/fast_depends/library/model.py` & `fast_depends-2.0.3/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.2/LICENSE` & `fast_depends-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.2/README.md` & `fast_depends-2.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -127,15 +127,7 @@
 def my_func(header_field: int = Header()):
     return header_field
 
 assert my_func(
     headers={ "header_field": "1" }
 ) == 1
 ```
-
----
-
-### Note
-Library was based on **0.95.0 FastAPI** version.
-
-If we are too far behind, please, contact [me](mailto:diementros@yandex.ru)
-or contubute yourself. Really appreciate your help.
```

### Comparing `fast_depends-2.0.2/pyproject.toml` & `fast_depends-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.0.2/PKG-INFO` & `fast_depends-2.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 2.0.2
+Version: 2.0.3
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -180,15 +180,7 @@
 def my_func(header_field: int = Header()):
     return header_field
 
 assert my_func(
     headers={ "header_field": "1" }
 ) == 1
 ```
-
----
-
-### Note
-Library was based on **0.95.0 FastAPI** version.
-
-If we are too far behind, please, contact [me](mailto:diementros@yandex.ru)
-or contubute yourself. Really appreciate your help.
```

