# Comparing `tmp/k3down2-0.1.8.tar.gz` & `tmp/k3down2-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "k3down2-0.1.8.tar", last modified: Thu Jan  7 16:40:11 2021, max compression
+gzip compressed data, was "k3down2-0.1.9.tar", last modified: Fri Jan  8 06:31:22 2021, max compression
```

## Comparing `k3down2-0.1.8.tar` & `k3down2-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-07 16:40:11.873642 k3down2-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2021-01-07 16:40:11.873642 k3down2-0.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-07 16:40:11.873642 k3down2-0.1.8/k3down2/
--rw-r--r--   0 runner    (1001) docker     (116)      813 2021-01-07 16:40:00.000000 k3down2-0.1.8/k3down2/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    11829 2021-01-07 16:40:00.000000 k3down2-0.1.8/k3down2/down2.py
--rw-r--r--   0 runner    (1001) docker     (116)    42484 2021-01-07 16:40:00.000000 k3down2-0.1.8/k3down2/mime.py
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2021-01-07 16:40:00.000000 k3down2-0.1.8/k3down2/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     2346 2021-01-07 16:40:00.000000 k3down2-0.1.8/k3down2/syntax_highlight.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-07 16:40:11.873642 k3down2-0.1.8/k3down2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2021-01-07 16:40:11.000000 k3down2-0.1.8/k3down2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      260 2021-01-07 16:40:11.000000 k3down2-0.1.8/k3down2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-07 16:40:11.000000 k3down2-0.1.8/k3down2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      126 2021-01-07 16:40:11.000000 k3down2-0.1.8/k3down2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2021-01-07 16:40:11.000000 k3down2-0.1.8/k3down2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-07 16:40:11.873642 k3down2-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2173 2021-01-07 16:40:10.000000 k3down2-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 06:31:22.668339 k3down2-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     2157 2021-01-08 06:31:22.668339 k3down2-0.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 06:31:22.668339 k3down2-0.1.9/k3down2/
+-rw-r--r--   0 runner    (1001) docker     (116)      813 2021-01-08 06:31:13.000000 k3down2-0.1.9/k3down2/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    12075 2021-01-08 06:31:13.000000 k3down2-0.1.9/k3down2/down2.py
+-rw-r--r--   0 runner    (1001) docker     (116)    42484 2021-01-08 06:31:13.000000 k3down2-0.1.9/k3down2/mime.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2173 2021-01-08 06:31:13.000000 k3down2-0.1.9/k3down2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2625 2021-01-08 06:31:13.000000 k3down2-0.1.9/k3down2/syntax_highlight.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-08 06:31:22.668339 k3down2-0.1.9/k3down2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2157 2021-01-08 06:31:22.000000 k3down2-0.1.9/k3down2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      260 2021-01-08 06:31:22.000000 k3down2-0.1.9/k3down2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-08 06:31:22.000000 k3down2-0.1.9/k3down2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      126 2021-01-08 06:31:22.000000 k3down2-0.1.9/k3down2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        8 2021-01-08 06:31:22.000000 k3down2-0.1.9/k3down2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-08 06:31:22.668339 k3down2-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2173 2021-01-08 06:31:22.000000 k3down2-0.1.9/setup.py
```

### Comparing `k3down2-0.1.8/PKG-INFO` & `k3down2-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k3down2
-Version: 0.1.8
+Version: 0.1.9
 Summary: convert markdown segment into easy to transfer media sucha images.
 Home-page: https://github.com/pykit3/k3down2
 Author: Zhang Yanpo
 Author-email: drdr.xp@gmail.com
 License: MIT
 Description: # k3down2
```

### Comparing `k3down2-0.1.8/k3down2/__init__.py` & `k3down2-0.1.9/k3down2/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 - google-chrome to render svg/html to png.
 - imagemagick to process images.
 - mmdc to convert mermaid chart to svg. See: https://mermaid-js.github.io/mermaid/#
 
 
 """
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __name__ = "k3down2"
 
 from .down2 import convert
 
 from .down2 import tex_to_zhihu
 from .down2 import tex_to_zhihu_compatible
 from .down2 import tex_to_zhihu_url
```

### Comparing `k3down2-0.1.8/k3down2/down2.py` & `k3down2-0.1.9/k3down2/down2.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,25 @@
                       '?tex={texurl}{align}"'
                       ' alt="{tex}{altalign}"'
                       ' class="ee_img'
                       ' tr_noresize"'
                       ' eeimg="1">')
 
 
-def convert(input_typ, input, output_typ):
+def convert(input_typ, input, output_typ, opt=None):
     conv = mappings[(input_typ, output_typ)]
     if callable(conv):
-        return conv(input)
+        kwargs = {}
+        if opt is not None and input_typ in opt:
+            kwargs = opt[input_typ]
+        return conv(input, **kwargs)
     else:
         #  indirect convertion
-        inp = convert(input_typ, input, conv)
-        return convert(conv, inp, output_typ)
+        inp = convert(input_typ, input, conv, opt=opt)
+        return convert(conv, inp, output_typ, opt=opt)
 
 
 def tex_to_zhihu_compatible(tex):
     r"""
     Convert tex to zhihu compatible format.
     - ``>`` in img alt mess up the next escaped brace: ``\{ q > 1 \} --> \{ q > 1 }``.
     """
@@ -305,15 +308,15 @@
     '''
 
     intyp = pagefn.rsplit('.')[-1]
     page = fread(pagefn)
     return render_to_img(intyp, page, typ)
 
 
-def render_to_img(mime, input, typ):
+def render_to_img(mime, input, typ, width=1000, height=2000):
     '''
     Render content that is renderable in chrome to image.
     Such as html, svg etc into image.
     It uses a headless chrome to render the page.
     Requirement: Chrome, imagemagick
 
     Args:
@@ -333,19 +336,21 @@
 
     chrome = 'google-chrome'
     if sys.platform == 'darwin':
         # mac
         chrome = "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome"
 
     with tempfile.TemporaryDirectory() as tdir:
+        tdir = '.'
+
         k3proc.command_ex(
             chrome,
             "--headless",
             "--screenshot",
-            "--window-size=1000,2000",
+            "--window-size={},{}".format(width, height),
             "--default-background-color=0",
             datauri,
             cwd=tdir,
         )
 
         if typ == 'png':
             moreargs = []
@@ -493,16 +498,16 @@
 
 
 mappings = {
     ('md', 'html'): md_to_html,
     ('md', 'jpg'): 'html',
     ('md', 'png'): 'html',
 
-    ('html', 'jpg'): lambda x: render_to_img('html', x, 'jpg'),
-    ('html', 'png'): lambda x: render_to_img('html', x, 'png'),
+    ('html', 'jpg'): lambda x, **kwargs: render_to_img('html', x, 'jpg', **kwargs),
+    ('html', 'png'): lambda x, **kwargs: render_to_img('html', x, 'png', **kwargs),
 
     # markdown table
     ('table', 'html'): mdtable_to_barehtml,
     ('table', 'jpg'): 'html',
     ('table', 'png'): 'html',
 
     ('mermaid', 'svg'): mermaid_to_svg,
```

### Comparing `k3down2-0.1.8/k3down2/mime.py` & `k3down2-0.1.9/k3down2/mime.py`

 * *Files identical despite different names*

### Comparing `k3down2-0.1.8/k3down2/setup.py` & `k3down2-0.1.9/k3down2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # DO NOT EDIT!!! built with `python _building/build_setup.py`
 import setuptools
 setuptools.setup(
     name="k3down2",
     packages=["k3down2"],
-    version="0.1.8",
+    version="0.1.9",
     license='MIT',
     description='convert markdown segment into easy to transfer media sucha images.',
     long_description='# k3down2\n\n[![Build Status](https://travis-ci.com/pykit3/k3down2.svg?branch=master)](https://travis-ci.com/pykit3/k3down2)\n![Python package](https://github.com/pykit3/k3down2/workflows/Python%20package/badge.svg)\n[![Documentation Status](https://readthedocs.org/projects/k3down2/badge/?version=stable)](https://k3down2.readthedocs.io/en/stable/?badge=stable)\n[![Package](https://img.shields.io/pypi/pyversions/k3down2)](https://pypi.org/project/k3down2)\n\nconvert markdown segment into easy to transfer media sucha images.\n\nk3down2 is a component of [pykit3] project: a python3 toolkit set.\n\n\nk3down2 is utility to convert markdown segment into easy to transfer media sucha images.\nIt depends on:\n\n- pandoc to render markdown snippet to html, such as tables.\n- chrome to render svg/html to png.\n\n\n\n\n\n# Install\n\n```\npip install k3down2\n```\n\n# Synopsis\n\n```python\n\n```\n\n#   Author\n\nZhang Yanpo (张炎泼) <drdr.xp@gmail.com>\n\n#   Copyright and License\n\nThe MIT License (MIT)\n\nCopyright (c) 2015 Zhang Yanpo (张炎泼) <drdr.xp@gmail.com>\n\n\n[pykit3]: https://github.com/pykit3',
     long_description_content_type="text/markdown",
     author='Zhang Yanpo',
     author_email='drdr.xp@gmail.com',
     url='https://github.com/pykit3/k3down2',
```

### Comparing `k3down2-0.1.8/k3down2/syntax_highlight.py` & `k3down2-0.1.9/k3down2/syntax_highlight.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,26 +66,36 @@
 
     lines = text.strip().split('\n')
 
     # extract code language: ```go
     lang = lines[0][3:].strip()
     text = '\n'.join(lines[1:-1])
 
-    if lang == '':
-        text = text.strip()
-        return u'<pre><code>%s</code></pre>\n' % escape(text)
-
     linenos = False
     style = Base16Style
 
+    prestyles = (r'line-height: 1.8 !important;'
+                 ' margin: 0 !important;'
+                 ' padding: 1em;'
+                 ' white-space: pre-wrap;'
+                 ' background: {};'
+                 ' color: {};').format(
+                         style.background_color,
+                         style.default_style,
+                 )
+
+    if lang == '':
+        text = text.strip()
+        return u'<pre style="%s"><code>%s</code></pre>\n' % (prestyles, escape(text))
+
     try:
         lexer = get_lexer_by_name(lang, stripall=True)
         formatter = HtmlFormatter(
             noclasses=True, linenos=linenos, style=style,
-                prestyles=r'line-height: 1.8 !important; margin: 0 !important; padding: 1em; background: {}'.format(style.background_color)
+                prestyles=prestyles
         )
         code = highlight(text, lexer, formatter)
         if linenos:
             return '<div class="highlight-wrapper">%s</div>\n' % code
         return code
     except BaseException:
         return '<pre class="%s"><code>%s</code></pre>\n' % (
```

### Comparing `k3down2-0.1.8/k3down2.egg-info/PKG-INFO` & `k3down2-0.1.9/k3down2.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k3down2
-Version: 0.1.8
+Version: 0.1.9
 Summary: convert markdown segment into easy to transfer media sucha images.
 Home-page: https://github.com/pykit3/k3down2
 Author: Zhang Yanpo
 Author-email: drdr.xp@gmail.com
 License: MIT
 Description: # k3down2
```

### Comparing `k3down2-0.1.8/setup.py` & `k3down2-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # DO NOT EDIT!!! built with `python _building/build_setup.py`
 import setuptools
 setuptools.setup(
     name="k3down2",
     packages=["k3down2"],
-    version="0.1.8",
+    version="0.1.9",
     license='MIT',
     description='convert markdown segment into easy to transfer media sucha images.',
     long_description='# k3down2\n\n[![Build Status](https://travis-ci.com/pykit3/k3down2.svg?branch=master)](https://travis-ci.com/pykit3/k3down2)\n![Python package](https://github.com/pykit3/k3down2/workflows/Python%20package/badge.svg)\n[![Documentation Status](https://readthedocs.org/projects/k3down2/badge/?version=stable)](https://k3down2.readthedocs.io/en/stable/?badge=stable)\n[![Package](https://img.shields.io/pypi/pyversions/k3down2)](https://pypi.org/project/k3down2)\n\nconvert markdown segment into easy to transfer media sucha images.\n\nk3down2 is a component of [pykit3] project: a python3 toolkit set.\n\n\nk3down2 is utility to convert markdown segment into easy to transfer media sucha images.\nIt depends on:\n\n- pandoc to render markdown snippet to html, such as tables.\n- chrome to render svg/html to png.\n\n\n\n\n\n# Install\n\n```\npip install k3down2\n```\n\n# Synopsis\n\n```python\n\n```\n\n#   Author\n\nZhang Yanpo (张炎泼) <drdr.xp@gmail.com>\n\n#   Copyright and License\n\nThe MIT License (MIT)\n\nCopyright (c) 2015 Zhang Yanpo (张炎泼) <drdr.xp@gmail.com>\n\n\n[pykit3]: https://github.com/pykit3',
     long_description_content_type="text/markdown",
     author='Zhang Yanpo',
     author_email='drdr.xp@gmail.com',
     url='https://github.com/pykit3/k3down2',
```

