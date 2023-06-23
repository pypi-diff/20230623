# Comparing `tmp/ez_cqrs-1.2.0.tar.gz` & `tmp/ez_cqrs-1.3.0.tar.gz`

## Comparing `ez_cqrs-1.2.0.tar` & `ez_cqrs-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/components.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/error.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/framework.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/py.typed
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/requirements/core.txt
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/README.md
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ez_cqrs-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/error.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/framework.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/py.typed
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/requirements/core.txt
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/README.md
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ez_cqrs-1.3.0/PKG-INFO
```

### Comparing `ez_cqrs-1.2.0/.github/workflows/release.yml` & `ez_cqrs-1.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/.github/workflows/test.yml` & `ez_cqrs-1.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/.vscode/settings.json` & `ez_cqrs-1.3.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/ez_cqrs/acid_exec.py` & `ez_cqrs-1.3.0/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/ez_cqrs/components.py` & `ez_cqrs-1.3.0/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/ez_cqrs/error.py` & `ez_cqrs-1.3.0/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/ez_cqrs/framework.py` & `ez_cqrs-1.3.0/ez_cqrs/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         if not isinstance(validated, Ok):
             return Err(validated.err())
 
         execution_result = await asyncio.create_task(
             coro=self.cmd_handler.handle(
                 command=cmd,
                 ops_registry=OpsRegistry[Any](max_lenght=max_transactions),
+                event_registry=[],
             ),
         )
         if not isinstance(execution_result, Ok):
             return Err(execution_result.err())
 
         event_dispatch_tasks: list[Coroutine[Any, Any, None]] = []
```

### Comparing `ez_cqrs-1.2.0/ez_cqrs/handler.py` & `ez_cqrs-1.3.0/ez_cqrs/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         """Validate command data."""
 
     @abc.abstractmethod
     async def handle(
         self,
         command: C,
         ops_registry: OpsRegistry[Any],
+        event_registry: list[E],
     ) -> Result[tuple[Any, list[E]], ExecutionError]:
         """
         Consume and process commands.
 
         The result should be either a vector of events if the command is successful,
         or an error is the command is rejected.
```

### Comparing `ez_cqrs-1.2.0/ez_cqrs/testing.py` & `ez_cqrs-1.3.0/ez_cqrs/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     ) -> Self:
         """Execute command while asserting and validating framework's rules."""
         ops_registry = OpsRegistry[Any](max_lenght=max_transactions)
         execution_result = await asyncio.create_task(
             self.cmd_handler.handle(
                 command=self.cmd,
                 ops_registry=ops_registry,
+                event_registry=[],
             ),
         )
         if not ops_registry.is_empty():
             msg = "OpsRegistry is not empty after cmd execution."
             raise RuntimeError(msg)
 
         self._result = execution_result
```

### Comparing `ez_cqrs-1.2.0/ez_cqrs/utilities/cli.py` & `ez_cqrs-1.3.0/ez_cqrs/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/requirements/core.txt` & `ez_cqrs-1.3.0/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/requirements/dev.txt` & `ez_cqrs-1.3.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/scripts/new_release.py` & `ez_cqrs-1.3.0/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/tests/integration/conftest.py` & `ez_cqrs-1.3.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/tests/integration/test_execution.py` & `ez_cqrs-1.3.0/tests/integration/test_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,18 @@
 
         assert_never(command)
 
     async def handle(  # noqa: D102
         self,
         command: BankAccountCommand,
         ops_registry: OpsRegistry[Any],
+        event_registry: list[BankAccountEvent],
     ) -> Result[tuple[Any, list[BankAccountEvent]], ExecutionError]:
         _ = ops_registry
+        _ = event_registry
 
         if isinstance(command, OpenAccount):
             return Ok(
                 (
                     None,
                     [
                         AccountOpened(
@@ -158,14 +160,15 @@
         """Test handle method."""
         cmd_handler = BankAccountCommandHandler()
 
         execution_result = await asyncio.create_task(
             cmd_handler.handle(
                 command=command,
                 ops_registry=OpsRegistry[Any](max_lenght=0),
+                event_registry=[],
             ),
         )
         _, resultant_events = execution_result.unwrap()
         assert resultant_events == expected_events
 
     @pytest.mark.parametrize(
         argnames=["cmd_handler", "cmd", "expected_value", "expected_events"],
```

### Comparing `ez_cqrs-1.2.0/tests/unit/test_acid_exec.py` & `ez_cqrs-1.3.0/tests/unit/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/.gitignore` & `ez_cqrs-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/LICENSE` & `ez_cqrs-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.2.0/pyproject.toml` & `ez_cqrs-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "1.2.0"
+version = "1.3.0"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-1.2.0/PKG-INFO` & `ez_cqrs-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 1.2.0
+Version: 1.3.0
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

