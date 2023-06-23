# Comparing `tmp/meshwell-0.0.1.tar.gz` & `tmp/meshwell-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshwell-0.0.1.tar", last modified: Sat May  6 23:37:39 2023, max compression
+gzip compressed data, was "meshwell-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `meshwell-0.0.1.tar` & `meshwell-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-04-10 22:02:02.583866 meshwell-0.0.1/LICENSE
--rw-r--r--   0        0        0     2187 2023-05-06 12:42:43.352131 meshwell-0.0.1/README.md
--rw-r--r--   0        0        0      137 2023-05-05 20:47:25.186466 meshwell-0.0.1/meshwell/__init__.py
--rw-r--r--   0        0        0      465 2023-05-05 20:47:24.446464 meshwell-0.0.1/meshwell/config.py
--rw-r--r--   0        0        0     1207 2023-05-05 20:47:25.336466 meshwell-0.0.1/meshwell/entity.py
--rw-r--r--   0        0        0     2906 2023-05-05 20:47:25.336466 meshwell-0.0.1/meshwell/geometry.py
--rw-r--r--   0        0        0     3767 2023-05-05 20:47:24.826465 meshwell-0.0.1/meshwell/mesh.msh
--rw-r--r--   0        0        0     5789 2023-05-06 22:09:41.894758 meshwell-0.0.1/meshwell/mesh.py
--rw-r--r--   0        0        0    12379 2023-05-06 16:06:39.804750 meshwell-0.0.1/meshwell/mesh2D.msh
--rw-r--r--   0        0        0   114374 2023-05-06 16:06:40.244750 meshwell-0.0.1/meshwell/mesh3D.msh
--rw-r--r--   0        0        0     2976 2023-05-06 22:09:41.894758 meshwell-0.0.1/meshwell/polysurface.py
--rw-r--r--   0        0        0     7798 2023-05-06 22:09:41.894758 meshwell-0.0.1/meshwell/prism.py
--rw-r--r--   0        0        0      747 2023-05-05 20:47:25.266466 meshwell-0.0.1/meshwell/refinement.py
--rw-r--r--   0        0        0     1744 2023-05-05 20:47:25.336466 meshwell-0.0.1/meshwell/tag.py
--rw-r--r--   0        0        0      527 2023-05-05 20:48:07.536477 meshwell-0.0.1/meshwell/validation.py
--rw-r--r--   0        0        0     3235 2023-05-06 21:35:31.254729 meshwell-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3662 1970-01-01 00:00:00.000000 meshwell-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-23 20:43:34.791260 meshwell-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2866 2023-06-23 20:43:34.791260 meshwell-0.0.2/README.md
+-rw-r--r--   0        0        0      137 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/__init__.py
+-rw-r--r--   0        0        0      465 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/config.py
+-rw-r--r--   0        0        0     1315 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/labeledentity.py
+-rw-r--r--   0        0        0    10669 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/model.py
+-rw-r--r--   0        0        0     2435 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/polysurface.py
+-rw-r--r--   0        0        0     5973 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/prism.py
+-rw-r--r--   0        0        0      715 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/refinement.py
+-rw-r--r--   0        0        0     2220 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/tag.py
+-rw-r--r--   0        0        0      527 2023-06-23 20:43:34.799260 meshwell-0.0.2/meshwell/validation.py
+-rw-r--r--   0        0        0     3235 2023-06-23 20:43:34.799260 meshwell-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 meshwell-0.0.2/PKG-INFO
```

### Comparing `meshwell-0.0.1/LICENSE` & `meshwell-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.1/meshwell/entity.py` & `meshwell-0.0.2/meshwell/labeledentity.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import gmsh
 
 
 class LabeledEntities:
-    """Class to track entities, boundaries, and physical labels."""
+    """Class to track entities, boundaries, and physical labels during meshing."""
 
-    def __init__(self, model, index, dimtags, label, base_resolution):
-        self.model = model
+    def __init__(self, index, dimtags, label, base_resolution, keep, model):
         self.index = index
+        self.model = model
         self.dimtags = self._fuse_self(dimtags)
         self.label = label
         self.base_resolution = base_resolution
         self.boundaries = self.update_boundaries()
         self.interfaces = []
+        self.keep = keep
 
     def _fuse_self(self, dimtags):
-        if len(dimtags) != 1:
-            dimtags = self.model.fuse(
+        if len(dimtags) == 0:
+            return []
+        elif len(dimtags) != 1:
+            dimtags = gmsh.model.occ.fuse(
                 [dimtags[0]],
                 dimtags[1:],
                 removeObject=True,
                 removeTool=True,
             )[0]
-            self.model.synchronize()
+            self.model.occ.synchronize()
         return dimtags
 
     def get_tags(self):
         tags = [tag for dim, tag in self.dimtags]
         if any(isinstance(el, list) for el in tags):
             tags = [item for sublist in tags for item in sublist]
         return tags
```

### Comparing `meshwell-0.0.1/meshwell/geometry.py` & `meshwell-0.0.2/meshwell/polysurface.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,73 @@
-class Geometry:
+class PolySurface:
     """
-    Base Geometry class inherited by Prism and PolySurface.
+    Creates bottom-up GMSH polygonal surfaces formed by list of shapely (multi)polygon.
 
     Attributes:
         polygons: list of shapely (Multi)Polygon
-        buffers: dict of {z: buffer} used to shrink/grow base polygons at specified z-values
         model: GMSH model to synchronize
     """
 
     def __init__(
         self,
-        model,
         polygons,
-        buffers,
+        model,
     ):
-        self.model = model
-
-        # Parse buffers
-        self.buffered_polygons = self._get_buffered_polygons(polygons, buffers)
+        # Parse (multi)polygons
+        self.polygons = list(
+            polygons.geoms if hasattr(polygons, "geoms") else [polygons]
+        )
 
         # Track gmsh entities for bottom-up volume definition
-        self.points = {}
-        self.segments = {}
+        self.model = model
 
-    def _add_get_point(self, x, y, z):
-        """Add a point to the model, or reuse a previously-defined point.
-        Args:
-            x: float, x-coordinate
-            y: float, y-coordinate
-            z: float, z-coordinate
-        Returns:
-            ID of the added or retrieved point
-        """
-        if (x, y, z) not in self.points.keys():
-            self.points[(x, y, z)] = self.model.add_point(x, y, z)
-        return self.points[(x, y, z)]
-
-    def _add_get_segment(self, xyz1, xyz2):
-        """Add a segment (2-point line) to the gmsh model, or retrieve a previously-defined segment.
-        The OCC kernel does not care about orientation.
-        Args:
-            xyz1: first [x,y,z] coordinate
-            xyz2: second [x,y,z] coordinate
-        Returns:
-            ID of the added or retrieved line segment
-        """
-        if (xyz1, xyz2) in self.segments.keys():
-            return self.segments[(xyz1, xyz2)]
-        elif (xyz2, xyz1) in self.segments.keys():
-            return self.segments[(xyz2, xyz1)]
-        else:
-            self.segments[(xyz1, xyz2)] = self.model.add_line(
-                self._add_get_point(xyz1[0], xyz1[1], xyz1[2]),
-                self._add_get_point(xyz2[0], xyz2[1], xyz2[2]),
+    def _parse_coords(self, coords):
+        """Chooses z=0 if the provided coordinates are 2D."""
+        return (coords[0], coords[1], 0) if len(coords) == 2 else coords
+
+    def get_gmsh_polygons(self):
+        """Returns the fused GMSH surfaces within model from the polygons."""
+        surfaces = [self.add_surface_with_holes(entry) for entry in self.polygons]
+        if len(surfaces) <= 1:
+            return surfaces
+        dimtags = self.model.occ.fuse(
+            [(2, surfaces[0])],
+            [(2, tag) for tag in surfaces[1:]],
+            removeObject=True,
+            removeTool=True,
+        )[0]
+        self.model.occ.synchronize()
+        return [tag for dim, tag in dimtags]
+
+    def add_surface_with_holes(self, polygon):
+        """Returns surface, removing intersection with hole surfaces."""
+        exterior = self.model.add_surface(
+            [self._parse_coords(coords) for coords in polygon.exterior.coords]
+        )
+        interior_tags = [
+            self.model.add_surface(
+                [self._parse_coords(coords) for coords in interior.coords],
             )
-            return self.segments[(xyz1, xyz2)]
-
-    def _channel_loop_from_vertices(self, vertices):
-        """Add a curve loop from the list of vertices.
-        Args:
-            model: GMSH model
-            vertices: list of [x,y,z] coordinates
-        Returns:
-            ID of the added curve loop
-        """
-        edges = []
-        for vertex1, vertex2 in [
-            (vertices[i], vertices[i + 1]) for i in range(len(vertices) - 1)
-        ]:
-            gmsh_line = self._add_get_segment(vertex1, vertex2)
-            edges.append(gmsh_line)
-        return self.model.add_curve_loop(edges)
-
-    def _add_surface(self, vertices):
-        """Add a surface composed of the segments formed by vertices.
-
-        Args:
-            vertices: List of xyz coordinates, whose subsequent entries define a closed loop.
-        Returns:
-            ID of the added surface
-        """
-        channel_loop = self._channel_loop_from_vertices(vertices)
-        return self.model.add_plane_surface([channel_loop])
+            for interior in polygon.interiors
+        ]
+        for interior_tag in interior_tags:
+            exterior = self.model.occ.cut(
+                [(2, exterior)], [(2, interior_tag)], removeObject=True, removeTool=True
+            )
+            self.model.occ.synchronize()
+            exterior = exterior[0][0][1]  # Parse `outDimTags', `outDimTagsMap'
+        return exterior
+
+    def instanciate(self):
+        polysurface = self.get_gmsh_polygons()
+        self.model.occ.synchronize()
+        return [(2, polysurface)]
+
+
+# def PolySurface(
+#     polygons,
+#     model,
+# ):
+#     """Functional wrapper around PolySurfaceClass."""
+#     polysurface = PolySurfaceClass(polygons=polygons, model=model).get_gmsh_polygons()
+#     model.occ.synchronize()
+#     return polysurface
```

### Comparing `meshwell-0.0.1/meshwell/tag.py` & `meshwell-0.0.2/meshwell/tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,19 +22,32 @@
         else:
             common_interfaces = list(
                 set(entity1.boundaries).intersection(entity2.boundaries)
             )
             # Remember which boundaries were interfaces with another entity
             entity1.interfaces.extend(common_interfaces)
             entity2.interfaces.extend(common_interfaces)
-            gmsh.model.addPhysicalGroup(
-                max_dim - 1,
-                common_interfaces,
-                name=f"{entity1.label}{boundary_delimiter}{entity2.label}",
-            )
+            if entity1.keep is False:
+                gmsh.model.addPhysicalGroup(
+                    max_dim - 1,
+                    common_interfaces,
+                    name=f"{entity1.label}",
+                )
+            elif entity2.keep is False:
+                gmsh.model.addPhysicalGroup(
+                    max_dim - 1,
+                    common_interfaces,
+                    name=f"{entity2.label}",
+                )
+            else:
+                gmsh.model.addPhysicalGroup(
+                    max_dim - 1,
+                    common_interfaces,
+                    name=f"{entity1.label}{boundary_delimiter}{entity2.label}",
+                )
 
     return entity_list
 
 
 def tag_boundaries(entity_list, max_dim, boundary_delimiter, mesh_edge_name):
     """Adds physical labels to the boundaries of the entities in entity_list."""
     for entity in entity_list:
```

### Comparing `meshwell-0.0.1/meshwell/validation.py` & `meshwell-0.0.2/meshwell/validation.py`

 * *Files identical despite different names*

### Comparing `meshwell-0.0.1/pyproject.toml` & `meshwell-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 	"Programming Language :: Python :: 3.7",
 	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Operating System :: OS Independent",
 ]
-version="0.0.1"
+version="0.0.2"
 authors = [
     {name = "Simon Bilodeau", email = "sb30@princeton.edu"},
 ]
 keywords = ["python"]
 license = {file = "LICENSE"}
 dependencies = [
     "shapely",
     "gmsh",
+    "meshio"
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 tests = ["pytest", "pytest-cov"]
 dev = [
@@ -34,15 +35,14 @@
     "pytest",
     "pytest-cov",
     "pytest_regressions",
     ]
 full = [
     "matplotlib",
     "scikit-fem",
-    "meshio"
 ]
 docs = [
     "jupytext",
     "autodoc_pydantic",
     "jupytext",
     "jupyter-book==0.15.1",
     "sphinx-autodoc-typehints",
```

### Comparing `meshwell-0.0.1/PKG-INFO` & `meshwell-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: meshwell
-Version: 0.0.1
+Version: 0.0.2
 Summary: GMSH wrapper, with integrated photonics focus
 Keywords: python
 Author-email: Simon Bilodeau <sb30@princeton.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Dist: shapely
 Requires-Dist: gmsh
+Requires-Dist: meshio
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest_regressions ; extra == "dev"
 Requires-Dist: jupytext ; extra == "docs"
 Requires-Dist: autodoc_pydantic ; extra == "docs"
 Requires-Dist: jupytext ; extra == "docs"
@@ -25,28 +26,35 @@
 Requires-Dist: sphinx-autodoc-typehints ; extra == "docs"
 Requires-Dist: sphinx-click ; extra == "docs"
 Requires-Dist: matplotlib ; extra == "docs"
 Requires-Dist: scikit-fem ; extra == "docs"
 Requires-Dist: meshio ; extra == "docs"
 Requires-Dist: matplotlib ; extra == "full"
 Requires-Dist: scikit-fem ; extra == "full"
-Requires-Dist: meshio ; extra == "full"
 Requires-Dist: pytest ; extra == "tests"
 Requires-Dist: pytest-cov ; extra == "tests"
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: full
 Provides-Extra: tests
 
+# Meshwell
 <p align="center">
-  <img src="meshwell.png" width="300" height="300">
+  <img src=https://raw.githubusercontent.com/simbilod/meshwell/main/meshwell.png
+ width="300" height="300">
 </p>
 
 ---
 
+[![Docs](https://github.com/simbilod/meshwell/actions/workflows/pages.yml/badge.svg)](https://github.com/simbilod/meshwell/actions/workflows/pages.yml)
+[![Tests](https://github.com/simbilod/meshwell/actions/workflows/test_code.yml/badge.svg)](https://github.com/simbilod/meshwell/actions/workflows/test_code.yml)
+[![PiPy](https://img.shields.io/pypi/v/meshwell)](https://pypi.org/project/meshwell/)
+
+**Project is under active development, stay tuned for improved features, documentation, and releases!**
+
 Meshwell is a Python wrapper around [GMSH](https://gmsh.info/) that provides:
 
 (1) a Prism class that simplifies, to the point of automating, the definition of solids from arbitrary (multi)polygons with "buffered" extrusions;
 
 (2) a simple API where such Prisms and regular GMSH OCC objects are specified in an ordered dictionary of mesh priority, and whose keys are then used to label the mesh entities and their interfaces unambiguously;
 
 For instance:
@@ -64,12 +72,14 @@
 * [femwell](https://github.com/HelgeGehring/femwell): open-source scikit-fem based finite-element simulations, with emphasis on photonics
 * [DEVSIM](https://github.com/devsim/devsim): open-source finite-volume simulator, with emphasis on semiconductor TCAD
 
 ### Other notable GMSH Python interfaces:
 * [gmsh](https://gitlab.onelab.info/gmsh/gmsh): the gmsh Python API itself has significantly improved over the years
 * [pygmsh](https://github.com/meshpro/pygmsh): manipulate Python objects instead of gmsh entity tags
 * [objectgmsh](https://github.com/nemocrys/objectgmsh): class wrappers around entities
+* [gyptis](https://gyptis.gitlab.io/): uses basic gmsh for photonic geometries
 
-### Contributors
+###
+* Simon Bilodeau (Princeton): maintainer
 * Helge Gehring (Google X): beta testing, use cases, bug fixes
 * Joaquin Matres Abril (Google X): code improvements
```

