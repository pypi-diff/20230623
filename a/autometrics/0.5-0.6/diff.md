# Comparing `tmp/autometrics-0.5.tar.gz` & `tmp/autometrics-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autometrics-0.5.tar", max compression
+gzip compressed data, was "autometrics-0.6.tar", max compression
```

## Comparing `autometrics-0.5.tar` & `autometrics-0.6.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0     1022 2023-04-12 17:23:29.278864 autometrics-0.5/LICENSE
--rw-r--r--   0        0        0     7398 2023-05-11 14:31:00.584949 autometrics-0.5/README.md
--rw-r--r--   0        0        0     2052 2023-05-12 08:30:51.478225 autometrics-0.5/pyproject.toml
--rw-r--r--   0        0        0       25 2023-05-11 14:31:00.585437 autometrics-0.5/src/autometrics/__init__.py
--rw-r--r--   0        0        0     1269 2023-05-11 12:02:53.378510 autometrics-0.5/src/autometrics/constants.py
--rw-r--r--   0        0        0     3979 2023-05-11 14:31:00.585878 autometrics-0.5/src/autometrics/decorator.py
--rw-r--r--   0        0        0     3050 2023-04-13 12:18:19.449416 autometrics-0.5/src/autometrics/objectives.py
--rw-r--r--   0        0        0     2197 2023-05-11 12:02:53.378737 autometrics-0.5/src/autometrics/prometheus_url.py
--rw-r--r--   0        0        0     9729 2023-05-10 12:22:44.149925 autometrics-0.5/src/autometrics/test_decorator.py
--rw-r--r--   0        0        0     3065 2023-05-11 12:02:53.378981 autometrics-0.5/src/autometrics/test_prometheus_url.py
--rw-r--r--   0        0        0       23 2023-05-05 10:51:08.826284 autometrics-0.5/src/autometrics/tracker/__init__.py
--rw-r--r--   0        0        0     4565 2023-05-11 12:02:53.379215 autometrics-0.5/src/autometrics/tracker/opentelemetry.py
--rw-r--r--   0        0        0     3520 2023-05-11 12:02:53.379424 autometrics-0.5/src/autometrics/tracker/prometheus.py
--rw-r--r--   0        0        0     2693 2023-05-11 12:02:53.379696 autometrics-0.5/src/autometrics/tracker/test_tracker.py
--rw-r--r--   0        0        0     2277 2023-05-11 12:02:53.380041 autometrics-0.5/src/autometrics/tracker/tracker.py
--rw-r--r--   0        0        0     1820 2023-05-10 15:25:28.523451 autometrics-0.5/src/autometrics/utils.py
--rw-r--r--   0        0        0     8547 1970-01-01 00:00:00.000000 autometrics-0.5/PKG-INFO
+-rw-r--r--   0        0        0     1022 2023-04-12 17:23:29.278864 autometrics-0.6/LICENSE
+-rw-r--r--   0        0        0     9529 2023-06-23 15:57:11.581730 autometrics-0.6/README.md
+-rw-r--r--   0        0        0     2081 2023-06-23 15:57:11.584556 autometrics-0.6/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-05-16 18:06:49.422047 autometrics-0.6/src/autometrics/__init__.py
+-rw-r--r--   0        0        0       84 2023-06-20 09:32:43.127205 autometrics-0.6/src/autometrics/admin_panel/__init__.py
+-rw-r--r--   0        0        0      574 2023-06-20 09:32:43.127678 autometrics-0.6/src/autometrics/admin_panel/function_registry.py
+-rw-r--r--   0        0        0     1489 2023-06-23 15:57:11.585010 autometrics-0.6/src/autometrics/constants.py
+-rw-r--r--   0        0        0     4967 2023-06-23 15:57:11.585208 autometrics-0.6/src/autometrics/decorator.py
+-rw-r--r--   0        0        0     3050 2023-04-13 12:18:19.449416 autometrics-0.6/src/autometrics/objectives.py
+-rw-r--r--   0        0        0     2197 2023-05-11 12:02:53.378737 autometrics-0.6/src/autometrics/prometheus_url.py
+-rw-r--r--   0        0        0    12055 2023-06-23 15:57:11.585450 autometrics-0.6/src/autometrics/test_decorator.py
+-rw-r--r--   0        0        0     3065 2023-05-11 12:02:53.378981 autometrics-0.6/src/autometrics/test_prometheus_url.py
+-rw-r--r--   0        0        0       23 2023-05-05 10:51:08.826284 autometrics-0.6/src/autometrics/tracker/__init__.py
+-rw-r--r--   0        0        0      680 2023-06-15 09:09:44.376855 autometrics-0.6/src/autometrics/tracker/exemplar.py
+-rw-r--r--   0        0        0     5982 2023-06-23 15:57:11.585695 autometrics-0.6/src/autometrics/tracker/opentelemetry.py
+-rw-r--r--   0        0        0     4347 2023-06-23 15:57:11.585945 autometrics-0.6/src/autometrics/tracker/prometheus.py
+-rw-r--r--   0        0        0     2319 2023-06-23 15:57:11.586326 autometrics-0.6/src/autometrics/tracker/test_concurrency.py
+-rw-r--r--   0        0        0     3027 2023-06-16 11:01:50.465190 autometrics-0.6/src/autometrics/tracker/test_tracker.py
+-rw-r--r--   0        0        0     2615 2023-06-23 15:57:11.586581 autometrics-0.6/src/autometrics/tracker/tracker.py
+-rw-r--r--   0        0        0     1820 2023-05-10 15:25:28.523451 autometrics-0.6/src/autometrics/utils.py
+-rw-r--r--   0        0        0    10678 1970-01-01 00:00:00.000000 autometrics-0.6/PKG-INFO
```

### Comparing `autometrics-0.5/LICENSE` & `autometrics-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autometrics-0.5/README.md` & `autometrics-0.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 ![GitHub_headerImage](https://user-images.githubusercontent.com/3262610/221191767-73b8a8d9-9f8b-440e-8ab6-75cb3c82f2bc.png)
 
-# autometrics-py
+[![Discord Shield](https://discordapp.com/api/guilds/950489382626951178/widget.png?style=shield)](https://discord.gg/kHtwcH8As9)
 
-A Python library that exports a decorator that makes it easy to understand the error rate, response time, and production usage of any function in your code. Jump straight from your IDE to live Prometheus charts for each HTTP/RPC handler, database method, or other piece of application logic.
+> A Python port of the Rust
+> [autometrics-rs](https://github.com/fiberplane/autometrics-rs) library
+
+**Autometrics is a library that exports a decorator that makes it easy to understand the error rate, response time, and production usage of any function in your code.** Jump straight from your IDE to live Prometheus charts for each HTTP/RPC handler, database method, or other piece of application logic.
 
 Autometrics for Python provides:
 
 1. A decorator that can create [Prometheus](https://prometheus.io/) metrics for your functions and class methods throughout your code base.
 2. A helper function that will write corresponding Prometheus queries for you in a Markdown file.
 
 See [Why Autometrics?](https://github.com/autometrics-dev#why-autometrics) for more details on the ideas behind autometrics.
@@ -18,14 +21,15 @@
 - 💡 Writes Prometheus queries so you can understand the data generated without
   knowing PromQL
 - 🔗 Create links to live Prometheus charts directly into each function's docstring
 - [🔍 Identify commits](#identifying-commits-that-introduced-problems) that introduced errors or increased latency
 - [🚨 Define alerts](#alerts--slos) using SLO best practices directly in your source code
 - [📊 Grafana dashboards](#dashboards) work out of the box to visualize the performance of instrumented functions & SLOs
 - [⚙️ Configurable](#metrics-libraries) metric collection library (`opentelemetry`, `prometheus`, or `metrics`)
+- [📍 Attach exemplars](#exemplars) to connect metrics with traces
 - ⚡ Minimal runtime overhead
 
 ## Using autometrics-py
 
 - Set up a [Prometheus instance](https://prometheus.io/download/)
 - Configure prometheus to scrape your application ([check our instructions if you need help](https://github.com/autometrics-dev#5-configuring-prometheus))
 - Include a .env file with your prometheus endpoint `PROMETHEUS_URL=your endpoint`. If this is not defined, the default endpoint will be `http://localhost:9090/`
@@ -37,14 +41,16 @@
 
 @autometrics
 def sayHello:
    return "hello"
 
 ```
 
+- You can also track the number of concurrent calls to a function by using the `track_concurrency` argument: `@autometrics(track_concurrency=True)`. Note: currently only supported by the `prometheus` tracker.
+
 - To access the PromQL queries for your decorated functions, run `help(yourfunction)` or `print(yourfunction.__doc__)`.
 
 - To show tooltips over decorated functions in VSCode, with links to Prometheus queries, try installing [the VSCode extension](https://marketplace.visualstudio.com/items?itemName=Fiberplane.autometrics).
 
 > Note that we cannot support tooltips without a VSCode extension due to behavior of the [static analyzer](https://github.com/davidhalter/jedi/issues/1921) used in VSCode.
 
 ## Dashboards
@@ -53,27 +59,33 @@
 
 ## Alerts / SLOs
 
 Autometrics makes it easy to add Prometheus alerts using Service-Level Objectives (SLOs) to a function or group of functions.
 
 In order to receive alerts you need to add a set of rules to your Prometheus set up. You can find out more about those rules here: [Prometheus alerting rules](https://github.com/autometrics-dev/autometrics-shared#prometheus-recording--alerting-rules). Once added, most of the recording rules are dormant. They are enabled by specific metric labels that can be automatically attached by autometrics.
 
-To use autometrics SLOs and alerts, create one or multiple `Objective`s based on the function(s) success rate and/or latency, as shown below. The `Objective` can be passed as an argument to the `autometrics` macro to include the given function in that objective.
+To use autometrics SLOs and alerts, create one or multiple `Objective`s based on the function(s) success rate and/or latency, as shown below. The `Objective` can be passed as an argument to the `autometrics` decorator to include the given function in that objective.
 
 ```python
 from autometrics import autometrics
 from autometrics.objectives import Objective, ObjectiveLatency, ObjectivePercentile
 
-API_SLO = Objective(
-    "random",
+# Create an objective for a high success rate
+API_SLO_HIGH_SUCCESS = Objective(
+    "My API SLO for High Success Rate (99.9%)",
     success_rate=ObjectivePercentile.P99_9,
+)
+
+# Or you can also create an objective for low latency
+API_SLO_LOW_LATENCY = Objective(
+    "My API SLO for Low Latency (99th percentile < 250ms)",
     latency=(ObjectiveLatency.Ms250, ObjectivePercentile.P99),
 )
 
-@autometrics(objective=API_SLO)
+@autometrics(objective=API_SLO_HIGH_SUCCESS)
 def api_handler():
   # ...
 ```
 
 Autometrics by default will try to store information on which function calls a decorated function. As such you may want to place the autometrics in the top/first decorator, as otherwise you may get `inner` or `wrapper` as the caller function.
 
 So instead of writing:
@@ -106,34 +118,49 @@
 @noop
 def api_handler():
   # ...
 ```
 
 #### Metrics Libraries
 
-Configure the crate that autometrics will use to produce metrics by using one of the following feature flags:
+Configure the package that autometrics will use to produce metrics with the `AUTOMETRICS_TRACKER` environment variable.
 
-- `opentelemetry` - (enabled by default, can also be explicitly set using the AUTOMETRICS_TRACKER="OPEN_TELEMETERY" env var) uses
-- `prometheus` - (using the AUTOMETRICS_TRACKER env var set to "PROMETHEUS")
+- `opentelemetry` - Enabled by default, can also be explicitly set using the env var `AUTOMETRICS_TRACKER="OPEN_TELEMETERY"`. Look in `pyproject.toml` for the versions of the OpenTelemetry packages that will be used.
+- `prometheus` - Can be set using the env var `AUTOMETRICS_TRACKER="PROMETHEUS"`. Look in `pyproject.toml` for the version of the `prometheus-client` package that will be used.
 
 ## Identifying commits that introduced problems
 
 > **NOTE** - As of writing, `build_info` will not work correctly when using the default tracker (`AUTOMETRICS_TRACKER=OPEN_TELEMETRY`).
 > This will be fixed once the following PR is merged on the opentelemetry-python project: https://github.com/open-telemetry/opentelemetry-python/pull/3306
 >
 > autometrics-py will track support for build_info using the OpenTelemetry tracker via #38
 
 Autometrics makes it easy to identify if a specific version or commit introduced errors or increased latencies.
 
-It uses a separate metric (`build_info`) to track the version and, optionally, git commit of your service. It then writes queries that group metrics by the `version` and `commit` labels so you can spot correlations between those and potential issues.
+It uses a separate metric (`build_info`) to track the version and, optionally, git commit of your service. It then writes queries that group metrics by the `version`, `commit` and `branch` labels so you can spot correlations between those and potential issues.
+Configure the labels by setting the following environment variables:
 
-The `version` is read from the `AUTOMETRICS_VERSION` environment variable, and the `commit` value uses the environment variable `AUTOMETRICS_COMMIT`.
+| Label     | Run-Time Environment Variables        | Default value |
+| --------- | ------------------------------------- | ------------- |
+| `version` | `AUTOMETRICS_VERSION`                 | `""`          |
+| `commit`  | `AUTOMETRICS_COMMIT` or `COMMIT_SHA`  | `""`          |
+| `branch`  | `AUTOMETRICS_BRANCH` or `BRANCH_NAME` | `""`          |
 
 This follows the method outlined in [Exposing the software version to Prometheus](https://www.robustperception.io/exposing-the-software-version-to-prometheus/).
 
+## Exemplars
+
+> **NOTE** - As of writing, exemplars aren't supported by the default tracker (`AUTOMETRICS_TRACKER=OPEN_TELEMETRY`).
+> You can track the progress of this feature here: https://github.com/autometrics-dev/autometrics-py/issues/41
+
+Exemplars are a way to associate a metric sample to a trace by attaching `trace_id` and `span_id` to it. You can then use this information to jump from a metric to a trace in your tracing system (for example Jaeger). If you have an OpenTelemetry tracer configured, autometrics will automatically pick up the current span from it.
+
+To use exemplars, you need to first switch to a tracker that supports them by setting `AUTOMETRICS_TRACKER=prometheus` and enable
+exemplar collection by setting `AUTOMETRICS_EXEMPLARS=true`. You also need to enable exemplars in Prometheus by launching Prometheus with the `--enable-feature=exemplar-storage` flag.
+
 ## Development of the package
 
 This package uses [poetry](https://python-poetry.org) as a package manager, with all dependencies separated into three groups:
 
 - root level dependencies, required
 - `dev`, everything that is needed for development or in ci
 - `examples`, dependencies of everything in `examples/` directory
```

### Comparing `autometrics-0.5/pyproject.toml` & `autometrics-0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autometrics"
-version = "0.5"
+version = "0.6"
 description = "Easily add metrics to your system – and actually understand them using automatically customized Prometheus queries"
 authors = ["Fiberplane <info@fiberplane.com>"]
 license = "MIT OR Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/autometrics-dev/autometrics-py"
 homepage = "https://github.com/autometrics-dev/autometrics-py"
 keywords = ["metrics", "telemetry", "prometheus", "monitoring", "observability", "instrumentation"]
@@ -40,15 +40,15 @@
 bleach = "6.0.0"
 build = "0.10.0"
 certifi = "2022.12.7"
 charset-normalizer = "3.1.0"
 click = "8.1.3"
 django = "^4.2"
 docutils = "0.19"
-fastapi = "0.95.0"
+fastapi = "0.97.0"
 h11 = "0.14.0"
 idna = "3.4"
 # pinned importlib-metadat to version ~6.0.0 because of opentelemetry-api
 importlib-metadata = "~6.0.0"
 jaraco-classes = "3.2.3"
 keyring = "23.13.1"
 markdown-it-py = "2.2.0"
@@ -56,23 +56,24 @@
 more-itertools = "9.1.0"
 packaging = "23.0"
 pkginfo = "1.9.6"
 pydantic = "1.10.6"
 pygments = "2.14.0"
 pyproject-hooks = "1.0.0"
 readme-renderer = "37.3"
-requests = "2.28.2"
+requests = "2.31.0"
 requests-toolbelt = "0.10.1"
 rfc3986 = "2.0.0"
 rich = "13.3.2"
 six = "1.16.0"
 sniffio = "1.3.0"
-starlette = "0.26.1"
+starlette = ">=0.27.0,<0.28.0"
 twine = "4.0.2"
 urllib3 = "1.26.15"
 uvicorn = "0.21.1"
 webencodings = "0.5.1"
 zipp = "3.15.0"
+locust = "^2.15.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autometrics-0.5/src/autometrics/constants.py` & `autometrics-0.6/src/autometrics/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """Constants used by autometrics"""
 
 COUNTER_NAME = "function.calls.count"
 HISTOGRAM_NAME = "function.calls.duration"
+CONCURRENCY_NAME = "function.calls.concurrent"
 # NOTE - The Rust implementation does not use `build.info`, instead opts for just `build_info`
 BUILD_INFO_NAME = "build_info"
 
+
 COUNTER_NAME_PROMETHEUS = COUNTER_NAME.replace(".", "_")
 HISTOGRAM_NAME_PROMETHEUS = HISTOGRAM_NAME.replace(".", "_")
+CONCURRENCY_NAME_PROMETHEUS = CONCURRENCY_NAME.replace(".", "_")
 
 COUNTER_DESCRIPTION = "Autometrics counter for tracking function calls"
 HISTOGRAM_DESCRIPTION = "Autometrics histogram for tracking function call duration"
+CONCURRENCY_DESCRIPTION = "Autometrics gauge for tracking function call concurrency"
 BUILD_INFO_DESCRIPTION = (
     "Autometrics info metric for tracking software version and build details"
 )
 
 # The following constants are used to create the labels
 OBJECTIVE_NAME = "objective.name"
 OBJECTIVE_PERCENTILE = "objective.percentile"
 OBJECTIVE_LATENCY_THRESHOLD = "objective.latency_threshold"
 VERSION_KEY = "version"
 COMMIT_KEY = "commit"
+BRANCH_KEY = "branch"
 
 # The values are updated to use underscores instead of periods to avoid issues with prometheus.
 # A similar thing is done in the rust library, which supports multiple exporters
 OBJECTIVE_NAME_PROMETHEUS = OBJECTIVE_NAME.replace(".", "_")
 OBJECTIVE_PERCENTILE_PROMETHEUS = OBJECTIVE_PERCENTILE.replace(".", "_")
 OBJECTIVE_LATENCY_THRESHOLD_PROMETHEUS = OBJECTIVE_LATENCY_THRESHOLD.replace(".", "_")
```

### Comparing `autometrics-0.5/src/autometrics/decorator.py` & `autometrics-0.6/src/autometrics/decorator.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import inspect
 
 from functools import wraps
 from typing import overload, TypeVar, Callable, Optional, Awaitable
 from typing_extensions import ParamSpec
 from .objectives import Objective
 from .tracker import get_tracker, Result
+from .admin_panel import register_function_info
 from .utils import get_module_name, get_caller_function, append_docs_to_docstring
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
@@ -23,32 +24,41 @@
 @overload
 def autometrics(func: Callable[P, Awaitable[T]]) -> Callable[P, Awaitable[T]]:
     ...
 
 
 # Decorator with arguments
 @overload
-def autometrics(*, objective: Optional[Objective] = None) -> Callable:
+def autometrics(
+    *, objective: Optional[Objective] = None, track_concurrency: Optional[bool] = False
+) -> Callable:
     ...
 
 
 def autometrics(
     func: Optional[Callable] = None,
     *,
     objective: Optional[Objective] = None,
+    track_concurrency: Optional[bool] = False,
 ):
     """Decorator for tracking function calls and duration. Supports synchronous and async functions."""
 
+    def track_start(function: str, module: str):
+        get_tracker().start(
+            function=function, module=module, track_concurrency=track_concurrency
+        )
+
     def track_result_ok(start_time: float, function: str, module: str, caller: str):
         get_tracker().finish(
             start_time,
             function=function,
             module=module,
             caller=caller,
             objective=objective,
+            track_concurrency=track_concurrency,
             result=Result.OK,
         )
 
     def track_result_error(
         start_time: float,
         function: str,
         module: str,
@@ -56,29 +66,33 @@
     ):
         get_tracker().finish(
             start_time,
             function=function,
             module=module,
             caller=caller,
             objective=objective,
+            track_concurrency=track_concurrency,
             result=Result.ERROR,
         )
 
     def sync_decorator(func: Callable[P, T]) -> Callable[P, T]:
         """Helper for decorating synchronous functions, to track calls and duration."""
 
         module_name = get_module_name(func)
         func_name = func.__name__
+        register_function_info(func_name, module_name)
 
         @wraps(func)
         def sync_wrapper(*args: P.args, **kwds: P.kwargs) -> T:
             start_time = time.time()
             caller = get_caller_function()
 
             try:
+                if track_concurrency:
+                    track_start(module=module_name, function=func_name)
                 result = func(*args, **kwds)
                 track_result_ok(
                     start_time, function=func_name, module=module_name, caller=caller
                 )
 
             except Exception as exception:
                 result = exception.__class__.__name__
@@ -96,21 +110,24 @@
         return sync_wrapper
 
     def async_decorator(func: Callable[P, Awaitable[T]]) -> Callable[P, Awaitable[T]]:
         """Helper for decorating async functions, to track calls and duration."""
 
         module_name = get_module_name(func)
         func_name = func.__name__
+        register_function_info(func_name, module_name)
 
         @wraps(func)
         async def async_wrapper(*args: P.args, **kwds: P.kwargs) -> T:
             start_time = time.time()
             caller = get_caller_function()
 
             try:
+                if track_concurrency:
+                    track_start(module=module_name, function=func_name)
                 result = await func(*args, **kwds)
                 track_result_ok(
                     start_time, function=func_name, module=module_name, caller=caller
                 )
 
             except Exception as exception:
                 result = exception.__class__.__name__
@@ -123,13 +140,19 @@
                 # Reraise exception
                 raise exception
             return result
 
         async_wrapper.__doc__ = append_docs_to_docstring(func, func_name, module_name)
         return async_wrapper
 
+    def pick_decorator(func: Callable) -> Callable:
+        """Pick the correct decorator based on the function type."""
+        if inspect.iscoroutinefunction(func):
+            return async_decorator(func)
+        return sync_decorator(func)
+
     if func is None:
-        return sync_decorator
+        return pick_decorator
     elif inspect.iscoroutinefunction(func):
         return async_decorator(func)
     else:
         return sync_decorator(func)
```

### Comparing `autometrics-0.5/src/autometrics/objectives.py` & `autometrics-0.6/src/autometrics/objectives.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.5/src/autometrics/prometheus_url.py` & `autometrics-0.6/src/autometrics/prometheus_url.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.5/src/autometrics/test_decorator.py` & `autometrics-0.6/src/autometrics/test_decorator.py`

 * *Files 11% similar despite different names*

```diff
@@ -144,14 +144,58 @@
 
         duration_count = f"""function_calls_duration_count{{function="{function_name}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}}"""
         assert duration_count in data
 
         duration_sum = f"""function_calls_duration_sum{{function="{function_name}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}}"""
         assert duration_sum in data
 
+    @pytest.mark.asyncio
+    async def test_objectives_async(self):
+        """This is a test that covers objectives for async functions."""
+
+        # set up the function + objective variables
+        caller = get_caller_function(depth=1)
+        assert caller is not None
+        assert caller != ""
+        objective_name = "test_objective"
+        success_rate = ObjectivePercentile.P90
+        latency = (ObjectiveLatency.Ms100, ObjectivePercentile.P99)
+        objective = Objective(
+            name=objective_name, success_rate=success_rate, latency=latency
+        )
+        function_name = basic_async_function.__name__
+        wrapped_function = autometrics(objective=objective)(basic_async_function)
+
+        sleep_duration = 0.25
+
+        # Test that the function is *still* async after we wrapped it
+        assert asyncio.iscoroutinefunction(wrapped_function) == True
+
+        await wrapped_function(sleep_duration)
+
+        # get the metrics
+        blob = generate_latest()
+        assert blob is not None
+        data = blob.decode("utf-8")
+
+        total_count = f"""function_calls_count_total{{caller="{caller}",function="{function_name}",module="test_decorator",objective_name="{objective_name}",objective_percentile="{success_rate.value}",result="ok"}} 1.0"""
+        assert total_count in data
+
+        # Check the latency buckets
+        for objective in ObjectiveLatency:
+            count = 0 if float(objective.value) <= sleep_duration else 1
+            query = f"""function_calls_duration_bucket{{function="{function_name}",le="{objective.value}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}} {count}"""
+            assert query in data
+
+        duration_count = f"""function_calls_duration_count{{function="{function_name}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}}"""
+        assert duration_count in data
+
+        duration_sum = f"""function_calls_duration_sum{{function="{function_name}",module="test_decorator",objective_latency_threshold="{latency[0].value}",objective_name="{objective_name}",objective_percentile="{latency[1].value}"}}"""
+        assert duration_sum in data
+
     def test_exception(self):
         """This is a test that covers exceptions."""
         caller = get_caller_function(depth=1)
         assert caller is not None
         assert caller != ""
 
         function_name = error_function.__name__
```

### Comparing `autometrics-0.5/src/autometrics/test_prometheus_url.py` & `autometrics-0.6/src/autometrics/test_prometheus_url.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.5/src/autometrics/tracker/opentelemetry.py` & `autometrics-0.6/src/autometrics/tracker/prometheus.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,150 +1,148 @@
+import os
 import time
 from typing import Optional
-from opentelemetry.metrics import (
-    Meter,
-    Counter,
-    Histogram,
-    UpDownCounter,
-    set_meter_provider,
-)
-
-from opentelemetry.sdk.metrics import MeterProvider
-from opentelemetry.sdk.metrics.export import (
-    MetricReader,
-)
-from opentelemetry.sdk.metrics.view import View, ExplicitBucketHistogramAggregation
+from prometheus_client import Counter, Histogram, Gauge
 
-from opentelemetry.exporter.prometheus import PrometheusMetricReader
-from .tracker import Result
-from ..objectives import Objective, ObjectiveLatency
 from ..constants import (
+    COUNTER_NAME_PROMETHEUS,
+    HISTOGRAM_NAME_PROMETHEUS,
+    CONCURRENCY_NAME_PROMETHEUS,
+    BUILD_INFO_NAME,
     COUNTER_DESCRIPTION,
-    COUNTER_NAME,
     HISTOGRAM_DESCRIPTION,
-    HISTOGRAM_NAME,
-    BUILD_INFO_NAME,
+    CONCURRENCY_DESCRIPTION,
     BUILD_INFO_DESCRIPTION,
-    OBJECTIVE_NAME,
-    OBJECTIVE_PERCENTILE,
-    OBJECTIVE_LATENCY_THRESHOLD,
+    OBJECTIVE_NAME_PROMETHEUS,
+    OBJECTIVE_PERCENTILE_PROMETHEUS,
+    OBJECTIVE_LATENCY_THRESHOLD_PROMETHEUS,
+    COMMIT_KEY,
+    VERSION_KEY,
+    BRANCH_KEY,
 )
 
-FUNCTION_CALLS_DURATION_NAME = "function.calls.duration"
+from .exemplar import get_exemplar
+from .tracker import Result
+from ..objectives import Objective
+
 
+class PrometheusTracker:
+    """A tracker for Prometheus metrics."""
 
-def get_objective_boundaries():
-    """Get the objective latency boundaries as float values in seconds (instead of strings)"""
-    return list(map(lambda c: float(c.value), ObjectiveLatency))
-
-
-class OpenTelemetryTracker:
-    """Tracker for OpenTelemetry."""
-
-    __counter_instance: Counter
-    __histogram_instance: Histogram
-    __up_down_counter_instance: UpDownCounter
-
-    def __init__(self):
-        exporter = PrometheusMetricReader("")
-        view = View(
-            name=HISTOGRAM_NAME,
-            description=HISTOGRAM_DESCRIPTION,
-            instrument_name=HISTOGRAM_NAME,
-            aggregation=ExplicitBucketHistogramAggregation(
-                boundaries=get_objective_boundaries()
-            ),
-        )
-        meter_provider = MeterProvider(metric_readers=[exporter], views=[view])
-        set_meter_provider(meter_provider)
-        meter = meter_provider.get_meter(name="autometrics")
-        self.__counter_instance = meter.create_counter(
-            name=COUNTER_NAME, description=COUNTER_DESCRIPTION
-        )
-        self.__histogram_instance = meter.create_histogram(
-            name=HISTOGRAM_NAME,
-            description=HISTOGRAM_DESCRIPTION,
-        )
-        self.__up_down_counter_instance = meter.create_up_down_counter(
-            name=BUILD_INFO_NAME,
-            description=BUILD_INFO_DESCRIPTION,
-        )
+    prom_counter = Counter(
+        COUNTER_NAME_PROMETHEUS,
+        COUNTER_DESCRIPTION,
+        [
+            "function",
+            "module",
+            "result",
+            "caller",
+            OBJECTIVE_NAME_PROMETHEUS,
+            OBJECTIVE_PERCENTILE_PROMETHEUS,
+        ],
+    )
+    prom_histogram = Histogram(
+        HISTOGRAM_NAME_PROMETHEUS,
+        HISTOGRAM_DESCRIPTION,
+        [
+            "function",
+            "module",
+            OBJECTIVE_NAME_PROMETHEUS,
+            OBJECTIVE_PERCENTILE_PROMETHEUS,
+            OBJECTIVE_LATENCY_THRESHOLD_PROMETHEUS,
+        ],
+    )
+    prom_gauge_build_info = Gauge(
+        BUILD_INFO_NAME, BUILD_INFO_DESCRIPTION, [COMMIT_KEY, VERSION_KEY, BRANCH_KEY]
+    )
+    prom_gauge_concurrency = Gauge(
+        CONCURRENCY_NAME_PROMETHEUS, CONCURRENCY_DESCRIPTION, ["function", "module"]
+    )
+
+    def __init__(self) -> None:
         self._has_set_build_info = False
 
-    def __count(
+    def _count(
         self,
-        function: str,
-        module: str,
+        func_name: str,
+        module_name: str,
         caller: str,
-        objective: Optional[Objective],
-        result: Result,
+        objective: Optional[Objective] = None,
+        exemplar: Optional[dict] = None,
+        result: Result = Result.OK,
     ):
+        """Increment the counter for the function call."""
         objective_name = "" if objective is None else objective.name
         percentile = (
             ""
             if objective is None or objective.success_rate is None
             else objective.success_rate.value
         )
-        self.__counter_instance.add(
-            1,
-            attributes={
-                "function": function,
-                "module": module,
-                "result": result.value,
-                "caller": caller,
-                OBJECTIVE_NAME: objective_name,
-                OBJECTIVE_PERCENTILE: percentile,
-            },
-        )
 
-    def __histogram(
+        self.prom_counter.labels(
+            func_name,
+            module_name,
+            result.value,
+            caller,
+            objective_name,
+            percentile,
+        ).inc(1, exemplar)
+
+    def _histogram(
         self,
-        function: str,
-        module: str,
+        func_name: str,
+        module_name: str,
         start_time: float,
-        objective: Optional[Objective],
+        objective: Optional[Objective] = None,
+        exemplar: Optional[dict] = None,
     ):
+        """Observe the duration of the function call."""
         duration = time.time() - start_time
 
         objective_name = "" if objective is None else objective.name
         latency = None if objective is None else objective.latency
         percentile = ""
         threshold = ""
-
         if latency is not None:
             threshold = latency[0].value
             percentile = latency[1].value
 
-        self.__histogram_instance.record(
-            duration * 1000,
-            attributes={
-                "function": function,
-                "module": module,
-                OBJECTIVE_NAME: objective_name,
-                OBJECTIVE_PERCENTILE: percentile,
-                OBJECTIVE_LATENCY_THRESHOLD: threshold,
-            },
-        )
+        self.prom_histogram.labels(
+            func_name,
+            module_name,
+            objective_name,
+            percentile,
+            threshold,
+        ).observe(duration, exemplar)
 
-    def set_build_info(self, commit: str, version: str):
+    def set_build_info(self, commit: str, version: str, branch: str):
         if not self._has_set_build_info:
             self._has_set_build_info = True
-            self.__up_down_counter_instance.add(
-                1.0,
-                attributes={
-                    "commit": commit,
-                    "version": version,
-                },
-            )
+            self.prom_gauge_build_info.labels(commit, version, branch).set(1)
+
+    def start(
+        self, function: str, module: str, track_concurrency: Optional[bool] = False
+    ):
+        """Start tracking metrics for a function call."""
+        if track_concurrency:
+            self.prom_gauge_concurrency.labels(function, module).inc()
 
     def finish(
         self,
         start_time: float,
         function: str,
         module: str,
         caller: str,
         result: Result = Result.OK,
         objective: Optional[Objective] = None,
+        track_concurrency: Optional[bool] = False,
     ):
         """Finish tracking metrics for a function call."""
-        self.__count(function, module, caller, objective, result)
-        self.__histogram(function, module, start_time, objective)
+        exemplar = None
+        if os.getenv("AUTOMETRICS_EXEMPLARS") == "true":
+            exemplar = get_exemplar()
+
+        self._count(function, module, caller, objective, exemplar, result)
+        self._histogram(function, module, start_time, objective, exemplar)
+
+        if track_concurrency:
+            self.prom_gauge_concurrency.labels(function, module).dec()
```

### Comparing `autometrics-0.5/src/autometrics/tracker/test_tracker.py` & `autometrics-0.6/src/autometrics/tracker/test_tracker.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,52 +28,62 @@
 
 
 def test_init_prometheus_tracker_set_build_info(monkeypatch):
     """Test that init_tracker (for a Prometheus tracker) calls set_build_info using env vars."""
 
     commit = "d6abce3"
     version = "1.0.1"
+    branch = "main"
 
     monkeypatch.setenv("AUTOMETRICS_COMMIT", commit)
     monkeypatch.setenv("AUTOMETRICS_VERSION", version)
+    monkeypatch.setenv("AUTOMETRICS_BRANCH", branch)
 
     prom_tracker = init_tracker(TrackerType.PROMETHEUS)
     assert isinstance(prom_tracker, PrometheusTracker)
 
     blob = generate_latest()
     assert blob is not None
     data = blob.decode("utf-8")
 
-    prom_build_info = f"""build_info{{commit="{commit}",version="{version}"}} 1.0"""
+    prom_build_info = (
+        f"""build_info{{branch="{branch}",commit="{commit}",version="{version}"}} 1.0"""
+    )
     assert prom_build_info in data
 
     monkeypatch.delenv("AUTOMETRICS_VERSION", raising=False)
     monkeypatch.delenv("AUTOMETRICS_COMMIT", raising=False)
+    monkeypatch.delenv("AUTOMETRICS_BRANCH", raising=False)
 
 
 def test_init_otel_tracker_set_build_info(monkeypatch):
     """
     Test that init_tracker (for an OTEL tracker) calls set_build_info using env vars.
     Note that the OTEL collector translates metrics to Prometheus.
     """
     pytest.skip(
         "Skipping test because OTEL collector does not create a gauge when it translates UpDownCounter to Prometheus"
     )
 
     commit = "a29a178"
     version = "0.0.1"
+    branch = "main"
 
     monkeypatch.setenv("AUTOMETRICS_COMMIT", commit)
     monkeypatch.setenv("AUTOMETRICS_VERSION", version)
+    monkeypatch.setenv("AUTOMETRICS_BRANCH", branch)
 
     otel_tracker = init_tracker(TrackerType.OPENTELEMETRY)
     assert isinstance(otel_tracker, OpenTelemetryTracker)
 
     blob = generate_latest()
     assert blob is not None
     data = blob.decode("utf-8")
 
-    prom_build_info = f"""build_info{{commit="{commit}",version="{version}"}} 1.0"""
+    prom_build_info = (
+        f"""build_info{{branch="{branch}",commit="{commit}",version="{version}"}} 1.0"""
+    )
     assert prom_build_info in data
 
     monkeypatch.delenv("AUTOMETRICS_VERSION", raising=False)
     monkeypatch.delenv("AUTOMETRICS_COMMIT", raising=False)
+    monkeypatch.delenv("AUTOMETRICS_BRANCH", raising=False)
```

### Comparing `autometrics-0.5/src/autometrics/tracker/tracker.py` & `autometrics-0.6/src/autometrics/tracker/tracker.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,25 +12,31 @@
     OK = "ok"
     ERROR = "error"
 
 
 class TrackMetrics(Protocol):
     """Protocol for tracking metrics."""
 
-    def set_build_info(self, commit: str, version: str):
+    def set_build_info(self, commit: str, version: str, branch: str):
         """Observe the build info. Should only be called once per tracker instance"""
 
+    def start(
+        self, function: str, module: str, track_concurrency: Optional[bool] = False
+    ):
+        """Start tracking metrics for a function call."""
+
     def finish(
         self,
         start_time: float,
         function: str,
         module: str,
         caller: str,
         result: Result = Result.OK,
         objective: Optional[Objective] = None,
+        track_concurrency: Optional[bool] = False,
     ):
         """Finish tracking metrics for a function call."""
 
 
 class TrackerType(Enum):
     """Type of tracker."""
 
@@ -51,16 +57,17 @@
         # pylint: disable=import-outside-toplevel
         from .prometheus import PrometheusTracker
 
         tracker_instance = PrometheusTracker()
 
     # NOTE - Only set the build info when the tracker is initialized
     tracker_instance.set_build_info(
-        commit=os.getenv("AUTOMETRICS_COMMIT") or "",
+        commit=os.getenv("AUTOMETRICS_COMMIT") or os.getenv("COMMIT_SHA") or "",
         version=os.getenv("AUTOMETRICS_VERSION") or "",
+        branch=os.getenv("AUTOMETRICS_BRANCH") or os.getenv("BRANCH_NAME") or "",
     )
 
     return tracker_instance
 
 
 def get_tracker_type() -> TrackerType:
     """Get the tracker type."""
```

### Comparing `autometrics-0.5/src/autometrics/utils.py` & `autometrics-0.6/src/autometrics/utils.py`

 * *Files identical despite different names*

### Comparing `autometrics-0.5/PKG-INFO` & `autometrics-0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autometrics
-Version: 0.5
+Version: 0.6
 Summary: Easily add metrics to your system – and actually understand them using automatically customized Prometheus queries
 Home-page: https://github.com/autometrics-dev/autometrics-py
 License: MIT OR Apache-2.0
 Keywords: metrics,telemetry,prometheus,monitoring,observability,instrumentation
 Author: Fiberplane
 Author-email: info@fiberplane.com
 Requires-Python: >=3.8,<4.0
@@ -21,17 +21,20 @@
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/autometrics-dev/autometrics-py
 Description-Content-Type: text/markdown
 
 ![GitHub_headerImage](https://user-images.githubusercontent.com/3262610/221191767-73b8a8d9-9f8b-440e-8ab6-75cb3c82f2bc.png)
 
-# autometrics-py
+[![Discord Shield](https://discordapp.com/api/guilds/950489382626951178/widget.png?style=shield)](https://discord.gg/kHtwcH8As9)
 
-A Python library that exports a decorator that makes it easy to understand the error rate, response time, and production usage of any function in your code. Jump straight from your IDE to live Prometheus charts for each HTTP/RPC handler, database method, or other piece of application logic.
+> A Python port of the Rust
+> [autometrics-rs](https://github.com/fiberplane/autometrics-rs) library
+
+**Autometrics is a library that exports a decorator that makes it easy to understand the error rate, response time, and production usage of any function in your code.** Jump straight from your IDE to live Prometheus charts for each HTTP/RPC handler, database method, or other piece of application logic.
 
 Autometrics for Python provides:
 
 1. A decorator that can create [Prometheus](https://prometheus.io/) metrics for your functions and class methods throughout your code base.
 2. A helper function that will write corresponding Prometheus queries for you in a Markdown file.
 
 See [Why Autometrics?](https://github.com/autometrics-dev#why-autometrics) for more details on the ideas behind autometrics.
@@ -43,14 +46,15 @@
 - 💡 Writes Prometheus queries so you can understand the data generated without
   knowing PromQL
 - 🔗 Create links to live Prometheus charts directly into each function's docstring
 - [🔍 Identify commits](#identifying-commits-that-introduced-problems) that introduced errors or increased latency
 - [🚨 Define alerts](#alerts--slos) using SLO best practices directly in your source code
 - [📊 Grafana dashboards](#dashboards) work out of the box to visualize the performance of instrumented functions & SLOs
 - [⚙️ Configurable](#metrics-libraries) metric collection library (`opentelemetry`, `prometheus`, or `metrics`)
+- [📍 Attach exemplars](#exemplars) to connect metrics with traces
 - ⚡ Minimal runtime overhead
 
 ## Using autometrics-py
 
 - Set up a [Prometheus instance](https://prometheus.io/download/)
 - Configure prometheus to scrape your application ([check our instructions if you need help](https://github.com/autometrics-dev#5-configuring-prometheus))
 - Include a .env file with your prometheus endpoint `PROMETHEUS_URL=your endpoint`. If this is not defined, the default endpoint will be `http://localhost:9090/`
@@ -62,14 +66,16 @@
 
 @autometrics
 def sayHello:
    return "hello"
 
 ```
 
+- You can also track the number of concurrent calls to a function by using the `track_concurrency` argument: `@autometrics(track_concurrency=True)`. Note: currently only supported by the `prometheus` tracker.
+
 - To access the PromQL queries for your decorated functions, run `help(yourfunction)` or `print(yourfunction.__doc__)`.
 
 - To show tooltips over decorated functions in VSCode, with links to Prometheus queries, try installing [the VSCode extension](https://marketplace.visualstudio.com/items?itemName=Fiberplane.autometrics).
 
 > Note that we cannot support tooltips without a VSCode extension due to behavior of the [static analyzer](https://github.com/davidhalter/jedi/issues/1921) used in VSCode.
 
 ## Dashboards
@@ -78,27 +84,33 @@
 
 ## Alerts / SLOs
 
 Autometrics makes it easy to add Prometheus alerts using Service-Level Objectives (SLOs) to a function or group of functions.
 
 In order to receive alerts you need to add a set of rules to your Prometheus set up. You can find out more about those rules here: [Prometheus alerting rules](https://github.com/autometrics-dev/autometrics-shared#prometheus-recording--alerting-rules). Once added, most of the recording rules are dormant. They are enabled by specific metric labels that can be automatically attached by autometrics.
 
-To use autometrics SLOs and alerts, create one or multiple `Objective`s based on the function(s) success rate and/or latency, as shown below. The `Objective` can be passed as an argument to the `autometrics` macro to include the given function in that objective.
+To use autometrics SLOs and alerts, create one or multiple `Objective`s based on the function(s) success rate and/or latency, as shown below. The `Objective` can be passed as an argument to the `autometrics` decorator to include the given function in that objective.
 
 ```python
 from autometrics import autometrics
 from autometrics.objectives import Objective, ObjectiveLatency, ObjectivePercentile
 
-API_SLO = Objective(
-    "random",
+# Create an objective for a high success rate
+API_SLO_HIGH_SUCCESS = Objective(
+    "My API SLO for High Success Rate (99.9%)",
     success_rate=ObjectivePercentile.P99_9,
+)
+
+# Or you can also create an objective for low latency
+API_SLO_LOW_LATENCY = Objective(
+    "My API SLO for Low Latency (99th percentile < 250ms)",
     latency=(ObjectiveLatency.Ms250, ObjectivePercentile.P99),
 )
 
-@autometrics(objective=API_SLO)
+@autometrics(objective=API_SLO_HIGH_SUCCESS)
 def api_handler():
   # ...
 ```
 
 Autometrics by default will try to store information on which function calls a decorated function. As such you may want to place the autometrics in the top/first decorator, as otherwise you may get `inner` or `wrapper` as the caller function.
 
 So instead of writing:
@@ -131,34 +143,49 @@
 @noop
 def api_handler():
   # ...
 ```
 
 #### Metrics Libraries
 
-Configure the crate that autometrics will use to produce metrics by using one of the following feature flags:
+Configure the package that autometrics will use to produce metrics with the `AUTOMETRICS_TRACKER` environment variable.
 
-- `opentelemetry` - (enabled by default, can also be explicitly set using the AUTOMETRICS_TRACKER="OPEN_TELEMETERY" env var) uses
-- `prometheus` - (using the AUTOMETRICS_TRACKER env var set to "PROMETHEUS")
+- `opentelemetry` - Enabled by default, can also be explicitly set using the env var `AUTOMETRICS_TRACKER="OPEN_TELEMETERY"`. Look in `pyproject.toml` for the versions of the OpenTelemetry packages that will be used.
+- `prometheus` - Can be set using the env var `AUTOMETRICS_TRACKER="PROMETHEUS"`. Look in `pyproject.toml` for the version of the `prometheus-client` package that will be used.
 
 ## Identifying commits that introduced problems
 
 > **NOTE** - As of writing, `build_info` will not work correctly when using the default tracker (`AUTOMETRICS_TRACKER=OPEN_TELEMETRY`).
 > This will be fixed once the following PR is merged on the opentelemetry-python project: https://github.com/open-telemetry/opentelemetry-python/pull/3306
 >
 > autometrics-py will track support for build_info using the OpenTelemetry tracker via #38
 
 Autometrics makes it easy to identify if a specific version or commit introduced errors or increased latencies.
 
-It uses a separate metric (`build_info`) to track the version and, optionally, git commit of your service. It then writes queries that group metrics by the `version` and `commit` labels so you can spot correlations between those and potential issues.
+It uses a separate metric (`build_info`) to track the version and, optionally, git commit of your service. It then writes queries that group metrics by the `version`, `commit` and `branch` labels so you can spot correlations between those and potential issues.
+Configure the labels by setting the following environment variables:
 
-The `version` is read from the `AUTOMETRICS_VERSION` environment variable, and the `commit` value uses the environment variable `AUTOMETRICS_COMMIT`.
+| Label     | Run-Time Environment Variables        | Default value |
+| --------- | ------------------------------------- | ------------- |
+| `version` | `AUTOMETRICS_VERSION`                 | `""`          |
+| `commit`  | `AUTOMETRICS_COMMIT` or `COMMIT_SHA`  | `""`          |
+| `branch`  | `AUTOMETRICS_BRANCH` or `BRANCH_NAME` | `""`          |
 
 This follows the method outlined in [Exposing the software version to Prometheus](https://www.robustperception.io/exposing-the-software-version-to-prometheus/).
 
+## Exemplars
+
+> **NOTE** - As of writing, exemplars aren't supported by the default tracker (`AUTOMETRICS_TRACKER=OPEN_TELEMETRY`).
+> You can track the progress of this feature here: https://github.com/autometrics-dev/autometrics-py/issues/41
+
+Exemplars are a way to associate a metric sample to a trace by attaching `trace_id` and `span_id` to it. You can then use this information to jump from a metric to a trace in your tracing system (for example Jaeger). If you have an OpenTelemetry tracer configured, autometrics will automatically pick up the current span from it.
+
+To use exemplars, you need to first switch to a tracker that supports them by setting `AUTOMETRICS_TRACKER=prometheus` and enable
+exemplar collection by setting `AUTOMETRICS_EXEMPLARS=true`. You also need to enable exemplars in Prometheus by launching Prometheus with the `--enable-feature=exemplar-storage` flag.
+
 ## Development of the package
 
 This package uses [poetry](https://python-poetry.org) as a package manager, with all dependencies separated into three groups:
 
 - root level dependencies, required
 - `dev`, everything that is needed for development or in ci
 - `examples`, dependencies of everything in `examples/` directory
```

