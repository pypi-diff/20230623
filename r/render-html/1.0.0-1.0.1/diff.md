# Comparing `tmp/render_html-1.0.0.tar.gz` & `tmp/render_html-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_html-1.0.0.tar", last modified: Fri Jun 23 11:46:00 2023, max compression
+gzip compressed data, was "render_html-1.0.1.tar", last modified: Fri Jun 23 11:52:21 2023, max compression
```

## Comparing `render_html-1.0.0.tar` & `render_html-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:46:00.248766 render_html-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-23 11:45:31.000000 render_html-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-23 11:46:00.248766 render_html-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-23 11:45:31.000000 render_html-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-23 11:45:31.000000 render_html-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 11:46:00.248766 render_html-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:46:00.244766 render_html-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:46:00.244766 render_html-1.0.0/src/render_html/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 11:45:31.000000 render_html-1.0.0/src/render_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-23 11:45:31.000000 render_html-1.0.0/src/render_html/_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-23 11:45:31.000000 render_html-1.0.0/src/render_html/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:46:00.244766 render_html-1.0.0/src/render_html.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-23 11:46:00.000000 render_html-1.0.0/src/render_html.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-23 11:46:00.000000 render_html-1.0.0/src/render_html.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:46:00.000000 render_html-1.0.0/src/render_html.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 11:46:00.000000 render_html-1.0.0/src/render_html.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:46:00.248766 render_html-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-23 11:45:31.000000 render_html-1.0.0/tests/test_render_html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:52:21.637443 render_html-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-23 11:52:01.000000 render_html-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-23 11:52:21.637443 render_html-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-23 11:52:01.000000 render_html-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-23 11:52:01.000000 render_html-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 11:52:21.637443 render_html-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:52:21.633443 render_html-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:52:21.637443 render_html-1.0.1/src/render_html/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 11:52:01.000000 render_html-1.0.1/src/render_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-23 11:52:01.000000 render_html-1.0.1/src/render_html/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-23 11:52:01.000000 render_html-1.0.1/src/render_html/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:52:21.637443 render_html-1.0.1/src/render_html.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-23 11:52:21.000000 render_html-1.0.1/src/render_html.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-23 11:52:21.000000 render_html-1.0.1/src/render_html.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:52:21.000000 render_html-1.0.1/src/render_html.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 11:52:21.000000 render_html-1.0.1/src/render_html.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:52:21.637443 render_html-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-23 11:52:01.000000 render_html-1.0.1/tests/test_render_html.py
```

### Comparing `render_html-1.0.0/LICENSE` & `render_html-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `render_html-1.0.0/PKG-INFO` & `render_html-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_html
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library that provides a simple way to render HTML content in a web browser.
 Author-email: Bartlomiej Mika <bmika1@icloud.com>
 Project-URL: Homepage, https://github.com/bmika1/render-html
 Project-URL: Bug Tracker, https://github.com/bmika1/render-html/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `render_html-1.0.0/README.md` & `render_html-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `render_html-1.0.0/pyproject.toml` & `render_html-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "render_html"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Bartlomiej Mika", email="bmika1@icloud.com" },
 ]
 description = "Python library that provides a simple way to render HTML content in a web browser."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `render_html-1.0.0/src/render_html/_renderer.py` & `render_html-1.0.1/src/render_html/_renderer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 
     with tempfile.NamedTemporaryFile(
         mode="w", delete=autodelete, suffix=".html"
     ) as tmp_file:
         tmp_file.write(html_string)
         file_path = tmp_file.name
         if autodelete:
+            _open_in_browser(file_path, browser)
             # Adding a short sleep so that the file does not get cleaned
             # up immediately in case the browser takes a while to boot.
             time.sleep(3)
-            _open_in_browser(file_path, browser)
     if not autodelete:
         _open_in_browser(file_path, browser)
         time.sleep(3)
         os.unlink(file_path)  # Cleaning up the file in case of Windows
 
 
 def _handle_open_from_regular_file(
```

### Comparing `render_html-1.0.0/src/render_html.egg-info/PKG-INFO` & `render_html-1.0.1/src/render_html.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-html
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library that provides a simple way to render HTML content in a web browser.
 Author-email: Bartlomiej Mika <bmika1@icloud.com>
 Project-URL: Homepage, https://github.com/bmika1/render-html
 Project-URL: Bug Tracker, https://github.com/bmika1/render-html/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `render_html-1.0.0/tests/test_render_html.py` & `render_html-1.0.1/tests/test_render_html.py`

 * *Files identical despite different names*

