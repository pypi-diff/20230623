# Comparing `tmp/gofigr-0.11.1.tar.gz` & `tmp/gofigr-0.11.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gofigr-0.11.1.tar", last modified: Thu May 11 18:41:37 2023, max compression
+gzip compressed data, was "gofigr-0.11.2.tar", last modified: Fri Jun 23 13:39:31 2023, max compression
```

## Comparing `gofigr-0.11.1.tar` & `gofigr-0.11.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 18:41:37.333640 gofigr-0.11.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-05-11 18:22:11.000000 gofigr-0.11.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-05-11 18:22:11.000000 gofigr-0.11.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-05-11 18:41:37.333640 gofigr-0.11.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6023 2023-05-11 18:22:11.000000 gofigr-0.11.1/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 18:41:37.333640 gofigr-0.11.1/gofigr/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12765 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4991 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/gfconfig.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18524 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/jupyter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42702 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/models.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 18:41:37.333640 gofigr-0.11.1/gofigr/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   584424 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/resources/FreeMono.ttf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3097 2023-05-11 18:22:11.000000 gofigr-0.11.1/gofigr/watermarks.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 18:41:37.333640 gofigr-0.11.1/gofigr.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-05-11 18:41:37.000000 gofigr-0.11.1/gofigr.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-05-11 18:22:11.000000 gofigr-0.11.1/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-11 18:41:37.333640 gofigr-0.11.1/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 18:41:37.333640 gofigr-0.11.1/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40823 2023-05-11 18:22:11.000000 gofigr-0.11.1/tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1967 2023-05-11 18:22:11.000000 gofigr-0.11.1/tests/test_logs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-05-11 18:22:11.000000 gofigr-0.11.1/tests/test_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1007 2023-05-11 18:22:11.000000 gofigr-0.11.1/tests/test_watermarks.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 13:39:31.187308 gofigr-0.11.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-06-23 13:18:52.000000 gofigr-0.11.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-06-23 13:18:52.000000 gofigr-0.11.2/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-06-23 13:39:31.187308 gofigr-0.11.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6023 2023-06-23 13:18:52.000000 gofigr-0.11.2/README.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 13:39:31.187308 gofigr-0.11.2/gofigr/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12765 2023-06-23 13:18:52.000000 gofigr-0.11.2/gofigr/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4991 2023-06-23 13:18:52.000000 gofigr-0.11.2/gofigr/gfconfig.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21114 2023-06-23 13:18:52.000000 gofigr-0.11.2/gofigr/jupyter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42702 2023-06-23 13:18:52.000000 gofigr-0.11.2/gofigr/models.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 13:39:31.187308 gofigr-0.11.2/gofigr/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   584424 2023-06-23 13:18:52.000000 gofigr-0.11.2/gofigr/resources/FreeMono.ttf
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-06-23 13:18:52.000000 gofigr-0.11.2/gofigr/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3170 2023-06-23 13:18:52.000000 gofigr-0.11.2/gofigr/watermarks.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 13:39:31.187308 gofigr-0.11.2/gofigr.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-06-23 13:39:31.000000 gofigr-0.11.2/gofigr.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-06-23 13:39:31.000000 gofigr-0.11.2/gofigr.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-23 13:39:31.000000 gofigr-0.11.2/gofigr.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-23 13:39:31.000000 gofigr-0.11.2/gofigr.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      255 2023-06-23 13:39:31.000000 gofigr-0.11.2/gofigr.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-06-23 13:39:31.000000 gofigr-0.11.2/gofigr.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1631 2023-06-23 13:18:52.000000 gofigr-0.11.2/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-23 13:39:31.187308 gofigr-0.11.2/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-23 13:39:31.187308 gofigr-0.11.2/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40823 2023-06-23 13:18:52.000000 gofigr-0.11.2/tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1967 2023-06-23 13:18:52.000000 gofigr-0.11.2/tests/test_logs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-06-23 13:18:52.000000 gofigr-0.11.2/tests/test_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1007 2023-06-23 13:18:52.000000 gofigr-0.11.2/tests/test_watermarks.py
```

### Comparing `gofigr-0.11.1/LICENSE` & `gofigr-0.11.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.1/PKG-INFO` & `gofigr-0.11.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gofigr
-Version: 0.11.1
+Version: 0.11.2
 Summary: GoFigr client library
 Author-email: Maciej Pacula <maciej@gofigr.io>
 License: Copyright 2022-2023 Flagstaff Solutions, LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
         the Software without restriction, including without limitation the rights to
@@ -20,28 +20,28 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://www.gofigr.io
-Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.11.1/
+Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.11.2/
 Keywords: science,visualization,version control,plotting,data,reproducibility
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.11.1)
+GoFigr - Python Client (0.11.2)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.11.1/README.rst` & `gofigr-0.11.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.11.1)
+GoFigr - Python Client (0.11.2)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.11.1/gofigr/__init__.py` & `gofigr-0.11.2/gofigr/__init__.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.1/gofigr/gfconfig.py` & `gofigr-0.11.2/gofigr/gfconfig.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.1/gofigr/jupyter.py` & `gofigr-0.11.2/gofigr/jupyter.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,28 @@
 # pylint: disable=cyclic-import, no-member, global-statement, protected-access
 
 import inspect
 import io
 import json
 import os
 import subprocess
+import sys
 from collections import namedtuple
 from functools import wraps
 from uuid import UUID
 
 import PIL
 import ipynbname
 import matplotlib.pyplot as plt
 import six
-from IPython.core.display_functions import display
+
+try:
+    from IPython.core.display_functions import display
+except ModuleNotFoundError:
+    from IPython.core.display import display
 
 from gofigr import GoFigr, CodeLanguage, API_URL
 from gofigr.watermarks import DefaultWatermark
 
 
 class _GoFigrExtension:
     """\
@@ -142,16 +147,18 @@
 
     """
     try:
         return str(UUID(val))
     except ValueError:
         return None
 
+
 ApiId = namedtuple("ApiId", ["api_id"])
 
+
 class FindByName:
     """\
     Used as argument to configure() to specify that we want to find an analysis/workspace by name instead
     of using an API ID
     """
     def __init__(self, name, description=None, create=False):
         self.name = name
@@ -202,25 +209,60 @@
 
 class NotebookNameAnnotator(Annotator):
     """"Annotates revisions with the name & path of the current notebook"""
     def annotate(self, revision):
         if revision.metadata is None:
             revision.metadata = {}
 
-        revision.metadata['notebook_name'] = ipynbname.name()
-        revision.metadata['notebook_path'] = str(ipynbname.path())
+        try:
+            if 'notebook_name' not in revision.metadata:
+                revision.metadata['notebook_name'] = ipynbname.name()
+            if 'notebook_path' not in revision.metadata:
+                revision.metadata['notebook_path'] = str(ipynbname.path())
+
+        except Exception:  # pylint: disable=broad-exception-caught
+            print("GoFigr could not automatically obtain the name of the currently running notebook. To fix this error,"
+                  " you can manually specify the notebook name & path in the call to configure(). "
+                  "Please see https://gofigr.io/docs/gofigr-python/latest/customization.html#notebook-name-path "
+                  "for details.",
+                  file=sys.stderr)
+
+            revision.metadata['notebook_name'] = "N/A"
+            revision.metadata['notebook_path'] = "N/A"
+
+        return revision
+
+
+class CellIdAnnotator(Annotator):
+    """Annotates revisions with the ID of the Jupyter cell"""
+    def annotate(self, revision):
+        if revision.metadata is None:
+            revision.metadata = {}
+
+        try:
+            cell_id = _GF_EXTENSION.cell.cell_id
+        except AttributeError:
+            cell_id = None
+
+        revision.metadata['cell_id'] = cell_id
+
         return revision
 
 
 class CellCodeAnnotator(Annotator):
     """"Annotates revisions with cell contents"""
     def annotate(self, revision):
+        if _GF_EXTENSION.cell is not None:
+            code = _GF_EXTENSION.cell.raw_cell
+        else:
+            code = "N/A"
+
         revision.data.append(_GF_EXTENSION.gf.CodeData(name="Jupyter Cell",
                                                        language=CodeLanguage.PYTHON,
-                                                       contents=_GF_EXTENSION.cell.raw_cell))
+                                                       contents=code))
         return revision
 
 
 class PipFreezeAnnotator(Annotator):
     """Annotates revisions with the output of pip freeze"""
     def annotate(self, revision):
         try:
@@ -240,15 +282,16 @@
         except subprocess.CalledProcessError as e:
             output = e.output
 
         revision.data.append(_GF_EXTENSION.gf.TextData(name="System Info", contents=output))
         return revision
 
 
-DEFAULT_ANNOTATORS = (NotebookNameAnnotator(), CellCodeAnnotator(), SystemAnnotator(), PipFreezeAnnotator())
+DEFAULT_ANNOTATORS = (NotebookNameAnnotator(), CellIdAnnotator(), CellCodeAnnotator(), SystemAnnotator(),
+                      PipFreezeAnnotator())
 
 
 def figure_to_bytes(fig, fmt):
     """\
     Converts a matplotlib figure to raw bytes
 
     :param fig: matplotlib figure
@@ -304,19 +347,19 @@
             suptitle = getattr(fig, "_suptitle", "")
             title = fig.axes[0].get_title() if len(fig.axes) > 0 else None
             if suptitle is not None and suptitle.strip() != "":
                 fig_name = suptitle
             elif title is not None and title.strip() != "":
                 fig_name = title
             else:
-                cell_id = _GF_EXTENSION.cell.cell_id
-                if cell_id is None:
-                    cell_id = "Unknown"
-
-                fig_name = f"Cell {cell_id}, Figure #{fig.number}"
+                print("Your figure doesn't have a title and will be published as 'Anonymous Figure'. "
+                      "To avoid this warning, set a figure title or manually call publish() with a target figure. "
+                      "See https://gofigr.io/docs/gofigr-python/latest/start.html#publishing-your-first-figure for "
+                      "an example.", file=sys.stderr)
+                fig_name = "Anonymous Figure"
 
             return _GF_EXTENSION.analysis.get_figure(fig_name, create=True)
         else:
             return parse_model_instance(gf.Figure,
                                         target,
                                         lambda search: _GF_EXTENSION.analysis.get_figure(name=search.name,
                                                                                          description=search.description,
@@ -333,15 +376,22 @@
         :param dataframes: dictionary of dataframes to associate & publish with the figure
         :param metadata: metadata (JSON) to attach to this revision
         :param return_revision: whether to return a FigureRevision object. This is optional, because in normal Jupyter \
         usage this will cause Jupyter to print the whole object which we don't want.
         :return: FigureRevision instance
 
         """
-        # pylint: disable=too-many-locals
+        # pylint: disable=too-many-locals, too-many-branches
+
+        if _GF_EXTENSION.cell is None:
+            print("Information about current cell is unavailable and certain features like source code capture will " +
+                  "not work. Did you call configure() and try to publish a " +
+                  "figure in the same cell? If so, we recommend keeping GoFigr configuration and figures in " +
+                  "separate cells",
+                  file=sys.stderr)
 
         if gf is None:
             gf = _GF_EXTENSION.gf
         if fig is None:
             fig = plt.gcf()
 
         target = self._resolve_target(gf, fig, target)
@@ -470,30 +520,34 @@
     elif len(matches) > 1:
         raise RuntimeError(f'Multiple (n={len(matches)}) workspaces match name "{search.name}". '
                            f'Please use an API ID instead.')
     else:
         return matches[0]
 
 
+# pylint: disable=too-many-arguments
 @from_config_or_env("GF_", os.path.join(os.environ['HOME'], '.gofigr'))
 def configure(username, password, workspace=None, analysis=None, url=API_URL,
               default_metadata=None, auto_publish=True,
-              watermark=None, annotators=DEFAULT_ANNOTATORS):
+              watermark=None, annotators=DEFAULT_ANNOTATORS,
+              notebook_name=None, notebook_path=None):
     """\
     Configures the Jupyter plugin for use.
 
     :param username: GoFigr username
     :param password: GoFigr password
     :param url: API URL
     :param workspace: one of: API ID (string), ApiId instance, or FindByName instance
     :param analysis: one of: API ID (string), ApiId instance, or FindByName instance
     :param default_metadata: dictionary of default metadata values to save for each revision
     :param auto_publish: if True, all figures will be published automatically without needing to call publish()
     :param watermark: custom watermark instance (e.g. DefaultWatermark with custom arguments)
     :param annotators: list of annotators to use. Default: DEFAULT_ANNOTATORS
+    :param notebook_name: name of the notebook (if you don't want it to be inferred automatically)
+    :param notebook_path: path to the notebook (if you don't want it to be inferred automatically)
     :return: None
 
     """
     extension = _GF_EXTENSION
 
     if isinstance(auto_publish, str):
         auto_publish = auto_publish.lower() == "true"  # in case it's coming from an environment variable
@@ -513,14 +567,23 @@
         analysis = parse_model_instance(gf.Analysis, analysis,
                                         lambda search: workspace.get_analysis(name=search.name,
                                                                               description=search.description,
                                                                               create=search.create))
 
     analysis.fetch()
 
+    if default_metadata is None:
+        default_metadata = {}
+
+    if notebook_path is not None:
+        default_metadata['notebook_path'] = notebook_path
+
+    if notebook_name is not None:
+        default_metadata['notebook_name'] = notebook_name
+
     publisher = Publisher(gf, default_metadata=default_metadata,
                           watermark=watermark, annotators=annotators)
     extension.gf = gf
     extension.analysis = analysis
     extension.workspace = workspace
     extension.publisher = publisher
```

### Comparing `gofigr-0.11.1/gofigr/models.py` & `gofigr-0.11.2/gofigr/models.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.1/gofigr/resources/FreeMono.ttf` & `gofigr-0.11.2/gofigr/resources/FreeMono.ttf`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.1/gofigr/watermarks.py` & `gofigr-0.11.2/gofigr/watermarks.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,22 +46,22 @@
 
 class DefaultWatermark:
     """\
     Draws QR codes + URL watermark on figures.
 
     """
     def __init__(self,
-                 show_qr_code=True,
+                 show_qr_code=False,
                  margin_px=10,
                  qr_background=(0x00, 0x00, 0x00, 0x00),
                  qr_foreground=(0x00, 0x00, 0x00, 0x99),
                  qr_scale=2, font=None):
         """
 
-        :param show_qr_code: whether to show the QR code. Default is True
+        :param show_qr_code: whether to show the QR code. Default is False
         :param margin_px: margin for the QR code, in pixels
         :param qr_background: RGBA tuple for QR background color
         :param qr_foreground: RGBA tuple for QR foreground color
         :param qr_scale: QR scale, as an integer
         :param font: font for the identifier
         """
         self.margin_px = margin_px
@@ -76,29 +76,29 @@
         Adds a QR watermark to an image.
 
         :param image: PIL.Image
         :param revision: instance of FigureRevision
         :return: PIL.Image containing the watermarked image
 
         """
-        identifier = f'GoFigr: {revision.api_id}'
-
-        qr_img = _qr_to_image(f'{APP_URL}/r/{revision.api_id}', scale=self.qr_scale,
-                              module_color=self.qr_foreground,
-                              background=self.qr_background)
+        identifier = f'GoFigr: {revision.api_id}' if self.show_qr_code else f'{APP_URL}/r/{revision.api_id}'
 
         left, top, right, bottom = self.font.getbbox(identifier)
         text_height = bottom - top
         text_width = right - left
 
         res_img = Image.new(mode="RGBA", size=(image.width, image.height + (bottom - top) + self.margin_px * 2))
 
         draw = ImageDraw.Draw(res_img)
         draw.text(((res_img.width - text_width) / 2, res_img.height - text_height - self.margin_px),
                   identifier, fill="black", font=self.font)
 
         res_img.paste(image, (0, 0))
 
         if self.show_qr_code:
+            qr_img = _qr_to_image(f'{APP_URL}/r/{revision.api_id}', scale=self.qr_scale,
+                                  module_color=self.qr_foreground,
+                                  background=self.qr_background)
+
             res_img.paste(qr_img, (res_img.width - qr_img.width, res_img.height - qr_img.height))
 
         return res_img
```

### Comparing `gofigr-0.11.1/gofigr.egg-info/PKG-INFO` & `gofigr-0.11.2/gofigr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gofigr
-Version: 0.11.1
+Version: 0.11.2
 Summary: GoFigr client library
 Author-email: Maciej Pacula <maciej@gofigr.io>
 License: Copyright 2022-2023 Flagstaff Solutions, LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
         the Software without restriction, including without limitation the rights to
@@ -20,28 +20,28 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://www.gofigr.io
-Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.11.1/
+Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.11.2/
 Keywords: science,visualization,version control,plotting,data,reproducibility
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.11.1)
+GoFigr - Python Client (0.11.2)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.11.1/pyproject.toml` & `gofigr-0.11.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,43 +2,44 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gofigr"
-version = "0.11.1"
+version = "0.11.2"
 description = "GoFigr client library"
 readme = "README.rst"
 authors = [{ name = "Maciej Pacula", email = "maciej@gofigr.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["science", "visualization", "version control", "plotting", "data", "reproducibility"]
 dependencies = [
     "numpy", "pandas", "pyqrcode", "pillow", "matplotlib", "dateutils",
     "python-dateutil", "ipython", "requests", "pypng", "ipynbname"
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 
 [project.optional-dependencies]
-dev = ["pip-tools", "bumpver", "build", "twine", "pylint", "flake8", "sphinx", "sphinx_rtd_theme", "sphinxcontrib-jquery"]
+dev = ["pip-tools", "bumpver", "build", "twine", "pylint", "flake8", "sphinx", "sphinx_rtd_theme", "sphinxcontrib-jquery",
+       "seaborn", "matplotlib", "tqdm", "selenium", "webdriver-manager", "openpyxl"]
 
 [project.urls]
 Homepage = "https://www.gofigr.io"
-Documentation = "https://gofigr.io/docs/gofigr-python/0.11.1/"
+Documentation = "https://gofigr.io/docs/gofigr-python/0.11.2/"
 
 [project.scripts]
 gfconfig = "gofigr.gfconfig:main"
 
 [tool.bumpver]
-current_version = "0.11.1"
+current_version = "0.11.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gofigr-0.11.1/tests/test_client.py` & `gofigr-0.11.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.1/tests/test_logs.py` & `gofigr-0.11.2/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.1/tests/test_models.py` & `gofigr-0.11.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.11.1/tests/test_watermarks.py` & `gofigr-0.11.2/tests/test_watermarks.py`

 * *Files identical despite different names*

