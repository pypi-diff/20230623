# Comparing `tmp/pysvgedit-0.0.2.tar.gz` & `tmp/pysvgedit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysvgedit-0.0.2.tar", last modified: Thu Jun 22 18:11:04 2023, max compression
+gzip compressed data, was "pysvgedit-0.0.3.tar", last modified: Thu Jun 22 22:08:45 2023, max compression
```

## Comparing `pysvgedit-0.0.2.tar` & `pysvgedit-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/
--rw-------   0 joe       (1000) joe       (1000)    35142 2023-06-18 18:53:00.000000 pysvgedit-0.0.2/LICENSE
--rw-------   0 joe       (1000) joe       (1000)     1178 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/PKG-INFO
--rw-------   0 joe       (1000) joe       (1000)      207 2023-06-20 07:23:51.000000 pysvgedit-0.0.2/README.md
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/pysvgedit/
--rw-------   0 joe       (1000) joe       (1000)      975 2023-06-22 13:27:51.000000 pysvgedit-0.0.2/pysvgedit/Exceptions.py
--rw-------   0 joe       (1000) joe       (1000)     4993 2023-06-22 16:21:37.000000 pysvgedit-0.0.2/pysvgedit/SVGAnimation.py
--rw-------   0 joe       (1000) joe       (1000)     1377 2023-06-22 17:42:00.000000 pysvgedit-0.0.2/pysvgedit/SVGCircle.py
--rw-------   0 joe       (1000) joe       (1000)     1005 2023-06-18 08:01:04.000000 pysvgedit-0.0.2/pysvgedit/SVGDefs.py
--rw-------   0 joe       (1000) joe       (1000)     3084 2023-06-18 18:50:45.000000 pysvgedit-0.0.2/pysvgedit/SVGDocument.py
--rw-------   0 joe       (1000) joe       (1000)     1422 2023-06-18 17:58:55.000000 pysvgedit-0.0.2/pysvgedit/SVGGroup.py
--rw-------   0 joe       (1000) joe       (1000)     4372 2023-06-22 17:41:48.000000 pysvgedit-0.0.2/pysvgedit/SVGObject.py
--rw-------   0 joe       (1000) joe       (1000)     2294 2023-06-22 15:54:39.000000 pysvgedit-0.0.2/pysvgedit/SVGPath.py
--rw-------   0 joe       (1000) joe       (1000)     1513 2023-06-22 17:50:27.000000 pysvgedit-0.0.2/pysvgedit/SVGRect.py
--rw-------   0 joe       (1000) joe       (1000)     4340 2023-06-22 17:34:07.000000 pysvgedit-0.0.2/pysvgedit/SVGStyle.py
--rw-------   0 joe       (1000) joe       (1000)     2574 2023-06-22 17:30:05.000000 pysvgedit-0.0.2/pysvgedit/SVGText.py
--rw-------   0 joe       (1000) joe       (1000)     1700 2023-06-22 15:55:00.000000 pysvgedit-0.0.2/pysvgedit/SVGTransformation.py
--rw-------   0 joe       (1000) joe       (1000)     2466 2023-06-22 15:53:47.000000 pysvgedit-0.0.2/pysvgedit/SVGValidator.py
--rw-------   0 joe       (1000) joe       (1000)     1693 2023-06-22 18:01:49.000000 pysvgedit-0.0.2/pysvgedit/Vector2D.py
--rw-------   0 joe       (1000) joe       (1000)     1967 2023-06-18 18:50:02.000000 pysvgedit-0.0.2/pysvgedit/XMLTools.py
--rw-------   0 joe       (1000) joe       (1000)     1273 2023-06-22 18:10:57.000000 pysvgedit-0.0.2/pysvgedit/__init__.py
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/pysvgedit/apps/
--rw-------   0 joe       (1000) joe       (1000)     3109 2023-06-22 16:15:36.000000 pysvgedit-0.0.2/pysvgedit/apps/AnimationRendererApp.py
--rw-------   0 joe       (1000) joe       (1000)     3101 2023-06-18 08:03:19.000000 pysvgedit-0.0.2/pysvgedit/apps/FriendlyArgumentParser.py
--rw-------   0 joe       (1000) joe       (1000)     4243 2023-06-22 15:58:07.000000 pysvgedit-0.0.2/pysvgedit/apps/MakoRendererApp.py
--rw-------   0 joe       (1000) joe       (1000)     1536 2023-06-22 15:58:00.000000 pysvgedit-0.0.2/pysvgedit/apps/ValidatorApp.py
--rw-------   0 joe       (1000) joe       (1000)      841 2023-06-18 08:03:02.000000 pysvgedit-0.0.2/pysvgedit/apps/__init__.py
-drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/pysvgedit.egg-info/
--rw-------   0 joe       (1000) joe       (1000)     1178 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/pysvgedit.egg-info/PKG-INFO
--rw-------   0 joe       (1000) joe       (1000)      738 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/pysvgedit.egg-info/SOURCES.txt
--rw-------   0 joe       (1000) joe       (1000)        1 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/pysvgedit.egg-info/dependency_links.txt
--rw-------   0 joe       (1000) joe       (1000)      229 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/pysvgedit.egg-info/entry_points.txt
--rw-------   0 joe       (1000) joe       (1000)       10 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/pysvgedit.egg-info/top_level.txt
--rw-------   0 joe       (1000) joe       (1000)       38 2023-06-22 18:11:04.478366 pysvgedit-0.0.2/setup.cfg
--rw-------   0 joe       (1000) joe       (1000)     1438 2023-06-22 18:11:04.000000 pysvgedit-0.0.2/setup.py
+drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/
+-rw-------   0 joe       (1000) joe       (1000)    35142 2023-06-18 18:53:00.000000 pysvgedit-0.0.3/LICENSE
+-rw-------   0 joe       (1000) joe       (1000)     1178 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/PKG-INFO
+-rw-------   0 joe       (1000) joe       (1000)      207 2023-06-20 07:23:51.000000 pysvgedit-0.0.3/README.md
+drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/pysvgedit/
+-rw-------   0 joe       (1000) joe       (1000)      975 2023-06-22 13:27:51.000000 pysvgedit-0.0.3/pysvgedit/Exceptions.py
+-rw-------   0 joe       (1000) joe       (1000)     4993 2023-06-22 16:21:37.000000 pysvgedit-0.0.3/pysvgedit/SVGAnimation.py
+-rw-------   0 joe       (1000) joe       (1000)     1377 2023-06-22 17:42:00.000000 pysvgedit-0.0.3/pysvgedit/SVGCircle.py
+-rw-------   0 joe       (1000) joe       (1000)     1005 2023-06-18 08:01:04.000000 pysvgedit-0.0.3/pysvgedit/SVGDefs.py
+-rw-------   0 joe       (1000) joe       (1000)     3259 2023-06-22 20:08:06.000000 pysvgedit-0.0.3/pysvgedit/SVGDocument.py
+-rw-------   0 joe       (1000) joe       (1000)     1422 2023-06-18 17:58:55.000000 pysvgedit-0.0.3/pysvgedit/SVGGroup.py
+-rw-------   0 joe       (1000) joe       (1000)     4774 2023-06-22 20:09:10.000000 pysvgedit-0.0.3/pysvgedit/SVGObject.py
+-rw-------   0 joe       (1000) joe       (1000)     7539 2023-06-22 21:53:42.000000 pysvgedit-0.0.3/pysvgedit/SVGPath.py
+-rw-------   0 joe       (1000) joe       (1000)     1513 2023-06-22 17:50:27.000000 pysvgedit-0.0.3/pysvgedit/SVGRect.py
+-rw-------   0 joe       (1000) joe       (1000)     4340 2023-06-22 17:34:07.000000 pysvgedit-0.0.3/pysvgedit/SVGStyle.py
+-rw-------   0 joe       (1000) joe       (1000)     3007 2023-06-22 21:05:48.000000 pysvgedit-0.0.3/pysvgedit/SVGText.py
+-rw-------   0 joe       (1000) joe       (1000)     1708 2023-06-22 18:25:55.000000 pysvgedit-0.0.3/pysvgedit/SVGTransformation.py
+-rw-------   0 joe       (1000) joe       (1000)     2466 2023-06-22 15:53:47.000000 pysvgedit-0.0.3/pysvgedit/SVGValidator.py
+-rw-------   0 joe       (1000) joe       (1000)     1693 2023-06-22 18:01:49.000000 pysvgedit-0.0.3/pysvgedit/Vector2D.py
+-rw-------   0 joe       (1000) joe       (1000)     1967 2023-06-18 18:50:02.000000 pysvgedit-0.0.3/pysvgedit/XMLTools.py
+-rw-------   0 joe       (1000) joe       (1000)     1385 2023-06-22 22:08:02.000000 pysvgedit-0.0.3/pysvgedit/__init__.py
+drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/pysvgedit/apps/
+-rw-------   0 joe       (1000) joe       (1000)     3109 2023-06-22 16:15:36.000000 pysvgedit-0.0.3/pysvgedit/apps/AnimationRendererApp.py
+-rw-------   0 joe       (1000) joe       (1000)     3101 2023-06-18 08:03:19.000000 pysvgedit-0.0.3/pysvgedit/apps/FriendlyArgumentParser.py
+-rw-------   0 joe       (1000) joe       (1000)     4243 2023-06-22 15:58:07.000000 pysvgedit-0.0.3/pysvgedit/apps/MakoRendererApp.py
+-rw-------   0 joe       (1000) joe       (1000)     1536 2023-06-22 15:58:00.000000 pysvgedit-0.0.3/pysvgedit/apps/ValidatorApp.py
+-rw-------   0 joe       (1000) joe       (1000)      841 2023-06-18 08:03:02.000000 pysvgedit-0.0.3/pysvgedit/apps/__init__.py
+drwx------   0 joe       (1000) joe       (1000)        0 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/pysvgedit.egg-info/
+-rw-------   0 joe       (1000) joe       (1000)     1178 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/pysvgedit.egg-info/PKG-INFO
+-rw-------   0 joe       (1000) joe       (1000)      738 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/pysvgedit.egg-info/SOURCES.txt
+-rw-------   0 joe       (1000) joe       (1000)        1 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/pysvgedit.egg-info/dependency_links.txt
+-rw-------   0 joe       (1000) joe       (1000)      229 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/pysvgedit.egg-info/entry_points.txt
+-rw-------   0 joe       (1000) joe       (1000)       10 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/pysvgedit.egg-info/top_level.txt
+-rw-------   0 joe       (1000) joe       (1000)       38 2023-06-22 22:08:45.335953 pysvgedit-0.0.3/setup.cfg
+-rw-------   0 joe       (1000) joe       (1000)     1438 2023-06-22 22:08:45.000000 pysvgedit-0.0.3/setup.py
```

### Comparing `pysvgedit-0.0.2/LICENSE` & `pysvgedit-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/PKG-INFO` & `pysvgedit-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysvgedit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Native Python library to create and edit SVG documents
 Home-page: https://github.com/johndoe31415/pysvgedit
-Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.2.tar.gz
+Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.3.tar.gz
 Author: Johannes Bauer
 Author-email: joe@johannes-bauer.com
 License: gpl-3.0
 Keywords: svg
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pysvgedit-0.0.2/pysvgedit/Exceptions.py` & `pysvgedit-0.0.3/pysvgedit/Exceptions.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/SVGAnimation.py` & `pysvgedit-0.0.3/pysvgedit/SVGAnimation.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/SVGCircle.py` & `pysvgedit-0.0.3/pysvgedit/SVGCircle.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/SVGDefs.py` & `pysvgedit-0.0.3/pysvgedit/SVGDefs.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/SVGDocument.py` & `pysvgedit-0.0.3/pysvgedit/SVGDocument.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,20 +14,24 @@
 #	GNU General Public License for more details.
 #
 #	You should have received a copy of the GNU General Public License
 #	along with pysvgedit; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
+import functools
 import xml.dom.minidom
-from .SVGObject import SVGObject
+from .SVGObject import SVGObject, SVGWidthHeightObject
+from .SVGDefs import SVGDefs
 from .XMLTools import XMLTools
 
-class SVGDocument(SVGObject):
+class SVGDocument(SVGObject, SVGWidthHeightObject):
 	_TAG_NAME = "svg"
+	_DEFAULT_WIDTH = 300
+	_DEFAULT_HEIGHT = 150
 	_NAMESPACES = {
 		"inkscape": "http://www.inkscape.org/namespaces/inkscape",
 		"sodipodi": "http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd",
 		"svg": "http://www.w3.org/2000/svg",
 		"rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
 		"cc": "http://creativecommons.org/ns#",
 		"dc": "http://purl.org/dc/elements/1.1/",
@@ -42,51 +46,51 @@
 		ctr = len(self._used_ids) + 1
 		while True:
 			attempt_id = f"id{ctr}"
 			if attempt_id not in self._used_ids:
 				self._used_ids.add(attempt_id)
 				return attempt_id
 
-	@property
-	def width(self):
-		return float(self._default_get_attribute("width", 300))
-
-	@width.setter
-	def width(self, value):
-		self.node.setAttribute("width", str(value))
-
-	@property
-	def height(self):
-		return float(self._default_get_attribute("height", 150))
-
-	@height.setter
-	def height(self, value):
-		self.node.setAttribute("height", str(value))
+	@functools.cached_property
+	def defs(self):
+		try:
+			return self.get_first("defs")
+		except StopIteration:
+			return self.add(SVGDefs.new())
 
 	@classmethod
 	def new(cls):
 		doc = xml.dom.minidom.Document()
 		root = doc.createElement("svg")
 		root.setAttribute("xmlns", cls._NAMESPACES["svg"])
 		for (nsname, nsvalue) in cls._NAMESPACES.items():
 			root.setAttribute(f"xmlns:{nsname}", nsvalue)
 		doc.appendChild(root)
 		return cls(svg_node = root)
 
 	@classmethod
+	def frombytes(cls, bytes_data):
+		doc = xml.dom.minidom.parseString(bytes_data)
+		root = XMLTools.find_first_element(doc, "svg")
+		return cls(root)
+
+	@classmethod
 	def read(cls, f):
 		doc = xml.dom.minidom.parse(f)
 		root = XMLTools.find_first_element(doc, "svg")
 		return cls(root)
 
 	@classmethod
 	def readfile(cls, filename):
 		with open(filename, "rb") as f:
 			return cls.read(f)
 
+	def asbytes(self):
+		return self.node.ownerDocument.toxml(encoding = "utf-8")
+
 	def write(self, f):
 		self.node.ownerDocument.writexml(f)
 
 	def writefile(self, filename):
 		with open(filename, "w") as f:
 			self.write(f)
 
@@ -94,8 +98,8 @@
 		constraint = lambda node: node.getAttribute("id") == element_id
 		try:
 			return next(XMLTools.walk_elements(self.node, constraint = constraint))
 		except StopIteration:
 			return None
 
 	def __str__(self):
-		return f"SVGDocument<{self.width:.0f} x {self.height:.0f}>"
+		return f"SVGDocument<{self.extents.x:.0f} x {self.extents.y:.0f}>"
```

### Comparing `pysvgedit-0.0.2/pysvgedit/SVGGroup.py` & `pysvgedit-0.0.3/pysvgedit/SVGGroup.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/SVGObject.py` & `pysvgedit-0.0.3/pysvgedit/SVGObject.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,17 +32,29 @@
 
 	@pos.setter
 	def pos(self, value: Vector2D):
 		self.node.setAttribute(self._X_ATTRIBUTE_NAME, str(value.x))
 		self.node.setAttribute(self._Y_ATTRIBUTE_NAME, str(value.y))
 
 class SVGWidthHeightObject():
+	_DEFAULT_WIDTH = 0
+	_DEFAULT_HEIGHT = 0
+
+	def _deunify(self, name, default_value):
+		value = self._default_get_attribute(name)
+		if value is None:
+			return default_value
+		if value.endswith("mm"):
+			return float(value[:-2]) / 25.4 * 96
+		else:
+			return float(value)
+
 	@property
 	def extents(self):
-		return Vector2D(x = self._get_float_attribute("width"), y = self._get_float_attribute("height"))
+		return Vector2D(x = self._deunify("width", self._DEFAULT_WIDTH), y = self._deunify("height", self._DEFAULT_HEIGHT))
 
 	@extents.setter
 	def extents(self, value: Vector2D):
 		self.node.setAttribute("width", str(value.x))
 		self.node.setAttribute("height", str(value.y))
 
 
@@ -96,14 +108,17 @@
 		return XMLTools.new_element(cls.get_tagname())
 
 	def add(self, svg_object):
 		self.node.appendChild(svg_object.node)
 		svg_object.node.ownerDocument = self.node.ownerDocument
 		if svg_object.svgid is None:
 			svg_object.svgid = self.svg_document.get_unused_id()
+		if hasattr(svg_object, "post_add_hook"):
+			svg_object.post_add_hook(self)
+			svg_object.post_add_hook = None
 		return svg_object
 
 	@classmethod
 	def get_tagname(cls):
 		assert(cls._TAG_NAME is not None)
 		return cls._TAG_NAME
```

### Comparing `pysvgedit-0.0.2/pysvgedit/SVGRect.py` & `pysvgedit-0.0.3/pysvgedit/SVGRect.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/SVGStyle.py` & `pysvgedit-0.0.3/pysvgedit/SVGStyle.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/SVGText.py` & `pysvgedit-0.0.3/pysvgedit/SVGText.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #	GNU General Public License for more details.
 #
 #	You should have received a copy of the GNU General Public License
 #	along with pysvgedit; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
+from .SVGRect import SVGRect
 from .SVGObject import SVGObject, SVGXYObject, SVGStyleObject
 from .XMLTools import XMLTools
 
 @SVGObject.register
 class SVGTextSpan(SVGObject, SVGXYObject, SVGStyleObject):
 	_TAG_NAME = "tspan"
 
@@ -58,19 +59,28 @@
 		return f"tspan<{self.text}>"
 
 @SVGObject.register
 class SVGText(SVGObject, SVGStyleObject):
 	_TAG_NAME = "text"
 
 	@classmethod
-	def new(cls, pos = None, text = ""):
+	def new(cls, pos = None, rect_extents = None, text = ""):
 		svg_text = cls(cls._new_element())
 		svg_text.node.setAttribute("xml:space", "preserve")
-		if pos is not None:
+		if (pos is not None) and (rect_extents is None):
+			# Normal text with position
 			svg_text.pos = pos
+		elif (pos is not None) and (rect_extents is not None):
+			# Text within rectangle (as definition)
+			def post_add_hook(parent):
+				rect = parent.svg_document.defs.add(SVGRect.new(pos = pos, extents = rect_extents))
+				rect.style.clear()
+				svg_text.style.shape_inside = rect
+			svg_text.post_add_hook = post_add_hook
+
 		svg_text.style.default_text()
 		svg_text.node.appendChild(SVGTextSpan.new(pos = pos, text = text).node)
 		return svg_text
 
 	@property
 	def tspans(self):
 		return (SVGTextSpan(node) for node in XMLTools.find_all_elements(self.node, "tspan"))
```

### Comparing `pysvgedit-0.0.2/pysvgedit/SVGTransformation.py` & `pysvgedit-0.0.3/pysvgedit/SVGTransformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,17 +36,18 @@
 	_IDENTIFIER = "format_text"
 
 	def __init__(self, svg_object, template_vars):
 		super().__init__(svg_object)
 		self._template_vars = template_vars
 
 	def apply(self):
-		for tspan in self.svg_object.tspans:
+		for tspan in self.svg_object.walk("tspan"):
 			tspan.text = tspan.text.format(**self._template_vars)
 
+
 class ChangeVisibilityTransformation(SVGTransformation):
 	_IDENTIFIER = "visibility"
 
 	def __init__(self, svg_object, visible):
 		super().__init__(svg_object)
 		self._visible = visible
```

### Comparing `pysvgedit-0.0.2/pysvgedit/SVGValidator.py` & `pysvgedit-0.0.3/pysvgedit/SVGValidator.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/Vector2D.py` & `pysvgedit-0.0.3/pysvgedit/Vector2D.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/XMLTools.py` & `pysvgedit-0.0.3/pysvgedit/XMLTools.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/__init__.py` & `pysvgedit-0.0.3/pysvgedit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 #
 #	You should have received a copy of the GNU General Public License
 #	along with pysvgedit; if not, write to the Free Software
 #	Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
 #
 
 from .Vector2D import Vector2D
-from .SVGDocument import SVGDocument
 from .SVGDefs import SVGDefs
+from .SVGDocument import SVGDocument
 from .SVGGroup import SVGGroup
 from .SVGStyle import SVGStyle
-from .SVGText import SVGText
-from .SVGPath import SVGPath
 from .SVGRect import SVGRect
 from .SVGCircle import SVGCircle
+from .SVGText import SVGText
+from .SVGPath import SVGPath
 from .SVGAnimation import SVGAnimation, SVGAnimationMode
-from .SVGValidator import SVGValidator
+from .SVGValidator import SVGValidator, SVGValidatorErrorClass
+from .SVGTransformation import FormatTextTransformation, ChangeVisibilityTransformation
 from .Exceptions import SVGException
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
```

### Comparing `pysvgedit-0.0.2/pysvgedit/apps/AnimationRendererApp.py` & `pysvgedit-0.0.3/pysvgedit/apps/AnimationRendererApp.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/apps/FriendlyArgumentParser.py` & `pysvgedit-0.0.3/pysvgedit/apps/FriendlyArgumentParser.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/apps/MakoRendererApp.py` & `pysvgedit-0.0.3/pysvgedit/apps/MakoRendererApp.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/apps/ValidatorApp.py` & `pysvgedit-0.0.3/pysvgedit/apps/ValidatorApp.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit/apps/__init__.py` & `pysvgedit-0.0.3/pysvgedit/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/pysvgedit.egg-info/PKG-INFO` & `pysvgedit-0.0.3/pysvgedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysvgedit
-Version: 0.0.2
+Version: 0.0.3
 Summary: Native Python library to create and edit SVG documents
 Home-page: https://github.com/johndoe31415/pysvgedit
-Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.2.tar.gz
+Download-URL: https://github.com/johndoe31415/pysvgedit/archive/v0.0.3.tar.gz
 Author: Johannes Bauer
 Author-email: joe@johannes-bauer.com
 License: gpl-3.0
 Keywords: svg
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pysvgedit-0.0.2/pysvgedit.egg-info/SOURCES.txt` & `pysvgedit-0.0.3/pysvgedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysvgedit-0.0.2/setup.py` & `pysvgedit-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 with open("README.md") as f:
 	long_description = f.read()
 
 setuptools.setup(
 	name = "pysvgedit",
 	packages = setuptools.find_packages(),
-	version = "0.0.2",
+	version = "0.0.3",
 	license = "gpl-3.0",
 	description = "Native Python library to create and edit SVG documents",
 	long_description = long_description,
 	long_description_content_type = "text/markdown",
 	author = "Johannes Bauer",
 	author_email = "joe@johannes-bauer.com",
 	url = "https://github.com/johndoe31415/pysvgedit",
-	download_url = "https://github.com/johndoe31415/pysvgedit/archive/v0.0.2.tar.gz",
+	download_url = "https://github.com/johndoe31415/pysvgedit/archive/v0.0.3.tar.gz",
 	keywords = [ "svg" ],
 	install_requires = [
 	],
 	entry_points = {
 		"console_scripts": [
 			"svgmakorender = pysvgedit.apps.MakoRendererApp:MakoRendererApp.main",
 			"svganimationrender = pysvgedit.apps.AnimationRendererApp:AnimationRendererApp.main",
```

