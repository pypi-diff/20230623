# Comparing `tmp/processpiper-0.4.0.tar.gz` & `tmp/processpiper-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processpiper-0.4.0.tar", last modified: Tue May 16 08:20:34 2023, max compression
+gzip compressed data, was "processpiper-0.4.1.tar", last modified: Fri Jun 23 09:11:15 2023, max compression
```

## Comparing `processpiper-0.4.0.tar` & `processpiper-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 08:20:34.402413 processpiper-0.4.0/
--rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     6817 2023-05-16 08:20:34.402413 processpiper-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     6262 2023-05-16 08:18:24.000000 processpiper-0.4.0/README.md
--rw-rw-rw-   0        0        0     1014 2023-04-09 04:12:22.000000 processpiper-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 08:20:34.402413 processpiper-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 08:20:34.350463 processpiper-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 08:20:34.381407 processpiper-0.4.0/src/processpiper/
--rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.4.0/src/processpiper/__init__.py
--rw-rw-rw-   0        0        0     2386 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/activity.py
--rw-rw-rw-   0        0        0    11673 2023-05-16 08:03:51.000000 processpiper-0.4.0/src/processpiper/colourtheme.py
--rw-rw-rw-   0        0        0     1753 2023-04-21 08:48:40.000000 processpiper-0.4.0/src/processpiper/constants.py
--rw-rw-rw-   0        0        0    12143 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/event.py
--rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.4.0/src/processpiper/footer.py
--rw-rw-rw-   0        0        0     4359 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/gateway.py
--rw-rw-rw-   0        0        0     1658 2023-04-10 03:27:48.000000 processpiper-0.4.0/src/processpiper/helper.py
--rw-rw-rw-   0        0        0    11631 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/lane.py
--rw-rw-rw-   0        0        0    39008 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/painter.py
--rw-rw-rw-   0        0        0     5518 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/pool.py
--rw-rw-rw-   0        0        0    26293 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/processmap.py
--rw-rw-rw-   0        0        0    19377 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/shape.py
--rw-rw-rw-   0        0        0    10307 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/text2diagram.py
--rw-rw-rw-   0        0        0     2263 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/title.py
--rw-rw-rw-   0        0        0     1189 2023-05-16 08:14:49.000000 processpiper-0.4.0/src/processpiper/version.py
-drwxrwxrwx   0        0        0        0 2023-05-16 08:20:34.399413 processpiper-0.4.0/src/processpiper.egg-info/
--rw-rw-rw-   0        0        0     6817 2023-05-16 08:20:34.000000 processpiper-0.4.0/src/processpiper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-05-16 08:20:34.000000 processpiper-0.4.0/src/processpiper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 08:20:34.000000 processpiper-0.4.0/src/processpiper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-16 08:20:34.000000 processpiper-0.4.0/src/processpiper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-16 08:20:34.000000 processpiper-0.4.0/src/processpiper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 08:20:34.401413 processpiper-0.4.0/src/tests/
--rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.4.0/src/tests/__init__.py
--rw-rw-rw-   0        0        0     2170 2023-04-17 09:21:44.000000 processpiper-0.4.0/src/tests/github_action_test.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:11:15.102582 processpiper-0.4.1/
+-rw-rw-rw-   0        0        0     1084 2023-01-11 04:26:51.000000 processpiper-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     6885 2023-06-23 09:11:15.101581 processpiper-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6330 2023-06-23 09:06:58.000000 processpiper-0.4.1/README.md
+-rw-rw-rw-   0        0        0     1014 2023-06-23 09:06:58.000000 processpiper-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 09:11:15.102582 processpiper-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 09:11:15.065266 processpiper-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-23 09:11:15.083582 processpiper-0.4.1/src/processpiper/
+-rw-rw-rw-   0        0        0      188 2023-04-09 10:02:01.000000 processpiper-0.4.1/src/processpiper/__init__.py
+-rw-rw-rw-   0        0        0     2372 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/activity.py
+-rw-rw-rw-   0        0        0    11722 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/colourtheme.py
+-rw-rw-rw-   0        0        0     1881 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/constants.py
+-rw-rw-rw-   0        0        0    12129 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/event.py
+-rw-rw-rw-   0        0        0     2339 2023-04-09 09:10:37.000000 processpiper-0.4.1/src/processpiper/footer.py
+-rw-rw-rw-   0        0        0     4359 2023-05-16 08:14:49.000000 processpiper-0.4.1/src/processpiper/gateway.py
+-rw-rw-rw-   0        0        0     2849 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/helper.py
+-rw-rw-rw-   0        0        0     9263 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/lane.py
+-rw-rw-rw-   0        0        0    17162 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/layout.py
+-rw-rw-rw-   0        0        0    45124 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/painter.py
+-rw-rw-rw-   0        0        0     4946 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/pool.py
+-rw-rw-rw-   0        0        0    19547 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/processmap.py
+-rw-rw-rw-   0        0        0    39735 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/shape.py
+-rw-rw-rw-   0        0        0    11494 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/text2diagram.py
+-rw-rw-rw-   0        0        0     2263 2023-05-16 08:14:49.000000 processpiper-0.4.1/src/processpiper/title.py
+-rw-rw-rw-   0        0        0     1189 2023-06-23 09:06:58.000000 processpiper-0.4.1/src/processpiper/version.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:11:15.099580 processpiper-0.4.1/src/processpiper.egg-info/
+-rw-rw-rw-   0        0        0     6885 2023-06-23 09:11:15.000000 processpiper-0.4.1/src/processpiper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      762 2023-06-23 09:11:15.000000 processpiper-0.4.1/src/processpiper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 09:11:15.000000 processpiper-0.4.1/src/processpiper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-23 09:11:15.000000 processpiper-0.4.1/src/processpiper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-23 09:11:15.000000 processpiper-0.4.1/src/processpiper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 09:11:15.100582 processpiper-0.4.1/src/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-09 04:19:21.000000 processpiper-0.4.1/src/tests/__init__.py
+-rw-rw-rw-   0        0        0     2170 2023-04-17 09:21:44.000000 processpiper-0.4.1/src/tests/github_action_test.py
```

### Comparing `processpiper-0.4.0/LICENSE` & `processpiper-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.0/PKG-INFO` & `processpiper-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processpiper
-Version: 0.4.0
+Version: 0.4.1
 Summary: Processpiper. An open source python library to generate business process diagram using code.
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/processpiper
 Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -81,16 +81,16 @@
 * Ubuntu
 * MacOS
 
 ## Documentation
 Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this library.
 
 ## Examples
-### (Method 1) Generate diagram using plain text
-This is a sample code to generate a business process diagram using plain text. 
+### (Method 1) Generate diagram using English like PiperFlow syntax
+This is a sample code to generate a business process diagram using PiperFlow syntax. 
 ```python
 from processpiper.text2diagram import render
 
 input_syntax = """
 title: Sample Test Process
 colourtheme: BLUEMOUNTAIN
     lane: End User
@@ -158,16 +158,16 @@
 The generated diagram is as follows:
 ![Process Map](https://github.com/csgoh/processpiper/blob/main/images/test/test_auto_case1.png)
 
 
 ## Development Status
 Initial first release would only cover the following basic business process elements. Other element types will be introduced in subsequence releases.
 
-* Event: Start, End, Timer, Intermediate
+* Event: Start, End, Timer, Intermediate, Message, Signal, Conditional, Link
 * Activity: Task, Subprocess
-* Gateway: Inclusive, Exclusive, Parallel
+* Gateway: Inclusive, Exclusive, Parallel, Event
 
 Any ideas or suggestions, please send it to me via [GitHub Discussions](https://github.com/csgoh/processmapper/discussions).
```

### Comparing `processpiper-0.4.0/README.md` & `processpiper-0.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -67,16 +67,16 @@
 * Ubuntu
 * MacOS
 
 ## Documentation
 Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this library.
 
 ## Examples
-### (Method 1) Generate diagram using plain text
-This is a sample code to generate a business process diagram using plain text. 
+### (Method 1) Generate diagram using English like PiperFlow syntax
+This is a sample code to generate a business process diagram using PiperFlow syntax. 
 ```python
 from processpiper.text2diagram import render
 
 input_syntax = """
 title: Sample Test Process
 colourtheme: BLUEMOUNTAIN
     lane: End User
@@ -144,16 +144,16 @@
 The generated diagram is as follows:
 ![Process Map](https://github.com/csgoh/processpiper/blob/main/images/test/test_auto_case1.png)
 
 
 ## Development Status
 Initial first release would only cover the following basic business process elements. Other element types will be introduced in subsequence releases.
 
-* Event: Start, End, Timer, Intermediate
+* Event: Start, End, Timer, Intermediate, Message, Signal, Conditional, Link
 * Activity: Task, Subprocess
-* Gateway: Inclusive, Exclusive, Parallel
+* Gateway: Inclusive, Exclusive, Parallel, Event
 
 Any ideas or suggestions, please send it to me via [GitHub Discussions](https://github.com/csgoh/processmapper/discussions).
```

### Comparing `processpiper-0.4.0/pyproject.toml` & `processpiper-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ['Pillow>=9.4.0']
+dependencies = ['Pillow>=9.5.0']
 
 [project.urls]
 "Homepage" = "https://github.com/csgoh/processpiper"
 "Bug Tracker" = "https://github.com/csgoh/processpiper/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"] # list of folders that contain the packages (["."] by default)
```

### Comparing `processpiper-0.4.0/src/processpiper/activity.py` & `processpiper-0.4.1/src/processpiper/activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,22 @@
 from .shape import Box
 from .painter import Painter
 
 
 class Activity(Box):
     """Represents an activity types in a process flow diagram."""
 
-    ...
-
 
 class Task(Activity):
     """A task is a special type of activity that is represented by a box."""
 
-    ...
-
 
 class Subprocess(Activity):
-    """A subprocess is a special type of activity that is represented by a box with a plus sign in it."""
+    """A subprocess is a special type of activity that
+    is represented by a box with a plus sign in it."""
 
     def draw(self, painter: Painter):
         super().draw(painter)
 
         ### Draw a plus sign in a box
         subprocess_width, subprocess_height = painter.get_text_dimension(
             "[+]", painter.element_font, 14
@@ -59,8 +56,9 @@
 class ServiceTask(Activity):
     def draw(self, painter: Painter):
         super().draw(painter)
 
         raise NotImplementedError("ServiceTask is not implemented yet.")
 
 
-### To implement: User Task,Script Task,Business Rule Task, Manual Task, Received Task,Send Task, Receive Task
+### To implement: User Task,Script Task,Business Rule Task,
+# Manual Task, Received Task,Send Task, Receive Task
```

### Comparing `processpiper-0.4.0/src/processpiper/colourtheme.py` & `processpiper-0.4.1/src/processpiper/colourtheme.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,32 +293,33 @@
 
 
 @dataclass
 class ColourTheme:
     """Colour theme for the ProcessPiper."""
 
     def __init__(self, colour_theme_name: str) -> None:
+        # sourcery skip: simplify-boolean-comparison, use-any
         """Initialise the colour theme."""
 
         found = False
         for theme in ColourThemesSettings:
             if theme["theme"] == colour_theme_name:
                 found = True
 
-        if found == False:
+        if found is False:
             raise ValueError(f"Colour theme {colour_theme_name} not recognised.")
 
         self._colour_theme_name = colour_theme_name
 
     def get_colour_theme_settings(self, processmap_component: str) -> tuple:
         """Get the colour theme settings for the specified roadmap component."""
 
         colour_settings = None
 
-        for _, value in enumerate(ColourThemesSettings):
+        for value in ColourThemesSettings:
             if value["theme"] == self._colour_theme_name:
                 colour_settings = value["settings"]
                 break
 
         ### get the colour scheme for the specified roadmap component
         ### values() returns a list of dictionaries, convert it to tuple. e.g. {1, 2} -> (1, 2)
         return tuple(colour_settings[processmap_component].values())
```

### Comparing `processpiper-0.4.0/src/processpiper/constants.py` & `processpiper-0.4.1/src/processpiper/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,14 +35,20 @@
     LANE_TEXT_WIDTH = 50
 
     LANE_SHAPE_TOP_MARGIN = 50
     LANE_SHAPE_BOTTOM_MARGIN = 50
     LANE_SHAPE_LEFT_MARGIN = 50
     LANE_SHAPE_RIGHT_MARGIN = 30
 
-    HSPACE_BETWEEN_SHAPES = 50
+    HSPACE_BETWEEN_SHAPES = 80
     VSPACE_BETWEEN_SHAPES = 100
 
     VSPACE_BETWEEN_POOLS = 10
     VSPACE_BETWEEN_LANES = 2
 
     HSPACE_BETWEEN_POOL_AND_LANE = 2
+
+    BOX_WIDTH = 100
+    BOX_HEIGHT = 60
+    CIRCLE_RADIUS = 20
+    DIAMOND_WIDTH = 40
+    DIAMOND_HEIGHT = DIAMOND_WIDTH
```

### Comparing `processpiper-0.4.0/src/processpiper/event.py` & `processpiper-0.4.1/src/processpiper/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,22 +51,18 @@
         outline_width=3,
     )
 
 
 class Event(Circle):
     """Event class for representing events in a process."""
 
-    ...
-
 
 class Start(Event):
     """Start event class for representing start event in a process."""
 
-    ...
-
 
 class End(Event):
     """End event class for representing end event in a process."""
 
     def draw(self, painter: Painter):
         super().draw(painter)
         draw_stop_circle(painter, self.x, self.y, self.radius)
@@ -164,18 +160,18 @@
         envelope_width = self.radius * 1.2
         envelope_height = self.radius * 0.9
         circle_center = (self.x, self.y)
         envelope_top_left = (
             circle_center[0] - envelope_width // 2,
             circle_center[1] - envelope_height // 2,
         )
-        envelope_bottom_right = (
-            circle_center[0] + envelope_width // 2,
-            circle_center[1] + envelope_height // 2,
-        )
+        # envelope_bottom_right = (
+        #     circle_center[0] + envelope_width // 2,
+        #     circle_center[1] + envelope_height // 2,
+        # )
 
         painter.draw_box_with_outline(
             envelope_top_left[0],
             envelope_top_left[1],
             envelope_width,
             envelope_height,
             box_outline_colour="black",
```

### Comparing `processpiper-0.4.0/src/processpiper/footer.py` & `processpiper-0.4.1/src/processpiper/footer.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.0/src/processpiper/gateway.py` & `processpiper-0.4.1/src/processpiper/gateway.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.0/src/processpiper/helper.py` & `processpiper-0.4.1/src/processpiper/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,29 +15,10 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-import logging
 
-
-class Helper:
-    @staticmethod
-    def printc(message: str, color: str = "30"):
-        """Print text in color"""
-
-        root_logger = logging.getLogger()
-
-        if root_logger.getEffectiveLevel() == logging.DEBUG:
-            print(f"\033[1;{color}m{message}\033[0m")
-
-    @staticmethod
-    def debug_log(message: str):
-        """Log debug message"""
-        logging.debug(message)
-
-    @staticmethod
-    def info_log(message: str):
-        """Log info message"""
-        logging.info(message)
+"""Version information for processpiper."""
+__version__ = "v0.4.1"
```

### Comparing `processpiper-0.4.0/src/processpiper/painter.py` & `processpiper-0.4.1/src/processpiper/painter.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 import sys
 from PIL import Image, ImageDraw, ImageFont, ImageColor, ImageFilter, ImageEnhance
 import textwrap
 from .colourtheme import ColourTheme
 from .helper import Helper
 
 
+class UnsupportedOSException(Exception):
+    pass
+
+
 class Painter:
     """Painter class to draw the diagram"""
 
     width: int
     height: int
     output_type: str
 
@@ -141,32 +145,31 @@
         if sys.platform.startswith("win"):  # Windows
             return os.path.join("C:\\", "Windows", "Fonts", f"{font_name}.ttf")
         elif sys.platform.startswith("darwin"):  # macOS
             return os.path.join(
                 "/", "System", "Library", "Fonts", "Supplemental", f"{font_name}.ttf"
             )
         elif sys.platform.startswith("linux"):  # Linux
-            font_dir = f"/usr/share/fonts/truetype/msttcorefonts"
+            font_dir = "/usr/share/fonts/truetype/msttcorefonts"
 
             if os.path.exists(os.path.join(font_dir, f"{font_name}.ttf")):
                 return os.path.join(font_dir, f"{font_name}.ttf")
-            else:
-                ### This is cater for cases where msttcorefonts is not installed
-                linux_font_name = "DejaVuSans"  # Default font for Linux
-                return os.path.join(
-                    "/",
-                    "usr",
-                    "share",
-                    "fonts",
-                    "truetype",
-                    "dejavu",  # Use the DejaVu font directory instead of msttcorefonts
-                    f"{linux_font_name}.ttf",
-                )
+            ### This is cater for cases where msttcorefonts is not installed
+            linux_font_name = "DejaVuSans"  # Default font for Linux
+            return os.path.join(
+                "/",
+                "usr",
+                "share",
+                "fonts",
+                "truetype",
+                "dejavu",  # Use the DejaVu font directory instead of msttcorefonts
+                f"{linux_font_name}.ttf",
+            )
         else:
-            raise Exception("Unsupported operating system")
+            raise UnsupportedOSException("Unsupported operating system")
 
     def draw_grid(self):
         """Draw a grid of dots to help with alignment"""
         ### Set the dot size and spacing
         spacing = 10
 
         ### Draw the grid of dots
@@ -251,15 +254,15 @@
             x (int): X coordinate
             y (int): Y coordinate
             width (int): Rectangle width
             height (int): Rectangle height
             box_fill_colour (str: HTML colour name or hex code. Eg. #FFFFFF or LightGreen)
         """
         arrowhead_width = 10
-        width = width - arrowhead_width
+        width -= arrowhead_width
         shape = [(x, y), (x + width, y + height)]
 
         ### Draw the rectangle
         self.__cr.rectangle(shape, fill=box_fill_colour)
 
         ### Set the coordinates of the arrowhead
         vertical_midpoint = (height / 2) + y
@@ -378,15 +381,15 @@
 
         multi_lines = []
         wrap_lines = []
 
         ### Make '\n' work
         multi_lines = text.splitlines()
 
-        left, _, right, bottom = font.getbbox("a")
+        left, _, right, _ = font.getbbox("a")
         single_char_width = right - left
 
         ### wrap text
         for line in multi_lines:
             wrap_lines.extend(textwrap.wrap(line, int(box_height / single_char_width)))
 
         box_x1, box_y1, box_x2, box_y2 = (
@@ -489,15 +492,15 @@
         radius: float,
         outline_colour: str,
         outline_width: int = 1,
         fill_colour: str = "",
     ) -> None:
         """Draw a circle"""
         outline_red, outline_green, outline_blue = ImageColor.getrgb(outline_colour)
-        if fill_colour == "":
+        if not fill_colour:
             ### If no fill colour is specified, use the outline colour as the fill colour.
             fill_red, fill_green, fill_blue = outline_red, outline_green, outline_blue
             self.__cr.ellipse(
                 (x - radius, y - radius, x + radius, y + radius),
                 fill=(fill_red, fill_green, fill_blue),
                 outline=(outline_red, outline_green, outline_blue),
                 width=outline_width,
@@ -585,36 +588,30 @@
         self,
         x1: int,
         y1: int,
         x2: int,
         y2: int,
         connector_line_width,
         connector_line_colour,
-    ):
+    ):  # sourcery skip: remove-unnecessary-cast
         """Draw a vertical dashed line"""
         gap_size = 10
         y1 = int(y1)
         y2 = int(y2)
         if y1 > y2:
             for i in range(y2, y1, gap_size):
-                if i - 5 < y2:
-                    new_y = y2
-                else:
-                    new_y = i - 5
+                new_y = max(i - 5, y2)
                 self.__cr.line(
                     (x1, i, x2, new_y),
                     fill=connector_line_colour,
                     width=connector_line_width,
                 )
         else:
             for i in range(y1, y2, gap_size):
-                if i + 5 > y2:
-                    new_y = y2
-                else:
-                    new_y = i + 5
+                new_y = min(i + 5, y2)
                 self.__cr.line(
                     (x1, i, x2, new_y),
                     fill=connector_line_colour,
                     width=connector_line_width,
                 )
 
     def draw_horizontal_dashed_line(
@@ -631,45 +628,32 @@
         x1 = int(x1)
         x2 = int(x2)
 
         if x1 > x2:
             x1 += 10
             for i in range(x2, x1, gap_size):
                 # print(f">> {i}, {y1}, {x2}, {y2}")
-                if i - 5 < x2:
-                    new_x = x2
-                else:
-                    new_x = i - 5
+                new_x = max(i - 5, x2)
                 # print(f"x1 > x2    {i}, {y1}, {new_x}, {y2}")
                 self.__cr.line((i, y1, new_x, y2), fill="black", width=1)
         else:
             for i in range(x1, x2, gap_size):
-                if i + 5 > x2:
-                    new_x = x2
-                else:
-                    new_x = i + 5
+                new_x = min(i + 5, x2)
                 # print(f"x2 < x1    {i}, {y1}, {new_x}, {y2}")
                 self.__cr.line((i, y1, new_x, y2), fill="black", width=1)
 
         # for i in range(x1, x2, gap_size):
         #     print(f"    {i}, {y1}, {i + 5}, {y2}")
         #     self.__cr.line((i, y1, i + 5, y2), fill="black", width=1)
 
     def draw_right_angle_dot_line(self, x1: int, y1: int, x2: int, y2: int):
-        if x1 < x2:
-            if y1 < y2:
-                right_angle_point = (x2, y1)
-            else:
-                right_angle_point = (x1, y2)
+        if x1 < x2 and y1 < y2 or x1 >= x2 and y1 >= y2:
+            right_angle_point = (x2, y1)
         else:
-            if y1 < y2:
-                right_angle_point = (x1, y2)
-            else:
-                right_angle_point = (x2, y1)
-
+            right_angle_point = (x1, y2)
         self.draw_horizontal_dashed_line(
             x1, y1, right_angle_point[0], right_angle_point[1]
         )
         self.draw_vertical_dashed_line(
             right_angle_point[0], right_angle_point[1], x2, y2
         )
 
@@ -688,177 +672,307 @@
                     x1, y1, x2, y2, connector_line_width, connector_line_colour
                 )
             elif y1 == y2:
                 self.draw_horizontal_dashed_line(
                     x1, y1, x2, y2, connector_line_width, connector_line_colour
                 )
 
+    def get_points(
+        self,
+        nearest_points,
+    ):
+        """Get the points to draw a line between two elements"""
+        x1, y1 = nearest_points["source_points"]
+        x2, y2 = nearest_points["target_points"]
+        face_source = nearest_points["source_name"]
+        face_target = nearest_points["target_name"]
+
+        Helper.printc(
+            f"      GET_POINTS(): {x1=}, {y1=}, {face_source=}, {x2=}, {y2=}, {face_target=}",
+            show_level="draw_connection",
+        )
+        points, _ = self.get_connection_points(x1, y1, face_source, x2, y2, face_target)
+
+        return points
+
     def draw_right_angle_line(
         self,
         x1: int,
         y1: int,
         face_source: str,
         x2: int,
         y2: int,
         face_target: str,
         connection_style: str,
         connector_line_width: int = 0,
         connector_line_colour: str = "",
     ):
         """Draw a right angle line between two points"""
         Helper.printc(
-            f"      x1: {x1}, y1: {y1}, face1: {face_source}, x2: {x2}, y2: {y2}, face2: {face_target}"
+            f"      DRAW_RIGHT_ANGLE_LINE() {x1=}, {y1=}, {face_source=}, {x2=}, {y2=}, {face_target=}",
+            show_level="draw_connection",
         )
+        points, right_angle_points = self.get_connection_points(
+            x1, y1, face_source, x2, y2, face_target
+        )
+
+        if connection_style == "dashed":
+            self.draw_dashed_line(points, connector_line_width, connector_line_colour)
+        else:
+            self.__cr.line(
+                points, fill=(connector_line_colour), width=connector_line_width
+            )
+        return right_angle_points
+
+    def get_connection_points(self, x1, y1, face_source, x2, y2, face_target):
+        """Get the points to draw a line between two elements"""
         if x1 == x2 and y1 == y2:
+            # Shapes are on top of each other / overlapping. NOTE: This should never happen
             Helper.printc(
-                f"   A: right_angle_line: x1 == x2 and y1 == y2: {x1}, {y1}, {x2}, {y2}"
+                f"      A: right_angle_line: x1 == x2 and y1 == y2: {x1}, {y1}, {x2}, {y2}",
+                show_level="draw_connection",
             )
             points = [(x1, y1)]
-            right_angle_point = (x1, y1)
+            right_angle_point = points
 
         if x1 != x2 and y1 == y2:
+            # Shapes are on the same horizontal line
             Helper.printc(
-                f"   B: right_angle_line: x1 != x2 and y1 == y2: {x1}, {y1}, {x2}, {y2}"
+                f"      B: right_angle_line: x1 != x2 and y1 == y2: {x1}, {y1}, {x2}, {y2}",
+                show_level="draw_connection",
             )
-            points = [(x1, y1), (x2, y1)]
-            right_angle_point = (x1, y1)
+            elbow_height = 40
+            if face_source.find("top") != -1:
+                points = [
+                    (x1, y1),
+                    (x1, y1 - elbow_height),
+                    (x2, y2 - elbow_height),
+                    (x2, y2),
+                ]
+                right_angle_point = [(x1, y1 - elbow_height), (x2, y2 - elbow_height)]
+            elif face_source.find("bottom") != -1:
+                points = [(x1, y1), (x1, y1 + elbow_height), (x2, y2 + elbow_height)]
+                right_angle_point = [(x1, y1 + elbow_height)]
+            else:
+                points = [(x1, y1), (x2, y1)]
+                right_angle_point = [(x1, y1)]
 
         if x1 == x2 and y1 != y2:
+            # Shapes are on the same vertical line
             Helper.printc(
-                f"   C: right_angle_line: x1 == x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}"
+                f"      C: right_angle_line: x1 == x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
+                show_level="draw_connection",
             )
             points = [(x1, y1), (x1, y2)]
-            right_angle_point = (x1, y1)
+            right_angle_point = [(x1, y1)]
 
         if x1 != x2 and y1 != y2:
+            # Shapes are on different horizontal and vertical lines
             # check if face1 string contained the word "right"
             if face_source.find("bottom") != -1:
                 Helper.printc(
-                    f"   D-bottom: right_angle_line: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}"
+                    f"      D-bottom: right_angle_line: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
+                    show_level="draw_connection",
                 )
                 # if so, then the line should be drawn from the bottom side of the box
                 points = [(x1, y1), (x1, y2), (x2, y2)]
-                right_angle_point = (x1, y2)
+                right_angle_point = [(x1, y2)]
             elif face_source.find("right") != -1:
                 Helper.printc(
-                    f"   D-right: right_angle_line: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}"
+                    f"      D-right: right_angle_line: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
+                    show_level="draw_connection",
                 )
                 if face_target.find("left") != -1:
                     # points = [(x1, y1), (x1, y2), (x2, y2)]
                     elbow_height = 40
                     points = [
                         (x1, y1),
                         (x1 + elbow_height, y1),
                         (x1 + elbow_height, y2),
                         (x2, y2),
                     ]
-                    right_angle_point = (x1 + elbow_height, y2)
+                    # right_angle_point = (x1 + elbow_height, y2)
+                    right_angle_point = [
+                        (x1 + elbow_height, y1),
+                        (x1 + elbow_height, y2),
+                    ]
+                elif face_target.find("right") != -1:
+                    # points = [(x1, y1), (x2, y1), (x2, y2)]
+                    # right_angle_point = [(x2, y1)]
+                    elbow_height = 40
+                    # points = [(x1, y1), (x2, y1), (x2, y2)]
+                    ### both faces are right
+                    Helper.printc(
+                        "      D-right-right (x1 < x2)", show_level="draw_connection"
+                    )
+                    points = [
+                        (x1, y1),
+                        (x2 + elbow_height, y1),
+                        (x2 + elbow_height, y2),
+                        (x2, y2),
+                    ]
+                    right_angle_point = [
+                        (x2 + elbow_height, y1),
+                        (x2 + elbow_height, y2),
+                    ]
+                elif face_target.find("top") != -1:
+                    if y1 < y2:
+                        Helper.printc(
+                            "      D-right-top (y1 < y2)", show_level="draw_connection"
+                        )
+                        points = [
+                            (x1, y1),
+                            (x2, y1),
+                            (x2, y2),
+                        ]
+                        right_angle_point = [
+                            (x2, y1),
+                        ]
+                    else:
+                        Helper.printc(
+                            "      D-right-top (y1 >= y2)",
+                            show_level="draw_connection",
+                        )
+                        vertical_elbow_height = 40
+                        horizontal_elbow_height = 60
+                        points = [
+                            (x1, y1),
+                            (x2 + horizontal_elbow_height, y1),
+                            (x2 + horizontal_elbow_height, y2 - vertical_elbow_height),
+                            (x2, y2 - vertical_elbow_height),
+                            (x2, y2),
+                        ]
+                        right_angle_point = [
+                            (x2 + horizontal_elbow_height, y1),
+                            (x2 + horizontal_elbow_height, y2 - vertical_elbow_height),
+                            (x2, y2 - vertical_elbow_height),
+                        ]
                 else:
-                    points = [(x1, y1), (x2, y1), (x2, y2)]
-                    right_angle_point = (x2, y1)
+                    Helper.printc("      D-right-bottom", show_level="draw_connection")
+                    points = [
+                        (x1, y1),
+                        (x2, y1),
+                        (x2, y2),
+                    ]
+                    right_angle_point = [
+                        (x2, y1),
+                    ]
             elif face_source.find("top") != -1 and face_target.find("top") != -1:
                 Helper.printc(
-                    f"   D-top: right_angle_line: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}"
+                    f"      D-top: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
+                    show_level="draw_connection",
                 )
                 # draw 1 right angle line
                 elbow_height = 40
                 points = [
                     (x1, y1),
                     (x1, y1 - elbow_height),
                     (x2, y1 - elbow_height),
                     (x2, y2),
                 ]
-                right_angle_point = (x2, y2 - elbow_height)
+                # right_angle_point = (x2, y2 - elbow_height)
+                right_angle_point = [(x1, y1 - elbow_height), (x2, y1 - elbow_height)]
             elif face_source.find("top") != -1 and face_target.find("bottom") != -1:
                 Helper.printc(
-                    f"   D-top/bottom: right_angle_line: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}"
+                    f"      D-top/bottom: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
+                    show_level="draw_connection",
                 )
                 # draw 1 right angle line
                 elbow_height = 20
                 points = [
                     (x1, y1),
                     (x1, y1 - elbow_height),
                     (x2, y1 - elbow_height),
                     (x2, y2),
                 ]
-                right_angle_point = (x2, y1 - elbow_height)
+                # right_angle_point = (x2, y1 - elbow_height)
+                right_angle_point = [(x1, y1 - elbow_height), (x2, y1 - elbow_height)]
             else:
                 Helper.printc(
-                    f"   D-else: right_angle_line: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}"
+                    f"      D-else: x1 != x2 and y1 != y2: {x1}, {y1}, {x2}, {y2}",
+                    show_level="draw_connection",
                 )
                 # if so, then the line should be drawn from the bottom side of the box
                 points = [(x1, y1), (x1, y2), (x2, y2)]
-                right_angle_point = (x1, y2)
-            # for point in points:
-            #     self.draw_circle(point[0], point[1], 4, "yellow")
+                right_angle_point = [(x1, y2)]
+                # for point in points:
+                #     self.draw_circle(point[0], point[1], 4, "yellow")
 
         if x1 > x2:
             if y1 <= y2:
                 if abs(y1 - y2) == 10:
                     Helper.printc(
-                        f"   E: right_angle_line: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}"
+                        f"      E: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}",
+                        show_level="draw_connection",
                     )
                     elbow_height = 40
                     points = [
                         (x1, y1),
                         (x1, y1 - elbow_height),
                         (x2, y1 - elbow_height),
                         (x2, y2),
                     ]
-                    right_angle_point = (x2, y1 - elbow_height)
+                    # right_angle_point = (x2, y1 - elbow_height)
+                    right_angle_point = [
+                        (x1, y1 - elbow_height),
+                        (x2, y1 - elbow_height),
+                    ]
                 if abs(y1 - y2) >= 100:
+                    elbow_height = 40
                     if (
-                        face_source.find("bottom") != -1
-                        and face_target.find("right") != -1
+                        face_source.find("bottom") == -1
+                        or face_target.find("right") == -1
                     ):
                         Helper.printc(
-                            f"   F1: right_angle_line: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}"
+                            f"      F2: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}",
+                            show_level="draw_connection",
                         )
-                        elbow_height = 40
                         points = [
                             (x1, y1),
-                            (x1, y2),
+                            (x1, y1 + elbow_height),
+                            (x2, y1 + elbow_height),
                             (x2, y2),
                         ]
-                        right_angle_point = (x1, y2)
+                        # right_angle_point = (x2, y1 - elbow_height)
+                        right_angle_point = [
+                            (x1, y1 - elbow_height),
+                            (x2, y1 - elbow_height),
+                        ]
                     else:
                         Helper.printc(
-                            f"   F2: right_angle_line: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}"
+                            f"      F1: x1 > x2 and y1 <= y2: {x1}, {y1}, {x2}, {y2}",
+                            show_level="draw_connection",
                         )
-                        elbow_height = 40
                         points = [
                             (x1, y1),
-                            (x1, y1 + elbow_height),
-                            (x2, y1 + elbow_height),
+                            (x1, y2),
                             (x2, y2),
                         ]
-                        right_angle_point = (x2, y1 - elbow_height)
-            elif y1 > y2:
-                if len(points) == 0:
-                    Helper.printc(
-                        f"   G: right_angle_line: x1 > x2 and y1 > y2: {x1}, {y1}, {x2}, {y2}"
-                    )
-                    elbow_height = (y1 - y2) / 2
-                    points = [
-                        (x1, y1),
-                        (x1, y1 - elbow_height),
-                        (x2, y2 + elbow_height),
-                        (x2, y2),
-                    ]
-                    # for point in points:
-                    #     self.draw_circle(point[0], point[1], 2, "green")
-                    right_angle_point = (x2, y2 + elbow_height)
+                        right_angle_point = [(x1, y2)]
+            elif len(points) == 0:
+                Helper.printc(
+                    f"      G: x1 > x2 and y1 > y2: {x1=}, {y1=}, {x2=}, {y2=}",
+                    show_level="draw_connection",
+                )
+                elbow_height = (y1 - y2) / 2
+                points = [
+                    (x1, y1),
+                    (x1, y1 - elbow_height),
+                    (x2, y2 + elbow_height),
+                    (x2, y2),
+                ]
+                # for point in points:
+                #     self.draw_circle(point[0], point[1], 2, "green")
+                # right_angle_point = (x2, y2 + elbow_height)
+                right_angle_point = [
+                    (x1, y1 - elbow_height),
+                    (x2, y1 - elbow_height),
+                ]
 
-        if connection_style == "dashed":
-            self.draw_dashed_line(points, connector_line_width, connector_line_colour)
-        else:
-            self.__cr.line(
-                points, fill=(connector_line_colour), width=connector_line_width
-            )
-        return right_angle_point
+        return points, right_angle_point
 
     def draw_line_and_arrow(
         self,
         x1: int,
         y1: int,
         face1: str,
         x2: int,
@@ -872,36 +986,74 @@
         connector_line_width: int = 0,
         connector_line_colour: str = "",
         connector_arrow_colour: str = "",
         connector_arrow_size: int = 0,
     ):
         """Draw a line and arrow between two boxes"""
 
-        right_angle_point = self.draw_right_angle_line(
+        right_angle_points = self.draw_right_angle_line(
             x1,
             y1,
             face1,
             x2,
             y2,
             face2,
             connection_style,
             connector_line_width,
             connector_line_colour,
         )
 
-        label_x_pos, label_y_pos = right_angle_point
+        # if len(right_angle_points) >= 3:
+        #     label_x_pos, label_y_pos = right_angle_points[1]
+        #     arrow_angle_points = right_angle_points[2]
+        # elif len(right_angle_points) == 2:
+        #     label_x_pos, label_y_pos = right_angle_points[0]
+        #     arrow_angle_points = right_angle_points[1]
+        # else:
+        #     label_x_pos, label_y_pos = right_angle_points[0]
+        #     arrow_angle_points = right_angle_points[0]
+
+        label_x_pos, label_y_pos = right_angle_points[-1]
+        arrow_angle_points = right_angle_points[-1]
 
         label_w, label_h = self.get_multitext_dimension(label, connector_font, 12)
         if label_x_pos == x1 and label_y_pos == y1:
             ### There is no right angle point
             label_x_pos = max(x1 + 5, x1 + (((x2 - x1) - label_w) / 2))
-            label_y_pos = y1 - label_h - 3
+            if y1 == y2:
+                label_y_pos = y1 - label_h - 3
+            else:
+                label_y_pos = y1 + ((y2 - y1) / 2) - (label_h / 2)
+            Helper.printc(
+                f"        @@@ {label=} No right angle point",
+                35,
+                show_level="draw_connection",
+            )
+
         else:
             label_x_pos += 5
-            label_y_pos = label_y_pos - label_h - 3
+            if y1 == y2 or (abs(y1 - y2) <= 10):
+                Helper.printc(
+                    f"        @@@ {label=} {y1} == {y2}",
+                    35,
+                    show_level="draw_connection",
+                )
+                label_y_pos = label_y_pos + label_h
+            else:
+                Helper.printc(
+                    f"        @@@ {label=} {y1} != {y2}",
+                    35,
+                    show_level="draw_connection",
+                )
+                label_y_pos = y1 + ((y2 - y1) / 2) - (label_h / 2)
+            Helper.printc(
+                f"        @@@ {label=} With right angle point",
+                35,
+                show_level="draw_connection",
+            )
 
         self.draw_text(
             label_x_pos,
             label_y_pos,
             label,
             connector_font,
             connector_font_size,
@@ -917,26 +1069,26 @@
                 outline_colour=connector_arrow_colour,
                 fill_colour="white",
             )
 
             ### Draw white arrow head at the end of the line
 
             self.draw_arrow_head(
-                right_angle_point[0],
-                right_angle_point[1],
+                arrow_angle_points[0],
+                arrow_angle_points[1],
                 x2,
                 y2,
                 connector_arrow_colour,
                 connector_arrow_size,
                 "white",
             )
         else:
             self.draw_arrow_head(
-                right_angle_point[0],
-                right_angle_point[1],
+                arrow_angle_points[0],
+                arrow_angle_points[1],
                 x2,
                 y2,
                 connector_arrow_colour,
                 connector_arrow_size,
             )
 
     def draw_arrow_head(
@@ -972,19 +1124,18 @@
         left_x = x2 - length * normalised_dx + height * perpendicular_vector_x
         left_y = y2 - length * normalised_dy + height * perpendicular_vector_y
 
         right_x = x2 - length * normalised_dx - height * perpendicular_vector_x
         right_y = y2 - length * normalised_dy - height * perpendicular_vector_y
 
         shape = [(x2, y2), (left_x, left_y), (right_x, right_y), (x2, y2)]
-        if connector_arrow_fill_colour == "":
-            outline_colour = connector_arrow_outline_colour
+        outline_colour = connector_arrow_outline_colour
+        if not connector_arrow_fill_colour:
             fill_colour = outline_colour
         else:
-            outline_colour = connector_arrow_outline_colour
             fill_colour = connector_arrow_fill_colour
         # self.__cr.polygon(shape, fill=connector_arrow_colour)
         self.__cr.polygon(shape, fill=fill_colour, outline=outline_colour, width=2)
 
     def draw_text(
         self, x: int, y: int, text: str, font: str, font_size: int, font_colour: str
     ) -> None:
@@ -1055,15 +1206,15 @@
             wrap_lines.extend(textwrap.wrap(line, 70))
 
         pad = 4
         line_count = len(wrap_lines)
 
         max_width = 0
         max_height = 0
-        for i, line in enumerate(wrap_lines):
+        for line in wrap_lines:
             font_width, font_height = self.get_text_dimension(
                 line, text_font, text_font_size
             )
             max_width = max(max_width, font_width)
             max_height += font_height + pad
 
         return max_width, max_height
@@ -1074,37 +1225,23 @@
         Args:
             width (int): Surface width
             height (int): Surface height
         """
         left, top, right, bottom = 0, 0, width, height
 
         self.__surface = self.__surface.crop((left, top, right, bottom))
+        
 
     def save_surface(self, filename: str) -> None:
         """Save surface to PNG file
 
         Args:
             filename (str): PNG file name
         """
-        if self.output_type == "PNG":
-            if self.__surface is not None:
-                # anti_alias_image = self.__surface.filter(ImageFilter.SMOOTH_MORE)
-                # anti_alias_image.save(filename)
-                # Set the DPI to 300
-                # info = self.__surface.info.copy()
-                # info["dpi"] = (600, 600)
-
-                # Save the image with the new DPI
-                # self.__surface.save(filename, **info)
-
-                length_x, width_y = self.__surface.size
-                factor = min(1, float(1024.0 / length_x))
-
-                factor = 1
-                size = int(factor * length_x), int(factor * width_y)
-                image_resize = self.__surface.resize(size, resample=Image.LANCZOS)
-                image_resize.save(filename, dpi=(1200, 1200), optimize=False)
-
-                # enhancer = ImageEnhance.Sharpness(self.__surface)
-                # im_s_1 = enhancer.enhance(3)
-                # im_s_1.save("sharp.png")
-                # self.__surface.save(filename)
+        if self.output_type == "PNG" and self.__surface is not None:
+            length_x, width_y = self.__surface.size
+            factor = min(1, float(1024.0 / length_x))
+
+            factor = 1
+            size = int(factor * length_x), int(factor * width_y)
+            image_resize = self.__surface.resize(size, resample=Image.LANCZOS)
+            image_resize.save(filename, dpi=(1200, 1200), optimize=False)
```

### Comparing `processpiper-0.4.0/src/processpiper/pool.py` & `processpiper-0.4.1/src/processpiper/pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,29 +41,29 @@
     x: int = field(init=False, default=0)
     y: int = field(init=False, default=0)
     width: int = field(init=False, default=0)
     height: int = field(init=False, default=0)
 
     next_shape_x: int = field(init=False, default=0)
 
-    _lanes: list = field(init=False, default_factory=list)
+    lanes: list = field(init=False, default_factory=list)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         ...
 
     def set_draw_position(self, x: int, y: int, painter: Painter) -> tuple:
         """Set the position of the pool and return the position of the next shape to be drawn"""
         self.x = x
         self.y = y
         self.painter = painter
-        last_lane_y = self._lanes[-1].y
-        last_lane_height = self._lanes[-1].height
+        last_lane_y = self.lanes[-1].y
+        last_lane_height = self.lanes[-1].height
 
         self.width, self.height = (
             Configs.POOL_TEXT_WIDTH,
             last_lane_y + last_lane_height - self.y,
         )
         return self.x, self.y, self.width, self.height
 
@@ -105,27 +105,14 @@
             text_alignment (str, optional): _lane text alignement. Defaults to "".
             background_fill_colour (str, optional): land background fill colour. Defaults to "".
 
         Returns:
             Lane: Lane object
         """
 
-        # if font == "":
-        #     font = self.painter.lane_font
-        # if font_size == 0:
-        #     font_size = self.painter.lane_font_size
-        # if font_colour == "":
-        #     font_colour = self.painter.lane_font_colour
-        # if fill_colour == "":
-        #     fill_colour = self.painter.lane_fill_colour
-        # if text_alignment == "":
-        #     text_alignment = self.painter.lane_text_alignment
-        # if background_fill_colour == "":
-        #     background_fill_colour = self.painter.lane_background_fill_colour
-
         font = font or self.painter.lane_font
         font_size = font_size or self.painter.lane_font_size
         font_colour = font_colour or self.painter.lane_font_colour
         fill_colour = fill_colour or self.painter.lane_fill_colour
         text_alignment = text_alignment or self.painter.lane_text_alignment
         background_fill_colour = (
             background_fill_colour or self.painter.lane_background_fill_colour
@@ -138,9 +125,9 @@
             font_size,
             font_colour,
             fill_colour,
             text_alignment,
             background_fill_colour,
             self.painter,
         )
-        self._lanes.append(lane)
+        self.lanes.append(lane)
         return lane
```

### Comparing `processpiper-0.4.0/src/processpiper/processmap.py` & `processpiper-0.4.1/src/processpiper/processmap.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from dataclasses import dataclass, field
+import time
 from .event import *
 from .lane import Lane, ElementType, EventType
 from .pool import Pool
 from .painter import Painter
 from .shape import *
 from .title import Title
 from .footer import Footer
 from .constants import Configs
 from .helper import Helper
-from PIL import Image
-import time
+from .layout import Grid
+
 import logging
-import PIL
 
 
 class UnconnectedElementException(Exception):
     pass
 
 
 class EmptyProcessMapException(Exception):
@@ -44,16 +44,16 @@
 
 
 @dataclass
 class ProcessMap:
     """Process Map Class"""
 
     title: str = field(init=True, default="<Process Map Title>")
-    width: int = field(init=True, default=3200)
-    height: int = field(init=True, default=3200)
+    width: int = field(init=True, default=5000)
+    height: int = field(init=True, default=5000)
     auto_size: bool = field(init=True, default=True)
     colour_theme: str = field(init=True, default="DEFAULT")
 
     _title: Title = field(init=False)
     _footer: Footer = field(init=False, default=None)
     _pools: list = field(init=False, default_factory=list)
 
@@ -62,28 +62,29 @@
     lane_y_pos: int = field(init=False, default=0)
     lane_max_width: int = field(init=False, default=0)
 
     def __post_init__(self):
         """Initialise the Process Map Class"""
         logging.basicConfig(
             # filename="processpiper.log",
-            level=logging.INFO,
+            level=logging.DEBUG,
             format="%(asctime)s [%(levelname)s] : %(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
         )
         self.start_time = time.time()
         self.__painter = Painter(self.width, self.height)
         self.__set_colour_theme(self.colour_theme)
         self.__painter.set_background_colour(self.__painter.background_colour)
         self._title = Title(
             self.title,
             self.__painter.title_font,
             self.__painter.title_font_size,
             self.__painter.title_font_colour,
         )
+        self._layout_grid = Grid()
 
     def add_pool(
         self,
         pool_name: str,
         font: str = "",
         font_size: int = 0,
         font_colour: str = "",
@@ -116,482 +117,344 @@
         font_size: int = 0,
         font_colour: str = "",
         fill_colour: str = "",
         text_alignment: str = "centre",
         background_fill_colour: str = "",
     ) -> Lane:
         """Add a Lane to the Process Map"""
-        # if font == "":
-        #     font = self.__painter.lane_font
-        # if font_size == 0:
-        #     font_size = self.__painter.lane_font_size
-        # if font_colour == "":
-        #     font_colour = self.__painter.lane_font_colour
-        # if fill_colour == "":
-        #     fill_colour = self.__painter.lane_fill_colour
-        # if text_alignment == "":
-        #     text_alignment = self.__painter.lane_text_alignment
-        # if background_fill_colour == "":
-        #     background_fill_colour = self.__painter.lane_background_fill_colour
 
         font = font or self.__painter.lane_font
         font_size = font_size or self.__painter.lane_font_size
         font_colour = font_colour or self.__painter.lane_font_colour
         fill_colour = fill_colour or self.__painter.lane_fill_colour
         text_alignment = text_alignment or self.__painter.lane_text_alignment
         background_fill_colour = (
             background_fill_colour or self.__painter.lane_background_fill_colour
         )
 
         pool = self.add_pool("Default Pool")
-        lane = pool.add_lane(
+        return pool.add_lane(
             lane_name,
             font,
             font_size,
             font_colour,
             fill_colour,
             text_alignment,
             background_fill_colour,
         )
-        return lane
 
     def set_footer(
         self,
         footer_name: str,
         font: str = "",
         font_size: int = 0,
         font_colour: str = "",
     ):
         """Set the footer text for the Process Map"""
-        if font == "":
+        if not font:
             font = self.__painter.footer_font
         if font_size == 0:
             font_size = self.__painter.footer_font_size
-        if font_colour == "":
+        if not font_colour:
             font_colour = self.__painter.footer_font_colour
 
         self._footer = Footer(footer_name, font, font_size, font_colour)
 
-    def get_current_x_position(self) -> int:
-        """Get the current x position for the next shape to be added"""
-        if self.next_shape_x == 0:
-            self.next_shape_x = (
-                Configs.SURFACE_LEFT_MARGIN
-                + Configs.POOL_TEXT_WIDTH
-                + Configs.HSPACE_BETWEEN_POOL_AND_LANE
-                + Configs.LANE_TEXT_WIDTH
-                + Configs.LANE_SHAPE_LEFT_MARGIN
-            )
-
-        return self.next_shape_x
-
-    def get_next_x_position(self, previous_shape_width: str) -> int:
-        """Get the next x position for the next shape to be added"""
-        if self.next_shape_x == 0:
-            self.next_shape_x = (
-                Configs.SURFACE_LEFT_MARGIN
-                + Configs.POOL_TEXT_WIDTH
-                + Configs.HSPACE_BETWEEN_POOL_AND_LANE
-                + Configs.LANE_TEXT_WIDTH
-                + Configs.LANE_SHAPE_LEFT_MARGIN
-            )
-            Helper.printc(f"            [0]get_next_x_position: {self.next_shape_x}")
-        else:
-            self.next_shape_x += previous_shape_width + Configs.VSPACE_BETWEEN_SHAPES
-            Helper.printc(f"            [1]get_next_x_position: {self.next_shape_x}")
-        return self.next_shape_x
-
-    def find_start_shape(self) -> Shape:
-        """Find the start shape in the process map"""
-        for pool in self._pools:
-            for lane in pool._lanes:
-                for shape in lane.shapes:
-                    ### If the shape has no connection_from, it is the start shape
-                    Helper.printc(f"{shape.name} - {len(shape.connection_from)}")
-                    if len(shape.connection_from) == 0:
-                        return shape
-        return None
-
-    def get_lane_by_id(self, lane_id: int) -> Lane:
+    def _get_lane_by_id(self, lane_id: int) -> Lane:
         """Get a lane by its id"""
         for pool in self._pools:
-            for lane in pool._lanes:
+            for lane in pool.lanes:
                 if lane.id == lane_id:
                     return lane
         return None
 
-    def get_pool_by_name(self, name: str) -> Pool:
+    def _get_pool_by_name(self, name: str) -> Pool:
         """Get a pool by its name"""
         for pool in self._pools:
             if pool.name == name:
                 return pool
         return None
 
-    def set_shape_x_position(
+    def _set_shape_x_position(
         self,
-        previous_shape: Shape,
-        current_shape: Shape,
-        index: int = 0,
-        x_pos: int = 0,
     ):
-        """Set the x position for the shape"""
-        current_lane = self.get_lane_by_id(current_shape.lane_id)
         Helper.printc(
-            f"set_shape_x_position: {current_lane.name}, {current_shape.name}", "34"
+            "~~~ Setting shapes' x position...", "32", show_level="x_position"
         )
-        if index == 0:
-            if previous_shape is not None:
-                if previous_shape.pool_name == current_shape.pool_name:
-                    if previous_shape.lane_id == current_shape.lane_id:
-                        current_shape.x = self.get_next_x_position(previous_shape.width)
-                        Helper.printc(f"          same pool same lane")
+        for lane_id, lane in self._layout_grid.get_grid_items():
+            Helper.printc(f"{lane_id=}", show_level="x_position")
+            for row_number, col in lane.items():
+                Helper.printc(f"{row_number=}", end=":\n", show_level="x_position")
+                for col_idx, item in enumerate(col):
+                    if item is not None:
+                        item.x = (
+                            Configs.SURFACE_LEFT_MARGIN
+                            + Configs.POOL_TEXT_WIDTH
+                            + Configs.HSPACE_BETWEEN_POOL_AND_LANE
+                            + Configs.LANE_TEXT_WIDTH
+                            + Configs.LANE_SHAPE_LEFT_MARGIN
+                        ) + (
+                            col_idx
+                            * (Configs.BOX_WIDTH + Configs.HSPACE_BETWEEN_SHAPES)
+                        )
+                        Helper.printc(
+                            f"    {item.name=}, {col_idx+1=}, {item.x=}",
+                            show_level="x_position",
+                        )
                     else:
-                        current_shape.x = self.get_next_x_position(previous_shape.width)
-                        Helper.printc(f"          same pool diff lane")
-                else:
-                    current_shape.x = self.get_next_x_position(previous_shape.width)
-                    Helper.printc(f"          diff pool")
-            else:
-                current_shape.x = self.get_next_x_position(0)
-                Helper.printc(f"          previous = none")
-        else:
-            ### If previous shape is connecting to multiple shapes,
-            ### the x position of the shape is the same as the previous shape
-            current_shape.x = x_pos
-        current_lane.width = max(current_lane.width, current_shape.x + 100)
-        Helper.printc(
-            f"          x={current_shape.x}, y={current_shape.y}, w={current_shape.width}, [{current_lane.name}]"
-        )
-
-        self.lane_max_width = max(self.lane_max_width, current_lane.width)
-        current_shape.x_pos_traversed = True
+                        Helper.printc("    {'None'}", show_level="x_position")
+            Helper.printc("", show_level="x_position")
 
-        preserved_x_pos = 0
-        for index, next_connection in enumerate(current_shape.connection_to):
-            next_shape = next_connection.target
-            if next_shape.x_pos_traversed is True:
-                continue
-            Helper.printc(f"    |{index}| - <{next_shape.name}>")
-            if index == 0:
-                preserved_x_pos = self.set_shape_x_position(
-                    current_shape, next_shape, index, preserved_x_pos
-                )
-            else:
-                self.set_shape_x_position(
-                    current_shape, next_shape, index, preserved_x_pos
-                )
-
-        return current_shape.x
-
-    def set_shape_y_position(self, shape: Shape, index: int = 0):
-        """Set the y position for the shape"""
-        lane = self.get_lane_by_id(shape.lane_id)
+    def _set_shape_y_position(self):
         Helper.printc(
-            f">>>>set_shape_y_position: {lane.name}, {shape.name}, {index}", "34"
+            "~~~ Setting shapes' y position...", "32", show_level="y_position"
         )
-        if index == 0:
-            ### If previous shape is connecting to one shape,
-            ### the y position of the shape is the same as the previous shape
-            Helper.printc(
-                f"    get_current_y_position()-Before: {lane.shape_row_count}", "32"
-            )
-            shape.y = lane.get_current_y_position()
-            Helper.printc(
-                f"    get_current_y_position()-After: {lane.shape_row_count}", "32"
-            )
-        else:
-            ### Otherwise, the y position of the shape is the next y position
+        for lane_id, lane in self._layout_grid.get_grid_items():
+            Helper.printc(f"{lane_id=}", show_level="y_position")
+            this_lane = self._get_lane_by_id(lane_id)
             Helper.printc(
-                f"    get_next_y_position()-Before: {lane.shape_row_count}", "32"
+                f"{this_lane.name=}, {this_lane.x=}, {this_lane.y=}",
+                show_level="y_position",
             )
-            shape.y = lane.get_next_y_position()
-            Helper.printc(
-                f"    get_next_y_position()-After: {lane.shape_row_count}", "32"
-            )
-
-        shape.set_draw_position(self.__painter)
-
-        shape.y_pos_traversed = True
-
-        # for shape in lane.shapes:
-        Helper.printc(f"         {shape.name} looping..", "32")
-        for index, connection in enumerate(shape.connection_to):
-            next_shape = connection.target
-            Helper.printc(
-                f"             {next_shape.name}, {next_shape.y_pos_traversed}", "32"
-            )
-            if next_shape.y_pos_traversed is True:
-                continue
-
-            self.set_shape_y_position(next_shape, index)
+            for row_number, col in lane.items():
+                Helper.printc(f"{row_number=}", end=":\n", show_level="y_position")
+                row_idx = int(row_number.replace("row", "")) - 1
+                for col_idx, item in enumerate(col):
+                    if item is not None:
+                        item.y = (
+                            this_lane.y
+                            + (Configs.LANE_SHAPE_TOP_MARGIN)
+                            + (
+                                row_idx
+                                * (Configs.BOX_HEIGHT + Configs.VSPACE_BETWEEN_SHAPES)
+                            )
+                        )
+
+                        Helper.printc(
+                            f"    {item.name=}, {row_idx=}, {col_idx+1=}, {item.x=}, {item.y=}",
+                            show_level="y_position",
+                        )
+                        item.set_draw_position(self.__painter)
+                    else:
+                        Helper.printc("    {'None'}", show_level="y_position")
+            self.lane_max_width = max(self.lane_max_width, this_lane.width)
+            Helper.printc("", show_level="y_position")
 
-    def set_draw_position(self, painter: Painter) -> tuple:
+    def _set_draw_position(self) -> tuple:
         """Set the draw position for the process map"""
         ### Set process map title
         self._title.set_draw_position(
-            Configs.SURFACE_LEFT_MARGIN, Configs.SURFACE_TOP_MARGIN, painter
+            Configs.SURFACE_LEFT_MARGIN, Configs.SURFACE_TOP_MARGIN, self.__painter
         )
 
-        Helper.printc("*** Setting elements' x position...")
-        start_shape = self.find_start_shape()
-
-        self.set_shape_x_position(None, start_shape, 0, 0)
-
-        Helper.printc(f"*** Setting elements' y position...")
-        self.set_shape_y_position(start_shape)
+        ### Put shapes into grid
+        self._layout_grid.set_grid(self._pools)
+        self._layout_grid.print_grid()
 
-        Helper.printc(f"*** Calculating pool and lane width and height...")
-        x, y = (
+        Helper.printc(
+            "~~~ Calculating pool and lane width and height...", show_level="pool_lane"
+        )
+        x_pos, y_pos = (
             0,
             self._title.y + self._title.height + Configs.VSPACE_BETWEEN_TITLE_AND_POOL,
         )
         for pool in self._pools:
-            for lane in pool._lanes:
-                lane.painter = painter
-                lane.x = (
-                    x
-                    if x > 0
-                    else Configs.SURFACE_LEFT_MARGIN
-                    + Configs.POOL_TEXT_WIDTH
-                    + Configs.HSPACE_BETWEEN_POOL_AND_LANE
-                )
-                lane.y = y if y > 0 else Configs.SURFACE_TOP_MARGIN
-                lane.width = self.lane_max_width
-
-                # lane.shape_row_count = self.check_lane_row_count(lane)
-                Helper.printc(
-                    f"*** {lane.name} shape row count: {lane.shape_row_count}", 35
-                )
-                lane.height = (
-                    (lane.shape_row_count * 60)
-                    + ((lane.shape_row_count - 1) * Configs.VSPACE_BETWEEN_SHAPES)
-                    + Configs.LANE_SHAPE_TOP_MARGIN
-                    + Configs.LANE_SHAPE_BOTTOM_MARGIN
-                )
-                Helper.printc(
-                    f"{lane.name}, height: {lane.height} = ({lane.shape_row_count} * 60) + ({lane.shape_row_count} - 1) * {Configs.VSPACE_BETWEEN_SHAPES} + {Configs.LANE_SHAPE_TOP_MARGIN} + {Configs.LANE_SHAPE_BOTTOM_MARGIN}"
+            for lane in pool.lanes:
+                x_pos, y_pos, _, _ = lane.set_draw_position(
+                    x_pos, y_pos, self._layout_grid
                 )
-                y = lane.y + lane.height + Configs.VSPACE_BETWEEN_LANES
 
-            y += Configs.VSPACE_BETWEEN_POOLS
+            y_pos += Configs.VSPACE_BETWEEN_POOLS
 
-            first_lane_y = pool._lanes[0].y
+            first_lane_y = pool.lanes[0].y
 
-            pool.set_draw_position(Configs.SURFACE_LEFT_MARGIN, first_lane_y, painter)
+            pool.set_draw_position(
+                Configs.SURFACE_LEFT_MARGIN, first_lane_y, self.__painter
+            )
 
-        ### Reset traversed flags
-        self.reset_traversed_flags()
+        ### Set shape x position
+        # start_shape = self._find_start_shape()
+        self._set_shape_x_position()
 
-        ### Set shape y position one more time, so that it aligns with the lane y position
-        self.set_shape_y_position(start_shape)
+        ### Set shape y position
+        self._set_shape_y_position()
 
         ### Set process map footer
-        if self._footer != None:
+        if self._footer is not None:
             self._footer.set_draw_position(
                 Configs.SURFACE_LEFT_MARGIN,
-                y + Configs.VSPACE_BETWEEN_POOL_AND_FOOTER,
-                painter,
+                y_pos + Configs.VSPACE_BETWEEN_POOL_AND_FOOTER,
+                self.__painter,
             )
             self.height = (
                 self._footer.y + self._footer.height + Configs.SURFACE_BOTTOM_MARGIN
             )
         else:
             self.height = (
-                y
+                y_pos
                 + Configs.VSPACE_BETWEEN_POOL_AND_FOOTER
                 + Configs.SURFACE_BOTTOM_MARGIN
             )
 
         self.width = (
             Configs.SURFACE_LEFT_MARGIN
             + Configs.POOL_TEXT_WIDTH
             + self.lane_max_width
             + Configs.SURFACE_LEFT_MARGIN
         )
 
-    def reset_traversed_flags(self):
-        """Reset the traversed flags for all shapes in the process map"""
-        Helper.printc("*** Resetting traversed flags...", "32")
-        for pool in self._pools:
-            for lane in pool._lanes:
-                lane.next_shape_y = 0
-                lane.shape_row_count = 0
-                for shape in lane.shapes:
-                    Helper.printc(f"    {shape.name}", "32")
-                    shape.y_pos_traversed = False
-
-    def get_orphan_elements(self) -> list:
+    def _get_orphan_elements(self) -> list:
         orphan_elements = []
         for pool in self._pools:
-            for lane in pool._lanes:
+            for lane in pool.lanes:
                 for shape in lane.shapes:
                     if (
                         len(shape.connection_to) == 0
                         and len(shape.connection_from) == 0
                     ):
                         orphan_elements.append(shape.name)
 
         return orphan_elements
 
-    def print_connection(self, shape: Shape):
-        Helper.printc(f"*****    {shape.name}", "32")
-        for connection in shape.connection_to:
-            Helper.printc(f"            {connection.target.name}", "32")
-            self.print_connection(connection.target)
-
     def draw(self) -> None:
         """Draw the process map"""
 
+        ### --Validate the process map--
+
         ### Ensure title is defined
-        if (len(self.title) == 0) and (self._title == None):
+        if (len(self.title) == 0) and (self._title is None):
             raise ValueError("The process map must contain a title")
 
         ### Ensure at least a pool is defined
         if len(self._pools) == 0:
             raise EmptyProcessMapException(
                 "The process map must contain at least one pool or lane"
             )
 
         ### Ensure at least one shape is defined
         for pool in self._pools:
-            if len(pool._lanes) > 0:
-                if len(pool._lanes[0].shapes) == 0:
-                    raise EmptyProcessMapException(
-                        "The process map must contain at least one shape"
-                    )
+            if len(pool.lanes) > 0 and len(pool.lanes[0].shapes) == 0:
+                raise EmptyProcessMapException(
+                    "The process map must contain at least one shape"
+                )
 
         ### Ensure connections are defined
-        orphan_elements = self.get_orphan_elements()
+        orphan_elements = self._get_orphan_elements()
         if len(orphan_elements) > 0:
             raise UnconnectedElementException(
                 f"The following element(s) are defined but not connected to other element(s): \n{orphan_elements}"
             )
 
         ### Replace the class type of shapes with the correct class type
-        # self.print_connection(self.find_start_shape())
         for pool in self._pools:
-            for lane in pool._lanes:
+            for lane in pool.lanes:
                 for index, shape in enumerate(lane.shapes):
-                    self.replace_signal_element(lane, index, shape)
-                    self.replace_conditional_element(lane, index, shape)
-                    self.replace_message_element(lane, index, shape)
+                    self._replace_signal_element(lane, index, shape)
+                    self._replace_conditional_element(lane, index, shape)
+                    self._replace_message_element(lane, index, shape)
 
-        # self.print_connection(self.find_start_shape())
-        self.set_draw_position(self.__painter)
+        ### Set the draw position of pools, lanes, shapes and connections
+        self._set_draw_position()
 
+        ### Draw the process map
         self._title.draw()
 
+        all_shapes = self._layout_grid.get_all_shapes()
+
         if self._pools:
             for pool in self._pools:
                 ### Draw the pools first
                 pool.draw()
-                if pool._lanes:
+                if pool.lanes:
                     ### Draw the lanes second
-                    for lane in pool._lanes:
+                    for lane in pool.lanes:
                         lane.draw()
 
             for pool in self._pools:
-                if pool._lanes:
+                if pool.lanes:
                     ### Then draw the shapes in the lanes
-                    for lane in pool._lanes:
+                    for lane in pool.lanes:
+                        Helper.printc(
+                            f"Drawing shape for ({pool.name}, {lane.name})",
+                            34,
+                            show_level="draw",
+                        )
                         lane.draw_shape()
 
                     ### Finally draw the connections between the shapes
-                    for lane in pool._lanes:
-                        lane.draw_connection()
+                    for lane in pool.lanes:
+                        lane.draw_connection(all_shapes)
 
-        if self._footer != None:
+        if self._footer is not None:
             self._footer.draw()
 
-        if self.auto_size == True:
+        if self.auto_size is True:
             self.__painter.set_surface_size(self.width, self.height)
 
-    def replace_message_element(self, lane, index, shape):
+    def _replace_message_element(self, lane, index, shape):
         if type(shape) == Message:
-            Helper.debug_log(f"  matched with Message")
             ### Check if the signal is a start signal. i.e it has no connection from
             if len(shape.connection_to) > 0 and len(shape.connection_from) == 0:
-                Helper.debug_log(f"      start MESSAGE")
-                new_shape = self.replace_element_type(lane, shape, ElementType.MESSAGE)
-
-                lane.shapes[index] = self.replace_connections(shape, new_shape)
+                new_shape = self._replace_element_type(lane, shape, ElementType.MESSAGE)
 
             elif (  ### Check if the signal is an intermediate signal. i.e it has both connection from and to
                 len(shape.connection_to) > 0 and len(shape.connection_from) > 0
             ):
-                Helper.debug_log(f"      MESSAGE_INTERMEDIATE")
-                new_shape = self.replace_element_type(
+                new_shape = self._replace_element_type(
                     lane, shape, ElementType.MESSAGE_INTERMEDIATE
                 )
-                lane.shapes[index] = self.replace_connections(shape, new_shape)
-
             else:  ### Check if the signal is an end signal. i.e it has no connection to
-                Helper.debug_log(f"      MESSAGE_END")
-                new_shape = self.replace_element_type(
+                new_shape = self._replace_element_type(
                     lane, shape, ElementType.MESSAGE_END
                 )
-                lane.shapes[index] = self.replace_connections(shape, new_shape)
 
-    def replace_conditional_element(self, lane, index, shape):
-        if type(shape) == Conditional:
-            Helper.debug_log(f"  matched with Conditional")
-            ### Check if the signal is a start signal. i.e it has no connection from
-            if len(shape.connection_to) > 0 and len(shape.connection_from) == 0:
-                Helper.debug_log(f"      start CONDITIONAL")
-                new_shape = self.replace_element_type(
+            lane.shapes[index] = self._replace_connections(shape, new_shape)
+
+    def _replace_conditional_element(self, lane, index, shape):
+        if type(shape) == Conditional and len(shape.connection_to) > 0:
+            if len(shape.connection_from) == 0:
+                new_shape = self._replace_element_type(
                     lane, shape, ElementType.CONDITIONAL
                 )
 
-                lane.shapes[index] = self.replace_connections(shape, new_shape)
+                lane.shapes[index] = self._replace_connections(shape, new_shape)
 
-            elif (  ### Check if the signal is an intermediate signal. i.e it has both connection from and to
-                len(shape.connection_to) > 0 and len(shape.connection_from) > 0
-            ):
-                Helper.debug_log(f"      intermediate CONDITIONAL_INTERMEDIATE")
-                new_shape = self.replace_element_type(
+            elif len(shape.connection_from) > 0:
+                new_shape = self._replace_element_type(
                     lane, shape, ElementType.CONDITIONAL_INTERMEDIATE
                 )
-                lane.shapes[index] = self.replace_connections(shape, new_shape)
+                lane.shapes[index] = self._replace_connections(shape, new_shape)
 
-    def replace_signal_element(self, lane, index, shape):
+    def _replace_signal_element(self, lane, index, shape):
         if type(shape) == Signal:
-            Helper.debug_log(f"  matched with Signal")
             ### Check if the signal is a start signal. i.e it has no connection from
             if len(shape.connection_to) > 0 and len(shape.connection_from) == 0:
-                Helper.debug_log(f"      start signal")
-                new_shape = self.replace_element_type(lane, shape, ElementType.SIGNAL)
-
-                lane.shapes[index] = self.replace_connections(shape, new_shape)
+                new_shape = self._replace_element_type(lane, shape, ElementType.SIGNAL)
 
             elif (  ### Check if the signal is an intermediate signal. i.e it has both connection from and to
                 len(shape.connection_to) > 0 and len(shape.connection_from) > 0
             ):
-                Helper.debug_log(f"      intermediate signal")
-                new_shape = self.replace_element_type(
+                new_shape = self._replace_element_type(
                     lane, shape, ElementType.SIGNAL_INTERMEDIATE
                 )
-                lane.shapes[index] = self.replace_connections(shape, new_shape)
-
             else:  ### Check if the signal is an end signal. i.e it has no connection to
-                Helper.debug_log(f"      end signal")
-                new_shape = self.replace_element_type(
+                new_shape = self._replace_element_type(
                     lane, shape, ElementType.SIGNAL_END
                 )
-                lane.shapes[index] = self.replace_connections(shape, new_shape)
 
-    def replace_element_type(self, lane, shape, new_shape_type: ElementType):
+            lane.shapes[index] = self._replace_connections(shape, new_shape)
+
+    def _replace_element_type(self, lane, shape, new_shape_type: ElementType):
         event_class = globals()[new_shape_type]
-        new_shape = event_class(
+        return event_class(
             shape.name,
             lane.name,
         )
 
-        return new_shape
-
-    def replace_connections(self, current_shape, new_shape):
+    def _replace_connections(self, current_shape, new_shape):
         new_shape.lane_id = current_shape.lane_id
         new_shape.pool_name = current_shape.pool_name
         new_shape.font = current_shape.font
         new_shape.font_size = current_shape.font_size
         new_shape.font_colour = current_shape.font_colour
         new_shape.fill_colour = current_shape.fill_colour
         new_shape.text_alignment = current_shape.text_alignment
@@ -599,24 +462,22 @@
         for connection_index, connection in enumerate(current_shape.connection_to):
             new_connection = Connection(
                 new_shape,
                 connection.target,
                 connection.label,
                 connection.connection_type,
             )
-            Helper.printc(
-                f"      creating new connection: {new_connection.source.name}"
-            )
+
             new_shape.connection_to[connection_index] = new_connection
-        self.replace_connection_from(current_shape, new_shape)
+        self._replace_connection_from(current_shape, new_shape)
         return new_shape
 
-    def replace_connection_from(self, current_shape, new_shape):
+    def _replace_connection_from(self, current_shape, new_shape):
         for shape_index, shape in enumerate(current_shape.connection_from):
-            for connection_index, connection_to in enumerate(shape.connection_to):
+            for connection_to in shape.connection_to:
                 new_connection = Connection(
                     connection_to.source,
                     new_shape,
                     connection_to.label,
                     connection_to.connection_type,
                 )
                 shape.connection_to[shape_index] = new_connection
@@ -628,19 +489,14 @@
     def save(self, filename: str) -> None:
         """This method saves the process map to a file"""
         self.__painter.save_surface(filename)
 
         elapsed_time = (time.time() - self.start_time) * 1000
         Helper.info_log(f"Took [{elapsed_time:.2f}ms] to generate '{filename}' diagram")
 
-    def getImage(self) -> PIL.Image:
-        """This method returns the process map image"""
-        image = self.__painter.__surface
-        return image
-
     def __enter__(self):
         """This method is called when the 'with' statement is used"""
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         """This method is called when the 'with' statement is used"""
         pass
```

### Comparing `processpiper-0.4.0/src/processpiper/text2diagram.py` & `processpiper-0.4.1/src/processpiper/text2diagram.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime
 import re
 import os
-from processpiper.helper import Helper
 from PIL import Image
 
 
 def parse_and_generate_code(input_str, png_output_file):
     """
     Parse input string and generate code to create a diagram
     """
@@ -14,29 +13,43 @@
     lines = [
         line.strip()
         for line in input_str.strip().split("\n")
         if not line.startswith("#") and line.strip()
     ]
 
     process_map_title = parse_title(lines)
+    process_map_width = int(parse_width(lines))
 
-    if len(lines) == 0:
+    if not lines:
         raise ValueError(
             "No business process definition found. Please add pool(s), lane(s) and element(s)."
         )
 
     colour_theme = parse_colour_theme(lines)
 
+    colour_theme_code = f', colour_theme="{colour_theme}"'
+    process_map_width_code = f", width={process_map_width}"
     code_lines = [
         "from processpiper import ProcessMap, EventType, ActivityType, GatewayType",
-        f'with ProcessMap("{process_map_title}") as my_process_map:'
-        if colour_theme is None
-        else f'with ProcessMap("{process_map_title}", colour_theme="{colour_theme}") as my_process_map:',
+        f'with ProcessMap("{process_map_title}"{colour_theme_code if colour_theme is not None else ""}{process_map_width_code if process_map_width > 0 else ""}) as my_process_map:',
     ]
 
+    # if colour_theme is None and process_map_width is None:
+    #     code_lines.append(f'with ProcessMap("{process_map_title}") as my_process_map:')
+    # elif colour_theme is None:
+    #     code_lines.append(f'with ProcessMap("{process_map_title}", width="{process_map_width}") as my_process_map:')
+    # else:
+    #     code_lines.append(f'with ProcessMap("{process_map_title}", colour_theme="{colour_theme}") as my_process_map:')
+
+    #     if colour_theme is None
+    #     elif process_map_width is None:
+    #         f'with ProcessMap("{process_map_title}", colour_theme="{colour_theme}") as my_process_map:',
+    #     else f'with ProcessMap("{process_map_title}", colour_theme="{colour_theme}", width="{process_map_width}) as my_process_map:',
+    # ]
+
     indent = ""
     pool_id = 1
     lane_id = 0
     pool_found = False
     while lines:
         line = lines.pop(0).strip()
         if line.startswith("pool:"):
@@ -170,14 +183,27 @@
     if "title" in lines[0]:
         process_map_title = lines.pop(0).split(":")[1].strip()
     else:
         raise ValueError("The first line must contain the word 'title'.")
     return process_map_title
 
 
+def parse_width(lines):
+    """
+    The function extracts the title from a list of lines if the first line contains the word "title".
+    """
+
+    if "width" in lines[0]:
+        process_map_width = lines.pop(0).split(":")[1].strip()
+    else:
+        process_map_width = 0
+
+    return process_map_width
+
+
 def parse_lane_element(element_str):
     """
     The function parses a string representing a BPMN element and returns its type, name, and variable
     name.
     """
     """Detect element type"""
     ### EventType
@@ -259,26 +285,26 @@
     if "add_element" not in code:
         raise ValueError("There is no element defined. Please add elements to lane.")
 
 
 def render(text: str, png_output_file: str = ""):
     """Render text to diagram"""
     output_file_provided = True
-    if png_output_file.strip() == "":
+    if not png_output_file.strip():
         output_file_provided = False
         # add datetime to the file name
         png_output_file = (
             f"piper_{datetime.datetime.now().strftime('%Y%m%d_%H%M%S')}.png"
         )
 
     generated_code = parse_and_generate_code(text, png_output_file)
     validate_generated_code(generated_code)
     # show_code_with_line_number(generated_code)
     # print(generated_code)
     exec(generated_code)
     generated_image = Image.open(png_output_file)
     generated_image.load()
     # Clean up the generated image file
-    if output_file_provided == False:
+    if not output_file_provided:
         os.remove(png_output_file)
 
     return generated_code, generated_image
```

### Comparing `processpiper-0.4.0/src/processpiper/title.py` & `processpiper-0.4.1/src/processpiper/title.py`

 * *Files identical despite different names*

### Comparing `processpiper-0.4.0/src/processpiper.egg-info/PKG-INFO` & `processpiper-0.4.1/src/processpiper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processpiper
-Version: 0.4.0
+Version: 0.4.1
 Summary: Processpiper. An open source python library to generate business process diagram using code.
 Author: CS Goh
 Project-URL: Homepage, https://github.com/csgoh/processpiper
 Project-URL: Bug Tracker, https://github.com/csgoh/processpiper/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -81,16 +81,16 @@
 * Ubuntu
 * MacOS
 
 ## Documentation
 Please refer to [Processpiper Wiki](https://github.com/csgoh/processpiper/wiki) for more information on how to use this library.
 
 ## Examples
-### (Method 1) Generate diagram using plain text
-This is a sample code to generate a business process diagram using plain text. 
+### (Method 1) Generate diagram using English like PiperFlow syntax
+This is a sample code to generate a business process diagram using PiperFlow syntax. 
 ```python
 from processpiper.text2diagram import render
 
 input_syntax = """
 title: Sample Test Process
 colourtheme: BLUEMOUNTAIN
     lane: End User
@@ -158,16 +158,16 @@
 The generated diagram is as follows:
 ![Process Map](https://github.com/csgoh/processpiper/blob/main/images/test/test_auto_case1.png)
 
 
 ## Development Status
 Initial first release would only cover the following basic business process elements. Other element types will be introduced in subsequence releases.
 
-* Event: Start, End, Timer, Intermediate
+* Event: Start, End, Timer, Intermediate, Message, Signal, Conditional, Link
 * Activity: Task, Subprocess
-* Gateway: Inclusive, Exclusive, Parallel
+* Gateway: Inclusive, Exclusive, Parallel, Event
 
 Any ideas or suggestions, please send it to me via [GitHub Discussions](https://github.com/csgoh/processmapper/discussions).
```

### Comparing `processpiper-0.4.0/src/processpiper.egg-info/SOURCES.txt` & `processpiper-0.4.1/src/processpiper.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/processpiper/colourtheme.py
 src/processpiper/constants.py
 src/processpiper/event.py
 src/processpiper/footer.py
 src/processpiper/gateway.py
 src/processpiper/helper.py
 src/processpiper/lane.py
+src/processpiper/layout.py
 src/processpiper/painter.py
 src/processpiper/pool.py
 src/processpiper/processmap.py
 src/processpiper/shape.py
 src/processpiper/text2diagram.py
 src/processpiper/title.py
 src/processpiper/version.py
```

### Comparing `processpiper-0.4.0/src/tests/github_action_test.py` & `processpiper-0.4.1/src/tests/github_action_test.py`

 * *Files identical despite different names*

