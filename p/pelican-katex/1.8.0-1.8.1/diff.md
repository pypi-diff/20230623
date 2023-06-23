# Comparing `tmp/pelican_katex-1.8.0.tar.gz` & `tmp/pelican_katex-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_katex-1.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pelican_katex-1.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pelican_katex-1.8.0.tar` & `pelican_katex-1.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       58 2023-05-19 10:58:13.918511 pelican_katex-1.8.0/.gitignore
--rw-r--r--   0        0        0      645 2023-06-11 07:24:12.051475 pelican_katex-1.8.0/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-05-19 10:58:13.918511 pelican_katex-1.8.0/LICENSE
--rw-r--r--   0        0        0     4801 2023-06-11 07:22:41.648749 pelican_katex-1.8.0/README.md
--rw-r--r--   0        0        0      144 2023-06-11 07:24:18.252096 pelican_katex-1.8.0/pelican_katex/__init__.py
--rw-r--r--   0        0        0   629396 2023-04-28 11:42:18.000000 pelican_katex-1.8.0/pelican_katex/katex.js
--rw-r--r--   0        0        0     4058 2023-06-11 07:19:59.880631 pelican_katex-1.8.0/pelican_katex/markdown.py
--rw-r--r--   0        0        0     1888 2023-05-19 11:24:24.927500 pelican_katex-1.8.0/pelican_katex/plugin.py
--rw-r--r--   0        0        0     4044 2023-05-19 10:58:13.921844 pelican_katex-1.8.0/pelican_katex/render-katex.js
--rw-r--r--   0        0        0    10541 2023-05-19 10:58:13.921844 pelican_katex-1.8.0/pelican_katex/rendering.py
--rw-r--r--   0        0        0     1565 2023-05-19 11:24:24.927500 pelican_katex-1.8.0/pelican_katex/restructuredtext.py
--rw-r--r--   0        0        0      851 2023-05-19 11:24:24.924167 pelican_katex-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      206 2023-05-19 10:58:13.921844 pelican_katex-1.8.0/test/conftest.py
--rw-r--r--   0        0        0     2684 2023-05-19 10:58:13.921844 pelican_katex-1.8.0/test/html_template.py
--rw-r--r--   0        0        0     2212 2023-06-11 07:18:58.402214 pelican_katex-1.8.0/test/test_markdown.py
--rw-r--r--   0        0        0     5723 1970-01-01 00:00:00.000000 pelican_katex-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-05-19 10:58:13.918511 pelican_katex-1.8.1/.gitignore
+-rw-r--r--   0        0        0      733 2023-06-23 11:37:59.523581 pelican_katex-1.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-05-19 10:58:13.918511 pelican_katex-1.8.1/LICENSE
+-rw-r--r--   0        0        0     4801 2023-06-11 07:22:41.648749 pelican_katex-1.8.1/README.md
+-rw-r--r--   0        0        0      144 2023-06-23 11:38:22.294119 pelican_katex-1.8.1/pelican_katex/__init__.py
+-rw-r--r--   0        0        0   629396 2023-04-28 11:42:18.000000 pelican_katex-1.8.1/pelican_katex/katex.js
+-rw-r--r--   0        0        0     4242 2023-06-23 11:35:42.957032 pelican_katex-1.8.1/pelican_katex/markdown.py
+-rw-r--r--   0        0        0     1888 2023-05-19 11:24:24.927500 pelican_katex-1.8.1/pelican_katex/plugin.py
+-rw-r--r--   0        0        0     4044 2023-05-19 10:58:13.921844 pelican_katex-1.8.1/pelican_katex/render-katex.js
+-rw-r--r--   0        0        0    10541 2023-05-19 10:58:13.921844 pelican_katex-1.8.1/pelican_katex/rendering.py
+-rw-r--r--   0        0        0     1565 2023-05-19 11:24:24.927500 pelican_katex-1.8.1/pelican_katex/restructuredtext.py
+-rw-r--r--   0        0        0      851 2023-05-19 11:24:24.924167 pelican_katex-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0      206 2023-05-19 10:58:13.921844 pelican_katex-1.8.1/test/conftest.py
+-rw-r--r--   0        0        0     2684 2023-05-19 10:58:13.921844 pelican_katex-1.8.1/test/html_template.py
+-rw-r--r--   0        0        0     2517 2023-06-23 11:36:43.675125 pelican_katex-1.8.1/test/test_markdown.py
+-rw-r--r--   0        0        0     5723 1970-01-01 00:00:00.000000 pelican_katex-1.8.1/PKG-INFO
```

### Comparing `pelican_katex-1.8.0/CHANGELOG.md` & `pelican_katex-1.8.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 1.8.1
+
+- Ignore delimiters in markdown that are followed by alphanumeric characters
+
 ## 1.8.0
 
 - Allow escaping dollar delimiters in markdown with backslash
 
 ## 1.7.0
 
 - Update the bundled katex to 0.16.7
```

### Comparing `pelican_katex-1.8.0/LICENSE` & `pelican_katex-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.8.0/README.md` & `pelican_katex-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.8.0/pelican_katex/katex.js` & `pelican_katex-1.8.1/pelican_katex/katex.js`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.8.0/pelican_katex/markdown.py` & `pelican_katex-1.8.1/pelican_katex/markdown.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,22 @@
             if this_namespace != namespace:
                 node.attrib["xmlns"] = this_namespace
                 namespace = this_namespace
 
         candidates.extend((child, namespace) for child in node)
 
 
-PATTERN = r"(?P<preceding>\s?)(?P<delimiter>\$\$?)(?P<latex>[\S\n].*?)(?P=delimiter)"
+PATTERN = (
+    r"(?P<preceding>\s?)"
+    r"(?P<delimiter>\$\$?)"
+    r"(?P<latex>[\S\n].*?)"
+    # Only accept closing delimiters that are not followed by word characters
+    # (alpha-numeric or underscore) or at the end of the string.
+    r"(?P=delimiter)(?=\W|\Z)"
+)
 
 
 class KatexPattern(InlineProcessor):
     def __init__(self, md=None):
         super().__init__(pattern=PATTERN, md=md)
 
     def handleMatch(self, m, data):
```

### Comparing `pelican_katex-1.8.0/pelican_katex/plugin.py` & `pelican_katex-1.8.1/pelican_katex/plugin.py`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.8.0/pelican_katex/render-katex.js` & `pelican_katex-1.8.1/pelican_katex/render-katex.js`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.8.0/pelican_katex/rendering.py` & `pelican_katex-1.8.1/pelican_katex/rendering.py`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.8.0/pelican_katex/restructuredtext.py` & `pelican_katex-1.8.1/pelican_katex/restructuredtext.py`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.8.0/pyproject.toml` & `pelican_katex-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.8.0/test/html_template.py` & `pelican_katex-1.8.1/test/html_template.py`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.8.0/test/test_markdown.py` & `pelican_katex-1.8.1/test/test_markdown.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,18 +25,26 @@
     output = markdown.markdown(input, extensions=[KatexExtension()])
 
     template = HTMLTemplate('<p>Hello <span class="katex">...</span>!</p>')
     assert template == output
 
 
 def test_leaves_currencies_alone():
-    input = "I have 10$."
+    input = "I have 10$ and 20$."
     output = markdown.markdown(input, extensions=[KatexExtension()])
 
-    template = HTMLTemplate("<p>I have 10$.</p>")
+    template = HTMLTemplate("<p>I have 10$ and 20$.</p>")
+    assert template == output
+
+
+def test_ignores_dollar_followed_by_alnum_character():
+    input = "A coin is $1 and stored in $A register."
+    output = markdown.markdown(input, extensions=[KatexExtension()])
+
+    template = HTMLTemplate("<p>A coin is $1 and stored in $A register.</p>")
     assert template == output
 
 
 def test_double_dollar_renders_display_math():
     input = "$$x^2$$"
     output = markdown.markdown(input, extensions=[KatexExtension()])
```

### Comparing `pelican_katex-1.8.0/PKG-INFO` & `pelican_katex-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-katex
-Version: 1.8.0
+Version: 1.8.1
 Summary: LaTeX pre-rendering for pelican with katex.js
 Author-email: Marten Lienen <marten.lienen@gmail.com>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Pelican :: Plugins
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_ofatij3h_/tmpxqi5s0g3_TarContainer/0/15", line 184, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_ofatij3h_/tmpxqi5s0g3_TarContainer/0/15", line 184, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pelican-katex Version: 1.8.0 Summary: LaTeX pre-
+Metadata-Version: 2.1 Name: pelican-katex Version: 1.8.1 Summary: LaTeX pre-
 rendering for pelican with katex.js Author-email: Marten Lienen
 lienen@gmail.com> Requires-Python: >= 3.6 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier: Framework
 :: Pelican :: Plugins Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Education Requires-Dist:
```

