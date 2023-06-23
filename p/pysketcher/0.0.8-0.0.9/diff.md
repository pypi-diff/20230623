# Comparing `tmp/pysketcher-0.0.8.tar.gz` & `tmp/pysketcher-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysketcher-0.0.8.tar", max compression
+gzip compressed data, was "pysketcher-0.0.9.tar", max compression
```

## Comparing `pysketcher-0.0.8.tar` & `pysketcher-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,57 @@
--rw-r--r--   0        0        0     1071 2021-06-27 10:40:12.350473 pysketcher-0.0.8/LICENSE
--rw-r--r--   0        0        0     2354 2021-06-27 10:40:12.350473 pysketcher-0.0.8/README.rst
--rw-r--r--   0        0        0     3704 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2221 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/__init__.py
--rw-r--r--   0        0        0     2485 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_angle.py
--rw-r--r--   0        0        0     5692 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_arc.py
--rw-r--r--   0        0        0     2040 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_arrow.py
--rw-r--r--   0        0        0     1973 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_arrow_with_text.py
--rw-r--r--   0        0        0     1538 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_axis.py
--rw-r--r--   0        0        0      745 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_circle.py
--rw-r--r--   0        0        0      274 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_color.py
--rw-r--r--   0        0        0     2843 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_cubic_bezier_curve.py
--rw-r--r--   0        0        0     3021 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_curve.py
--rw-r--r--   0        0        0     7132 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_dashpot.py
--rw-r--r--   0        0        0     3947 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_distance_with_text.py
--rw-r--r--   0        0        0      199 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_drawable.py
--rw-r--r--   0        0        0     3308 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_figure.py
--rw-r--r--   0        0        0      677 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_force.py
--rw-r--r--   0        0        0     4562 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_line.py
--rw-r--r--   0        0        0     1556 2021-06-27 10:40:12.358473 pysketcher-0.0.8/pysketcher/_moment.py
--rw-r--r--   0        0        0     6146 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_point.py
--rw-r--r--   0        0        0     3234 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_rectangle.py
--rw-r--r--   0        0        0     4261 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_shape.py
--rw-r--r--   0        0        0     1773 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_simple_support.py
--rw-r--r--   0        0        0     4157 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_sketchy_func.py
--rw-r--r--   0        0        0     1623 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_spline.py
--rw-r--r--   0        0        0     2801 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_spring.py
--rw-r--r--   0        0        0     6447 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_style.py
--rw-r--r--   0        0        0     4203 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_text.py
--rw-r--r--   0        0        0     1440 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_triangle.py
--rw-r--r--   0        0        0     1296 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_uniform_load.py
--rw-r--r--   0        0        0       70 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_utils/__init__.py
--rw-r--r--   0        0        0      632 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_utils/doc_enum.py
--rw-r--r--   0        0        0     2419 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_velocity_profile.py
--rw-r--r--   0        0        0     2125 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_wall.py
--rw-r--r--   0        0        0      126 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_warning.py
--rw-r--r--   0        0        0     2105 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/_wheel.py
--rw-r--r--   0        0        0        0 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/backend/__init__.py
--rw-r--r--   0        0        0      792 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/backend/backend.py
--rw-r--r--   0        0        0      111 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/backend/matplotlib/__init__.py
--rw-r--r--   0        0        0      239 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/backend/matplotlib/_matplotlib_adapter.py
--rw-r--r--   0        0        0     3318 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/backend/matplotlib/_matplotlib_backend.py
--rw-r--r--   0        0        0      356 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/backend/matplotlib/_matplotlib_composition.py
--rw-r--r--   0        0        0     3748 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/backend/matplotlib/_matplotlib_curve.py
--rw-r--r--   0        0        0     3281 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/backend/matplotlib/_matplotlib_style.py
--rw-r--r--   0        0        0     1434 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/backend/matplotlib/_matplotlib_text.py
--rw-r--r--   0        0        0      336 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/composition/__init__.py
--rw-r--r--   0        0        0     6553 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/composition/_composition.py
--rw-r--r--   0        0        0        0 2021-06-27 10:40:12.362473 pysketcher-0.0.8/pysketcher/images/.gitignore
--rw-r--r--   0        0        0     3510 2021-06-27 10:47:11.830110 pysketcher-0.0.8/setup.py
--rw-r--r--   0        0        0     3262 2021-06-27 10:47:11.830562 pysketcher-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-06-20 10:59:16.783063 pysketcher-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2354 2021-11-05 08:16:32.363039 pysketcher-0.0.9/README.rst
+-rw-r--r--   0        0        0     3862 2021-11-05 08:10:08.523286 pysketcher-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2289 2021-07-22 05:33:22.119848 pysketcher-0.0.9/pysketcher/__init__.py
+-rw-r--r--   0        0        0     2485 2021-07-17 12:05:45.930750 pysketcher-0.0.9/pysketcher/_angle.py
+-rw-r--r--   0        0        0     4167 2021-07-22 05:33:22.121038 pysketcher-0.0.9/pysketcher/_arc.py
+-rw-r--r--   0        0        0     2040 2021-07-17 12:05:45.969920 pysketcher-0.0.9/pysketcher/_arrow.py
+-rw-r--r--   0        0        0     1299 2021-07-22 05:33:22.122431 pysketcher-0.0.9/pysketcher/_axis.py
+-rw-r--r--   0        0        0      788 2021-07-22 05:33:22.129212 pysketcher-0.0.9/pysketcher/_circle.py
+-rw-r--r--   0        0        0      274 2021-07-17 12:05:45.979888 pysketcher-0.0.9/pysketcher/_color.py
+-rw-r--r--   0        0        0     2843 2021-07-17 12:05:45.993837 pysketcher-0.0.9/pysketcher/_cubic_bezier_curve.py
+-rw-r--r--   0        0        0     3021 2021-07-17 12:05:46.010698 pysketcher-0.0.9/pysketcher/_curve.py
+-rw-r--r--   0        0        0     7132 2021-07-17 12:05:46.024447 pysketcher-0.0.9/pysketcher/_dashpot.py
+-rw-r--r--   0        0        0      199 2021-07-17 12:05:46.024924 pysketcher-0.0.9/pysketcher/_drawable.py
+-rw-r--r--   0        0        0     3308 2021-07-17 12:05:46.030436 pysketcher-0.0.9/pysketcher/_figure.py
+-rw-r--r--   0        0        0     1021 2021-07-22 05:33:22.130672 pysketcher-0.0.9/pysketcher/_force.py
+-rw-r--r--   0        0        0     4562 2021-07-17 12:05:46.038720 pysketcher-0.0.9/pysketcher/_line.py
+-rw-r--r--   0        0        0     2235 2021-07-22 05:33:22.131921 pysketcher-0.0.9/pysketcher/_moment.py
+-rw-r--r--   0        0        0     6157 2021-07-22 05:33:22.133187 pysketcher-0.0.9/pysketcher/_point.py
+-rw-r--r--   0        0        0     3079 2021-07-22 05:33:22.134511 pysketcher-0.0.9/pysketcher/_rectangle.py
+-rw-r--r--   0        0        0     4261 2021-07-19 05:27:11.208527 pysketcher-0.0.9/pysketcher/_shape.py
+-rw-r--r--   0        0        0     1817 2021-07-22 05:33:22.135828 pysketcher-0.0.9/pysketcher/_simple_support.py
+-rw-r--r--   0        0        0     4157 2021-07-17 12:05:46.071457 pysketcher-0.0.9/pysketcher/_sketchy_func.py
+-rw-r--r--   0        0        0     1623 2021-07-17 12:05:46.078243 pysketcher-0.0.9/pysketcher/_spline.py
+-rw-r--r--   0        0        0     2801 2021-07-17 12:05:46.083741 pysketcher-0.0.9/pysketcher/_spring.py
+-rw-r--r--   0        0        0     6445 2021-07-22 05:33:22.141271 pysketcher-0.0.9/pysketcher/_style.py
+-rw-r--r--   0        0        0     3907 2021-11-04 08:08:43.702280 pysketcher-0.0.9/pysketcher/_text.py
+-rw-r--r--   0        0        0     1440 2021-07-17 12:05:46.103581 pysketcher-0.0.9/pysketcher/_triangle.py
+-rw-r--r--   0        0        0     1580 2021-07-22 05:33:22.148192 pysketcher-0.0.9/pysketcher/_uniform_load.py
+-rw-r--r--   0        0        0       70 2021-07-17 12:05:46.108850 pysketcher-0.0.9/pysketcher/_utils/__init__.py
+-rw-r--r--   0        0        0      632 2021-07-17 12:05:46.109273 pysketcher-0.0.9/pysketcher/_utils/doc_enum.py
+-rw-r--r--   0        0        0     2362 2021-07-22 05:33:22.154908 pysketcher-0.0.9/pysketcher/_velocity_profile.py
+-rw-r--r--   0        0        0     2123 2021-07-22 05:33:22.177959 pysketcher-0.0.9/pysketcher/_wall.py
+-rw-r--r--   0        0        0      126 2021-07-17 12:05:46.123048 pysketcher-0.0.9/pysketcher/_warning.py
+-rw-r--r--   0        0        0     2105 2021-07-17 12:05:46.127785 pysketcher-0.0.9/pysketcher/_wheel.py
+-rw-r--r--   0        0        0      392 2021-07-22 05:33:22.178850 pysketcher-0.0.9/pysketcher/annotation/__init__.py
+-rw-r--r--   0        0        0      608 2021-07-22 05:33:22.179275 pysketcher-0.0.9/pysketcher/annotation/_arc_annotation.py
+-rw-r--r--   0        0        0     1174 2021-07-22 05:33:22.179732 pysketcher-0.0.9/pysketcher/annotation/_line_annotation.py
+-rw-r--r--   0        0        0      186 2021-07-22 05:33:22.180245 pysketcher-0.0.9/pysketcher/annotation/_text_position.py
+-rw-r--r--   0        0        0        0 2021-07-17 12:05:46.129851 pysketcher-0.0.9/pysketcher/backend/__init__.py
+-rw-r--r--   0        0        0      792 2021-07-17 12:05:46.130200 pysketcher-0.0.9/pysketcher/backend/backend.py
+-rw-r--r--   0        0        0      111 2021-07-17 12:05:46.130457 pysketcher-0.0.9/pysketcher/backend/matplotlib/__init__.py
+-rw-r--r--   0        0        0      239 2021-07-17 12:05:46.130918 pysketcher-0.0.9/pysketcher/backend/matplotlib/_matplotlib_adapter.py
+-rw-r--r--   0        0        0     3330 2021-07-22 05:33:22.189055 pysketcher-0.0.9/pysketcher/backend/matplotlib/_matplotlib_backend.py
+-rw-r--r--   0        0        0      356 2021-07-17 12:05:46.132829 pysketcher-0.0.9/pysketcher/backend/matplotlib/_matplotlib_composition.py
+-rw-r--r--   0        0        0     4360 2021-07-22 05:33:22.198034 pysketcher-0.0.9/pysketcher/backend/matplotlib/_matplotlib_curve.py
+-rw-r--r--   0        0        0     3281 2021-07-17 12:05:46.134873 pysketcher-0.0.9/pysketcher/backend/matplotlib/_matplotlib_style.py
+-rw-r--r--   0        0        0     1432 2021-07-22 05:33:22.208068 pysketcher-0.0.9/pysketcher/backend/matplotlib/_matplotlib_text.py
+-rw-r--r--   0        0        0      304 2021-07-22 05:33:22.214834 pysketcher-0.0.9/pysketcher/composition/__init__.py
+-rw-r--r--   0        0        0     6274 2021-07-22 05:33:22.230605 pysketcher-0.0.9/pysketcher/composition/_composition.py
+-rw-r--r--   0        0        0      316 2021-07-22 05:33:22.231299 pysketcher-0.0.9/pysketcher/dimension/__init__.py
+-rw-r--r--   0        0        0     5276 2021-07-22 05:33:22.231986 pysketcher-0.0.9/pysketcher/dimension/_angular_dimension.py
+-rw-r--r--   0        0        0     5483 2021-07-22 05:33:22.232902 pysketcher-0.0.9/pysketcher/dimension/_linear_dimension.py
+-rw-r--r--   0        0        0     4897 2021-07-22 05:33:22.233566 pysketcher-0.0.9/pysketcher/dimension/_radial_dimension.py
+-rw-r--r--   0        0        0        0 2021-06-20 18:39:54.795938 pysketcher-0.0.9/pysketcher/images/.gitignore
+-rw-r--r--   0        0        0     3630 2021-11-05 08:16:42.498767 pysketcher-0.0.9/setup.py
+-rw-r--r--   0        0        0     3388 2021-11-05 08:16:42.499208 pysketcher-0.0.9/PKG-INFO
```

### Comparing `pysketcher-0.0.8/LICENSE` & `pysketcher-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/README.rst` & `pysketcher-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pyproject.toml` & `pysketcher-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,74 @@
 [build-system]
-requires = ["poetry_core>=1.0.0"]
+requires = [
+    "poetry_core>=1.0.7",
+    "nox>=2021.10.1",
+    "poetry==1.1.11",
+    "nox-poetry==0.8.6"
+    ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pysketcher"
-version = "0.0.8"
+version = "0.0.9"
 description = "Geometric Sketching Utility for Python"
 license = "mit"
 authors = [
     "Richard Vodden <richard@vodden.com>",
     "Hans Petter Langtangen"
 ]
 readme = "README.rst"
 packages = [{ include = "pysketcher" }]
 repository = "https://github.com/rvodden/pysketcher"
 homepage = "https://github.com/rvodden/pysketcher"
 keywords = ['sketch','graphics','scientific','engineering','geometry']
 
-[tool.poetry.extras]
-docs = ["sphinx"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 numpy = "^1.19.5"
 matplotlib = "^3.2.1"
 scipy = "^1.6.0"
-importlib-metadata = {version = ">=2,<5", python = "<=3.7"}
 celluloid = "^0.2.0"
+sphinx = { version = "^4.1.1", optional=true }
+sphinx_rtd_theme = { version = ">=0.5,<1.1", optional=true }
+sphinx-autodoc-typehints = { version = "^1.11.1", optional=true }
 
 [tool.poetry.dev-dependencies]
-hypothesis = "^6.14.0"
+hypothesis = "^6.14.3"
 pytest = "^6.2.2"
-pylint = "^2.6.2"
-flake8 = "^3.9.0"
-coverage = "^5.3"
+pylint = "^2.9.6"
+flake8 = "^4.0.1"
+coverage = "^6.1"
 mypy = "^0.910"
 pydocstyle = "^6.1.1"
-black = "^21.4b2"
-'zest.releaser' = { version = "^6.22.1", extras = ['recommended'] }
+black = "^21.7b0"
 wheel = "^0.35.1"
-sphinx = "^4.0.2"
-sphinx_rtd_theme = "^0.5.0"
 recommonmark = "^0.7.1"
-pytest-cov = "^2.11.1"
+pytest-cov = "^3.0.0"
 nox = "^2021.6.12"
 pre-commit = "^2.11.1"
-flake8-black = "^0.2.1"
+flake8-black = "^0.2.3"
 flake8-import-order = "^0.18.1"
 flake8-bandit = "^2.1.2"
 nox-poetry = "^0.8.4"
 flake8-docstrings = "^1.6.0"
-sphinx-autodoc-typehints = "^1.11.1"
 six = "^1.15.0"
-zipp = "^3.4.0"
+zipp = "^3.5.0"
 darglint = "^1.7.0"
 blackdoc = "^0.3"
-commitizen = "^2.17.11"
+commitizen = "^2.17.13"
 safety = "^1.9.0"
 flake8-bugbear = "^21.3.2"
 typed-ast = "^1.4.1"
 codecov = "^2.1.10"
+'zest.releaser' = { version = "^6.22.2", extras = ['recommended'] }
+
+[tool.poetry.extras]
+docs = ["sphinx", "sphinx_rtd_theme", "sphinx-autodoc-typehints"]
 
 [tool.poetry.scripts]
 beam1 = "examples.beam1:main"
 
 [tool.pytest.ini_options]
 testpaths = ["tests", "pysketcher"]
 python_files = "test_*.py"
```

### Comparing `pysketcher-0.0.8/pysketcher/__init__.py` & `pysketcher-0.0.9/pysketcher/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 
 try:
     __version__ = version(__name__)
 except PackageNotFoundError:
     pass
 
 from pysketcher._angle import Angle
-from pysketcher._arc import Arc, ArcWithText
+from pysketcher._arc import Arc
 from pysketcher._arrow import Arrow, DoubleArrow
-from pysketcher._arrow_with_text import ArrowWithText
 from pysketcher._axis import Axis
 from pysketcher._circle import Circle
 from pysketcher._cubic_bezier_curve import CubicBezier
 from pysketcher._curve import Curve
 from pysketcher._dashpot import Dashpot
-from pysketcher._distance_with_text import DistanceWithText
 from pysketcher._drawable import Drawable
 from pysketcher._figure import Figure
 from pysketcher._force import Force, Gravity
 from pysketcher._line import Line
 from pysketcher._moment import Moment
 from pysketcher._point import Point
 from pysketcher._rectangle import Rectangle
@@ -36,49 +34,53 @@
 from pysketcher._style import Style, TextStyle
 from pysketcher._text import Text
 from pysketcher._triangle import Triangle
 from pysketcher._uniform_load import UniformLoad
 from pysketcher._velocity_profile import VelocityProfile
 from pysketcher._wall import Wall
 from pysketcher._wheel import Wheel
-from pysketcher.composition import Composition, ShapeWithText
+from pysketcher.annotation import ArcAnnotation, LineAnnotation, TextPosition
+from pysketcher.composition import Composition
+from pysketcher.dimension import AngularDimension, LinearDimension, RadialDimension
 
 __all__ = [
+    "AngularDimension",
+    "Axis",
     "Angle",
     "Arc",
-    "ArcWithText",
+    "ArcAnnotation",
     "Arrow",
     "DoubleArrow",
-    "ArrowWithText",
-    "Axis",
-    "SimpleSupport",
     "Circle",
     "CubicBezier",
     "Composition",
-    "ShapeWithText",
     "Curve",
     "Dashpot",
-    "DistanceWithText",
     "Drawable",
     "Figure",
     "Force",
     "Gravity",
     "Line",
+    "LineAnnotation",
+    "LinearDimension",
     "Moment",
     "Point",
+    "RadialDimension",
     "Rectangle",
     "Shape",
+    "SimpleSupport",
     "SketchyFunc1",
     "SketchyFunc2",
     "SketchyFunc3",
     "SketchyFunc4",
     "Spline",
     "Spring",
     "Style",
     "TextStyle",
+    "TextPosition",
     "Text",
     "Triangle",
     "UniformLoad",
     "VelocityProfile",
     "Wall",
     "Wheel",
 ]
```

### Comparing `pysketcher-0.0.8/pysketcher/_angle.py` & `pysketcher-0.0.9/pysketcher/_angle.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_arc.py` & `pysketcher-0.0.9/pysketcher/_point.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,188 +1,207 @@
+from typing import List, Tuple
+
 import numpy as np
 
 from pysketcher._angle import Angle
-from pysketcher._curve import Curve
-from pysketcher._point import Point
-from pysketcher._text import Text
-from pysketcher.composition import ShapeWithText
 
 
-class Arc(Curve):
-    """A representation of a continuous connected subset of a circle.
+class Point:
+    """Immutable Point class which implements basic point arithmetic.
 
     Args:
-        center: The center of the Arc.
-        radius: The radius of the Arc.
-        start_angle: The angle from the +ve horizontal where the Arc should start.
-        arc_angle: The angle (from the start_angle) where the Arc should end.
-        resolution: The number of points in the Arc.
-
-    Examples:
-        >>> arc = ps.Arc(ps.Point(0.0, 0.0), 1.0, Angle(0.0), Angle(np.pi / 2))
-        >>> fig = ps.Figure(-0.5, 1.5, -0.5, 1.5, backend=MatplotlibBackend)
-        >>> fig.add(arc)
-        >>> fig.save("pysketcher/images/arc.png")
-
-    .. figure:: images/arc.png
-        :alt: An example of an Arc.
-        :figclass: align-center
-
-        An example of an ``Arc``.
+        x: float
+            The x co-ordinate
+        y: float
+            The y co-ordinate
     """
 
-    _center: Point
-    _radius: float
-    _start_angle: Angle
-    _arc_angle: Angle
-    _resolution: int
-
-    def __init__(
-        self,
-        center: Point,
-        radius: float,
-        start_angle: Angle,
-        arc_angle: Angle,
-        resolution: int = 180,
-    ):
-        # Must record some parameters for __call__
-        self._center = center
-        self._radius = radius
-        self._start_angle = Angle(start_angle)
-        self._arc_angle = Angle(arc_angle)
-        self._resolution = resolution
-
-        if self._arc_angle == 0.0:
-            # assume a full circle
-            ts = np.linspace(0.0, 2.0 * np.pi, resolution + 1)
-        else:
-            ts = np.linspace(0.0, self._arc_angle, resolution + 1)
+    _x: float
+    _y: float
 
-        points = [self(t) for t in ts]
-        super().__init__(points)
+    def __init__(self, x: float, y: float):
+        self._x = float(x)
+        self._y = float(y)
 
-    def __call__(self, theta: Angle) -> Point:
-        """Provides a point on the arc ``theta`` of the way around.
+    def __add__(self, other: "Point") -> "Point":
+        """Sums the co-ordinates of the two points.
 
         Args:
-            theta: The angle from the ``start_angle`` from which the point should
-                be taken.
+            other: the point to add to ``self``.
 
         Returns:
-            the point ``theta`` of the way around the arc.
+            The sum of ``self`` and ``other``.
+        """
+        return Point(self.x + other._x, self.y + other.y)
 
-        Raises:
-            ValueError: if ``theta`` is beyond the bounds of the arc.
+    def __sub__(self, other: "Point") -> "Point":
+        """Subtracts the co-ordinates of the two points.
+
+        Args:
+            other: the point to subtract from ``self``.
+
+        Returns:
+            The difference between ``self`` and ``other``.
         """
-        if 0.0 < self._arc_angle < theta or theta < self._arc_angle < 0.0:
-            raise ValueError(
-                f"Theta ({theta}) is outside the bounds "
-                "of the arc (0.0 , {self._arc_angle})"
-            )
+        return Point(self.x - other._x, self.y - other.y)
+
+    def __mul__(self, scalar: float) -> "Point":
+        """Multiplies ``self`` by ``scalar``.
+
+        Args:
+            scalar: the factor to scale ``self`` by.
 
-        iota = Angle(self.start_angle + theta)
-        ret_point = Point(
-            self.center.x + self.radius * np.cos(iota),
-            self.center.y + self.radius * np.sin(iota),
+        Returns:
+            A point with each co-ordinate scaled from ``self`` by ``scalar``.
+        """
+        return Point(self.x * scalar, self.y * scalar)
+
+    def __abs__(self) -> float:
+        """The pythagorean length of ``self``.
+
+        Returns:
+            The cartesian distance from ``Point(0,0)`` to ``self``.
+        """
+        return np.hypot(self.x, self.y)
+
+    def __eq__(self, other: "Point") -> bool:
+        """Implementation of point equality.
+
+        Note that owing to the vagaries of floating point arithmetic
+        two points which have co-ordinates within 1e-4 will be
+        considered equal.
+
+        Args:
+            other: the ``Point`` to compare to ``self``.
+
+        Returns:
+            True if ``Point`` is equal to ``self``.
+        """
+        return self._is_close(self.x, other.x) and self._is_close(self.y, other.y)
+
+    def __str__(self):
+        """A string representation of ``self``."""
+        return self.__repr__()
+
+    def __repr__(self):
+        """An unambiguous string representation of ``self``."""
+        return "P(%s, %s)" % (
+            np.format_float_scientific(self.x),
+            np.format_float_scientific(self.y),
         )
-        return ret_point
 
-    @property
-    def start_angle(self) -> Angle:
-        """The angle from the +ve horizontal from where the arc starts."""
-        return self._start_angle
+    @staticmethod
+    def _is_close(x: float, y: float) -> bool:
+        return np.isclose(x, y, atol=1e-4)
 
     @property
-    def arc_angle(self) -> Angle:
-        """The angle from the ``start_angle`` to which the arc ends."""
-        return self._arc_angle
+    def x(self) -> float:
+        """The x co-ordinate of the Point."""
+        return self._x
 
     @property
-    def end_angle(self) -> Angle:
-        """The angle from the +ve horizontal to which the arc ends."""
-        return self._start_angle + self._arc_angle
+    def y(self) -> float:
+        """The y co-ordinate of the Point."""
+        return self._y
 
     @property
-    def radius(self) -> float:
-        """The radius of the arc."""
-        return self._radius
+    def unit_vector(self) -> "Point":
+        """Returns a ``Point`` of length 1 in the direction of the ``Point``."""
+        if self._is_close(abs(self), 0.0):
+            raise ZeroDivisionError("Length of Vector cannot be Zero")
+        return self * (1 / (abs(self)))
 
     @property
-    def center(self) -> Point:
-        """The center of the arc."""
-        return self._center
+    def angle(self) -> Angle:
+        """Returns the ``Angle`` the ``Point`` makes to the +ve horizontal."""
+        angle = Angle(np.arctan2(self.y, self.x))
+        return angle
 
     @property
-    def start(self) -> Point:
-        """The point at which the arc starts."""
-        return self(0.0)
+    def radius(self) -> float:
+        """Returns the distance from ``Point(0.,0.)`` to this point."""
+        return abs(self)
 
     @property
-    def end(self) -> Point:
-        """The point at which the arc ends."""
-        return self(self.arc_angle)
+    def normal(self) -> "Point":
+        r"""Returns a ``Point`` of length 1, :math:``$\frac{\pi}{2}$`` from ``self``."""
+        uv = self.unit_vector
+        return Point(-uv.y, uv.x)
 
-    def translate(self, vec: Point) -> "Arc":
-        """Translates the arc by the specified vector.
+    def rotate(self, angle: Angle, center: "Point") -> "Point":
+        """Returns a ``Point``, ``angle`` (in radians) around (`x`,`y`).
 
         Args:
-            vec: The vector through which the arc should be translated.
+            angle: The angle through which the rotation should be made.
+            center: The point about which the rotation should be made.
 
         Returns:
-            A copy of the arc which has been translated by ``vec``.
+            The rotated point.
         """
-        arc = Arc(
-            self._center + vec,
-            self._radius,
-            self._start_angle,
-            self._arc_angle,
-            self._resolution,
-        )
-        arc.style = self.style
-        return arc
+        if not type(angle) == Angle:
+            angle = Angle(angle)
 
+        # Check for a few degenerate cases:
+        if angle == Angle(0.0):
+            p = self
+        elif angle == Angle(np.pi / 2):
+            p = Point(center.x - self.y + center.y, center.y + self.x - center.x)
+        elif angle == Angle(np.pi):
+            p = Point(2 * center.x - self.x, 2 * center.y - self.y)
+        elif angle == Angle(-np.pi / 2):
+            p = Point(center.x + self.y - center.y, center.y - self.x + center.x)
+        else:
+            c = np.cos(angle)
+            s = np.sin(angle)
+            p = Point(
+                center.x + (self.x - center.x) * c - (self.y - center.y) * s,
+                center.y + (self.x - center.x) * s + (self.y - center.y) * c,
+            )
+        return p
 
-class ArcWithText(ShapeWithText):
-    """An ``Arc`` with a ``Text`` label.
+    def scale(self, factor: float) -> "Point":
+        """Scale point coordinates by `factor`: ``x = factor*x``, etc.
 
-    Args:
-        text: The text to be displayed.
-        center: The center of the ``Arc``.
-        radius: The radius of the ``Arc``.
-        start_angle: The angle from the +ve horizontal from which
-            the ``Arc`` should begin.
-        arc_angle: The angle from the ``start_angle`` at which
-            the ``Arc`` should end.
-        resolution: The number of points in the ``Arc``.
-        text_spacing: The spacing of the text from the midpoint of the ``Arc``.
-
-    Examples:
-        >>> arc_with_text = ps.ArcWithText(
-        ...     "$A$", ps.Point(0.0, 0.0), 1.0, Angle(0.0), Angle(np.pi / 2)
-        ... )
-        >>> fig = ps.Figure(-0.5, 1.5, -0.5, 1.5, backend=MatplotlibBackend)
-        >>> fig.add(arc_with_text)
-        >>> fig.save("pysketcher/images/arc_with_text.png")
-
-        .. figure:: images/arc_with_text.png
-            :alt: An example of an ArcWithText.
-            :figclass: align-center
+        Args:
+            factor: the amount the ``Point`` should be scaled by.
 
-            An example of an ``ArcWithText``.
-    """
+        Returns:
+            The scaled point.
+        """
+        return self * factor
+
+    def translate(self, vec: "Point") -> "Point":
+        """Translate point by a vector `vec`.
 
-    def __init__(
-        self,
-        text: str,
-        center: Point,
-        radius: float,
-        start_angle: Angle,
-        arc_angle: Angle,
-        resolution: int = 180,
-        text_spacing: float = 1 / 6.0,
-    ):
-        arc = Arc(center, radius, start_angle, arc_angle, resolution)
-        mid = arc(arc_angle / 2.0)
-        normal = (mid - center).unit_vector()
-        text_pos = mid - (normal * text_spacing)
-        text = Text(text, text_pos)
-        super().__init__(arc, text)
+        Args:
+            vec: The vector (``Point``) through which the point should be
+                translated.
+
+        Returns:
+            The translated vector.
+        """
+        return self + vec
+
+    @staticmethod
+    def from_coordinate_lists(xs: List[float], ys: List[float]) -> List["Point"]:
+        """Generates points from lists of co-ordinates.
+
+        Args:
+            xs: the x co-ordinates
+            ys: the y co-ordinates
+
+        Returns:
+            A list of ``Point`` made up of the respective co-ordinates.
+
+        Raises:
+            ValueError: When the co-ordinates lists are of different lengths.
+        """
+        if len(xs) != len(ys):
+            raise ValueError("xs and ys must be the same length")
+        return [Point(xs[i], ys[i]) for i in range(len(xs))]
+
+    @staticmethod
+    def to_coordinate_lists(ps: List["Point"]) -> Tuple[List[float], List[float]]:
+        """Generates lists of co-ordinates from points."""
+        xs = [p.x for p in ps]
+        ys = [p.y for p in ps]
+        return xs, ys
```

### Comparing `pysketcher-0.0.8/pysketcher/_arrow.py` & `pysketcher-0.0.9/pysketcher/_arrow.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_circle.py` & `pysketcher-0.0.9/pysketcher/_circle.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 
+from pysketcher._angle import Angle
 from pysketcher._arc import Arc
 from pysketcher._point import Point
 
 
 class Circle(Arc):
     """A representation of a 2D circle.
 
@@ -21,8 +22,8 @@
         :alt: An example of Circle.
         :figclass: align-center
 
         An example of ``Circle``.
     """
 
     def __init__(self, center: Point, radius: float, resolution=180):
-        super().__init__(center, radius, 0, 2 * np.pi, resolution)
+        super().__init__(center, radius, Angle(0), 2 * np.pi, resolution)
```

### Comparing `pysketcher-0.0.8/pysketcher/_cubic_bezier_curve.py` & `pysketcher-0.0.9/pysketcher/_cubic_bezier_curve.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_curve.py` & `pysketcher-0.0.9/pysketcher/_curve.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_dashpot.py` & `pysketcher-0.0.9/pysketcher/_dashpot.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_figure.py` & `pysketcher-0.0.9/pysketcher/_figure.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_line.py` & `pysketcher-0.0.9/pysketcher/_line.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_moment.py` & `pysketcher-0.0.9/pysketcher/_moment.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,77 @@
+from enum import auto, Enum, unique
+
 import numpy as np
 
-from pysketcher._arc import ArcWithText
+from pysketcher._angle import Angle
+from pysketcher._arc import Arc
 from pysketcher._style import Style
+from pysketcher.annotation import ArcAnnotation
+from pysketcher.composition import Composition
 
 
-class Moment(ArcWithText):
+class Moment(Composition):
     r"""A symbol which represents a moment.
 
     This is an ``ArcWithText`` with the ``arc_angle`` fixed at :math:`\pi`.
 
     Args:
         text: The text to display.
         center: The centre of the moment.
         radius: The radius of the moment.
         start_angle: The angle from the +ve horizontal at which the moment should
             start.
         text_spacing: The spacing of the text.
         resolution: The number of points on the arc.
 
     Examples:
-        >>> moment = ps.Moment("$M$", ps.Point(0, 0), 1.0, 0.0)
+        >>> moment = ps.Moment("$M$", ps.Point(0, 0), 1.0)
         >>> fig = ps.Figure(-1.2, 1.2, -1.2, 1.2, backend=MatplotlibBackend)
         >>> fig.add(moment)
         >>> fig.save("pysketcher/images/moment.png")
 
         .. figure:: images/moment.png
             :alt: An example of Moment.
             :figclass: align-center
 
             An example of ``Moment``.
     """
 
+    @unique
+    class Direction(Enum):
+        """Indicates the direction of the moment."""
+
+        CLOCKWISE = auto()
+        COUNTER_CLOCKWISE = auto()
+
+    @unique
+    class Orientation(Enum):
+        """Indicated the orientation of the moment."""
+
+        LEFT = auto()
+        RIGHT = auto()
+
+    _DEFAULT_DIRECTION: Direction = Direction.COUNTER_CLOCKWISE
+    _DEFAULT_ORIENTATION: Orientation = Orientation.LEFT
+
     def __init__(
         self,
         text,
         center,
         radius,
-        left=True,
-        counter_clockwise=True,
-        fontsize=0,
-        text_spacing=1 / 3.0,
     ):
-        style = Style.ArrowStyle.END if counter_clockwise else Style.ArrowStyle.START
-        start_angle = np.pi / 2 if left else -np.pi / 2
-        super().__init__(
-            text,
-            center,
-            radius,
-            start_angle,
-            np.pi,
-            text_spacing=text_spacing,
-            resolution=180,
+        self._direction = self._DEFAULT_DIRECTION
+        self._orientation = self._DEFAULT_ORIENTATION
+
+        style = (
+            Style.ArrowStyle.END
+            if self._direction == self.Direction.COUNTER_CLOCKWISE
+            else Style.ArrowStyle.START
+        )
+
+        start_angle = (
+            np.pi / 2 if self._orientation == self.Orientation.LEFT else -np.pi / 2
         )
-        self.set_arrow(style)  # Curve object
+
+        self._arc = Arc(center, radius, start_angle, Angle(np.pi)).set_arrow(style)
+        self._label = ArcAnnotation(text, self._arc)
+        super().__init__({"arc": self._arc, "label": self._label})
```

### Comparing `pysketcher-0.0.8/pysketcher/_shape.py` & `pysketcher-0.0.9/pysketcher/_shape.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_simple_support.py` & `pysketcher-0.0.9/pysketcher/_simple_support.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from pysketcher._distance_with_text import DistanceWithText
 from pysketcher._point import Point
 from pysketcher._rectangle import Rectangle
-from pysketcher._text import Text
 from pysketcher._triangle import Triangle
 from pysketcher.composition import Composition
 
 
 class SimpleSupport(Composition):
     """A representation of a simple support.
 
@@ -31,23 +29,23 @@
 
     """
 
     _position: Point
     _size: float
 
     def __init__(self, position: Point, size: float):
-        p0 = Point(position.x - size / 2.0, position.y - size)
-        p1 = Point(position.x + size / 2.0, position.y - size)
-        triangle = Triangle(p0, p1, position)
+        self._position = position
+        self._size = size
+        self._p0 = Point(position.x - size / 2.0, position.y - size)
+        self._p1 = Point(position.x + size / 2.0, position.y - size)
+        self._triangle = Triangle(self._p0, self._p1, position)
         gap = size / 5.0
-        h = size / 4.0  # height of rectangle
-        p2 = Point(p0.x, p0.y - gap - h)
-        rectangle = Rectangle(p2, size, h)
-        shapes = {"triangle": triangle, "rectangle": rectangle}
+        self._height = size / 4.0  # height of rectangle
+        self._p2 = Point(self._p0.x, self._p0.y - gap - self._height)
+        self._rectangle = Rectangle(self._p2, self._size, self._height)
+        shapes = {"triangle": self._triangle, "rectangle": self._rectangle}
         super().__init__(shapes)
 
-        self._dimensions = {
-            "position": Text("position", position),
-            "size": DistanceWithText(
-                "size", Point(p2.x, p2.y - size), Point(p2.x + size, p2.y - size)
-            ),
-        }
+    @property
+    def mid_support(self) -> Point:
+        """Returns the midpoint of the base of the support."""
+        return (self._rectangle.lower_left + self._rectangle.lower_right) * 0.5
```

### Comparing `pysketcher-0.0.8/pysketcher/_sketchy_func.py` & `pysketcher-0.0.9/pysketcher/_sketchy_func.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_spline.py` & `pysketcher-0.0.9/pysketcher/_spline.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_spring.py` & `pysketcher-0.0.9/pysketcher/_spring.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_style.py` & `pysketcher-0.0.9/pysketcher/_style.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     _fill_pattern: FillPattern
     _fill_color: Color
     _arrow: ArrowStyle
     _shadow: int
 
     def __init__(self):
         self._line_style = self.LineStyle.SOLID
-        self._line_width = 0.1
+        self._line_width = 1
         self._line_color = self.Color.BLACK
         self._fill_pattern = None
         self._fill_color = None
         self._arrow = None
         self._shadow = None
 
     @property
@@ -178,15 +178,15 @@
     _font_family: FontFamily
     _alignment: Alignment
 
     def __init__(
         self,
     ):
         super().__init__()
-        self._font_size = 12
+        self._font_size = 18
         self._font_family = self.FontFamily.SANS
         self._alignment = self.Alignment.CENTER
 
     @property
     def font_size(self) -> float:
         """The size of text."""
         return self._font_size
```

### Comparing `pysketcher-0.0.8/pysketcher/_text.py` & `pysketcher-0.0.9/pysketcher/_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from pysketcher._angle import Angle
 from pysketcher._point import Point
 from pysketcher._shape import Shape
 from pysketcher._style import TextStyle
 
 
 class Text(Shape):
-    """Some text which appears on the drawing at the specified location.
+    """Place `text` on the drawing at the Point(x, y) `position`
 
-    Place `text` at the (x,y) point `position`, with the given
-    fontsize (0 indicates that the default fontsize set in drawing_tool
-    is to be used). The text is centered around `position` if `alignment` is
-    'center'; if 'left', the text starts at `position`, and if
-    'right', the right and of the text is located at `position`.
+    The `text` will be drawn in the given `direction`
 
     Args:
         text: The text to be displayed.
-        position: The position at which the text should be displayed.
-        direction: The direction in which the text should flow.
+        position: Point, The position the text will be displayed at.
+        direction: Point, The direction the text will flow to.
 
     Examples:
         >>> fig = ps.Figure(0.0, 4.0, 0.0, 4.0, MatplotlibBackend)
         >>> code = ps.Text("This is some left text!", Point(2, 1))
         >>> code.style.alignment = ps.TextStyle.Alignment.LEFT
         >>> code.style.line_color = ps.TextStyle.Color.BLUE
         >>> code.style.font_family = ps.TextStyle.FontFamily.SERIF
```

### Comparing `pysketcher-0.0.8/pysketcher/_triangle.py` & `pysketcher-0.0.9/pysketcher/_triangle.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_uniform_load.py` & `pysketcher-0.0.9/pysketcher/_uniform_load.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,16 +22,24 @@
 
             An example of a ``UniformLoad``.
     """
 
     def __init__(
         self, lower_left_corner: Point, width: float, height: float, num_arrows=10
     ):
+        self._lower_left_corner = lower_left_corner
+        self._width = width
+        self._height = height
         box = Rectangle(lower_left_corner, width, height)
         shapes = {"box": box}
         dx = float(width) / (num_arrows - 1)
         for i in range(num_arrows):
             x = lower_left_corner.x + i * dx
             start = Point(x, lower_left_corner.y + height)
             end = Point(x, lower_left_corner.y)
             shapes["arrow%d" % i] = Arrow(start, end)
         super().__init__(shapes)
+
+    @property
+    def mid_top(self) -> Point:
+        """The middle of the top of the load."""
+        return self._lower_left_corner + Point(self._width / 2, self._height)
```

### Comparing `pysketcher-0.0.8/pysketcher/_utils/doc_enum.py` & `pysketcher-0.0.9/pysketcher/_utils/doc_enum.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/_velocity_profile.py` & `pysketcher-0.0.9/pysketcher/_velocity_profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-import logging
 from typing import Callable
 
 from pysketcher._arrow import Arrow
 from pysketcher._line import Line
 from pysketcher._point import Point
 from pysketcher._spline import Spline
 from pysketcher.composition import Composition
 
-logging.basicConfig(level=logging.DEBUG)
-
 
 class VelocityProfile(Composition):
     """A representation of the profile of velocity in laminar flow.
 
     Args:
         start: the point from which the profile should start.
         height: the height of the profile.
```

### Comparing `pysketcher-0.0.8/pysketcher/_wall.py` & `pysketcher-0.0.9/pysketcher/_wall.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         self._end = points[-1]
         self._thickness = thickness
 
         def _displace(point: Point, point_before: Point, point_after: Point):
             # Displaces a point on our curve by thickness.
             # find a normal to the line between the point_before and the point_after
             # then displace by thickness from point in the direction of that normal
-            return point + ((point_after - point_before).normal() * self._thickness)
+            return point + ((point_after - point_before).normal * self._thickness)
 
         # at the start, there isn't a point_before, so use the start point
         new_points: List[Point] = [_displace(points[0], points[0], points[1])]
 
         for i in range(1, len(points) - 1):
             new_points += [_displace(points[i], points[i - 1], points[i + 1])]
```

### Comparing `pysketcher-0.0.8/pysketcher/_wheel.py` & `pysketcher-0.0.9/pysketcher/_wheel.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/backend/backend.py` & `pysketcher-0.0.9/pysketcher/backend/backend.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/backend/matplotlib/_matplotlib_backend.py` & `pysketcher-0.0.9/pysketcher/backend/matplotlib/_matplotlib_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         plt.ion()
         self._x_min = x_min
         self._x_max = x_max
         self._y_min = y_min
         self._y_max = y_max
         self._camera = None
         self._fig = plt.figure(
-            figsize=[x_max - x_min, y_max - y_min], tight_layout=False
+            figsize=[(x_max - x_min) * 3, (y_max - y_min) * 3], tight_layout=False
         )
         self._axes = self._fig.gca()
         self._configure_axes()
 
     def _configure_axes(self):
         self._axes.set_xlim(self._x_min, self._x_max)
         self._axes.set_ylim(self._y_min, self._y_max)
```

### Comparing `pysketcher-0.0.8/pysketcher/backend/matplotlib/_matplotlib_curve.py` & `pysketcher-0.0.9/pysketcher/backend/matplotlib/_matplotlib_curve.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,72 @@
+from copy import copy
 from typing import List
 
 import matplotlib.pyplot as plt
+import numpy as np
 
 import pysketcher as ps
 from pysketcher._style import Style
 from pysketcher.backend.matplotlib._matplotlib_adapter import MatplotlibAdapter
 from pysketcher.backend.matplotlib._matplotlib_style import MatplotlibStyle
 
 
 class MatplotlibCurve(MatplotlibAdapter):
     types: List[type] = [ps.Curve]
 
     def plot(self, curve: ps.Curve, axes: plt.Axes) -> None:
         """Draw a curve with coordinates x and y (arrays)."""
         mpl_style = MatplotlibStyle(curve.style)
 
-        x = curve.xs
-        y = curve.ys
+        xs = curve.xs
+        ys = curve.ys
 
-        [line] = axes.plot(
-            x,
-            y,
-            mpl_style.line_color,
-            linewidth=mpl_style.line_width,
-            linestyle=mpl_style.line_style,
-        )
-        if mpl_style.fill_color or mpl_style.fill_pattern:
-            [line] = plt.fill(
-                x,
-                y,
-                mpl_style.fill_color,
-                edgecolor=mpl_style.line_color,
-                linewidth=mpl_style.line_width,
-                hatch=mpl_style.fill_pattern,
-            )
+        if len(xs) == 2 and curve.style.arrow == Style.ArrowStyle.DOUBLE:
+            # For multi-segment curves we can just make the first segment an
+            # arrow if the style is START or DOUBLE and the last segment an
+            # arrow if the style is END or DOUBLE. If there is only one segment
+            # and the style is DOUBLE this won't work, so we split into two segments
+            xs = np.linspace(xs[0], xs[1], 3)
+            ys = np.linspace(ys[0], ys[1], 3)
 
         if curve.style.arrow is not None:
             if curve.style.arrow in [Style.ArrowStyle.START, Style.ArrowStyle.DOUBLE]:
-                x_s, y_s = x[0], y[0]
-                dx_s, dy_s = x[1] - x[0], y[1] - y[0]
-                self._plot_arrow(x_s, y_s, dx_s, dy_s, curve.style, axes)
+                x_s, y_s = xs[0], ys[0]
+                dx_s, dy_s = xs[1] - xs[0], ys[1] - ys[0]
+                start_style = copy(curve.style)
+                start_style.arrow = Style.ArrowStyle.END
+                self._plot_arrow(x_s, y_s, dx_s, dy_s, start_style, axes)
+                xs = xs[1:]
+                ys = ys[1:]
             if curve.style.arrow in [Style.ArrowStyle.END, Style.ArrowStyle.DOUBLE]:
-                x_e, y_e = x[-1], y[-1]
-                dx_e, dy_e = x[-2] - x[-1], y[-2] - y[-1]
-                self._plot_arrow(x_e, y_e, dx_e, dy_e, curve.style, axes)
+                x_e, y_e = xs[-2], ys[-2]
+                dx_e, dy_e = xs[-1] - xs[-2], ys[-1] - ys[-2]
+                end_style = copy(curve.style)
+                end_style.arrow = Style.ArrowStyle.START
+                self._plot_arrow(x_e, y_e, dx_e, dy_e, end_style, axes)
+                xs = xs[:-1]
+                ys = ys[:-1]
+
+        if len(xs) >= 2:
+            [line] = axes.plot(
+                xs,
+                ys,
+                mpl_style.line_color,
+                linewidth=mpl_style.line_width,
+                linestyle=mpl_style.line_style,
+            )
+            if mpl_style.fill_color or mpl_style.fill_pattern:
+                [line] = plt.fill(
+                    xs,
+                    ys,
+                    mpl_style.fill_color,
+                    edgecolor=mpl_style.line_color,
+                    linewidth=mpl_style.line_width,
+                    hatch=mpl_style.fill_pattern,
+                )
 
         # if mpl_style.shadow:
         # http://matplotlib.sourceforge.net/users/transforms_tutorial.html
         # #using-offset-transforms-to-create-a-shadow-effect
         # shift the object over 2 points, and down 2 points
         #     dx, dy = mpl_style.shadow / 72.0, -mpl_style.shadow / 72.0
         #     offset = transforms.ScaledTranslation(dx, dy, fig.dpi_scale_trans)
@@ -61,38 +80,30 @@
         #         color="gray",
         #         transform=shadow_transform,
         #         zorder=0.5 * line.get_zorder(),
         #     )
 
     def _plot_arrow(self, x, y, dx, dy, style: Style, axes: plt.Axes):
         """Draw arrow (dx,dy) at (x,y). `style` is '->', '<-' or '<->'."""
+        if style.arrow == Style.ArrowStyle.DOUBLE:
+            raise ValueError("Only a single ended arrow is supported by this method.")
         mpl_style = MatplotlibStyle(style)
-        if style.arrow in [Style.ArrowStyle.START, Style.ArrowStyle.DOUBLE]:
-            axes.arrow(
-                x,
-                y,
-                dx,
-                dy,
-                facecolor=mpl_style.line_color,
-                edgecolor=mpl_style.line_color,
-                linestyle=mpl_style.line_style,
-                linewidth=mpl_style.line_width,
-                head_width=0.1,
-                # head_width=self.arrow_head_width,
-                # width=1,  # width of arrow body in coordinate scale
-                length_includes_head=True,
-                shape="full",
-            )
-        if style.arrow in [Style.ArrowStyle.END, Style.ArrowStyle.DOUBLE]:
-            axes.arrow(
-                x + dx,
-                y + dy,
-                -dx,
-                -dy,
-                facecolor=mpl_style.line_color,
-                edgecolor=mpl_style.line_color,
-                linewidth=mpl_style.line_width,
-                head_width=0.1,
-                # width=1,
-                length_includes_head=True,
-                shape="full",
-            )
+        if style.arrow == Style.ArrowStyle.END:
+            x = x + dx
+            y = y + dy
+            dx = -dx
+            dy = -dy
+        axes.arrow(
+            x,
+            y,
+            dx,
+            dy,
+            facecolor=mpl_style.line_color,
+            edgecolor=mpl_style.line_color,
+            linestyle=mpl_style.line_style,
+            linewidth=mpl_style.line_width,
+            head_width=0.05,
+            # head_width=self.arrow_head_width,
+            # width=1,  # width of arrow body in coordinate scale
+            length_includes_head=True,
+            shape="full",
+        )
```

### Comparing `pysketcher-0.0.8/pysketcher/backend/matplotlib/_matplotlib_style.py` & `pysketcher-0.0.9/pysketcher/backend/matplotlib/_matplotlib_style.py`

 * *Files identical despite different names*

### Comparing `pysketcher-0.0.8/pysketcher/backend/matplotlib/_matplotlib_text.py` & `pysketcher-0.0.9/pysketcher/backend/matplotlib/_matplotlib_text.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         if mpl_style.font_family is not None:
             kwargs["family"] = mpl_style.font_family
         if mpl_style.fill_color is not None:
             kwargs["backgroundcolor"] = mpl_style.fill_color
         if mpl_style.line_color is not None:
             kwargs["color"] = mpl_style.line_color
 
-        rotation_angle = text.direction.angle()
+        rotation_angle = text.direction.angle
         if rotation_angle != 0.0:
             kwargs["rotation"] = rotation_angle
 
         axes.text(
             text.position.x,
             text.position.y,
             text.text,
```

### Comparing `pysketcher-0.0.8/pysketcher/composition/_composition.py` & `pysketcher-0.0.9/pysketcher/composition/_composition.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,19 +190,7 @@
         Returns:
             A dictionary of results.
         """
         ret_dict = {}
         for key, shape in self._shapes.items():
             ret_dict[key] = func(shape)
         return ret_dict
-
-
-class ShapeWithText(Composition):
-    """A convenience class to combine a Shape with a Text Object.
-
-    Args:
-        shape: The shape.
-        text: The text.
-    """
-
-    def __init__(self, shape: Shape, text: Text):
-        super().__init__({"text": text, "shape": shape})
```

### Comparing `pysketcher-0.0.8/setup.py` & `pysketcher-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['pysketcher',
  'pysketcher._utils',
+ 'pysketcher.annotation',
  'pysketcher.backend',
  'pysketcher.backend.matplotlib',
- 'pysketcher.composition']
+ 'pysketcher.composition',
+ 'pysketcher.dimension']
 
 package_data = \
 {'': ['*'], 'pysketcher': ['images/.gitignore']}
 
 install_requires = \
 ['celluloid>=0.2.0,<0.3.0',
  'matplotlib>=3.2.1,<4.0.0',
  'numpy>=1.19.5,<2.0.0',
  'scipy>=1.6.0,<2.0.0']
 
 extras_require = \
-{':python_version <= "3.7"': ['importlib-metadata>=2,<5']}
+{'docs': ['sphinx>=4.1.1,<5.0.0',
+          'sphinx_rtd_theme>=0.5,<1.1',
+          'sphinx-autodoc-typehints>=1.11.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['beam1 = examples.beam1:main']}
 
 setup_kwargs = {
     'name': 'pysketcher',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Geometric Sketching Utility for Python',
     'long_description': '============\n PySketcher\n============\n\n.. image:: https://github.com/rvodden/pysketcher/workflows/Tests/badge.svg\n    :target: https://github.com/rvodden/pysketcher/actions?query=workflow%3ATests+branch%3Amaster\n\n.. image:: https://badgen.net/pypi/v/pysketcher?icon=pypi\n       :target: https://pypi.org/project/pysketcher/\n\n.. image:: https://api.codeclimate.com/v1/badges/eae2c2aa97080fbfed7e/maintainability\n    :target: https://codeclimate.com/github/rvodden/pysketcher/maintainability\n\n.. image:: https://codecov.io/gh/rvodden/pysketcher/branch/master/graph/badge.svg?token=AHCKOL75VY\n    :target: https://codecov.io/gh/rvodden/pysketcher\n\n.. image:: https://readthedocs.org/projects/pysketcher/badge/?version=latest&style=flat\n    :target: https://pysketcher.readthedocs.io/en/latest/\n\n.. image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n    :target: https://github.com/pre-commit/pre-commit\n\n.. image:: https://img.shields.io/badge/hypothesis-tested-brightgreen.svg\n    :target: https://hypothesis.readthedocs.io/\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n\n.. image:: https://badgen.net/github/dependabot/rvodden/pysketcher?icon=github\n    :target: https://github.com/rvodden/pysketcher\n\n**This is alpha software - the interface is likely to change with every release prior to 0.1.0.**\n\nPySketcher is a modern Python library designed to make creating geometric, mathematical and physical diagrams very\neasy.\n\nThis library is continues the legacy of Hans Petter Langtangen. Work done since he sadly passed in 2016 includes:\n\n1. The MatlibplotDraw object is no longer global and is no longer tightly coupled to the shape object. There is now a DrawingTool interface which this class implements.\n\n2. Code is organised into multiple files and published on pypi.\n\n3. Shapes are immutable. This means functions such as ``rotate`` return modified copies of the original shape, rather than altering the shape on which they are called.\n\n4. Angles are in radians not degrees.\n\n5. The Composition object is used more consistently. Previously objects such as Beam were direct children of Shape which led to code repetition.\n\n`Please see the documentation for more information <https://pysketcher.readthedocs.io/en/latest/index.html>`_.\n',
     'author': 'Richard Vodden',
     'author_email': 'richard@vodden.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/rvodden/pysketcher',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pysketcher-0.0.8/PKG-INFO` & `pysketcher-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: pysketcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: Geometric Sketching Utility for Python
 Home-page: https://github.com/rvodden/pysketcher
 License: MIT
 Keywords: sketch,graphics,scientific,engineering,geometry
 Author: Richard Vodden
 Author-email: richard@vodden.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: docs
 Requires-Dist: celluloid (>=0.2.0,<0.3.0)
-Requires-Dist: importlib-metadata (>=2,<5); python_version <= "3.7"
 Requires-Dist: matplotlib (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.19.5,<2.0.0)
 Requires-Dist: scipy (>=1.6.0,<2.0.0)
+Requires-Dist: sphinx (>=4.1.1,<5.0.0); extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints (>=1.11.1,<2.0.0); extra == "docs"
+Requires-Dist: sphinx_rtd_theme (>=0.5,<1.1); extra == "docs"
 Project-URL: Repository, https://github.com/rvodden/pysketcher
 Description-Content-Type: text/x-rst
 
 ============
  PySketcher
 ============
```

