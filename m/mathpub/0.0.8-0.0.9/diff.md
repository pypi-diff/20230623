# Comparing `tmp/mathpub-0.0.8.tar.gz` & `tmp/mathpub-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathpub-0.0.8.tar", last modified: Fri Jun 23 07:20:48 2023, max compression
+gzip compressed data, was "mathpub-0.0.9.tar", last modified: Fri Jun 23 18:46:45 2023, max compression
```

## Comparing `mathpub-0.0.8.tar` & `mathpub-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 07:20:48.492966 mathpub-0.0.8/
--rw-rw-rw-   0        0        0      159 2023-06-23 07:20:48.492966 mathpub-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-23 07:20:48.481968 mathpub-0.0.8/mathpub/
--rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.0.8/mathpub/__init__.py
--rw-rw-rw-   0        0        0     2575 2023-06-23 07:20:26.000000 mathpub-0.0.8/mathpub/page.py
--rw-rw-rw-   0        0        0     1590 2023-06-22 23:10:58.000000 mathpub-0.0.8/mathpub/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-23 07:20:48.490967 mathpub-0.0.8/mathpub.egg-info/
--rw-rw-rw-   0        0        0      159 2023-06-23 07:20:46.000000 mathpub-0.0.8/mathpub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-23 07:20:46.000000 mathpub-0.0.8/mathpub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 07:20:46.000000 mathpub-0.0.8/mathpub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 22:55:31.000000 mathpub-0.0.8/mathpub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-06-23 07:20:46.000000 mathpub-0.0.8/mathpub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 07:20:48.495965 mathpub-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-06-23 07:20:26.000000 mathpub-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:46:45.321788 mathpub-0.0.9/
+-rw-rw-rw-   0        0        0      159 2023-06-23 18:46:45.321788 mathpub-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-23 18:46:45.300789 mathpub-0.0.9/mathpub/
+-rw-rw-rw-   0        0        0       24 2023-06-22 22:13:13.000000 mathpub-0.0.9/mathpub/__init__.py
+-rw-rw-rw-   0        0        0     1855 2023-06-23 18:22:11.000000 mathpub-0.0.9/mathpub/page.py
+-rw-rw-rw-   0        0        0     3321 2023-06-23 18:29:55.000000 mathpub-0.0.9/mathpub/text_processing.py
+-rw-rw-rw-   0        0        0     1590 2023-06-22 23:10:58.000000 mathpub-0.0.9/mathpub/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:46:45.319788 mathpub-0.0.9/mathpub.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-06-23 18:46:44.000000 mathpub-0.0.9/mathpub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-23 18:46:44.000000 mathpub-0.0.9/mathpub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 18:46:44.000000 mathpub-0.0.9/mathpub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-23 18:44:47.000000 mathpub-0.0.9/mathpub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-23 18:46:44.000000 mathpub-0.0.9/mathpub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 18:46:45.323785 mathpub-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-06-23 18:40:19.000000 mathpub-0.0.9/setup.py
```

### Comparing `mathpub-0.0.8/mathpub/page.py` & `mathpub-0.0.9/mathpub/text_processing.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,101 +19,146 @@
     def __str__(self):
         return f"${self._s}$"
 
     def latex(self):
         return self._s
 
 
-class Line:
-    def __init__(self, atoms: list):
-        self._atoms = atoms
+class SpecialCharacter:
+    chars = {}
 
-    def __str__(self):
-        endl = "\n\n"
-        return f"{''.join(str(x) for x in self._atoms)}{endl}"
-
-    def latex(self):
-        endl = r"\\"
+    def __init_subclass__(cls, sym, **kwargs):  # noqa
+        super().__init_subclass__(**kwargs)
+        cls.chars[sym] = cls
+        cls.sym = sym
+
+    def __new__(cls, sym=None):
+        if sym is not None:
+            return cls.chars[sym]()
+        return super().__new__(cls)
 
-        return f"{''.join(x.latex() for x in self._atoms)}{endl}"
+    def __str__(self):
+        return self.sym
 
 
-class Page:
-    class DisplayPrinter:
-        def __init__(self, page):
-            self._page = page
+class Backslash(SpecialCharacter, sym="\\"):
+    def latex(self):
+        return r"\backslash"
 
-        def _repr_latex_(self):
-            return ''.join(x.latex() for x in self._page.lines)
 
-        __str__ = _repr_latex_
+class Circum(SpecialCharacter, sym="^"):
+    def latex(self):
+        return r"\textasciicircum"
 
-    @property
-    def display(self):
-        return self.DisplayPrinter(self)
 
-    @property
-    def markup(self):
-        return ''.join(str(x) for x in self.lines)
+class Tilde(SpecialCharacter, sym="~"):
+    def latex(self):
+        return r"\textasciitilde"
 
-    class DebugPrinter:
-        def __init__(self, page):
-            self._page = page
 
-        def __repr__(self):
-            return self._page.markup
+escapable_characters = {
+    "#": "Num",
+    "%": "Percent",
+    "&": "Ampersand",
+    "_": "Underscore",
+    "{": "LBrace",
+    "}": "RBrace"
+}
 
-    @property
-    def debug(self):
-        return self.DebugPrinter(self)
 
-    def __init__(self):
-        self.lines = []
-        self._last_length = 0
+def latex_gen(sym):
+    def latex(self):
+        return f"\\{sym}"
 
-    def _add_line(self, st: str):
-        res = []
+    return latex
 
-        ss = StringIO()
-        is_latex = False
 
-        for c in st:
-            if c == "$":
-                cur = ss.getvalue()
-                ss.close()
-
-                if is_latex:
-                    res.append(Latex(cur))
-                else:
-                    res.append(PlainText(cur))
+for sym, name in escapable_characters.items():
+    type(name, (SpecialCharacter,), {"latex": latex_gen(sym)}, sym=sym)
 
-                is_latex = not is_latex
-                ss = StringIO()
-            else:
-                ss.write(c)
 
-        cur = ss.getvalue()
-        if is_latex:
-            cur = "$" + cur
+def process_text(chr_iter):
+    res = []
+    esc = False
 
-        if cur:
-            res.append(PlainText(cur))
+    ss = StringIO()
 
-        self.lines.append(Line(res))
+    def get():
+        nonlocal ss
+        st = ss.getvalue()
+        ss.close()
+        ss = StringIO()
+        return st
 
-    def __iadd__(self, other):
-        for line in other.split("\n"):
-            self._add_line(line)
+    entered = False
 
-        return self
+    for c in chr_iter:
+        entered = True
+        if c == "\\":
+            if esc:
+                cur = get()
+                if cur:
+                    res.append(PlainText(cur))
+                res.append(Backslash())
+            esc = True
+        elif esc and c != "$":
+            cur = get()
+            if cur:
+                res.append(PlainText(cur))
+            res.append(Backslash())
+            ss.write(c)
+            esc = False
+        elif esc and c == "$":
+            ss.write("\\")
+            ss.write(c)
+            esc = False
+        elif c == "$":
+            cur = get()
+            if cur:
+                res.append(PlainText(cur))
+            break
+        elif c in SpecialCharacter.chars:
+            cur = get()
+            if cur:
+                res.append(PlainText(cur))
+
+            res.append(SpecialCharacter(c))
+        else:
+            ss.write(c)
+
+    if not entered:
+        raise StopIteration
+
+    cur = get()
+    if cur:
+        res.append(PlainText(cur))
+    ss.close()
+    return res
+
+
+def process_latex(char_iter):
+    esc = False
+
+    ss = StringIO()
+
+    entered = False
+
+    for c in char_iter:
+        entered = True
+        if not esc and c == "$":
+            res = ss.getvalue()
+            ss.close()
+            return [Latex(res)]
+
+        if c == "\\":
+            esc = True
+        else:
+            esc = False
+        ss.write(c)
 
-    def checkpoint(self):
-        self._last_length = len(self.lines)
+    if not entered:
+        raise StopIteration
 
-    def rollback(self):
-        self.lines = self.lines[:self._last_length]
+    res = ss.getvalue()
+    ss.close()
 
-    @property
-    def latest(self):
-        new_page = Page()
-        new_page.lines = self.lines[self._last_length:]
-        return new_page
+    return process_text(res)
```

### Comparing `mathpub-0.0.8/mathpub/utils.py` & `mathpub-0.0.9/mathpub/utils.py`

 * *Files identical despite different names*

