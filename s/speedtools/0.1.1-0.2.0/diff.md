# Comparing `tmp/speedtools-0.1.1.tar.gz` & `tmp/speedtools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtools-0.1.1.tar", last modified: Thu Jun  8 12:11:30 2023, max compression
+gzip compressed data, was "speedtools-0.2.0.tar", last modified: Fri Jun 23 21:02:04 2023, max compression
```

## Comparing `speedtools-0.1.1.tar` & `speedtools-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:11:30.728237 speedtools-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 12:11:13.000000 speedtools-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-08 12:11:30.728237 speedtools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-08 12:11:13.000000 speedtools-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-08 12:11:13.000000 speedtools-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:11:30.728237 speedtools-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-08 12:11:13.000000 speedtools-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:11:30.724237 speedtools-0.1.1/speedtools/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:11:30.728237 speedtools-0.1.1/speedtools/blender/
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/blender/io_nfs4_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/frd_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:11:30.728237 speedtools-0.1.1/speedtools/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/qfs_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/refpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:11:30.728237 speedtools-0.1.1/speedtools/specs/
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/specs/fce.ksy
--rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/specs/frd.ksy
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/specs/fsh.ksy
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/specs/qfs.ksy
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/specs/viv.ksy
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/speedtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/tr_ini.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/track_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-06-08 12:11:13.000000 speedtools-0.1.1/speedtools/viv_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:11:30.728237 speedtools-0.1.1/speedtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-08 12:11:30.000000 speedtools-0.1.1/speedtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-08 12:11:30.000000 speedtools-0.1.1/speedtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:11:30.000000 speedtools-0.1.1/speedtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 12:11:30.000000 speedtools-0.1.1/speedtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 12:11:30.000000 speedtools-0.1.1/speedtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 12:11:30.000000 speedtools-0.1.1/speedtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-23 21:01:49.000000 speedtools-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-23 21:02:04.323625 speedtools-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-23 21:01:49.000000 speedtools-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-23 21:01:49.000000 speedtools-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 21:02:04.323625 speedtools-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-23 21:01:49.000000 speedtools-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/speedtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/speedtools/blender/
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/blender/io_nfs4_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/frd_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/speedtools/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/qfs_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/refpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/speedtools/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/specs/fce.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/specs/frd.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/specs/fsh.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/specs/qfs.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/specs/viv.ksy
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/speedtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/tr_ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/track_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-06-23 21:01:49.000000 speedtools-0.2.0/speedtools/viv_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:02:04.323625 speedtools-0.2.0/speedtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 21:02:04.000000 speedtools-0.2.0/speedtools.egg-info/top_level.txt
```

### Comparing `speedtools-0.1.1/LICENSE` & `speedtools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/PKG-INFO` & `speedtools-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtools
-Version: 0.1.1
+Version: 0.2.0
 Summary: NFS4 HS (PC) resource utilities
 Author: Rafał Kuźnia
 Author-email: rafal.kuznia@protonmail.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -23,35 +23,47 @@
 - tracks
 - cars
 
 Additionally, Blender addon is provided to directly import track and car data.
 
 # Setup (Blender addon version)
 
-1. Open Blender and open the __Scripting__ tab
-2. In console, type paste the following two commands:
+1. Create new empty Blender project and save it
+   > **Warning**: Not saving the project may cause errors during import. The importer saves all texture images to `<project-dir>/images` directory.
+2. Open the __Scripting__ tab
+3. Copy-paste the following two commands into the Blender console:
    ```
    import sys, subprocess
    subprocess.call([sys.executable, "-m", "pip", "install", "speedtools"])
    ```
-   This command will install the `speedtools` package to your Blender Python installation.
+   This command will install the [`speedtools`][1] package to your Blender Python installation.
 
    > **Note**: Python installation that comes with Blender is completely separate from the global Python installation on your system. For this reason, it is necessary to use the Blender scripting console to install the package correctly.
-3. Copy and paste the content of [this](https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py) file to the Blender scripting window.
-4. Click the __▶__ button.
-5. You should see `Track resources` and `Car resources` under `File>Import`.
+4. Copy and paste the content of [this][2] file to the Blender scripting window.
+5. Click the __▶__ button.
+6. You should see `Track resources` and `Car resources` under `File > Import`.
 
 Until I figure out a better way to install Blender addons, this must suffice.
 
 # Setup (command line version)
 
 Install the package from PyPI:
 ```
 pip install speedtools
 ```
 
 Currently, the command line version does not provide any useful functionality.
 
+# Development dependencies
+
+To develop the project the following dependencies must be installed on your system:
+* [Kaitai Struct compiler][3]
+
+Make sure the binary directories are in your `PATH`.
+
 # Known issues and limitations
 
-* Some tracks are not imported with correct textures
 * Tested only with PC tracks
+
+[1]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
+[2]: https://pypi.org/project/speedtools/
+[3]: https://kaitai.io/
```

### Comparing `speedtools-0.1.1/README.md` & `speedtools-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -4,35 +4,47 @@
 - tracks
 - cars
 
 Additionally, Blender addon is provided to directly import track and car data.
 
 # Setup (Blender addon version)
 
-1. Open Blender and open the __Scripting__ tab
-2. In console, type paste the following two commands:
+1. Create new empty Blender project and save it
+   > **Warning**: Not saving the project may cause errors during import. The importer saves all texture images to `<project-dir>/images` directory.
+2. Open the __Scripting__ tab
+3. Copy-paste the following two commands into the Blender console:
    ```
    import sys, subprocess
    subprocess.call([sys.executable, "-m", "pip", "install", "speedtools"])
    ```
-   This command will install the `speedtools` package to your Blender Python installation.
+   This command will install the [`speedtools`][1] package to your Blender Python installation.
 
    > **Note**: Python installation that comes with Blender is completely separate from the global Python installation on your system. For this reason, it is necessary to use the Blender scripting console to install the package correctly.
-3. Copy and paste the content of [this](https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py) file to the Blender scripting window.
-4. Click the __▶__ button.
-5. You should see `Track resources` and `Car resources` under `File>Import`.
+4. Copy and paste the content of [this][2] file to the Blender scripting window.
+5. Click the __▶__ button.
+6. You should see `Track resources` and `Car resources` under `File > Import`.
 
 Until I figure out a better way to install Blender addons, this must suffice.
 
 # Setup (command line version)
 
 Install the package from PyPI:
 ```
 pip install speedtools
 ```
 
 Currently, the command line version does not provide any useful functionality.
 
+# Development dependencies
+
+To develop the project the following dependencies must be installed on your system:
+* [Kaitai Struct compiler][3]
+
+Make sure the binary directories are in your `PATH`.
+
 # Known issues and limitations
 
-* Some tracks are not imported with correct textures
-* Tested only with PC tracks
+* Tested only with PC tracks
+
+[1]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
+[2]: https://pypi.org/project/speedtools/
+[3]: https://kaitai.io/
```

### Comparing `speedtools-0.1.1/pyproject.toml` & `speedtools-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "speedtools"
-version = "0.1.1"
+version = "0.2.0"
 description = "NFS4 HS (PC) resource utilities"
 authors = [{ name = "Rafał Kuźnia" }, { email = "rafal.kuznia@protonmail.com" }]
 readme = { file = 'README.md', content-type = 'text/markdown' }
 dependencies = ["kaitaistruct", "pillow", "click", "more-itertools", "parse"]
 license = { text = "GPL-3.0-or-later" }
 classifiers = [
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
```

### Comparing `speedtools-0.1.1/setup.py` & `speedtools-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools/blender/io_nfs4_import.py` & `speedtools-0.2.0/speedtools/blender/io_nfs4_import.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 from functools import total_ordering
 from itertools import groupby
 from pathlib import Path
 from typing import Any
 
 import bpy
 import mathutils
-from bpy.props import BoolProperty, StringProperty
+from bpy.props import BoolProperty, EnumProperty, StringProperty
 from more_itertools import collapse
 
 from speedtools import TrackData, VivData
 from speedtools.types import (
     Animation,
     BaseMesh,
     DrawableMesh,
+    Light,
     Part,
     Polygon,
     Resource,
     Vector3d,
 )
 from speedtools.utils import export_resource
 
@@ -148,22 +149,56 @@
             for _, bpy_polygon in group:
                 bpy_polygon.use_smooth = True
                 bpy_polygon.material_index = index
         bpy_mesh.validate()
         bpy_obj = bpy.data.objects.new(name, bpy_mesh)
         return bpy_obj
 
+    def make_light_object(self, name: str, light: Light) -> bpy.types.Object:
+        bpy_light = bpy.data.lights.new(name=name, type="POINT")
+        bpy_light.color = light.attributes.color.rgb_float
+        bpy_light.use_custom_distance = True
+        bpy_light.cutoff_distance = 15.0
+        bpy_light.specular_factor = 0.2
+        bpy_light.energy = 500  # type: ignore[attr-defined]
+        bpy_light.use_shadow = False  # type: ignore[attr-defined]
+        bpy_obj = bpy.data.objects.new(name=name, object_data=bpy_light)
+        self.set_object_location(obj=bpy_obj, location=light.location)
+        return bpy_obj
+
 
 class TrackImportStrategy(metaclass=ABCMeta):
     @abstractmethod
     def import_track(self, track: TrackData) -> None:
         pass
 
 
-class TrackImportFlat(TrackImportStrategy, BaseImporter):
+class TrackImportSimple(TrackImportStrategy, BaseImporter):
+    def import_track(self, track: TrackData) -> None:
+        track_collection = bpy.data.collections.new("Track segments")
+        bpy.context.scene.collection.children.link(track_collection)
+        for index, segment in enumerate(track.track_segments):
+            name = f"Track segment {index}"
+            bpy_obj = self.make_drawable_object(name=name, mesh=segment.mesh)
+            track_collection.objects.link(bpy_obj)
+        for index, obj in enumerate(track.objects):
+            name = f"Track object {index}"
+            bpy_obj = self.make_drawable_object(name=name, mesh=obj.mesh)
+            if obj.location:
+                self.set_object_location(obj=bpy_obj, location=obj.location)
+            if obj.animation:
+                self.set_object_animation(obj=bpy_obj, animation=obj.animation)
+            track_collection.objects.link(bpy_obj)
+        for index, light in enumerate(track.lights):
+            name = f"Track light {index}"
+            bpy_obj = self.make_light_object(name=name, light=light)
+            track_collection.objects.link(bpy_obj)
+
+
+class TrackImportAdvanced(TrackImportStrategy, BaseImporter):
     def import_track(self, track: TrackData) -> None:
         track_collection = bpy.data.collections.new("Track segments")
         bpy.context.scene.collection.children.link(track_collection)
         for index, segment in enumerate(track.track_segments):
             name = f"Track segment {index}"
             bpy_obj = self.make_drawable_object(name=name, mesh=segment.mesh)
             track_collection.objects.link(bpy_obj)
@@ -181,23 +216,15 @@
             if obj.location:
                 self.set_object_location(obj=bpy_obj, location=obj.location)
             if obj.animation:
                 self.set_object_animation(obj=bpy_obj, animation=obj.animation)
             track_collection.objects.link(bpy_obj)
         for index, light in enumerate(track.lights):
             name = f"Track light {index}"
-            bpy_light = bpy.data.lights.new(name=name, type="POINT")
-            bpy_light.color = light.attributes.color.rgb_float
-            bpy_light.use_custom_distance = True
-            bpy_light.cutoff_distance = 15.0
-            bpy_light.specular_factor = 0.2
-            bpy_light.energy = 500  # type: ignore[attr-defined]
-            bpy_light.use_shadow = False  # type: ignore[attr-defined]
-            bpy_obj = bpy.data.objects.new(name=name, object_data=bpy_light)
-            self.set_object_location(obj=bpy_obj, location=light.location)
+            bpy_obj = self.make_light_object(name=name, light=light)
             track_collection.objects.link(bpy_obj)
 
 
 class CarImporterSimple(BaseImporter):
     def import_car(self, parts: Iterable[Part]) -> None:
         car_collection = bpy.data.collections.new("Car parts")
         bpy.context.scene.collection.children.link(car_collection)
@@ -219,14 +246,31 @@
 
     directory: StringProperty(  # type: ignore[valid-type]
         name="Directory Path",
         description="Directory containing the track files",
         maxlen=1024,
         default="",
     )
+    mode: EnumProperty(  # type: ignore[valid-type]
+        name="Mode",
+        items=(
+            (
+                "SIMPLE",
+                "Simple",
+                "Import only visible track geometry, lights and animations.",
+            ),
+            (
+                "ADVANCED",
+                "Advanced (experimental)",
+                "Parametrized import of visible track geometry, lights, animations, "
+                "collision geometry and more",
+            ),
+        ),
+        description="Select importer mode",
+    )
     night: BoolProperty(  # type: ignore[valid-type]
         name="Night on", description="Import night track variant", default=False
     )
     weather: BoolProperty(  # type: ignore[valid-type]
         name="Weather on", description="Import rainy track variant", default=False
     )
     mirrored: BoolProperty(  # type: ignore[valid-type]
@@ -241,15 +285,21 @@
     def execute(self, context: bpy.types.Context) -> set[int] | set[str]:
         track = TrackData(
             directory=self.directory,
             mirrored=self.mirrored,
             night=self.night,
             weather=self.weather,
         )
-        import_strategy = TrackImportFlat(material_map=track.get_polygon_material)
+        import_strategy: TrackImportStrategy
+        if self.mode == "SIMPLE":
+            import_strategy = TrackImportSimple(material_map=track.get_polygon_material)
+        elif self.mode == "ADVANCED":
+            import_strategy = TrackImportAdvanced(material_map=track.get_polygon_material)
+        else:
+            return {"CANCELLED"}
         import_strategy.import_track(track=track)
         return {"FINISHED"}
 
 
 class CarImporter(bpy.types.Operator):
     """Import NFS4 Car Operator"""
```

### Comparing `speedtools-0.1.1/speedtools/frd_data.py` & `speedtools-0.2.0/speedtools/frd_data.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools/qfs_data.py` & `speedtools-0.2.0/speedtools/qfs_data.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools/refpack.py` & `speedtools-0.2.0/speedtools/refpack.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools/specs/fce.ksy` & `speedtools-0.2.0/speedtools/specs/fce.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools/specs/frd.ksy` & `speedtools-0.2.0/speedtools/specs/frd.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools/specs/fsh.ksy` & `speedtools-0.2.0/speedtools/specs/fsh.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools/specs/viv.ksy` & `speedtools-0.2.0/speedtools/specs/viv.ksy`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools/speedtool.py` & `speedtools-0.2.0/speedtools/speedtool.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools/tr_ini.py` & `speedtools-0.2.0/speedtools/tr_ini.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools/track_data.py` & `speedtools-0.2.0/speedtools/track_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     LightAttributes,
     LightStub,
     Polygon,
     Resource,
     TrackObject,
     TrackSegment,
 )
+from speedtools.utils import count_repeats_and_map
 
 logger = logging.getLogger(__name__)
 T = TypeVar("T")
 
 
 class TrackData:
     def __init__(
@@ -107,28 +108,39 @@
     def track_segments(self) -> Iterator[TrackSegment]:
         return self.frd.track_segments
 
     @property
     def track_resources(self) -> Iterator[Resource]:
         return self.qfs.resources
 
+    @classmethod
+    def _make_unique_resource_name(cls, resource: Resource, repeats: int) -> Resource:
+        if repeats == 0:
+            return resource
+        return Resource(
+            name=f"{resource.name}-{repeats}",
+            image=resource.image,
+            mirrored=resource.mirrored,
+            nonmirrored=resource.nonmirrored,
+            additive=resource.additive,
+        )
+
+    def _init_resources(self) -> None:
+        if self.mirrored:
+            resources = filter(lambda resource: not resource.nonmirrored, self.qfs.resources)
+        else:
+            resources = filter(lambda resource: not resource.mirrored, self.qfs.resources)
+        unique_named_resources = count_repeats_and_map(
+            iterable=resources, func=self._make_unique_resource_name, key=lambda x: x.name
+        )
+        self.resources = dict(enumerate(unique_named_resources))
+
     def get_polygon_material(self, polygon: Polygon) -> Resource:
         if not self.resources:
-            if self.mirrored:
-                resources = filter(
-                    lambda resource: resource.mirrored or not resource.nonmirrored,
-                    self.qfs.resources,
-                )
-            else:
-                resources = filter(
-                    lambda resource: resource.nonmirrored or not resource.mirrored,
-                    self.qfs.resources,
-                )
-            for index, resource in enumerate(resources):
-                self.resources[index] = resource
+            self._init_resources()
         return self.resources[polygon.material]
 
     def _make_light(self, stub: LightStub) -> Light:
         attributes = self.light_glows[stub.glow_id]
         return Light(location=stub.location, attributes=attributes)
 
     @property
```

### Comparing `speedtools-0.1.1/speedtools/types.py` & `speedtools-0.2.0/speedtools/types.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools/utils.py` & `speedtools-0.2.0/speedtools/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,35 +3,46 @@
 # Copyright (c) 2023 Rafał Kuźnia <rafal.kuznia@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 
 import logging
 import os
-from collections.abc import Iterable, Iterator
+from collections.abc import Callable, Hashable, Iterable, Iterator
 from contextlib import suppress
 from functools import singledispatch
 from io import BytesIO
 from itertools import islice
 from pathlib import Path
-from typing import Any, TypeVar
+from typing import Any, Dict, TypeVar
 
 from PIL import Image as pil_Image
 
 from speedtools.types import Bitmap, Image, Resource
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
+Ty = TypeVar("Ty")
 
 
 def islicen(iterable: Iterable[T], start: int, num: int) -> Iterable[T]:
     return islice(iterable, start, start + num)
 
 
+def count_repeats_and_map(
+    iterable: Iterable[T], func: Callable[[T, int], Ty], key: Callable[[T], Hashable]
+) -> Iterable[Ty]:
+    count: Dict[Hashable, int] = {}
+    for item in iterable:
+        k = key(item)
+        count[k] = count.setdefault(k, -1) + 1
+        yield func(item, count[k])
+
+
 @singledispatch
 def create_pil_image(image: Image) -> Any:
     buffer = BytesIO(image.data)
     return pil_Image.open(fp=buffer)
 
 
 @create_pil_image.register
```

### Comparing `speedtools-0.1.1/speedtools/viv_data.py` & `speedtools-0.2.0/speedtools/viv_data.py`

 * *Files identical despite different names*

### Comparing `speedtools-0.1.1/speedtools.egg-info/PKG-INFO` & `speedtools-0.2.0/speedtools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtools
-Version: 0.1.1
+Version: 0.2.0
 Summary: NFS4 HS (PC) resource utilities
 Author: Rafał Kuźnia
 Author-email: rafal.kuznia@protonmail.com
 License: GPL-3.0-or-later
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -23,35 +23,47 @@
 - tracks
 - cars
 
 Additionally, Blender addon is provided to directly import track and car data.
 
 # Setup (Blender addon version)
 
-1. Open Blender and open the __Scripting__ tab
-2. In console, type paste the following two commands:
+1. Create new empty Blender project and save it
+   > **Warning**: Not saving the project may cause errors during import. The importer saves all texture images to `<project-dir>/images` directory.
+2. Open the __Scripting__ tab
+3. Copy-paste the following two commands into the Blender console:
    ```
    import sys, subprocess
    subprocess.call([sys.executable, "-m", "pip", "install", "speedtools"])
    ```
-   This command will install the `speedtools` package to your Blender Python installation.
+   This command will install the [`speedtools`][1] package to your Blender Python installation.
 
    > **Note**: Python installation that comes with Blender is completely separate from the global Python installation on your system. For this reason, it is necessary to use the Blender scripting console to install the package correctly.
-3. Copy and paste the content of [this](https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py) file to the Blender scripting window.
-4. Click the __▶__ button.
-5. You should see `Track resources` and `Car resources` under `File>Import`.
+4. Copy and paste the content of [this][2] file to the Blender scripting window.
+5. Click the __▶__ button.
+6. You should see `Track resources` and `Car resources` under `File > Import`.
 
 Until I figure out a better way to install Blender addons, this must suffice.
 
 # Setup (command line version)
 
 Install the package from PyPI:
 ```
 pip install speedtools
 ```
 
 Currently, the command line version does not provide any useful functionality.
 
+# Development dependencies
+
+To develop the project the following dependencies must be installed on your system:
+* [Kaitai Struct compiler][3]
+
+Make sure the binary directories are in your `PATH`.
+
 # Known issues and limitations
 
-* Some tracks are not imported with correct textures
 * Tested only with PC tracks
+
+[1]: https://github.com/e-rk/speedtools/blob/master/speedtools/blender/io_nfs4_import.py
+[2]: https://pypi.org/project/speedtools/
+[3]: https://kaitai.io/
```

### Comparing `speedtools-0.1.1/speedtools.egg-info/SOURCES.txt` & `speedtools-0.2.0/speedtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

