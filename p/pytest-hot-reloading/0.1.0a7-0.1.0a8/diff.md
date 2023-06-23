# Comparing `tmp/pytest_hot_reloading-0.1.0a7.tar.gz` & `tmp/pytest_hot_reloading-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_hot_reloading-0.1.0a7.tar", max compression
+gzip compressed data, was "pytest_hot_reloading-0.1.0a8.tar", max compression
```

## Comparing `pytest_hot_reloading-0.1.0a7.tar` & `pytest_hot_reloading-0.1.0a8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2023-06-16 20:01:51.315319 pytest_hot_reloading-0.1.0a7/LICENSE
--rw-r--r--   0        0        0     4916 2023-06-16 20:01:51.315319 pytest_hot_reloading-0.1.0a7/README.md
--rw-r--r--   0        0        0     1037 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/__init__.py
--rw-r--r--   0        0        0     2435 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/client.py
--rw-r--r--   0        0        0    10617 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/daemon.py
--rw-r--r--   0        0        0     9551 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/plugin.py
--rw-r--r--   0        0        0        1 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/py.typed
--rw-r--r--   0        0        0     2305 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/workarounds.py
--rw-r--r--   0        0        0     5414 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-23 00:51:16.873262 pytest_hot_reloading-0.1.0a8/LICENSE
+-rw-r--r--   0        0        0     5736 2023-06-23 00:51:16.873262 pytest_hot_reloading-0.1.0a8/README.md
+-rw-r--r--   0        0        0     1037 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/__init__.py
+-rw-r--r--   0        0        0     2450 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/client.py
+-rw-r--r--   0        0        0    10754 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/daemon.py
+-rw-r--r--   0        0        0     9705 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/plugin.py
+-rw-r--r--   0        0        0        1 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/py.typed
+-rw-r--r--   0        0        0     2305 2023-06-23 00:51:16.893262 pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/workarounds.py
+-rw-r--r--   0        0        0     6234 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a8/PKG-INFO
```

### Comparing `pytest_hot_reloading-0.1.0a7/LICENSE` & `pytest_hot_reloading-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a7/README.md` & `pytest_hot_reloading-0.1.0a8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,77 @@
 # A PyTest Hot Reloading Plugin
+![versions](https://img.shields.io/pypi/pyversions/pytest-hot-reloading)
+
 A hot reloading pytest daemon, implemented as a plugin.
 
-This uses the [jurigged](https://github.com/breuleux/jurigged) library to watch files.
+## Features
+- Uses the [jurigged](https://github.com/breuleux/jurigged) library to watch and hot reload files
+- Caches test discovery in many situations
+- Improved performance by not having to import libraries again and again and skipping initializtion logic
+- System for registering workarounds in case something doesn't work out of the box
+
+## Trade-offs
+- First run is slower
+- May not work with some libraries
+- Sometimes gets in a bad state and needs to be restarted
 
 If it takes less than 5 seconds to do all of the imports
-necessary to run a unit test, then you probably don't need this. If you use Django,
-you'll probably love this.
+necessary to run a unit test, then you probably don't need this.
+
+If you're using Django, recommended to use `--keep-db` to preserve the test database.
 
 The minimum Python version is 3.10
 
 ## Demo
 
 ### With hot reloading
+Slower initial start time but faster subsequent runs
+
 ![Hot reloading demo](docs/hot-reloading-demo.gif)
 
 ### Without hot reloading
 ![Not hot reloading demo](docs/not-hot-reloading-demo.gif)
 
 ## Installation
 Do not install in production code. This is exclusively for the developer environment.
 
-pip: Add `pytest-hot-reloading` to your `dev-requirements.txt` file and `pip install -r dev-requirements.txt`
+**pip**: Add `pytest-hot-reloading` to your `dev-requirements.txt` file and `pip install -r dev-requirements.txt`
 
-poetry: `poetry add --group=dev pytest-hot-reloading`
+**poetry**: `poetry add --group=dev pytest-hot-reloading`
 
 
 ## Usage
-Add the plugin to the pytest arguments. Example using pyproject.toml:
+Add the plugin to the pytest arguments.
+
+Example using pyproject.toml:
 ```toml
 [tool.pytest.ini_options]
 addopts = "-p pytest_hot_reloading.plugin"
 ```
 
 When running pytest, the plugin will detect whether the daemon is running, and start it if is not.
 Note that a pid file is created to track the pid.
 
-Imports are not reran on subsequent runs, which can be a huge time saver.
+Imports and in many cases initialization logic are not reran on subsequent runs, which can be a huge time saver.
 
 Currently, if you want to debug, you will want to run the daemon manually with debugging.
+
+### JetBrains (IDEA, PyCharm, etc)
+
+Create a REGULAR Python run configuration, with pytest as the *module*. For parameters, add `--daemon`. Strongly consider storing
+in the project so it is shared with other developers.
+
+![JetBrains Example](docs/jetbrains-hot-reloading-example.png)
+
+For more information on parameters, see the VS Code section below.
+
+### VS Code
+
+![Debugging demo](docs/hot-reloading-debug.gif)
+
 This can easily be done in VS Code with the following launch profile:
 
 ```json
         {
             "name": "Pytest Daemon",
             "type": "python",
             "request": "launch",
@@ -117,13 +147,11 @@
 module `_clear_hot_reload_workarounds.py`. If this is successfully imported, then workarounds for
 the given module will not be executed.
 
 ## Known Issues
 - This is early alpha
 - The jurigged library is not perfect and sometimes it gets in a bad state
 - Some libraries were not written with hot reloading in mind, and will not work without some changes.
-  There is going to be logic to work around other issues with other libraries, such as pytest-django's
-  mutation of the settings module that runs every session, but it hasn't been implemented yet.
 
 ## Notes
 - pytest-xdist will have its logic disabled, even if args are passed in to enable it
 - pytest-django will not create test database suffixes for multiworker runs such as tox.
```

### Comparing `pytest_hot_reloading-0.1.0a7/pyproject.toml` & `pytest_hot_reloading-0.1.0a8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 120
 
 [tool.black]
 line-length = 98
 
 [tool.poetry]
 name = "pytest-hot-reloading"
-version = "0.1.0-alpha.7"
+version = "0.1.0-alpha.8"
 description = ""
 authors = ["James Hutchison <jamesghutchison@proton.me>"]
 readme = "README.md"
 packages = [{ include = "pytest_hot_reloading" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/client.py` & `pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 
     def _get_server(self) -> xmlrpc.client.ServerProxy:
         server_url = f"http://{self._daemon_host}:{self._daemon_port}"
         server = xmlrpc.client.ServerProxy(server_url)
 
         return server
 
-    def run(self, args: list[str]) -> int:
+    def run(self, cwd: str, args: list[str]) -> int:
         self._start_daemon_if_needed()
 
         server = self._get_server()
 
         start = time.time()
-        result: dict = cast(dict, server.run_pytest(args))
+        result: dict = cast(dict, server.run_pytest(cwd, args))
         print(f"Daemon took {(time.time() - start):.3f} seconds to reply")
 
         stdout = result["stdout"].data.decode("utf-8")
         stderr = result["stderr"].data.decode("utf-8")
 
         print(stdout, file=sys.stdout)
         print(stderr, file=sys.stderr)
```

### Comparing `pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/daemon.py` & `pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         try:
             with open(self.pid_file, "r") as f:
                 pid = int(f.read())
             os.kill(pid, 9)
         except FileNotFoundError:
             raise Exception(f"Port {self._daemon_port} is already in use")
 
-    def run_pytest(self, args: list[str]) -> dict:
+    def run_pytest(self, cwd: str, args: list[str]) -> dict:
         # run pytest using command line args
         # run the pytest main logic
 
         in_progress_workarounds = self._workaround_library_issues_pre()
 
         import pytest_hot_reloading.plugin as plugin
 
@@ -146,18 +146,23 @@
 
         import _pytest.main
 
         # monkeypatch in the main that does test collection caching
         orig_main = _pytest.main._main
         _pytest.main._main = _pytest_main
 
+        # store current working directory
+        prev_cwd = os.getcwd()
+        os.chdir(cwd)
+
         try:
             # args must omit the calling program
             status_code = pytest.main(["--color=yes"] + args)
         finally:
+            os.chdir(prev_cwd)
             self._workaround_library_issues_post(in_progress_workarounds)
 
             # restore originals
             _pytest.main._main = orig_main
 
             sys.stdout = stdout_bak
             sys.stderr = stderr_bak
```

### Comparing `pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/plugin.py` & `pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,20 +194,24 @@
                 for x in sys.argv
             ]
         ):
             if val:
                 pytest_name_index = idx
                 break
         else:
-            print(sys.argv)
-            raise Exception(
-                "Could not find pytest name in args. "
-                "Check the configured name versus the actual name."
-            )
-        status_code = client.run(sys.argv[pytest_name_index + 1 :])
+            if "pytest_runner" in sys.argv[0]:
+                pytest_name_index = 0
+            else:
+                print(sys.argv)
+                raise Exception(
+                    "Could not find pytest name in args. "
+                    "Check the configured name versus the actual name."
+                )
+        cwd = os.getcwd()
+        status_code = client.run(cwd, sys.argv[pytest_name_index + 1 :])
         return status_code
 
 
 def _get_pattern_filters(config: Config) -> str | Callable[[str], bool]:
     """
     Jurigged takes in a pattern argument. The argument is either a glob string
     or a function that returns True if the path passed into it should be watched.
```

### Comparing `pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/workarounds.py` & `pytest_hot_reloading-0.1.0a8/pytest_hot_reloading/workarounds.py`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a7/PKG-INFO` & `pytest_hot_reloading-0.1.0a8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,92 @@
 Metadata-Version: 2.1
 Name: pytest-hot-reloading
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: 
 Author: James Hutchison
 Author-email: jamesghutchison@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cachetools (>=5.3.0,<6.0.0)
 Requires-Dist: jurigged (>=0.5.5,<0.6.0)
 Requires-Dist: types-cachetools (>=5.3.0.5,<6.0.0.0)
 Description-Content-Type: text/markdown
 
 # A PyTest Hot Reloading Plugin
+![versions](https://img.shields.io/pypi/pyversions/pytest-hot-reloading)
+
 A hot reloading pytest daemon, implemented as a plugin.
 
-This uses the [jurigged](https://github.com/breuleux/jurigged) library to watch files.
+## Features
+- Uses the [jurigged](https://github.com/breuleux/jurigged) library to watch and hot reload files
+- Caches test discovery in many situations
+- Improved performance by not having to import libraries again and again and skipping initializtion logic
+- System for registering workarounds in case something doesn't work out of the box
+
+## Trade-offs
+- First run is slower
+- May not work with some libraries
+- Sometimes gets in a bad state and needs to be restarted
 
 If it takes less than 5 seconds to do all of the imports
-necessary to run a unit test, then you probably don't need this. If you use Django,
-you'll probably love this.
+necessary to run a unit test, then you probably don't need this.
+
+If you're using Django, recommended to use `--keep-db` to preserve the test database.
 
 The minimum Python version is 3.10
 
 ## Demo
 
 ### With hot reloading
+Slower initial start time but faster subsequent runs
+
 ![Hot reloading demo](docs/hot-reloading-demo.gif)
 
 ### Without hot reloading
 ![Not hot reloading demo](docs/not-hot-reloading-demo.gif)
 
 ## Installation
 Do not install in production code. This is exclusively for the developer environment.
 
-pip: Add `pytest-hot-reloading` to your `dev-requirements.txt` file and `pip install -r dev-requirements.txt`
+**pip**: Add `pytest-hot-reloading` to your `dev-requirements.txt` file and `pip install -r dev-requirements.txt`
 
-poetry: `poetry add --group=dev pytest-hot-reloading`
+**poetry**: `poetry add --group=dev pytest-hot-reloading`
 
 
 ## Usage
-Add the plugin to the pytest arguments. Example using pyproject.toml:
+Add the plugin to the pytest arguments.
+
+Example using pyproject.toml:
 ```toml
 [tool.pytest.ini_options]
 addopts = "-p pytest_hot_reloading.plugin"
 ```
 
 When running pytest, the plugin will detect whether the daemon is running, and start it if is not.
 Note that a pid file is created to track the pid.
 
-Imports are not reran on subsequent runs, which can be a huge time saver.
+Imports and in many cases initialization logic are not reran on subsequent runs, which can be a huge time saver.
 
 Currently, if you want to debug, you will want to run the daemon manually with debugging.
+
+### JetBrains (IDEA, PyCharm, etc)
+
+Create a REGULAR Python run configuration, with pytest as the *module*. For parameters, add `--daemon`. Strongly consider storing
+in the project so it is shared with other developers.
+
+![JetBrains Example](docs/jetbrains-hot-reloading-example.png)
+
+For more information on parameters, see the VS Code section below.
+
+### VS Code
+
+![Debugging demo](docs/hot-reloading-debug.gif)
+
 This can easily be done in VS Code with the following launch profile:
 
 ```json
         {
             "name": "Pytest Daemon",
             "type": "python",
             "request": "launch",
@@ -132,14 +162,12 @@
 module `_clear_hot_reload_workarounds.py`. If this is successfully imported, then workarounds for
 the given module will not be executed.
 
 ## Known Issues
 - This is early alpha
 - The jurigged library is not perfect and sometimes it gets in a bad state
 - Some libraries were not written with hot reloading in mind, and will not work without some changes.
-  There is going to be logic to work around other issues with other libraries, such as pytest-django's
-  mutation of the settings module that runs every session, but it hasn't been implemented yet.
 
 ## Notes
 - pytest-xdist will have its logic disabled, even if args are passed in to enable it
 - pytest-django will not create test database suffixes for multiworker runs such as tox.
```

