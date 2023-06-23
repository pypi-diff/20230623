# Comparing `tmp/unitreport-0.1.0.tar.gz` & `tmp/unitreport-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unitreport-0.1.0.tar", last modified: Fri Jun 23 19:08:52 2023, max compression
+gzip compressed data, was "dist/unitreport-0.1.1.tar", last modified: Fri Jun 23 19:41:31 2023, max compression
```

## Comparing `unitreport-0.1.0.tar` & `unitreport-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:08:52.000000 unitreport-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-06-23 19:08:52.000000 unitreport-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-23 19:08:48.000000 unitreport-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:08:52.000000 unitreport-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-23 19:08:48.000000 unitreport-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:08:52.000000 unitreport-0.1.0/unitreport/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-23 19:08:48.000000 unitreport-0.1.0/unitreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-23 19:08:48.000000 unitreport-0.1.0/unitreport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-23 19:08:48.000000 unitreport-0.1.0/unitreport/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-23 19:08:48.000000 unitreport-0.1.0/unitreport/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:08:52.000000 unitreport-0.1.0/unitreport/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-23 19:08:48.000000 unitreport-0.1.0/unitreport/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-23 19:08:48.000000 unitreport-0.1.0/unitreport/templates/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:08:52.000000 unitreport-0.1.0/unitreport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-06-23 19:08:51.000000 unitreport-0.1.0/unitreport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-23 19:08:52.000000 unitreport-0.1.0/unitreport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:08:51.000000 unitreport-0.1.0/unitreport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 19:08:51.000000 unitreport-0.1.0/unitreport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 19:08:51.000000 unitreport-0.1.0/unitreport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:41:31.000000 unitreport-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-06-23 19:41:31.000000 unitreport-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-23 19:41:24.000000 unitreport-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 19:41:31.000000 unitreport-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-23 19:41:24.000000 unitreport-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:41:31.000000 unitreport-0.1.1/unitreport/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-23 19:41:24.000000 unitreport-0.1.1/unitreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-23 19:41:24.000000 unitreport-0.1.1/unitreport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-23 19:41:24.000000 unitreport-0.1.1/unitreport/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-23 19:41:24.000000 unitreport-0.1.1/unitreport/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:41:31.000000 unitreport-0.1.1/unitreport/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-23 19:41:24.000000 unitreport-0.1.1/unitreport/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-23 19:41:24.000000 unitreport-0.1.1/unitreport/templates/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:41:31.000000 unitreport-0.1.1/unitreport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-06-23 19:41:31.000000 unitreport-0.1.1/unitreport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-23 19:41:31.000000 unitreport-0.1.1/unitreport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:41:31.000000 unitreport-0.1.1/unitreport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 19:41:31.000000 unitreport-0.1.1/unitreport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 19:41:31.000000 unitreport-0.1.1/unitreport.egg-info/top_level.txt
```

### Comparing `unitreport-0.1.0/PKG-INFO` & `unitreport-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitreport
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small unittest-based tool for generating single page html reports in Python.
 Home-page: https://github.com/annahadji/unitreport
 Author: annahadji
 Author-email: annahadji@users.noreply.github.com
 License: UNKNOWN
 Description: # :page_facing_up: unitreport ![](https://github.com/annahadji/unitreport/workflows/Publish%20to%20PyPI/badge.svg) ![PyPI](https://img.shields.io/pypi/v/unitreport)
```

### Comparing `unitreport-0.1.0/README.md` & `unitreport-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `unitreport-0.1.0/setup.py` & `unitreport-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="unitreport",
-    version="0.1.0",
+    version="0.1.1",
     author="annahadji",
     author_email="annahadji@users.noreply.github.com",
     description="A small unittest-based tool for generating single page html reports in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="static unittest report generator Markdown plots tables",
     url="https://github.com/annahadji/unitreport",
```

### Comparing `unitreport-0.1.0/unitreport/__main__.py` & `unitreport-0.1.1/unitreport/__main__.py`

 * *Files identical despite different names*

### Comparing `unitreport-0.1.0/unitreport/decorators.py` & `unitreport-0.1.1/unitreport/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,51 +16,58 @@
 logger = logging.getLogger(__name__)
 
 # type which matches any subclass of unittest.TestCase
 TestCaseType = TypeVar("TestCaseType", bound=unittest.TestCase)
 
 
 def plotting(
-    func: Callable[[TestCaseType], Optional[matplotlib.figure.Figure]],
     figsize: Tuple[float, float] = (8, 6),
     dpi: int = 100,
     save_to_disk: bool = False,
 ):
     """Decorator for tests that generate matplotlib figures.
 
     Args:
-        func: function passed to decorator.
         figsize: (plt) figure size. Defaults to (8, 6).
         dpi: (plt) figure dpi. Defaults to 100.
         save_to_disk: save figure separately to disk. Defaults to False.
     """
 
-    def wrapper(testcase: TestCaseType):
-        # create clean figure for test case to utilise
-        plt.figure(figsize=figsize, dpi=dpi)
-        # call test case, if fails will raise error and rest of plot saving will not run
-        fig = func(testcase) or plt
-        # save to in-memory buffer to avoid writing to file
-        buffer = io.StringIO()
-        fig.savefig(buffer, format="svg", bbox_inches="tight")
-        if save_to_disk:
-            fig.savefig(f"{func.__name__}.png", transparent=True, bbox_inches="tight")
-        # dont include empty plot in report
-        testcase.assertTrue(len(buffer.getvalue()), "Generated plot with empty output.")
-        # if above assertion fails, following code will not be run
-        FIGURES[func.__name__] = {
-            "type": "plot",
-            "content": buffer.getvalue(),
-            "description": func.__doc__ or "",
-        }
-        logger.debug(
-            "Ran %s with buffer size %i.", func.__name__, len(buffer.getvalue())
-        )
+    def plotting_decorator(
+        func: Callable[[TestCaseType], Optional[matplotlib.figure.Figure]]
+    ):
+        def wrapper(testcase: TestCaseType):
+            # create clean figure for test case to utilise
+            plt.figure(figsize=figsize, dpi=dpi)
+            # call test case, if fails will raise error and rest of plot saving will not run
+            fig = func(testcase) or plt
+            # save to in-memory buffer to avoid writing to file
+            buffer = io.StringIO()
+            fig.savefig(buffer, format="svg", bbox_inches="tight")
+            if save_to_disk:
+                fig.savefig(
+                    f"{func.__name__}.png", transparent=True, bbox_inches="tight"
+                )
+            # dont include empty plot in report
+            testcase.assertTrue(
+                len(buffer.getvalue()), "Generated plot with empty output."
+            )
+            # if above assertion fails, following code will not be run
+            FIGURES[func.__name__] = {
+                "type": "plot",
+                "content": buffer.getvalue(),
+                "description": func.__doc__ or "",
+            }
+            logger.debug(
+                "Ran %s with buffer size %i.", func.__name__, len(buffer.getvalue())
+            )
+
+        return wrapper
 
-    return wrapper
+    return plotting_decorator
 
 
 def tabling(func: Callable[[TestCaseType], str]):
     """Decorator for tests that return (html) tables
 
     Args:
         func: function passed to decorator.
```

### Comparing `unitreport-0.1.0/unitreport/generate.py` & `unitreport-0.1.1/unitreport/generate.py`

 * *Files identical despite different names*

### Comparing `unitreport-0.1.0/unitreport/templates/index.html` & `unitreport-0.1.1/unitreport/templates/index.html`

 * *Files identical despite different names*

### Comparing `unitreport-0.1.0/unitreport/templates/main.css` & `unitreport-0.1.1/unitreport/templates/main.css`

 * *Files identical despite different names*

### Comparing `unitreport-0.1.0/unitreport.egg-info/PKG-INFO` & `unitreport-0.1.1/unitreport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitreport
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small unittest-based tool for generating single page html reports in Python.
 Home-page: https://github.com/annahadji/unitreport
 Author: annahadji
 Author-email: annahadji@users.noreply.github.com
 License: UNKNOWN
 Description: # :page_facing_up: unitreport ![](https://github.com/annahadji/unitreport/workflows/Publish%20to%20PyPI/badge.svg) ![PyPI](https://img.shields.io/pypi/v/unitreport)
```

