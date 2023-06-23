# Comparing `tmp/parsita-2.0.0b1.tar.gz` & `tmp/parsita-2.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsita-2.0.0b1.tar", max compression
+gzip compressed data, was "parsita-2.0.0b2.tar", max compression
```

## Comparing `parsita-2.0.0b1.tar` & `parsita-2.0.0b2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1062 2023-05-10 01:19:05.730334 parsita-2.0.0b1/LICENSE
--rw-r--r--   0        0        0     2649 2023-06-15 01:24:20.089115 parsita-2.0.0b1/README.md
--rw-r--r--   0        0        0     2115 2023-06-15 01:24:49.805056 parsita-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      363 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/__init__.py
--rw-r--r--   0        0        0     5488 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/metaclasses.py
--rw-r--r--   0        0        0      165 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/options.py
--rw-r--r--   0        0        0      833 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/__init__.py
--rw-r--r--   0        0        0     3845 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_alternative.py
--rw-r--r--   0        0        0      940 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_any.py
--rw-r--r--   0        0        0     7859 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_base.py
--rw-r--r--   0        0        0     1532 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_conversion.py
--rw-r--r--   0        0        0     2345 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_debug.py
--rw-r--r--   0        0        0      640 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_end_of_source.py
--rw-r--r--   0        0        0     2576 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_literal.py
--rw-r--r--   0        0        0     1266 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_optional.py
--rw-r--r--   0        0        0     1509 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_predicate.py
--rw-r--r--   0        0        0     1809 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_regex.py
--rw-r--r--   0        0        0     3863 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_repeated.py
--rw-r--r--   0        0        0     6112 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_repeated_seperated.py
--rw-r--r--   0        0        0     2512 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_sequential.py
--rw-r--r--   0        0        0     1817 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_success.py
--rw-r--r--   0        0        0     1298 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/parsers/_until.py
--rw-r--r--   0        0        0      207 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/state/__init__.py
--rw-r--r--   0        0        0      807 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/state/_exceptions.py
--rw-r--r--   0        0        0     8171 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/state/_reader.py
--rw-r--r--   0        0        0      500 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/state/_result.py
--rw-r--r--   0        0        0     1050 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/state/_state.py
--rw-r--r--   0        0        0     1688 2023-06-15 01:24:20.093115 parsita-2.0.0b1/src/parsita/util.py
--rw-r--r--   0        0        0     3653 1970-01-01 00:00:00.000000 parsita-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-10 01:19:05.730334 parsita-2.0.0b2/LICENSE
+-rw-r--r--   0        0        0     2649 2023-06-19 18:30:55.314799 parsita-2.0.0b2/README.md
+-rw-r--r--   0        0        0     2115 2023-06-19 20:53:20.299938 parsita-2.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      363 2023-06-19 18:30:55.314799 parsita-2.0.0b2/src/parsita/__init__.py
+-rw-r--r--   0        0        0     5488 2023-06-19 18:30:55.314799 parsita-2.0.0b2/src/parsita/metaclasses.py
+-rw-r--r--   0        0        0      165 2023-06-19 18:30:55.314799 parsita-2.0.0b2/src/parsita/options.py
+-rw-r--r--   0        0        0      833 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/__init__.py
+-rw-r--r--   0        0        0     3845 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_alternative.py
+-rw-r--r--   0        0        0      940 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_any.py
+-rw-r--r--   0        0        0     7859 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_base.py
+-rw-r--r--   0        0        0     1532 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_conversion.py
+-rw-r--r--   0        0        0     2345 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_debug.py
+-rw-r--r--   0        0        0      640 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_end_of_source.py
+-rw-r--r--   0        0        0     2576 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_literal.py
+-rw-r--r--   0        0        0     1266 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_optional.py
+-rw-r--r--   0        0        0     1489 2023-06-19 18:58:14.007247 parsita-2.0.0b2/src/parsita/parsers/_predicate.py
+-rw-r--r--   0        0        0     1809 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_regex.py
+-rw-r--r--   0        0        0     3863 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_repeated.py
+-rw-r--r--   0        0        0     6112 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_repeated_seperated.py
+-rw-r--r--   0        0        0     2512 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_sequential.py
+-rw-r--r--   0        0        0     1817 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_success.py
+-rw-r--r--   0        0        0     1298 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/parsers/_until.py
+-rw-r--r--   0        0        0      207 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/state/__init__.py
+-rw-r--r--   0        0        0      807 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/state/_exceptions.py
+-rw-r--r--   0        0        0     8450 2023-06-19 20:34:31.867158 parsita-2.0.0b2/src/parsita/state/_reader.py
+-rw-r--r--   0        0        0      500 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/state/_result.py
+-rw-r--r--   0        0        0     1050 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/state/_state.py
+-rw-r--r--   0        0        0     1688 2023-06-19 18:30:55.318799 parsita-2.0.0b2/src/parsita/util.py
+-rw-r--r--   0        0        0     3653 1970-01-01 00:00:00.000000 parsita-2.0.0b2/PKG-INFO
```

### Comparing `parsita-2.0.0b1/LICENSE` & `parsita-2.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/README.md` & `parsita-2.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/pyproject.toml` & `parsita-2.0.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parsita"
-version = "2.0.0b1"
+version = "2.0.0b2"
 description = "Parser combinator library for Python"
 authors = ["David Hagen <david@drhagen.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://parsita.drhagen.com"
 repository = "https://github.com/drhagen/parsita"
 keywords = ["text", "parsing", "parser",  "combinator"]
```

### Comparing `parsita-2.0.0b1/src/parsita/metaclasses.py` & `parsita-2.0.0b2/src/parsita/metaclasses.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/__init__.py` & `parsita-2.0.0b2/src/parsita/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_alternative.py` & `parsita-2.0.0b2/src/parsita/parsers/_alternative.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_any.py` & `parsita-2.0.0b2/src/parsita/parsers/_any.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_base.py` & `parsita-2.0.0b2/src/parsita/parsers/_base.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_conversion.py` & `parsita-2.0.0b2/src/parsita/parsers/_conversion.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_debug.py` & `parsita-2.0.0b2/src/parsita/parsers/_debug.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_end_of_source.py` & `parsita-2.0.0b2/src/parsita/parsers/_end_of_source.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_literal.py` & `parsita-2.0.0b2/src/parsita/parsers/_literal.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_optional.py` & `parsita-2.0.0b2/src/parsita/parsers/_optional.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_predicate.py` & `parsita-2.0.0b2/src/parsita/parsers/_predicate.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,20 @@
     def __init__(self, parser: Parser[Input, Output], predicate: Callable[[Output], bool], description: str):
         super().__init__()
         self.parser = parser
         self.predicate = predicate
         self.description = description
 
     def consume(self, state: State[Input], reader: Reader[Input]):
-        remainder = reader
-        status = self.parser.cached_consume(state, remainder)
+        status = self.parser.cached_consume(state, reader)
         if isinstance(status, Continue):
             if self.predicate(status.value):
                 return status
             else:
-                state.register_failure(self.description, reader)
+                state.register_failure(self.description, status.remainder)
                 return None
         else:
             return status
 
     def __repr__(self):
         return self.name_or_nothing() + f"pred({self.parser.name_or_repr()}, {self.description})"
```

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_regex.py` & `parsita-2.0.0b2/src/parsita/parsers/_regex.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_repeated.py` & `parsita-2.0.0b2/src/parsita/parsers/_repeated.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_repeated_seperated.py` & `parsita-2.0.0b2/src/parsita/parsers/_repeated_seperated.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_sequential.py` & `parsita-2.0.0b2/src/parsita/parsers/_sequential.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_success.py` & `parsita-2.0.0b2/src/parsita/parsers/_success.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/parsers/_until.py` & `parsita-2.0.0b2/src/parsita/parsers/_until.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/state/_exceptions.py` & `parsita-2.0.0b2/src/parsita/state/_exceptions.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/state/_reader.py` & `parsita-2.0.0b2/src/parsita/state/_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -166,31 +166,42 @@
         match = self.next_token_regex.match(self.source, self.position)
         if match is None:
             return self.source[self.position]
         else:
             return self.source[match.start() : match.end()]
 
     def current_line(self):
+        # StringIO is not consistent in how it treats empty strings
+        # and other strings not ending in newlines. Ensure that the
+        # source always ends in a newline.
+        # This also ensures that the loop below runs at least once
+        # and that `line` always ends with a newline.
+        if not self.source.endswith("\n"):
+            source = self.source + "\n"
+        else:
+            source = self.source
+
         characters_consumed = 0
-        for line_index, line in enumerate(StringIO(self.source)):
+        for line_index, line in enumerate(StringIO(source)):  # noqa: B007
             if characters_consumed + len(line) > self.position:
                 # The line with the error has been found
                 character_index = self.position - characters_consumed
-
-                # This creates a line like this '        ^                  '
-                pointer = (" " * character_index) + "^" + (" " * (len(line) - character_index - 1))
-
-                # This adds a newline to line in case it is the end of the file
-                if line[-1] != "\n":
-                    line = line + "\n"
-
-                # Add one to indexes to account for 0-indexes
-                return line_index + 1, character_index + 1, line, pointer
+                break
             else:
                 characters_consumed += len(line)
+        else:
+            # The error is at the end of the input
+            # Put the pointer just beyond the last non-newline character
+            character_index = len(line) - 1
+
+        # This creates a line like this '   ^'
+        pointer = " " * character_index + "^"
+
+        # Add one to indexes to account for 0-indexes
+        return line_index + 1, character_index + 1, line, pointer
 
     def expected_error(self, expected: str) -> str:
         """Generate a basic error to include the current state.
 
         A parser can supply only a representation of what it is expecting to
         this method and the reader will provide the context, including the line
         and character positions.
@@ -200,38 +211,37 @@
 
         Returns:
             A full error message
         """
         expected_string = " or ".join(expected)
 
         if self.finished:
-            return super().expected_error(expected)
+            next_string = "end of source"
         else:
-            line_index, character_index, line, pointer = self.current_line()
+            next_string = repr(self.next_token())
+
+        line_index, character_index, line, pointer = self.current_line()
 
-            return (
-                f"Expected {expected_string} but found {self.next_token()!r}\n"
-                f"Line {line_index}, character {character_index}\n\n{line}{pointer}"
-            )
+        return (
+            f"Expected {expected_string} but found {next_string}\n"
+            f"Line {line_index}, character {character_index}\n\n{line}{pointer}"
+        )
 
     def recursion_error(self, repeated_parser: str):
         """Generate an error to indicate that infinite recursion was encountered.
 
         A parser can supply a representation of itself to this method and the
         reader will supply the context, including the location where the
         parser stalled.
 
         Args:
             repeated_parser: A representation of the repeated parser
 
         Returns:
             A full error message
         """
-        if self.finished:
-            return super().recursion_error(repeated_parser)
-        else:
-            line_index, character_index, line, pointer = self.current_line()
+        line_index, character_index, line, pointer = self.current_line()
 
-            return (
-                f"Infinite recursion detected in {repeated_parser}; empty string was matched and will be matched "
-                f"forever\nLine {line_index}, character {character_index}\n\n{line}{pointer}"
-            )
+        return (
+            f"Infinite recursion detected in {repeated_parser}; empty string was matched and will be matched "
+            f"forever\nLine {line_index}, character {character_index}\n\n{line}{pointer}"
+        )
```

### Comparing `parsita-2.0.0b1/src/parsita/state/_state.py` & `parsita-2.0.0b2/src/parsita/state/_state.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/src/parsita/util.py` & `parsita-2.0.0b2/src/parsita/util.py`

 * *Files identical despite different names*

### Comparing `parsita-2.0.0b1/PKG-INFO` & `parsita-2.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsita
-Version: 2.0.0b1
+Version: 2.0.0b2
 Summary: Parser combinator library for Python
 Home-page: https://github.com/drhagen/parsita
 License: MIT
 Keywords: text,parsing,parser,combinator
 Author: David Hagen
 Author-email: david@drhagen.com
 Requires-Python: >=3.8.0,<4.0.0
```

