# Comparing `tmp/makolator-1.1.0.tar.gz` & `tmp/makolator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makolator-1.1.0.tar", max compression
+gzip compressed data, was "makolator-1.1.1.tar", max compression
```

## Comparing `makolator-1.1.0.tar` & `makolator-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-06-19 22:25:27.699704 makolator-1.1.0/LICENSE
--rw-r--r--   0        0        0     1140 2023-06-19 22:25:27.703704 makolator-1.1.0/README.md
--rw-r--r--   0        0        0     5034 2023-06-22 23:04:42.104996 makolator-1.1.0/makolator/__init__.py
--rw-r--r--   0        0        0     8064 2023-06-22 23:03:22.279567 makolator-1.1.0/makolator/_inplace.py
--rw-r--r--   0        0        0     2066 2023-06-21 13:54:07.929256 makolator-1.1.0/makolator/config.py
--rw-r--r--   0        0        0     2004 2023-06-19 22:00:06.937371 makolator-1.1.0/makolator/datamodel.py
--rw-r--r--   0        0        0      897 2023-06-20 10:17:27.576552 makolator-1.1.0/makolator/escape.py
--rw-r--r--   0        0        0      106 2023-06-19 07:58:57.579352 makolator-1.1.0/makolator/exceptions.py
--rw-r--r--   0        0        0     7571 2023-06-22 22:49:56.884585 makolator-1.1.0/makolator/makolator.py
--rw-r--r--   0        0        0     2186 2023-06-22 23:05:58.302356 makolator-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 makolator-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-19 22:25:27.699704 makolator-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1140 2023-06-19 22:25:27.703704 makolator-1.1.1/README.md
+-rw-r--r--   0        0        0     5034 2023-06-22 23:04:42.104996 makolator-1.1.1/makolator/__init__.py
+-rw-r--r--   0        0        0     8158 2023-06-23 07:21:22.575192 makolator-1.1.1/makolator/_inplace.py
+-rw-r--r--   0        0        0     2066 2023-06-21 13:54:07.929256 makolator-1.1.1/makolator/config.py
+-rw-r--r--   0        0        0     2004 2023-06-19 22:00:06.937371 makolator-1.1.1/makolator/datamodel.py
+-rw-r--r--   0        0        0      897 2023-06-20 10:17:27.576552 makolator-1.1.1/makolator/escape.py
+-rw-r--r--   0        0        0      106 2023-06-19 07:58:57.579352 makolator-1.1.1/makolator/exceptions.py
+-rw-r--r--   0        0        0     7571 2023-06-22 22:49:56.884585 makolator-1.1.1/makolator/makolator.py
+-rw-r--r--   0        0        0     2186 2023-06-23 07:23:04.852972 makolator-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 makolator-1.1.1/PKG-INFO
```

### Comparing `makolator-1.1.0/LICENSE` & `makolator-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `makolator-1.1.0/README.md` & `makolator-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `makolator-1.1.0/makolator/__init__.py` & `makolator-1.1.1/makolator/__init__.py`

 * *Files identical despite different names*

### Comparing `makolator-1.1.0/makolator/_inplace.py` & `makolator-1.1.1/makolator/_inplace.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,57 +72,38 @@
     inplace_marker: str
     templates: Tuple[Template, ...]
     ignore_unknown: bool
     context: dict
 
     def render(self, lookup: TemplateLookup, filepath: Path, outputfile, context: dict):
         """Render."""
-        # We know this is bad code - it is kept as best, but optimized for speed
-        # pylint: disable=too-many-locals,too-many-branches,too-many-nested-blocks
+        # pylint: disable=too-many-locals,too-many-nested-blocks
         inplace_marker = self.inplace_marker
         ibegin = re.compile(rf"(?P<indent>\s*).*{inplace_marker}\s+BEGIN\s(?P<funcname>[a-z_]+)\((?P<args>.*)\).*")
         iinfo = None
 
         template_marker = self.template_marker
         tplinfo = None
         tbegin = re.compile(rf"(?P<pre>.*)\s*{template_marker}\s+BEGIN.*")
-        tend = re.compile(rf"(?P<pre>.*)\s*{template_marker}\s+END.*")
         templates = list(self.templates)
 
         with open(filepath, encoding="utf-8") as inputfile:
             inputiter = enumerate(inputfile.readlines(), 1)
             try:
                 while True:
                     if iinfo:
-                        # search for "INPLACE END <funcname>"
-                        while True:
-                            lineno, line = next(inputiter)
-                            endmatch = iinfo.end.match(line)
-                            if endmatch:
-                                # fill
-                                self._fill_inplace(filepath, outputfile, iinfo, context)
-                                # propagate INPLACE END tag
-                                outputfile.write(line)
-                                self._check_indent(filepath, lineno, iinfo, endmatch.group("indent"))
-                                # consume INPLACE END
-                                iinfo = None
-                                break
+                        # GENERATE INPLACE
+                        self._process_inplace(filepath, outputfile, context, inputiter, iinfo)
+                        iinfo = None
+
                     elif tplinfo:
-                        # capture TEMPLATE
-                        while True:
-                            lineno, line = next(inputiter)
-                            # propagate
-                            outputfile.write(line)
-                            # search for "INPLACE END"
-                            endmatch = tend.match(line)
-                            if endmatch:
-                                templates.append(Template("".join(tplinfo.lines), lookup=lookup))
-                                tplinfo = None
-                                break
-                            tplinfo.lines.append(line.removeprefix(tplinfo.pre))
+                        # MAKO TEMPLATE
+                        self._process_template(lookup, outputfile, templates, inputiter, tplinfo)
+                        tplinfo = None
+
                     else:
                         # normal lines
                         while True:
                             lineno, line = next(inputiter)
                             outputfile.write(line)
                             if inplace_marker:
                                 # search for "INPLACE BEGIN <funcname>(<args>)"
@@ -142,14 +123,46 @@
             except StopIteration:
                 pass
         if iinfo:
             raise MakolatorError(f"{filepath!s}:{iinfo.lineno} BEGIN {iinfo.funcname}({iinfo.args})' without END.")
         if tplinfo:
             raise MakolatorError(f"{filepath!s}:{tplinfo.lineno} BEGIN without END.")
 
+    def _process_inplace(self, filepath: Path, outputfile, context: dict, inputiter, iinfo):
+        while True:
+            # search for "INPLACE END <funcname>"
+            lineno, line = next(inputiter)
+            endmatch = iinfo.end.match(line)
+            if endmatch:
+                # fill
+                self._fill_inplace(filepath, outputfile, iinfo, context)
+                # propagate INPLACE END tag
+                outputfile.write(line)
+                self._check_indent(filepath, lineno, iinfo, endmatch.group("indent"))
+                # consume INPLACE END
+                break
+
+    def _process_template(self, lookup: TemplateLookup, outputfile, templates, inputiter, tplinfo):
+        # capture TEMPLATE
+        pre = tplinfo.pre
+        prelen = len(pre)
+        tend = re.compile(rf"(?P<pre>.*)\s*{self.template_marker}\s+END.*")
+        while True:
+            _, line = next(inputiter)
+            # propagate
+            outputfile.write(line)
+            # search for "INPLACE END"
+            endmatch = tend.match(line)
+            if endmatch:
+                templates.append(Template("".join(tplinfo.lines), lookup=lookup))
+                break
+            if line.startswith(pre):
+                line = line[prelen:]
+            tplinfo.lines.append(line)
+
     def _start_inplace(
         self, templates: List[Template], filepath: Path, lineno: int, indent: str, funcname: str, args: str
     ) -> Optional[InplaceInfo]:
         for template in templates:
             try:
                 func = template.get_def(funcname)
             except AttributeError:
```

### Comparing `makolator-1.1.0/makolator/config.py` & `makolator-1.1.1/makolator/config.py`

 * *Files identical despite different names*

### Comparing `makolator-1.1.0/makolator/datamodel.py` & `makolator-1.1.1/makolator/datamodel.py`

 * *Files identical despite different names*

### Comparing `makolator-1.1.0/makolator/escape.py` & `makolator-1.1.1/makolator/escape.py`

 * *Files identical despite different names*

### Comparing `makolator-1.1.0/makolator/makolator.py` & `makolator-1.1.1/makolator/makolator.py`

 * *Files identical despite different names*

### Comparing `makolator-1.1.0/pyproject.toml` & `makolator-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makolator"
-version = "1.1.0"
+version = "1.1.1"
 description = "Extended Mako Templates for Python"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `makolator-1.1.0/PKG-INFO` & `makolator-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makolator
-Version: 1.1.0
+Version: 1.1.1
 Summary: Extended Mako Templates for Python
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

