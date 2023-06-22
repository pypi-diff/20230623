# Comparing `tmp/makolator-1.0.0.tar.gz` & `tmp/makolator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makolator-1.0.0.tar", max compression
+gzip compressed data, was "makolator-1.1.0.tar", max compression
```

## Comparing `makolator-1.0.0.tar` & `makolator-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-06-19 22:25:27.699704 makolator-1.0.0/LICENSE
--rw-r--r--   0        0        0     1140 2023-06-19 22:25:27.703704 makolator-1.0.0/README.md
--rw-r--r--   0        0        0     4414 2023-06-21 13:56:34.948091 makolator-1.0.0/makolator/__init__.py
--rw-r--r--   0        0        0     6106 2023-06-22 04:53:34.122764 makolator-1.0.0/makolator/_inplace.py
--rw-r--r--   0        0        0     2066 2023-06-21 13:54:07.929256 makolator-1.0.0/makolator/config.py
--rw-r--r--   0        0        0     2004 2023-06-19 22:00:06.937371 makolator-1.0.0/makolator/datamodel.py
--rw-r--r--   0        0        0      897 2023-06-20 10:17:27.576552 makolator-1.0.0/makolator/escape.py
--rw-r--r--   0        0        0      106 2023-06-19 07:58:57.579352 makolator-1.0.0/makolator/exceptions.py
--rw-r--r--   0        0        0     7205 2023-06-22 04:52:48.846012 makolator-1.0.0/makolator/makolator.py
--rw-r--r--   0        0        0     2186 2023-06-22 04:54:28.979683 makolator-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 makolator-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-19 22:25:27.699704 makolator-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1140 2023-06-19 22:25:27.703704 makolator-1.1.0/README.md
+-rw-r--r--   0        0        0     5034 2023-06-22 23:04:42.104996 makolator-1.1.0/makolator/__init__.py
+-rw-r--r--   0        0        0     8064 2023-06-22 23:03:22.279567 makolator-1.1.0/makolator/_inplace.py
+-rw-r--r--   0        0        0     2066 2023-06-21 13:54:07.929256 makolator-1.1.0/makolator/config.py
+-rw-r--r--   0        0        0     2004 2023-06-19 22:00:06.937371 makolator-1.1.0/makolator/datamodel.py
+-rw-r--r--   0        0        0      897 2023-06-20 10:17:27.576552 makolator-1.1.0/makolator/escape.py
+-rw-r--r--   0        0        0      106 2023-06-19 07:58:57.579352 makolator-1.1.0/makolator/exceptions.py
+-rw-r--r--   0        0        0     7571 2023-06-22 22:49:56.884585 makolator-1.1.0/makolator/makolator.py
+-rw-r--r--   0        0        0     2186 2023-06-22 23:05:58.302356 makolator-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 makolator-1.1.0/PKG-INFO
```

### Comparing `makolator-1.0.0/LICENSE` & `makolator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `makolator-1.0.0/README.md` & `makolator-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `makolator-1.0.0/makolator/__init__.py` & `makolator-1.1.0/makolator/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 Makolator is not makulation. It extends the https://www.makotemplates.org/ engine by the following features:
 
 * Simple API
 * Keep timestamp of generated files, if content did not change (a gift for every build system user)
 * Easy hierarchical template usage
 * Inplace File Rendering
 
-Getting Started
----------------
+This is how to use it
+---------------------
 
 Initialize
 ~~~~~~~~~~
 
 Just create your instance of :any:`Makulator`
 
 >>> from makolator import Makolator
@@ -53,27 +53,28 @@
 []
 
 ... and the replacement strategy for :any:`outputfile.Existing` files:
 
 >>> mklt.config.existing
 <Existing.KEEP_TIMESTAMP: 'keep_timestamp'>
 
-If you like want to place templates in the actual working directory - set it as search path:
+If you want to place templates in the actual working directory - set it as search path:
 
 >>> from pathlib import Path
 >>> mklt.config.template_paths = [Path('.')]
 
 If you like it verbose - try:
 
 >>> mklt.config.verbose = True
 
 Rendering
 ~~~~~~~~~
 
-Assume you have this template in a file:
+Assume you have this template in a file
+(please ignore the `...` here - they are just there for a proper python example):
 
 >>> Path('file.txt.mako').write_text('''\\
 ... <%def name="top(name)">\\
 ... generated-top: ${name}
 ... </%def>\\
 ... <%def name="bot(name, **kwargs)">\\
 ... generated-bot: ${name} ${kwargs}
@@ -112,14 +113,39 @@
 generated-bot: foo {'b': 4}
 
 and you get notified about the changed content:
 
 >>> mklt.render([Path('file.txt.mako')], dest=Path("file.txt"))
 'file.txt'... UPDATED.
 
+Differential output
+~~~~~~~~~~~~~~~~~~~
+
+If you like it even more verbose - try:
+
+>>> mklt.config.diffout = print
+
+This will send any diff of the updated files to stdout.
+
+>>> mklt.datamodel.mydata['b'] = 2
+>>> mklt.render([Path('file.txt.mako')], dest=Path("file.txt")) # doctest: +SKIP
+---
++++
+@@ -1,3 +1,3 @@
+-Datamodel(mydata={'a': 0, 'b': 1})
++Datamodel(mydata={'a': 0, 'b': 2})
+ generated-top: foo
+ generated-bot: foo {'b': 4}
+<BLANKLINE>
+'file.txt'... UPDATED.
+
+By default this is disabled:
+
+>>> mklt.config.diffout = None
+
 Inplace Rendering
 ~~~~~~~~~~~~~~~~~
 
 One key feature is the inplace rendering.
 
 Assume you have a handwritten file and you just want to update/generate a part of it.
 `GENERATE INPLACE` will become your new friend:
@@ -141,14 +167,15 @@
 This is handwritten text.
 GENERATE INPLACE BEGIN top('bar')
 generated-top: bar
 GENERATE INPLACE END top
 This is handwritten text too.
 <BLANKLINE>
 
+
 That's it.
 """
 
 # pylint: disable=unused-import
 from outputfile import Existing
 
 from .config import Config
```

### Comparing `makolator-1.0.0/makolator/config.py` & `makolator-1.1.0/makolator/config.py`

 * *Files identical despite different names*

### Comparing `makolator-1.0.0/makolator/datamodel.py` & `makolator-1.1.0/makolator/datamodel.py`

 * *Files identical despite different names*

### Comparing `makolator-1.0.0/makolator/escape.py` & `makolator-1.1.0/makolator/escape.py`

 * *Files identical despite different names*

### Comparing `makolator-1.0.0/makolator/makolator.py` & `makolator-1.1.0/makolator/makolator.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import hashlib
 import logging
 import sys
 import tempfile
 from contextlib import contextmanager
 from pathlib import Path
 from shutil import rmtree
-from typing import Generator, List, Optional
+from typing import Generator, List, Optional, Tuple
 
 from attrs import define, field
 from mako.lookup import TemplateLookup
 from mako.runtime import Context
 from mako.template import Template
 from outputfile import Existing, open_
 from uniquer import uniquelist
@@ -76,15 +76,15 @@
         >>> with mklt.open_outputfile("myfile.txt") as file:
         ...     file.write("data")
         'myfile.txt'... CREATED.
         >>> with mklt.open_outputfile("myfile.txt") as file:
         ...     file.write("data")
         'myfile.txt'... identical. untouched.
         """
-        with open_(filepath, encoding=encoding, mkdir=True, **kwargs) as file:
+        with open_(filepath, encoding=encoding, mkdir=True, diffout=self.config.diffout, **kwargs) as file:
             try:
                 yield file
             finally:
                 file.close()
                 if self.config.verbose:
                     print(f"'{filepath!s}'... {file.state.value}")
 
@@ -96,15 +96,18 @@
             template_filepaths: Templates.
 
         Keyword Args:
             dest: Output File.
             context: Key-Value Pairs pairs forwarded to the template.
         """
         LOGGER.debug("render(%r, %r)", [str(filepath) for filepath in template_filepaths], dest)
-        templates = self._create_templates(template_filepaths, self.config.template_paths)
+        tplfilepaths, lookup = self._create_template_lookup(
+            template_filepaths, self.config.template_paths, required=True
+        )
+        templates = self._create_templates(tplfilepaths, lookup)
         context = context or {}
         if dest is None:
             self._render(next(templates), sys.stdout, None, context)
         else:
             # Mako takes care about proper newline handling. Therefore we deactivate
             # the universal newline mode, by setting newline="".
             with self.open_outputfile(dest, newline="") as output:
@@ -129,71 +132,73 @@
             dest: File to update.
 
         Keyword Args:
             context: Key-Value Pairs pairs forwarded to the template.
             ignore_unknown: Ignore unknown inplace markers, instead of raising an error.
         """
         LOGGER.debug("render_inplace(%r, %r)", [str(filepath) for filepath in template_filepaths], filepath)
-        templates = tuple(self._create_templates(template_filepaths, self.config.template_paths))
+        tplfilepaths, lookup = self._create_template_lookup(template_filepaths, self.config.template_paths)
+        templates = tuple(self._create_templates(tplfilepaths, lookup))
         config = self.config
         context = context or {}
         inplace = InplaceRenderer(
             LOGGER, config.template_marker, config.inplace_marker, templates, ignore_unknown, context
         )
         with self.open_outputfile(filepath, existing=Existing.KEEP_TIMESTAMP, newline="") as outputfile:
             context = self._get_render_context(filepath, context or {})
-            inplace.render(filepath, outputfile, context)
+            inplace.render(lookup, filepath, outputfile, context)
 
-    def _create_templates(
-        self, template_filepaths: List[Path], searchpaths: List[Path]
-    ) -> Generator[Template, None, None]:
-        filepaths = list(self._find_files(template_filepaths, searchpaths))
-        lookuppaths = uniquelist([filepath.parent for filepath in filepaths] + searchpaths)
-        lookup = self._create_template_lookup(lookuppaths)
-        found = False
-        for filepath in filepaths:
-            yield lookup.get_template(filepath.name)
-            found = True
-        if template_filepaths and not found:
-            raise MakolatorError(
-                f"None of the templates {_humanify(template_filepaths)} found at {_humanify(searchpaths)}."
-            )
-
-    def _create_template_lookup(self, searchpaths: List[Path]) -> TemplateLookup:
+    def _create_templates(self, tplfilepaths: List[Path], lookup: TemplateLookup) -> Generator[Template, None, None]:
+        for tplfilepath in tplfilepaths:
+            yield lookup.get_template(tplfilepath.name)
+
+    def _create_template_lookup(
+        self, template_filepaths: List[Path], searchpaths: List[Path], required: bool = False
+    ) -> Tuple[List[Path], TemplateLookup]:
         cache_path = self.cache_path
+        tplfilepaths = list(self._find_files(template_filepaths, searchpaths, required=required))
+        lookuppaths = uniquelist([tplfilepath.parent for tplfilepath in tplfilepaths] + searchpaths)
 
         def get_module_filename(filepath: str, uri: str):
             # pylint: disable=unused-argument
             hash_ = hashlib.sha256()
             hash_.update(bytes(filepath, encoding="utf-8"))
             ident = hash_.hexdigest()
             return cache_path / f"{Path(filepath).name}_{ident}.py"
 
-        return TemplateLookup(
-            directories=[str(item) for item in searchpaths],
+        lookup = TemplateLookup(
+            directories=[str(item) for item in lookuppaths],
             cache_dir=self.cache_path,
             input_encoding="utf-8",
             output_encoding="utf-8",
             modulename_callable=get_module_filename,
         )
+        return tplfilepaths, lookup
 
     @staticmethod
-    def _find_files(filepaths: List[Path], searchpaths: List[Path]) -> Generator[Path, None, None]:
+    def _find_files(
+        filepaths: List[Path], searchpaths: List[Path], required: bool = False
+    ) -> Generator[Path, None, None]:
         """Find `filepath` in `searchpaths` and return first match."""
+        found = False
         for filepath in filepaths:
             if filepath.is_absolute():
                 # absolute
                 if filepath.exists():
                     yield filepath
+                    found = True
             else:
                 # relative
                 for searchpath in searchpaths:
                     joined = searchpath / filepath
                     if joined.exists():
                         yield joined
+                        found = True
+        if not found and required:
+            raise MakolatorError(f"None of the templates {_humanify(filepaths)} found at {_humanify(searchpaths)}.")
 
     def _get_render_context(self, output_filepath: Optional[Path], context: dict) -> dict:
         result = {
             "datamodel": self.datamodel,
             "output_filepath": output_filepath,
             "render": self.render,
             "render_inplace": self.render_inplace,
```

### Comparing `makolator-1.0.0/pyproject.toml` & `makolator-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makolator"
-version = "1.0.0"
+version = "1.1.0"
 description = "Extended Mako Templates for Python"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `makolator-1.0.0/PKG-INFO` & `makolator-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makolator
-Version: 1.0.0
+Version: 1.1.0
 Summary: Extended Mako Templates for Python
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

