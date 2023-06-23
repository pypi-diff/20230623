# Comparing `tmp/highlight_io-0.5.0.tar.gz` & `tmp/highlight_io-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlight_io-0.5.0.tar", max compression
+gzip compressed data, was "highlight_io-0.5.1.tar", max compression
```

## Comparing `highlight_io-0.5.0.tar` & `highlight_io-0.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      350 2023-06-03 00:42:53.945658 highlight_io-0.5.0/README.md
--rw-r--r--   0        0        0       64 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/__init__.py
--rw-r--r--   0        0        0      155 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/__init__.py
--rw-r--r--   0        0        0      717 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/aws.py
--rw-r--r--   0        0        0      740 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/azure.py
--rw-r--r--   0        0        0     1631 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/django.py
--rw-r--r--   0        0        0      722 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/fastapi.py
--rw-r--r--   0        0        0     1519 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/flask.py
--rw-r--r--   0        0        0      747 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/gcp.py
--rw-r--r--   0        0        0     1072 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/integrations/serverless.py
--rw-r--r--   0        0        0     7937 2023-06-03 00:42:53.945658 highlight_io-0.5.0/highlight_io/sdk.py
--rw-r--r--   0        0        0     1716 2023-06-03 00:42:53.945658 highlight_io-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 highlight_io-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      350 2023-06-23 19:53:45.556355 highlight_io-0.5.1/README.md
+-rw-r--r--   0        0        0       64 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/__init__.py
+-rw-r--r--   0        0        0      717 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/aws.py
+-rw-r--r--   0        0        0      740 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/azure.py
+-rw-r--r--   0        0        0     1631 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/django.py
+-rw-r--r--   0        0        0      722 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/fastapi.py
+-rw-r--r--   0        0        0     1519 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/flask.py
+-rw-r--r--   0        0        0      747 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/gcp.py
+-rw-r--r--   0        0        0     1072 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/integrations/serverless.py
+-rw-r--r--   0        0        0     8916 2023-06-23 19:53:45.556355 highlight_io-0.5.1/highlight_io/sdk.py
+-rw-r--r--   0        0        0     1716 2023-06-23 19:53:45.560356 highlight_io-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 highlight_io-0.5.1/PKG-INFO
```

### Comparing `highlight_io-0.5.0/highlight_io/integrations/aws.py` & `highlight_io-0.5.1/highlight_io/integrations/aws.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.0/highlight_io/integrations/azure.py` & `highlight_io-0.5.1/highlight_io/integrations/azure.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.0/highlight_io/integrations/django.py` & `highlight_io-0.5.1/highlight_io/integrations/django.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.0/highlight_io/integrations/fastapi.py` & `highlight_io-0.5.1/highlight_io/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.0/highlight_io/integrations/flask.py` & `highlight_io-0.5.1/highlight_io/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.0/highlight_io/integrations/gcp.py` & `highlight_io-0.5.1/highlight_io/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.0/highlight_io/integrations/serverless.py` & `highlight_io-0.5.1/highlight_io/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.0/highlight_io/sdk.py` & `highlight_io-0.5.1/highlight_io/sdk.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from opentelemetry.exporter.otlp.proto.http._log_exporter import OTLPLogExporter
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
 from opentelemetry.sdk._logs import LoggerProvider, LogRecord
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 from opentelemetry.sdk.trace import TracerProvider, Span
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
+from opentelemetry.trace import INVALID_SPAN
 
 from highlight_io.integrations import Integration
 
 
 class LogHandler(logging.Handler):
     def __init__(self, highlight: "H", level=logging.NOTSET):
         self.highlight = highlight
@@ -31,14 +32,15 @@
             self.highlight.log_hook(trace.get_current_span(), record)
 
 
 class H(object):
     REQUEST_HEADER = "X-Highlight-Request"
     OTLP_HTTP = "https://otel.highlight.io:4318"
     _instance: "H" = None
+    _logging_instrumented = False
 
     @classmethod
     def get_instance(cls) -> "H":
         if not cls._instance:
             raise NotImplementedError(
                 "highlight_io H object is not configured, please instantiate it by calling H()"
             )
@@ -77,29 +79,27 @@
         self._trace_provider = TracerProvider()
         self._trace_provider.add_span_processor(
             BatchSpanProcessor(
                 OTLPSpanExporter(
                     f"{self._otlp_endpoint}/v1/traces", compression=Compression.Gzip
                 ),
                 schedule_delay_millis=1000,
-                max_export_batch_size=64,
                 export_timeout_millis=5000,
             )
         )
         trace.set_tracer_provider(self._trace_provider)
         self.tracer = trace.get_tracer(__name__)
 
         self._log_provider = LoggerProvider()
         self._log_provider.add_log_record_processor(
             BatchLogRecordProcessor(
                 OTLPLogExporter(
                     f"{self._otlp_endpoint}/v1/logs", compression=Compression.Gzip
                 ),
                 schedule_delay_millis=1000,
-                max_export_batch_size=64,
                 export_timeout_millis=5000,
             )
         )
         _logs.set_logger_provider(self._log_provider)
         self.log = self._log_provider.get_logger(__name__)
 
         for integration in self._integrations:
@@ -110,39 +110,44 @@
         self._log_provider.force_flush()
 
     @contextlib.contextmanager
     def trace(
         self,
         session_id: typing.Optional[str] = "",
         request_id: typing.Optional[str] = "",
-    ) -> None:
+    ) -> Span:
         """
         Catch exceptions raised by your app using this context manager.
         Exceptions will be recorded with the Highlight project and
         associated with a frontend session when headers are provided.
 
         Example:
             import highlight_io
             H = highlight_io.H('project_id', ...)
 
             def my_fn():
-                with H.guard(headers={'X-Highlight-Request': '...'}):
+                with H.trace(headers={'X-Highlight-Request': '...'}):
                     raise Exception('fake error!')
 
 
         :param session_id: the highlight session that initiated this network request.
         :param request_id: the identifier of the current network request.
-        :return: None
+        :return: Span
         """
+        # in case the otel library is in a non-recording context, do nothing
+        if not hasattr(self, "tracer") or not self.tracer:
+            yield
+            return
+
         with self.tracer.start_as_current_span("highlight-ctx") as span:
             span.set_attributes({"highlight.project_id": self._project_id})
             span.set_attributes({"highlight.session_id": session_id})
             span.set_attributes({"highlight.trace_id": request_id})
             try:
-                yield
+                yield span
             except Exception as e:
                 self.record_exception(e)
                 raise
 
     @staticmethod
     def record_exception(e: Exception) -> None:
         """
@@ -211,10 +216,32 @@
                 body=record.getMessage(),
                 resource=span.resource,
                 attributes=attributes,
             )
             self.log.emit(r)
 
     def _instrument_logging(self):
+        if H._logging_instrumented:
+            return
+
         LoggingInstrumentor().instrument(
             set_logging_format=True, log_hook=self.log_hook
         )
+        otel_factory = logging.getLogRecordFactory()
+
+        def factory(*args, **kwargs) -> LogRecord:
+            span = trace.get_current_span()
+            if span != INVALID_SPAN:
+                manager = contextlib.nullcontext(enter_result=span)
+            else:
+                manager = self.trace()
+
+            try:
+                with manager:
+                    return otel_factory(*args, **kwargs)
+            except RecursionError:
+                # in case we are hitting a recusrive log from the `self.trace()` invocation
+                # (happens when we exceed the otel log queue depth)
+                return otel_factory(*args, **kwargs)
+
+        logging.setLogRecordFactory(factory)
+        H._logging_instrumented = True
```

### Comparing `highlight_io-0.5.0/pyproject.toml` & `highlight_io-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highlight-io"
-version = "0.5.0"
+version = "0.5.1"
 description = "Session replay and error monitoring: stop guessing why bugs happen!"
 license = "Apache-2.0"
 authors = [
     "Vadim Korolik <vadim@highlight.io>",
     "Jay Khatri <jay@highlight.io>",
 ]
 readme = "README.md"
```

### Comparing `highlight_io-0.5.0/PKG-INFO` & `highlight_io-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highlight-io
-Version: 0.5.0
+Version: 0.5.1
 Summary: Session replay and error monitoring: stop guessing why bugs happen!
 Home-page: https://www.highlight.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Vadim Korolik
 Author-email: vadim@highlight.io
 Requires-Python: >=3.8,<4.0
```

