# Comparing `tmp/docformatter-1.7.2.tar.gz` & `tmp/docformatter-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docformatter-1.7.2.tar", max compression
+gzip compressed data, was "docformatter-1.7.3.tar", max compression
```

## Comparing `docformatter-1.7.2.tar` & `docformatter-1.7.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.7.2/LICENSE
--rw-r--r--   0        0        0     6864 2023-06-06 14:28:12.772135 docformatter-1.7.2/README.rst
--rw-r--r--   0        0        0     6222 2023-06-07 03:06:35.281648 docformatter-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     1614 2023-06-06 14:28:12.798136 docformatter-1.7.2/src/docformatter/__init__.py
--rwxr-xr-x   0        0        0     6501 2023-06-07 03:06:35.281648 docformatter-1.7.2/src/docformatter/__main__.py
--rw-r--r--   0        0        0     1191 2023-06-07 03:06:35.282648 docformatter-1.7.2/src/docformatter/__pkginfo__.py
--rw-r--r--   0        0        0    13592 2023-06-07 03:06:35.282648 docformatter-1.7.2/src/docformatter/configuration.py
--rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.7.2/src/docformatter/encode.py
--rw-r--r--   0        0        0    21022 2023-06-07 03:06:35.282648 docformatter-1.7.2/src/docformatter/format.py
--rw-r--r--   0        0        0     6998 2023-06-06 14:28:12.821136 docformatter-1.7.2/src/docformatter/strings.py
--rw-r--r--   0        0        0    26471 2023-06-07 03:06:35.282648 docformatter-1.7.2/src/docformatter/syntax.py
--rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.7.2/src/docformatter/util.py
--rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 docformatter-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.7.3/LICENSE
+-rw-r--r--   0        0        0     6864 2023-06-06 14:28:12.772135 docformatter-1.7.3/README.rst
+-rw-r--r--   0        0        0     6343 2023-06-23 01:50:08.112575 docformatter-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1614 2023-06-06 14:28:12.798136 docformatter-1.7.3/src/docformatter/__init__.py
+-rwxr-xr-x   0        0        0     6417 2023-06-23 01:50:08.112575 docformatter-1.7.3/src/docformatter/__main__.py
+-rw-r--r--   0        0        0     1191 2023-06-23 01:50:08.113575 docformatter-1.7.3/src/docformatter/__pkginfo__.py
+-rw-r--r--   0        0        0    13592 2023-06-07 03:06:35.282648 docformatter-1.7.3/src/docformatter/configuration.py
+-rw-r--r--   0        0        0     3717 2023-06-23 01:50:08.113575 docformatter-1.7.3/src/docformatter/encode.py
+-rw-r--r--   0        0        0    21057 2023-06-23 01:50:08.113575 docformatter-1.7.3/src/docformatter/format.py
+-rw-r--r--   0        0        0     6998 2023-06-06 14:28:12.821136 docformatter-1.7.3/src/docformatter/strings.py
+-rw-r--r--   0        0        0    28407 2023-06-23 01:50:08.114575 docformatter-1.7.3/src/docformatter/syntax.py
+-rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.7.3/src/docformatter/util.py
+-rw-r--r--   0        0        0     8257 1970-01-01 00:00:00.000000 docformatter-1.7.3/PKG-INFO
```

### Comparing `docformatter-1.7.2/LICENSE` & `docformatter-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.2/README.rst` & `docformatter-1.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.2/pyproject.toml` & `docformatter-1.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docformatter"
-version = "1.7.2"
+version = "1.7.3"
 description = "Formats docstrings to follow PEP 257"
 authors = ["Steven Myint"]
 maintainers = [
     "Doyle Rowland <doyle.rowland@reliaqual.com>",
 ]
 license = "Expat"
 readme = "README.rst"
@@ -95,14 +95,20 @@
 [tool.docformatter]
 black = true
 non-strict = false
 non-cap = [
 	"docformatter",
 ]
 
+[tool.mypy]
+allow_subclassing_any = true
+follow_imports = "skip"
+implicit_reexport = true
+ignore_missing_imports = true
+
 [tool.pydocstyle]
 convention = "pep257"
 
 [tool.pytest.ini_options]
 markers = [
     "unit: mark the test as a unit test.",
     "system: mark the test as a system test.",
```

### Comparing `docformatter-1.7.2/src/docformatter/__init__.py` & `docformatter-1.7.3/src/docformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.2/src/docformatter/__main__.py` & `docformatter-1.7.3/src/docformatter/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Formats docstrings to follow PEP 257."""
 
 
-from __future__ import absolute_import, division, print_function, unicode_literals
-
 # Standard Library Imports
 import contextlib
 import signal
 import sys
 
 # docformatter Package Imports
 import docformatter.configuration as _configuration
```

### Comparing `docformatter-1.7.2/src/docformatter/__pkginfo__.py` & `docformatter-1.7.3/src/docformatter/__pkginfo__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Package information for docformatter."""
 
-__version__ = "1.7.2"
+__version__ = "1.7.3"
```

### Comparing `docformatter-1.7.2/src/docformatter/configuration.py` & `docformatter-1.7.3/src/docformatter/configuration.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.2/src/docformatter/encode.py` & `docformatter-1.7.3/src/docformatter/encode.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """This module provides docformatter's Encoder class."""
 
 # Standard Library Imports
 import collections
-import io
 import locale
 import sys
 from typing import Dict, List
 
 # Third Party Imports
 from charset_normalizer import from_path  # pylint: disable=import-error
 
@@ -42,19 +41,17 @@
     CR = "\r"
     LF = "\n"
     CRLF = "\r\n"
 
     def __init__(self):
         """Initialize an Encoder instance."""
         self.encoding = "latin-1"
-        self.system_encoding = (
-            locale.getpreferredencoding() or sys.getdefaultencoding()
-        )
+        self.system_encoding = locale.getpreferredencoding() or sys.getdefaultencoding()
 
-    def do_detect_encoding(self, filename: str) -> None:
+    def do_detect_encoding(self, filename) -> None:
         """Return the detected file encoding.
 
         Parameters
         ----------
         filename : str
             The full path name of the file whose encoding is to be detected.
         """
@@ -63,51 +60,58 @@
 
             # Check for correctness of encoding.
             with self.do_open_with_encoding(filename) as check_file:
                 check_file.read()
         except (SyntaxError, LookupError, UnicodeDecodeError):
             self.encoding = "latin-1"
 
-    def do_find_newline(self, source: List[str]) -> Dict[int, int]:
+    def do_find_newline(self, source: List[str]) -> str:
         """Return type of newline used in source.
 
         Parameters
         ----------
         source : list
             A list of lines.
 
         Returns
         -------
-        counter : dict
-            A dict with the count of new line types found.
+        newline : str
+            The most prevalent new line type found.
         """
         assert not isinstance(source, unicode)
 
-        counter = collections.defaultdict(int)
+        counter: Dict[str, int] = collections.defaultdict(int)
         for line in source:
             if line.endswith(self.CRLF):
                 counter[self.CRLF] += 1
             elif line.endswith(self.CR):
                 counter[self.CR] += 1
             elif line.endswith(self.LF):
                 counter[self.LF] += 1
 
-        return (sorted(counter, key=counter.get, reverse=True) or [self.LF])[0]
+        return (
+            sorted(
+                counter,
+                key=counter.get,  # type: ignore
+                reverse=True,
+            )
+            or [self.LF]
+        )[0]
 
-    def do_open_with_encoding(self, filename: str, mode: str = "r"):
+    def do_open_with_encoding(self, filename, mode: str = "r"):
         """Return opened file with a specific encoding.
 
         Parameters
         ----------
         filename : str
             The full path name of the file to open.
         mode : str
             The mode to open the file in.  Defaults to read-only.
 
         Returns
         -------
         contents : TextIO
             The contents of the file.
         """
-        return io.open(
+        return open(
             filename, mode=mode, encoding=self.encoding, newline=""
         )  # Preserve line endings
```

### Comparing `docformatter-1.7.2/src/docformatter/format.py` & `docformatter-1.7.3/src/docformatter/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         outcomes = collections.Counter()
         for filename in _util.find_py_files(
             set(self.args.files), self.args.recursive, self.args.exclude
         ):
             try:
                 result = self._do_format_file(filename)
                 outcomes[result] += 1
-            except IOError as exception:
+            except OSError as exception:
                 outcomes[FormatResult.error] += 1
                 print(unicode(exception), file=self.stderror)
 
         return_codes = [  # in order of preference
             FormatResult.error,
             FormatResult.check_failed,
             FormatResult.ok,
@@ -456,15 +456,18 @@
         with contextlib.suppress(IndexError):
             if _links[0][0] == 0 and _links[0][1] == len(contents):
                 return docstring
 
         summary, description = _strings.split_summary_and_description(contents)
 
         # Leave docstrings with only field lists alone.
-        if _syntax.is_some_sort_of_field_list(summary, self.args.style):
+        if _syntax.is_some_sort_of_field_list(
+            summary,
+            self.args.style,
+        ):
             return docstring
 
         # Leave docstrings with underlined descriptions alone.
         # TODO: Deprecate the remove_section_header method now that section headers
         #  are being handled.
         if _syntax.remove_section_header(description).strip() != description.strip():
             return docstring
```

### Comparing `docformatter-1.7.2/src/docformatter/strings.py` & `docformatter-1.7.3/src/docformatter/strings.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.2/src/docformatter/syntax.py` & `docformatter-1.7.3/src/docformatter/syntax.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,28 @@
 # EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-"""This module provides docformatter's Syntaxor class."""
+"""This module provides docformatter's syntax functions."""
 
 
 # Standard Library Imports
 import contextlib
 import re
 import textwrap
 from typing import Iterable, List, Tuple, Union
 
 DEFAULT_INDENT = 4
 
+ALEMBIC_REGEX = r"^ *[a-zA-Z0-9_\- ]*: "
+"""Regular expression to use for finding alembic headers."""
+
 BULLET_REGEX = r"\s*[*\-+] [\S ]+"
 """Regular expression to use for finding bullet lists."""
 
 ENUM_REGEX = r"\s*\d\."
 """Regular expression to use for finding enumerated lists."""
 
 EPYTEXT_REGEX = r"@[a-zA-Z0-9_\-\s]+:"
@@ -158,64 +161,69 @@
 (``|') matches a double back-tick or single quote.
 """
 
 HEURISTIC_MIN_LIST_ASPECT_RATIO = 0.4
 
 
 def description_to_list(
-    text: str,
+    description: str,
     indentation: str,
     wrap_length: int,
 ) -> List[str]:
     """Convert the description to a list of wrap length lines.
 
     Parameters
     ----------
-    text : str
+    description : str
         The docstring description.
     indentation : str
         The indentation (number of spaces or tabs) to place in front of each
         line.
     wrap_length : int
         The column to wrap each line at.
 
     Returns
     -------
-    _lines : list
-          A list containing each line of the description with any links put
-          back together.
+    _wrapped_lines : list
+          A list containing each line of the description wrapped at wrap_length.
     """
     # This is a description containing only one paragraph.
-    if len(re.findall(r"\n\n", text)) <= 0:
+    if len(re.findall(r"\n\n", description)) <= 0:
         return textwrap.wrap(
-            textwrap.dedent(text),
+            textwrap.dedent(description),
             width=wrap_length,
             initial_indent=indentation,
             subsequent_indent=indentation,
         )
 
     # This is a description containing multiple paragraphs.
-    _lines = []
-    for _line in text.split("\n\n"):
-        _text = textwrap.wrap(
+    _wrapped_lines = []
+    for _line in description.split("\n\n"):
+        _wrapped_line = textwrap.wrap(
             textwrap.dedent(_line),
             width=wrap_length,
             initial_indent=indentation,
             subsequent_indent=indentation,
         )
 
-        if _text:
-            _lines.extend(_text)
-        _lines.append("")
+        if _wrapped_line:
+            _wrapped_lines.extend(_wrapped_line)
+        _wrapped_lines.append("")
 
         with contextlib.suppress(IndexError):
-            if not _lines[-1] and not _lines[-2]:
-                _lines.pop(-1)
+            if not _wrapped_lines[-1] and not _wrapped_lines[-2]:
+                _wrapped_lines.pop(-1)
 
-    return _lines
+    if (
+        description[-len(indentation) - 1 : -len(indentation)] == "\n"
+        and description[-len(indentation) - 2 : -len(indentation)] != "\n\n"
+    ):
+        _wrapped_lines.pop(-1)
+
+    return _wrapped_lines
 
 
 def do_clean_url(url: str, indentation: str) -> str:
     r"""Strip newlines and multiple whitespace from URL string.
 
     This function deals with situations such as:
 
@@ -285,20 +293,24 @@
         position of each field list found in the passed description.
         A boolean indicating whether long field list lines should be wrapped.
     """
     _field_idx = []
     _wrap_parameters = False
 
     if style == "epytext":
-        _field_iter = re.finditer(EPYTEXT_REGEX, text)
-        _field_idx = [(_field.start(0), _field.end(0)) for _field in _field_iter]
+        _field_idx = [
+            (_field.start(0), _field.end(0))
+            for _field in re.finditer(EPYTEXT_REGEX, text)
+        ]
         _wrap_parameters = True
     elif style == "sphinx":
-        _field_iter = re.finditer(SPHINX_REGEX, text)
-        _field_idx = [(_field.start(0), _field.end(0)) for _field in _field_iter]
+        _field_idx = [
+            (_field.start(0), _field.end(0))
+            for _field in re.finditer(SPHINX_REGEX, text)
+        ]
         _wrap_parameters = True
 
     return _field_idx, _wrap_parameters
 
 
 def do_find_links(text: str) -> List[Tuple[int, int]]:
     r"""Determine if docstring contains any links.
@@ -375,26 +387,24 @@
     _lines: List[str] = []
     _text_idx = 0
 
     # Check if the description contains any URLs.
     _url_idx = do_find_links(text)
 
     # Check if the description contains any field lists.
-    _field_idx, _wrap_fields = do_find_field_lists(text, style)
+    _field_idx, _wrap_fields = do_find_field_lists(
+        text,
+        style,
+    )
 
     # Field list wrapping takes precedence over URL wrapping.
-    for _fieldl, _fieldu in _field_idx:
-        for _key, _value in enumerate(_url_idx):
-            if (
-                _value[0] == _fieldl
-                or _value[0] == _fieldu
-                or _value[1] == _fieldl
-                or _value[1] == _fieldu
-            ):
-                _url_idx.pop(_key)
+    _url_idx = _field_over_url(
+        _field_idx,
+        _url_idx,
+    )
 
     if not _url_idx and not (_field_idx and _wrap_fields):
         return description_to_list(
             text,
             indentation,
             wrap_length,
         )
@@ -415,23 +425,15 @@
             _lines,
             _text_idx,
             indentation,
             wrap_length,
         )
     else:
         # Finally, add everything after the last URL or field list directive.
-        with contextlib.suppress(IndexError):
-            _text = (
-                text[_text_idx + 1 :] if text[_text_idx] == "\n" else text[_text_idx:]
-            ).splitlines()
-            for _idx, _line in enumerate(_text):
-                if _line not in ["", "\n", f"{indentation}"]:
-                    _text[_idx] = f"{indentation}{_line.strip()}"
-
-            _lines += _text
+        _lines += _do_close_description(text, _text_idx, indentation)
 
     return _lines
 
 
 def do_wrap_field_lists(  # noqa: PLR0913
     text: str,
     field_idx: List[Tuple[int, int]],
@@ -475,21 +477,18 @@
 
     for _idx, __ in enumerate(field_idx):
         _field_name = text[field_idx[_idx][0] : field_idx[_idx][1]]
         _field_body = _do_join_field_body(
             text,
             field_idx,
             _idx,
-        ).strip()
+        )
 
-        if len(f"{_field_name} {_field_body}") <= (wrap_length - len(indentation)):
-            if _field_body.startswith("`") or not _field_body:
-                _field = f"{_field_name}{_field_body}"
-            else:
-                _field = f"{_field_name} {_field_body}"
+        if len(f"{_field_name}{_field_body}") <= (wrap_length - len(indentation)):
+            _field = f"{_field_name}{_field_body}"
             lines.append(f"{indentation}{_field}")
         else:
             lines.extend(
                 _do_wrap_field(_field_name, _field_body, indentation, wrap_length)
             )
 
         text_idx = field_idx[_idx][1]
@@ -664,15 +663,14 @@
             # "@type x:" <-- Epytext style
             re.match(EPYTEXT_REGEX, line)
             or
             # ":parameter: description" <-- Sphinx style
             re.match(SPHINX_REGEX, line)
             or
             # "parameter : description" <-- Numpy style
-            # "parameter: description" <-- Numpy style
             re.match(NUMPY_REGEX, line)
             or
             # "word\n----" <-- Numpy headings
             re.match(r"^\s*-+", line)
             or
             # "Args:" <-- Google style
             # "parameter:" <-- Google style
@@ -685,14 +683,22 @@
             re.match(r"\s*\S+\s+--\s+", line)
             or
             # Literal block
             re.match(LITERAL_REGEX, line)
             or
             # "@parameter"
             re.match(r"^ *@[a-zA-Z0-9_\- ]*(?:(?!:).)*$", line)
+            or
+            # "    c :math:`[0, `]`.
+            re.match(r" *\w *:[a-zA-Z0-9_\- ]*:", line)
+            or
+            # "Revision ID: <some id>>"
+            # "Revises: <some other id>"
+            # "Create Date: 2023-01-06 10:13:28.156709"
+            re.match(ALEMBIC_REGEX, line)
         )
         for line in split_lines
     )
 
 
 def is_some_sort_of_code(text: str) -> bool:
     """Return True if text looks like code."""
@@ -827,14 +833,47 @@
         return text
 
     lines = do_split_description(text, indentation, wrap_length, style)
 
     return indentation + "\n".join(lines).strip()
 
 
+def _do_close_description(
+    text: str,
+    text_idx: int,
+    indentation: str,
+) -> List[str]:
+    """Wrap any description following the last URL or field list.
+
+    Parameters
+    ----------
+    text : str
+        The docstring text.
+    text_idx : int
+        The index of the last URL or field list match.
+    indentation : str
+        The indentation string to use with docstrings.
+
+    Returns
+    -------
+    _split_lines : str
+        The text input split into individual lines.
+    """
+    _split_lines = []
+    with contextlib.suppress(IndexError):
+        _split_lines = (
+            text[text_idx + 1 :] if text[text_idx] == "\n" else text[text_idx:]
+        ).splitlines()
+        for _idx, _line in enumerate(_split_lines):
+            if _line not in ["", "\n", f"{indentation}"]:
+                _split_lines[_idx] = f"{indentation}{_line.strip()}"
+
+    return _split_lines
+
+
 def _do_join_field_body(text, field_idx, idx):
     """Join the filed body lines into a single line that can be wrapped.
 
     Parameters
     ----------
     text : str
         The docstring long description text that contains field lists.
@@ -851,17 +890,22 @@
     except IndexError:
         _field_body = text[field_idx[idx][1] :].strip()
 
     _field_body = " ".join(
         [_line.strip() for _line in _field_body.splitlines()]
     ).strip()
 
-    if _field_body:
+    # Add a space before the field body unless the field body is a link.
+    if not _field_body.startswith("`") and _field_body:
         _field_body = f" {_field_body}"
 
+    # Is there a blank line between field lists?  Keep it if so.
+    if text[field_idx[idx][1] : field_idx[idx][1] + 2] == "\n\n":
+        _field_body = "\n"
+
     return _field_body
 
 
 def _do_wrap_field(field_name, field_body, indentation, wrap_length):
     """Wrap complete field at wrap_length characters.
 
     Parameters
@@ -882,18 +926,50 @@
     """
     if len(indentation) > DEFAULT_INDENT:
         _subsequent = indentation + int(0.5 * len(indentation)) * " "
     else:
         _subsequent = 2 * indentation
 
     _wrapped_field = textwrap.wrap(
-        textwrap.dedent(f"{field_name} {field_body.strip()}"),
+        textwrap.dedent(f"{field_name}{field_body}"),
         width=wrap_length,
         initial_indent=indentation,
         subsequent_indent=_subsequent,
     )
 
     for _idx, _field in enumerate(_wrapped_field):
         _indent = indentation if _idx == 0 else _subsequent
         _wrapped_field[_idx] = f"{_indent}{re.sub(' +', ' ', _field.strip())}"
 
     return _wrapped_field
+
+
+def _field_over_url(
+    field_idx: List[Tuple[int, int]],
+    url_idx: List[Tuple[int, int]],
+):
+    """Remove URL indices that overlap with filed list indices.
+
+    Parameters
+    ----------
+    field_idx : list
+        The list of field list index tuples.
+    url_idx : list
+        The list of URL index tuples.
+
+    Returns
+    -------
+    url_idx : list
+        The url_idx list with any tuples that have indices overlapping with field
+        list indices removed.
+    """
+    for _fieldl, _fieldu in field_idx:
+        for _key, _value in enumerate(url_idx):
+            if (
+                _value[0] == _fieldl
+                or _value[0] == _fieldu
+                or _value[1] == _fieldl
+                or _value[1] == _fieldu
+            ):
+                url_idx.pop(_key)
+
+    return url_idx
```

### Comparing `docformatter-1.7.2/src/docformatter/util.py` & `docformatter-1.7.3/src/docformatter/util.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.2/PKG-INFO` & `docformatter-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docformatter
-Version: 1.7.2
+Version: 1.7.3
 Summary: Formats docstrings to follow PEP 257
 Home-page: https://github.com/PyCQA/docformatter
 License: Expat
 Keywords: PEP 257,pep257,style,formatter,docstrings
 Author: Steven Myint
 Maintainer: Doyle Rowland
 Maintainer-email: doyle.rowland@reliaqual.com
```

