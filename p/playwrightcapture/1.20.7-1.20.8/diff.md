# Comparing `tmp/playwrightcapture-1.20.7.tar.gz` & `tmp/playwrightcapture-1.20.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.20.7.tar", max compression
+gzip compressed data, was "playwrightcapture-1.20.8.tar", max compression
```

## Comparing `playwrightcapture-1.20.7.tar` & `playwrightcapture-1.20.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.7/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.7/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.7/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    36999 2023-06-20 10:33:48.545728 playwrightcapture-1.20.7/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.7/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.7/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.7/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1828 2023-06-20 10:37:46.358743 playwrightcapture-1.20.7/pyproject.toml
--rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.7/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.8/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.8/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.8/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    37285 2023-06-23 10:01:37.189758 playwrightcapture-1.20.8/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.8/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.20.8/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.8/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1828 2023-06-23 10:34:00.689887 playwrightcapture-1.20.8/pyproject.toml
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.20.8/PKG-INFO
```

### Comparing `playwrightcapture-1.20.7/LICENSE` & `playwrightcapture-1.20.8/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.7/README.md` & `playwrightcapture-1.20.8/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.7/playwrightcapture/capture.py` & `playwrightcapture-1.20.8/playwrightcapture/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 class CaptureResponse(TypedDict, total=False):
 
     last_redirected_url: str
     har: Optional[Dict[str, Any]]
     cookies: Optional[List['Cookie']]
     error: Optional[str]
+    error_name: Optional[str]
     html: Optional[str]
     png: Optional[bytes]
     downloaded_filename: Optional[str]
     downloaded_file: Optional[bytes]
     children: Optional[List[Any]]
 
 
@@ -265,16 +266,17 @@
                             new_headers[header.strip()] = h_value.strip()
         elif isinstance(headers, dict):
             # Check if they are valid
             new_headers = {name.strip(): value.strip() for name, value in headers.items() if isinstance(name, str) and isinstance(value, str) and name.strip() and value.strip()}
             if new_headers != headers:
                 self.logger.warning(f'Headers contains invalid values:\n{json.dumps(headers, indent=2)}')
         else:
-            # This shouldn't happen, but we also cannot ensure the calls leading to this are following the specs, and playwright dislikes invalid HTTP headers.
-            self.logger.warning(f'Wrong type of headers ({type(headers)}): {headers}')  # type: ignore[unreachable]
+            # This shouldn't happen, but we also cannot ensure the calls leading to this are following the specs,
+            # and playwright dislikes invalid HTTP headers so we rather drop them.
+            self.logger.info(f'Wrong type of headers ({type(headers)}): {headers}')  # type: ignore[unreachable]
             return
 
         # Validate the new headers, only a subset of characters are accepted
         # https://developers.cloudflare.com/rules/transform/request-header-modification/reference/header-format
         for name, value in new_headers.items():
             if re.match(r'^[\w-]+$', name) is None:
                 self.logger.warning(f'Invalid HTTP Header name: {name}')
@@ -557,14 +559,15 @@
 
         except PlaywrightTimeoutError as e:
             to_return['error'] = f"The capture took too long - {e.message}"
             self.should_retry = True
         except Error as e:
             self._update_exceptions(e)
             to_return['error'] = e.message
+            to_return['error_name'] = e.name
             # TODO: check e.message and figure out if it is worth retrying or not.
             # NOTE: e.name is generally (always?) "Error"
             if self._exception_is_network_error(e):
                 # Expected errors
                 self.logger.info(f'Unable to process {url}: {e.message}')
                 if e.name == 'net::ERR_CONNECTION_RESET':
                     self.should_retry = True
@@ -573,15 +576,17 @@
                             'NS_ERROR_PARSED_DATA_CACHED']:
                 # this one sounds like something we can retry...
                 self.logger.info(f'Issue with {url} (retrying): {e.message}')
                 self.should_retry = True
             elif e.name in ['Download is starting',
                             'Connection closed',
                             'Navigation interrupted by another one',
-                            'Navigation failed because page was closed!']:
+                            'Navigation failed because page was closed!',
+                            'Connection closed while reading from the driver',
+                            'Protocol error (Page.bringToFront): Not attached to an active page']:
                 # Other errors, let's give it another shot
                 self.logger.info(f'Issue with {url} (retrying): {e.message}')
                 self.should_retry = True
             else:
                 # Unexpected ones
                 self.logger.exception(f'Something went poorly with {url}: {e.message}')
         finally:
```

### Comparing `playwrightcapture-1.20.7/playwrightcapture/helpers.py` & `playwrightcapture-1.20.8/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.7/pyproject.toml` & `playwrightcapture-1.20.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.20.7"
+version = "1.20.8"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
```

### Comparing `playwrightcapture-1.20.7/PKG-INFO` & `playwrightcapture-1.20.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.20.7
+Version: 1.20.8
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

