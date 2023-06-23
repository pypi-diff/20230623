# Comparing `tmp/pptreport-1.0.0.tar.gz` & `tmp/pptreport-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptreport-1.0.0.tar", last modified: Fri Jun  2 14:44:33 2023, max compression
+gzip compressed data, was "pptreport-1.1.0.tar", last modified: Fri Jun 23 14:14:22 2023, max compression
```

## Comparing `pptreport-1.0.0.tar` & `pptreport-1.1.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:44:33.449181 pptreport-1.0.0/
--rwxr-xr-x   0 root         (0) root         (0)       61 2023-06-02 14:15:58.000000 pptreport-1.0.0/CHANGES.rst
--rwxr-xr-x   0 root         (0) root         (0)     1070 2023-04-21 09:55:42.000000 pptreport-1.0.0/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)       21 2023-06-02 14:44:02.000000 pptreport-1.0.0/MANIFEST.in
--rwxr-xr-x   0 root         (0) root         (0)      718 2023-06-02 14:44:33.574944 pptreport-1.0.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      190 2023-06-02 14:15:20.000000 pptreport-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:44:33.496050 pptreport-1.0.0/pptreport/
--rwxr-xr-x   0 root         (0) root         (0)      421 2023-04-21 09:55:42.000000 pptreport-1.0.0/pptreport/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       23 2023-06-02 12:20:09.000000 pptreport-1.0.0/pptreport/_version.py
--rwxr-xr-x   0 root         (0) root         (0)    23262 2023-06-02 10:28:36.000000 pptreport-1.0.0/pptreport/box.py
--rwxr-xr-x   0 root         (0) root         (0)     2427 2023-06-02 10:28:36.000000 pptreport-1.0.0/pptreport/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:44:33.559317 pptreport-1.0.0/pptreport/fonts/
--rwxr-xr-x   0 root         (0) root         (0)     4483 2023-04-21 09:55:42.000000 pptreport-1.0.0/pptreport/fonts/OFL.txt
--rwxr-xr-x   0 root         (0) root         (0)   129784 2023-04-21 09:55:42.000000 pptreport-1.0.0/pptreport/fonts/OpenSans-Bold.ttf
--rwxr-xr-x   0 root         (0) root         (0)   135380 2023-04-21 09:55:42.000000 pptreport-1.0.0/pptreport/fonts/OpenSans-Italic.ttf
--rwxr-xr-x   0 root         (0) root         (0)   129796 2023-04-21 09:55:42.000000 pptreport-1.0.0/pptreport/fonts/OpenSans-Regular.ttf
--rwxr-xr-x   0 root         (0) root         (0)    47876 2023-06-02 10:28:36.000000 pptreport-1.0.0/pptreport/powerpointreport.py
--rwxr-xr-x   0 root         (0) root         (0)    17996 2023-06-02 12:11:47.000000 pptreport-1.0.0/pptreport/slide.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:44:33.528070 pptreport-1.0.0/pptreport.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)      718 2023-06-02 14:44:33.000000 pptreport-1.0.0/pptreport.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      622 2023-06-02 14:44:33.000000 pptreport-1.0.0/pptreport.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2023-06-02 14:44:33.000000 pptreport-1.0.0/pptreport.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)       49 2023-06-02 14:44:33.000000 pptreport-1.0.0/pptreport.egg-info/entry_points.txt
--rwxr-xr-x   0 root         (0) root         (0)       50 2023-06-02 14:44:33.000000 pptreport-1.0.0/pptreport.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)       10 2023-06-02 14:44:33.000000 pptreport-1.0.0/pptreport.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)       94 2023-04-21 09:55:42.000000 pptreport-1.0.0/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      862 2023-06-02 14:44:33.574944 pptreport-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 14:44:33.574944 pptreport-1.0.0/tests/
--rwxr-xr-x   0 root         (0) root         (0)     2928 2023-06-02 10:28:36.000000 pptreport-1.0.0/tests/test_box.py
--rwxr-xr-x   0 root         (0) root         (0)     5830 2023-06-02 10:28:36.000000 pptreport-1.0.0/tests/test_classes.py
--rwxr-xr-x   0 root         (0) root         (0)     1820 2023-06-02 10:28:36.000000 pptreport-1.0.0/tests/test_cli.py
--rwxr-xr-x   0 root         (0) root         (0)    18677 2023-06-02 10:28:36.000000 pptreport-1.0.0/tests/test_input.py
--rwxr-xr-x   0 root         (0) root         (0)     2533 2023-06-02 10:28:36.000000 pptreport-1.0.0/tests/test_slide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:14:22.422603 pptreport-1.1.0/
+-rwxr-xr-x   0 root         (0) root         (0)      687 2023-06-23 14:01:25.000000 pptreport-1.1.0/CHANGES.rst
+-rwxr-xr-x   0 root         (0) root         (0)     1070 2023-04-21 09:55:42.000000 pptreport-1.1.0/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)       21 2023-06-23 13:24:22.000000 pptreport-1.1.0/MANIFEST.in
+-rwxr-xr-x   0 root         (0) root         (0)      717 2023-06-23 14:14:22.585316 pptreport-1.1.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)      190 2023-06-23 13:24:22.000000 pptreport-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:14:22.506151 pptreport-1.1.0/pptreport/
+-rwxr-xr-x   0 root         (0) root         (0)      421 2023-06-16 15:34:29.000000 pptreport-1.1.0/pptreport/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       23 2023-06-23 14:01:26.000000 pptreport-1.1.0/pptreport/_version.py
+-rwxr-xr-x   0 root         (0) root         (0)    25760 2023-06-23 14:01:26.000000 pptreport-1.1.0/pptreport/box.py
+-rwxr-xr-x   0 root         (0) root         (0)     2427 2023-06-23 13:24:22.000000 pptreport-1.1.0/pptreport/cli.py
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-23 14:01:26.000000 pptreport-1.1.0/pptreport/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:14:22.553440 pptreport-1.1.0/pptreport/fonts/
+-rwxr-xr-x   0 root         (0) root         (0)     4483 2023-04-21 09:55:42.000000 pptreport-1.1.0/pptreport/fonts/OFL.txt
+-rwxr-xr-x   0 root         (0) root         (0)   129784 2023-04-21 09:55:42.000000 pptreport-1.1.0/pptreport/fonts/OpenSans-Bold.ttf
+-rwxr-xr-x   0 root         (0) root         (0)   135380 2023-04-21 09:55:42.000000 pptreport-1.1.0/pptreport/fonts/OpenSans-Italic.ttf
+-rwxr-xr-x   0 root         (0) root         (0)   129796 2023-04-21 09:55:42.000000 pptreport-1.1.0/pptreport/fonts/OpenSans-Regular.ttf
+-rwxr-xr-x   0 root         (0) root         (0)    48318 2023-06-23 14:01:26.000000 pptreport-1.1.0/pptreport/powerpointreport.py
+-rwxr-xr-x   0 root         (0) root         (0)    17996 2023-06-23 13:24:22.000000 pptreport-1.1.0/pptreport/slide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:14:22.521777 pptreport-1.1.0/pptreport.egg-info/
+-rwxr-xr-x   0 root         (0) root         (0)      717 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)      642 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/SOURCES.txt
+-rwxr-xr-x   0 root         (0) root         (0)        1 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/dependency_links.txt
+-rwxr-xr-x   0 root         (0) root         (0)       49 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/entry_points.txt
+-rwxr-xr-x   0 root         (0) root         (0)       66 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/requires.txt
+-rwxr-xr-x   0 root         (0) root         (0)       10 2023-06-23 14:14:22.000000 pptreport-1.1.0/pptreport.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)       94 2023-04-21 09:55:42.000000 pptreport-1.1.0/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)     1012 2023-06-23 14:14:22.585316 pptreport-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:14:22.569094 pptreport-1.1.0/tests/
+-rwxr-xr-x   0 root         (0) root         (0)     4130 2023-06-23 14:01:26.000000 pptreport-1.1.0/tests/test_box.py
+-rwxr-xr-x   0 root         (0) root         (0)     5830 2023-06-23 13:24:23.000000 pptreport-1.1.0/tests/test_classes.py
+-rwxr-xr-x   0 root         (0) root         (0)     1732 2023-06-23 14:01:26.000000 pptreport-1.1.0/tests/test_cli.py
+-rwxr-xr-x   0 root         (0) root         (0)    18819 2023-06-23 14:01:26.000000 pptreport-1.1.0/tests/test_input.py
+-rwxr-xr-x   0 root         (0) root         (0)     2533 2023-06-23 13:24:23.000000 pptreport-1.1.0/tests/test_slide.py
```

### Comparing `pptreport-1.0.0/LICENSE` & `pptreport-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pptreport-1.0.0/PKG-INFO` & `pptreport-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pptreport
-Version: 1.0.0
-Home-page: https://github.com/msbentsen/pptreport
+Version: 1.1.0
+Home-page: https://github.com/loosolab/pptreport
 Author: Mette Bentsen
 Author-email: mette.bentsen@mpi-bn.mpg.de
 License: MIT
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pptreport-1.0.0/pptreport/box.py` & `pptreport-1.1.0/pptreport/box.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,26 +5,29 @@
 import numpy as np
 
 from pptx.enum.shapes import MSO_SHAPE
 from pptx.enum.text import MSO_ANCHOR, PP_ALIGN
 from pptx.dml.color import RGBColor
 from pptx.util import Pt
 from pptx.text.layout import TextFitter
+from pptx.oxml.xmlchemy import OxmlElement
+
+from pptreport.config import font_name, md_heading_sizes
 
 # For reading pictures
 from PIL import Image
 Image.MAX_IMAGE_PIXELS = None  # disable DecompressionBombError
 
 
 def split_string(string, length):
     """ Split a string into a list of strings of length 'length' """
     return [string[i:i + length] for i in range(0, len(string), length)]
 
 
-def estimate_fontsize(txt_frame, min_size=6, max_size=18, logger=None):
+def estimate_fontsize(txt_frame, text, min_size=6, max_size=18, logger=None):
     """
     Resize text to fit the textbox.
 
     Parameters
     ----------
     txt_frame : pptx.text.text.TextFrame
         The text frame to be resized.
@@ -35,20 +38,14 @@
 
     Returns
     --------
     size : int
         The estimated fontsize of the text.
     """
 
-    # Get the text across all runs
-    text = ""
-    for paragraph in txt_frame.paragraphs:
-        for run in paragraph.runs:
-            text += run.text
-
     # Get font
     font = pkg_resources.resource_filename("pptreport", "fonts/OpenSans-Regular.ttf")
 
     # Calculate best fontsize
     size = None
     try:
         size = TextFitter.best_fit_font_size(text, txt_frame._extents, max_size, font)
@@ -82,24 +79,100 @@
     # Make sure size is within bounds
     size = max(min_size, size)
     size = min(max_size, size)
 
     return size
 
 
-def format_textframe(txt_frame, size=12, name="Calibri"):
-    """ Set the fontsize of the text in the text frame. """
+def set_fontsize(run, size):
+    """ Set the fontsize of a run.
+
+    Parameters
+    ----------
+    run : pptx.text.text.Run
+        The run to be resized.
+    size : int
+        The fontsize of the text.
+    """
+
+    try:
+        run.font.size = Pt(size)
+    except Exception as e:
+        raise ValueError(f"Invalid value for 'fontsize' parameter: {size}. Error was: {e}")
+
+
+def set_fontname(run, font_name):
+    """ Set the fontname of a run.
+
+    Parameters
+    ----------
+    run : pptx.text.text.Run
+        The run to be resized.
+    font_name : str
+        The fontname of the text.
+    """
+    try:
+        run.font.name = font_name
+    except Exception as e:
+        raise ValueError(f"Invalid value for 'fontname' parameter: {font_name}. Error was: {e}")
+
+
+def set_highlight(run, color):
+    """ Set background highlight color of text in run. Method from https://github.com/MartinPacker/md2pptx.
+
+    Color is specified as a hex string, e.g. "#FF0000" for red.
+    """
+
+    # get run properties
+    rPr = run._r.get_or_add_rPr()
+
+    # Create highlight element
+    hl = OxmlElement("a:highlight")
+
+    # Create specify RGB Colour element with color specified
+    srgbClr = OxmlElement("a:srgbClr")
+    setattr(srgbClr, "val", color)
+
+    # Add colour specification to highlight element
+    hl.append(srgbClr)
+
+    # Add highlight element to run properties
+    rPr.append(hl)
+
+    return run
 
-    for paragraph in txt_frame.paragraphs:
-        for run in paragraph.runs:
-            try:
-                run.font.size = Pt(size)
-            except Exception as e:
-                raise ValueError(f"Invalid value for 'fontsize' parameter: {size}. Error was: {e}")
-            run.font.name = "Calibri"
+
+def parse_md_structure(data, current_path=[], info={}):
+    """ Recursive function to parse the markdown structure from mistune """
+
+    result = []
+    if isinstance(data, dict):
+
+        skip_keys = ["type", "children", "text", "alt"]
+        info = info.copy()
+        info.update({key: data[key] for key in data.keys() if key not in skip_keys})
+
+        if 'type' in data:
+            current_path.append(data['type'])
+            if 'children' not in data:  # leaf node
+                text = data.get('text', data.get('alt', ""))  # text or alt
+                result.append((current_path[:], (text, info)))
+                current_path.pop()
+
+            else:
+                if "children" in data:
+                    for child in data["children"]:
+                        result.extend(parse_md_structure(child, current_path, info))
+                    current_path.pop()
+
+    elif isinstance(data, list):
+        for i, item in enumerate(data):
+            result.extend(parse_md_structure(item, current_path, info))
+
+    return result
 
 
 class Box():
     """ A box is a constrained area of the slide which contains a single element e.g. text, a picture, a table, etc. """
 
     def __init__(self, slide, coordinates):
         """
@@ -409,136 +482,130 @@
         if horizontal == "left":
             self.content_left = self.left
         elif horizontal == "right":
             self.content_left = self.left + self.width - self.content_width
         elif horizontal == "center":
             self.content_left = self.left + (self.width - self.content_width) / 2
 
-    def _contains_md(self, text):
-        """ Checks if a string contains any md sequences.
-        """
-
-        # https://chubakbidpaa.com/interesting/2021/09/28/regex-for-md.html
-        md_regex = {"heading": r"(#{1,8}\s)(.*)",
-                    "emphasis": r"(\*|\_)+(\S+)(\*|\_)+",
-                    "links": r"(\[.*\])(\((http)(?:s)?(\:\/\/).*\))",
-                    "images": r"(\!)(\[(?:.*)?\])\(.*(\.(jpg|png|gif|tiff|bmp))(?:(\s\"|\')(\w|\W|\d)+(\"|\'))?\)",
-                    "uo-list": r"(^(\W{1})(\s)(.*)(?:$)?)+",
-                    "io-list": r"(^(\d+\.)(\s)(.*)(?:$)?)+",
-                    }
-
-        for reg in md_regex.values():
-            if re.search(reg, text):
-                return True
-
-        return False
-
-    def _get_text_all_children(self, parent):
-        """
-        Small helper to improve robustness.
-        Should normally be only one child per parent on this level.
-        ! Use only internally for ast tree from mistune!
-        """
-        text = ""
-        for c in parent["children"]:
-            text += c["text"]
-        return text
-
-    def _fill_md(self, p, text):
+    def _fill_md(self, p, text, font_size):
         """
         Fills a paragraph p with basic markdown formatted text, like **Bold**, *italic* ,...
         Supported types:
         - Bold     **bold** / __bold__
         - Italic    *ital*  /  _ital_
         - Link     	[title](https://www.example.com)
         - Heading   #H1 / ## H2 / ...
         (- Image    Only partly - if alternative text is given it will be shown, image should be add via add_image())
 
+        If text does not contain markdown, it will be added as plain text.
+
         Parameters
         ----------
         p : <pptx.text.text._Paragraph>
             paragraph to add to
         text : str
             The text to be added to the box.
+        font_size : int
+            The font size of the text. Header sizes are controlled by the fontsizes given in config.md_heading_sizes.
         """
 
         self.logger.debug(f"Adding markdown formatted text to box '{self.box_index}'.")
 
         # mistune is only needed for md, only import if needed
         import mistune
 
         # render input as html.ast
         markdown = mistune.create_markdown(renderer="ast")
 
+        supported_types = ["paragraph", "text", "heading", "newline", "image", "list", "list_item",
+                           "block_text", "block_quote", "strong", "emphasis", "link", "codespan", "thematic_break"]
+
         # traverse the tree
         for i, string in enumerate(text.split("\n")):
             for par in markdown(string):
-                if par["type"] == "paragraph":
 
-                    # Add newlines between paragraphs
-                    if i > 0:
-                        run = p.add_run()
-                        run.text = "\n"
-
-                    for child in par["children"]:  # children are the single md elements like bold, italic,...
-                        # italic
-                        if child["type"] == "emphasis":
-                            run = p.add_run()
-                            run.font.italic = True
-                            run.text = self._get_text_all_children(child)
-                        # bold
-                        elif child["type"] == "strong":
-                            run = p.add_run()
-                            run.text = self._get_text_all_children(child)
-                            run.font.bold = True
-                        # link
-                        elif child["type"] == "link":
-                            run = p.add_run()
-                            run.text = self._get_text_all_children(child)
-                            hlink = run.hyperlink
-                            hlink.address = child["link"]
-                        # alternative text for images
-                        elif child["type"] == "image":
-                            try:
-                                print("markdown images not supported. Trying alternative text.")
-                                text = child["alt"]
-                                run = p.add_run()
-                                run.text = text
-                            except KeyError:
-                                print("No alternative text given. Skipping entry.")
-                        # codespan
-                        # elif child["type"]=="codespan":
-                        # plain text & default case
-                        else:
-                            try:
-                                text = child["text"]
-                            except KeyError:
-                                print("Unknown child type. Trying to append children's content as plain text.")
-                                try:
-                                    text = self._get_text_all_children(child)
-                                except KeyError:
-                                    print(f"Child type {child['type']} is not supported.")
-                                    continue  # continue with next child
-                            run = p.add_run()
-                            run.text = text
+                # Add newlines between string elements (except for the first element)
+                if i > 0:
+                    run = p.add_run()
+                    run.text = "\n"
+                    set_fontsize(run, font_size)
 
-                elif par["type"] == "newline":
+                # Parse all types within this string
+                parse_result = parse_md_structure(par, [])
+
+                # Get prefix for the line in case of list / code / quote
+                first_element_types = parse_result[0][0]
+                if "list" in first_element_types:
+
+                    self.logger.warning("Markdown lists are not supported. Adding element as plain text with number/bullet prefix.")
+
+                    # Get number of whitespaces before the first text
+                    prefix = re.match(r"^(\s*).+", string).group(1)  # get number of whitespaces before the first text
+
+                    # Get list item number / bullet point
+                    info_dict = parse_result[0][1][1]
+                    if info_dict.get("ordered", False):  # ordered list
+                        prefix += f"{info_dict.get('start', 1)}. "
+                    else:  # unordered list
+                        prefix += "• "  # bullet point list
+
+                    parse_result.insert(0, (["paragraph"], (prefix, {})))  # insert prefix as first element (without any formatting)
+
+                elif "thematic_break" in first_element_types:
+                    self.logger.warning(f"Markdown horizontal rules are not supported. Adding literal string: '{string}'")
+                    parse_result = [(["paragraph"], (string, {}))]
+
+                elif "block_code" in first_element_types:
+                    self.logger.warning(f"Markdown code blocks are not supported. Adding literal string: '{string}'")
+                    parse_result = [(["paragraph"], (string, {}))]  # replace code block start/end with literal string
+
+                elif "block_quote" in first_element_types:
+                    self.logger.warning(f"Markdown block quotes are not supported. Adding literal string: '{string}'")
+                    parse_result = [(["paragraph"], (string, {}))]  # replace with literal string
+
+                # Add text to paragraph
+                for types, (text, info) in parse_result:
+                    # self.logger.debug(f"Adding markdown text to paragraph. Types: {types}. Text: {repr(text)}. Additional info: {info}.")
+
+                    # Check if type is supported
+                    for type in types:
+                        if type not in supported_types:
+                            self.logger.warning(f"pptreport does not support markdown type '{type}' found in string: '{string}'. Adding text instead: '{text}'")
+                        elif type == "image":
+                            self.logger.warning(f"Markdown images are not supported by pptreport. Adding alternative text instead: '{text}'")
+
+                    # Add run to paragraph
                     run = p.add_run()
-                    run.text = "\n"  # newline for new paragraph
+                    run.text = text
+
+                    # Adjust formatting
+                    run.font.bold = True if "strong" in types else False
+                    run.font.italic = True if "emphasis" in types else False
+
+                    # Add highlight for inline code
+                    if "codespan" in types:
+                        set_highlight(run, "e0e0e0")  # light grey
+
+                    # Add hyperlink
+                    if "link" in types:
+                        hlink = run.hyperlink
+                        hlink.address = info["link"]
+
+                    # Set font size for heading / normal text
+                    if "heading" in types:
+                        level = info["level"]
+                        try:
+                            header_fontsize = md_heading_sizes[level]
+                        except KeyError:
+                            self.logger.warning(f"Header level {level} is not supported. Using default font size.")
+                            header_fontsize = font_size
+                        set_fontsize(run, header_fontsize)
 
-                elif par["type"] == "heading":
-                    # implement heading (bold, bigger) ? Or add it only as plain txt
-                    pass
-
-                elif par["type"] == "list":
-                    # implement list
-                    pass
-                else:
-                    # will be handled in paragraph > codespan/link/block_code (they have duplicate entries in the tree)
-                    pass
+                    else:
+                        set_fontsize(run, font_size)  # font size for plain text
 
     def fill_text(self, text, is_filename=False):
         """
         Fill the box with text.
 
         Parameters
         ----------
@@ -548,32 +615,27 @@
             True if text contains a filename to be placed above image, False otherwise. Default: False
         """
 
         txt_box = self.slide.shapes.add_textbox(self.left, self.top, self.width, self.height)
         txt_frame = txt_box.text_frame
         txt_frame.word_wrap = True
 
-        # Check if text contains markdown
-        md = self._contains_md(text)
-
-        # Place all text in one paragraph
-        p = txt_frame.paragraphs[0]
-        if md:
-            self._fill_md(p=p, text=text)
-        else:
-            p.text = text
-
         # Try to fit text size to the box
         if self.fontsize is None:
-            self.logger.debug("Estimating fontsize...")
-            size = estimate_fontsize(txt_frame, logger=self.logger)
-            self.logger.debug(f"Found: {size}")
+            self.logger.debug("Estimating fontsize based on text...")
+            size = estimate_fontsize(txt_frame, text, logger=self.logger)
+            self.logger.debug(f"Fontsize set at: {size}")
         else:
             size = self.fontsize
-        format_textframe(txt_frame, size=size)
+
+        # Place all text in one paragraph
+        p = txt_frame.paragraphs[0]  # empty paragraph
+        self._fill_md(p=p, text=text, font_size=size)  # if text does not contain markdown, it will be added as plain text
+        for run in p.runs:
+            set_fontname(run, font_name)  # only format font name (size is set during markdown filling)
 
         # Set alignment of text in textbox
         if is_filename:
             vertical = "lower"
             horizontal = self._get_filename_alignment()
         else:
             vertical, horizontal = self._get_content_alignment()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pptreport-1.0.0/pptreport/cli.py` & `pptreport-1.1.0/pptreport/cli.py`

 * *Files identical despite different names*

### Comparing `pptreport-1.0.0/pptreport/fonts/OFL.txt` & `pptreport-1.1.0/pptreport/fonts/OFL.txt`

 * *Files identical despite different names*

### Comparing `pptreport-1.0.0/pptreport/fonts/OpenSans-Bold.ttf` & `pptreport-1.1.0/pptreport/fonts/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pptreport-1.0.0/pptreport/fonts/OpenSans-Italic.ttf` & `pptreport-1.1.0/pptreport/fonts/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pptreport-1.0.0/pptreport/fonts/OpenSans-Regular.ttf` & `pptreport-1.1.0/pptreport/fonts/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pptreport-1.0.0/pptreport/powerpointreport.py` & `pptreport-1.1.0/pptreport/powerpointreport.py`

 * *Files 2% similar despite different names*

```diff
@@ -476,14 +476,16 @@
             Whether to keep slides where no file pattern content was found (e.g. if missing_file is "text"/"empty"/"skip" but no files were found for content). Options are:
             - "keep" (default): slides are kept even if the content pattern was not found
             - "skip": slides without any content will not be added to the presentation
         dpi : int, default 300
             Dots per inch of the image. Only used when converting pdf to image.
         max_pixels : int, default 1e7
             Maximum number of pixels in an image. If an image has more pixels than this, it will be resized.
+        show_borders : bool, default False
+            Whether to show borders of content boxes. This option is useful for debugging layouts. If True, adds a black border to the content boxes. If False, no borders are added.
         """
 
         self.logger.debug("Started adding slide")
 
         # Get input parameters;
         parameters = {}
         parameters["content"] = content
@@ -551,15 +553,14 @@
                 slide._fill_slide()  # Fill slide with content
 
         # clean tmp files after adding content to slide(s)
         for tmp_file in tmp_files:
             os.remove(tmp_file)
 
         self.logger.debug("Finished adding slide")
-        self.logger.debug("-" * 60)  # separator between slide logging
 
     def _setup_slide(self, parameters):
         """ Initialize an empty slide with a given layout. """
 
         # How many slides are already in the presentation?
         n_slides = len(self._slides)
         self.logger.info("Adding slide {}".format(n_slides + 1))
@@ -843,19 +844,23 @@
         directory = os.path.dirname(pattern_clean)
         while not os.path.exists(directory):
             directory = os.path.dirname(directory)
             if directory == "":
                 break  # reached root directory
 
         # Prepare regex for file search
-        pattern = re.sub(r'(?<!\\)/', r'\\/', pattern)  # Automatically escape / in regex (if not already escaped)
+        pattern_escaped = re.sub(r'(?<!\\)/', r'\\/', pattern)  # Automatically escape / in regex (if not already escaped)
         try:
-            pattern_compiled = re.compile(pattern)
+            pattern_compiled = re.compile(pattern_escaped)
         except re.error:
-            raise ValueError(f"Invalid regex: {pattern}")
+            # Regex is invalid, assume the pattern is not a regex
+            self.logger.warning(f"Pattern is not a valid regex: '{pattern}'. Treating the content as text.")
+            return [pattern]
+        except Exception as e:
+            raise e
 
         # Find all files that match the regex
         search_glob = os.path.join(directory, "**")
         matched_files = []
         for file in glob.iglob(search_glob, recursive=True):
             if pattern_compiled.match(file):
                 matched_files.append(file)
@@ -1043,14 +1048,15 @@
         # Set global slide parameters
         if "global_parameters" in config:
             self.add_global_parameters(config["global_parameters"])
 
         # Fill in slides with information from slide config
         for slide_dict in config["slides"]:
             self.add_slide(**slide_dict)  # add all options from slide config
+            self.logger.debug("-" * 60)  # separator between slide logging
 
     def save(self, filename, pdf=False):
         """
         Save the presentation to a file.
 
         Parameters
         ----------
```

### Comparing `pptreport-1.0.0/pptreport/slide.py` & `pptreport-1.1.0/pptreport/slide.py`

 * *Files identical despite different names*

### Comparing `pptreport-1.0.0/pptreport.egg-info/PKG-INFO` & `pptreport-1.1.0/pptreport.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pptreport
-Version: 1.0.0
-Home-page: https://github.com/msbentsen/pptreport
+Version: 1.1.0
+Home-page: https://github.com/loosolab/pptreport
 Author: Mette Bentsen
 Author-email: mette.bentsen@mpi-bn.mpg.de
 License: MIT
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pptreport-1.0.0/pptreport.egg-info/SOURCES.txt` & `pptreport-1.1.0/pptreport.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 README.md
 pyproject.toml
 setup.cfg
 pptreport/__init__.py
 pptreport/_version.py
 pptreport/box.py
 pptreport/cli.py
+pptreport/config.py
 pptreport/powerpointreport.py
 pptreport/slide.py
 pptreport.egg-info/PKG-INFO
 pptreport.egg-info/SOURCES.txt
 pptreport.egg-info/dependency_links.txt
 pptreport.egg-info/entry_points.txt
 pptreport.egg-info/requires.txt
```

### Comparing `pptreport-1.0.0/setup.cfg` & `pptreport-1.1.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pptreport
 version = attr: pptreport._version.__version__
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/msbentsen/pptreport
+url = https://github.com/loosolab/pptreport
 author = Mette Bentsen
 author_email = mette.bentsen@mpi-bn.mpg.de
 license = MIT
 license_file = LICENSE
 platforms = Linux, Mac OS X, Windows
 classifiers = 
 	Intended Audience :: Science/Research
@@ -18,16 +18,17 @@
 [options]
 packages = pptreport
 python_requires = >=3
 install_requires = 
 	numpy
 	python-pptx>=0.6.18 # due to importerror from collections
 	pymupdf
+	pillow<10  # python-pptx dependency: "DeprecationWarning: getsize is deprecated and will be removed in Pillow 10"
 	natsort
-	mistune # for markdown
+	mistune>=2,<3  # for markdown; limit due to changes in API
 
 [options.package_data]
 pptreport = fonts/*
 
 [options.entry_points]
 console_scripts = 
 	pptreport = pptreport.cli:main
```

### Comparing `pptreport-1.0.0/tests/test_classes.py` & `pptreport-1.1.0/tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `pptreport-1.0.0/tests/test_input.py` & `pptreport-1.1.0/tests/test_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,25 @@
         report.add_slide(invalid_param="invalid")
 
 
 # ------------------------------------------------------------------- #
 @pytest.mark.parametrize("content, valid",
                          [(content_dir + "colored_animals/(.*)_blue.jpg", True),
                           (content_dir + "colored_animals/([*)_blue.jpg", False)])
-def test_regex_input(content, valid):
+def test_regex_input(caplog, content, valid):
     config = {"content": content}
 
     report = PowerPointReport()
+    report.add_slide(**config)
+
     if valid:
-        report.add_slide(**config)
+        assert "WARNING" not in caplog.text  # check that no warning is written
     else:
-        with pytest.raises(ValueError, match="Invalid regex"):
-            report.add_slide(**config)
+        assert "Pattern is not a valid regex:" in caplog.text  # check that warning is written
+        assert report._slides[0]._boxes[0].content == content
 
 
 # ------------------------------------------------------------------- #
 @pytest.mark.parametrize("content, valid",
                          [("A text", True),
                           (content_dir + "cat.jpg", True),
                           ([], True),
```

### Comparing `pptreport-1.0.0/tests/test_slide.py` & `pptreport-1.1.0/tests/test_slide.py`

 * *Files identical despite different names*

