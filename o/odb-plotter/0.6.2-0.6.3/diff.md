# Comparing `tmp/odb-plotter-0.6.2.tar.gz` & `tmp/odb-plotter-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.6.2.tar", last modified: Thu Jun 22 18:34:47 2023, max compression
+gzip compressed data, was "odb-plotter-0.6.3.tar", last modified: Thu Jun 22 22:32:00 2023, max compression
```

## Comparing `odb-plotter-0.6.2.tar` & `odb-plotter-0.6.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.2/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     3949 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)     1983 2023-06-22 18:34:28.000000 odb-plotter-0.6.2/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1294 2023-06-22 16:06:55.000000 odb-plotter-0.6.2/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.511051 odb-plotter-0.6.2/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.511051 odb-plotter-0.6.2/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     3949 2023-06-22 18:34:47.000000 odb-plotter-0.6.2/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-06-22 18:34:47.000000 odb-plotter-0.6.2/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-22 18:34:47.000000 odb-plotter-0.6.2/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      156 2023-06-22 18:34:47.000000 odb-plotter-0.6.2/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-22 18:34:47.000000 odb-plotter-0.6.2/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-22 18:34:28.000000 odb-plotter-0.6.2/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.2/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.2/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.2/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)    36534 2023-06-22 18:34:28.000000 odb-plotter-0.6.2/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.2/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 18:34:47.514384 odb-plotter-0.6.2/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)     9751 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/py2_scripts/converter.py
--rw-r--r--   0 clark     (1000) clark     (1000)     5298 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/py2_scripts/extractor.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3079 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/py2_scripts/state_collector.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/reader.py
--rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/util.py
--rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.2/src/odbp/writer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-06-02 13:55:59.000000 odb-plotter-0.6.3/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     3991 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)     2025 2023-06-22 22:31:54.000000 odb-plotter-0.6.3/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1298 2023-06-22 22:29:35.000000 odb-plotter-0.6.3/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.644376 odb-plotter-0.6.3/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     3991 2023-06-22 22:32:00.000000 odb-plotter-0.6.3/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      559 2023-06-22 22:32:00.000000 odb-plotter-0.6.3/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-06-22 22:32:00.000000 odb-plotter-0.6.3/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      166 2023-06-22 22:32:00.000000 odb-plotter-0.6.3/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-06-22 22:32:00.000000 odb-plotter-0.6.3/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-06-22 22:31:54.000000 odb-plotter-0.6.3/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.6.3/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    24792 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-06-01 00:43:21.000000 odb-plotter-0.6.3/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.6.3/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)    37294 2023-06-22 22:29:35.000000 odb-plotter-0.6.3/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     4851 2023-06-12 22:11:39.000000 odb-plotter-0.6.3/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-06-22 22:32:00.647709 odb-plotter-0.6.3/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)     9751 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/py2_scripts/converter.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     5298 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/py2_scripts/extractor.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3079 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/py2_scripts/state_collector.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2336 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/reader.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    26816 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2242 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/util.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     3938 2023-06-21 18:29:07.000000 odb-plotter-0.6.3/src/odbp/writer.py
```

### Comparing `odb-plotter-0.6.2/LICENSE` & `odb-plotter-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.2/PKG-INFO` & `odb-plotter-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -27,16 +27,16 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://www.cmml.me.msstate.edu
 Project-URL: Bug Reports, https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter/issues
 Project-URL: Source, https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter
 Keywords: abaqus,abq,fea,odb,waam,wa-ded,visualization
 Description-Content-Type: text/markdown
-Provides-Extra: plot
 Provides-Extra: all
+Provides-Extra: plot
 License-File: LICENSE
 
 # ODB Plotter
 
 ## Constraints:
 ODB Plotter is being developed by [CMML](https://www.cmml.me.msstate.edu), and as such has a focus on Additive Manufacturing and Temperature Data.
 
@@ -73,12 +73,13 @@
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
+    * 0.6.3: Actually filtering 3D plots.
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.2/README.md` & `odb-plotter-0.6.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,12 +36,13 @@
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
+    * 0.6.3: Actually filtering 3D plots.
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.2/pyproject.toml` & `odb-plotter-0.6.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,20 +14,18 @@
 "tomli_w",
 "pandas",
 "pyreadline3; platform_system == 'Windows'",
 ]
 dynamic = ["version",]
 
 [project.optional-dependencies]
+all = ['odb-plotter[plot]',]
 plot = [
     'pyvista',
 ]
-all = [
-    'pyvista',
-]
 
 [project.urls]
 "Homepage" = "https://www.cmml.me.msstate.edu"
 "Bug Reports" = "https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter/issues"
 "Source" = "https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter"
 
 [tool.setuptools]
```

### Comparing `odb-plotter-0.6.2/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.6.3/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python3 API for Abaqus .odb Files and related Command Line Visualization Tool. Focused on Additive Manufacturing Thermal Transfer
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
         
@@ -27,16 +27,16 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://www.cmml.me.msstate.edu
 Project-URL: Bug Reports, https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter/issues
 Project-URL: Source, https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter
 Keywords: abaqus,abq,fea,odb,waam,wa-ded,visualization
 Description-Content-Type: text/markdown
-Provides-Extra: plot
 Provides-Extra: all
+Provides-Extra: plot
 License-File: LICENSE
 
 # ODB Plotter
 
 ## Constraints:
 ODB Plotter is being developed by [CMML](https://www.cmml.me.msstate.edu), and as such has a focus on Additive Manufacturing and Temperature Data.
 
@@ -73,12 +73,13 @@
     * 0.5.1: Implement new system information (pypi tags, this changelog)
     * 0.5.2: Returning support to Python 3.8+ (type hinting)
     * 0.5.3: Patching conversion bugs
     * 0.5.4: Parametrize number of cpus for testing
 * 0.6.0: Extractor improvements, ODB interface tools (iteration, receiving ODB data), re-implementation of basic 3D plots over time (including melt-pool plots). Created two-dimensional plotting capabilities
     * 0.6.1: Update notices if pyvista isn't installed
     * 0.6.2: Improve data extraction for plotting. Ensure that plotting doesn't fork-bomb
+    * 0.6.3: Actually filtering 3D plots.
 * Upcoming:
     * 0.7.0: Improve user settings, parameterization, metadata. Let users select plotting colors, keep metadata of nodesets or spatial, thermal, temporal bounds within the .hdf5.
     * 0.8.0: Improve pyvista functionality: views, gifs, non-interactive image saving, leave the viewer.
     * 0.9.0: Rewrite CLI to use python's cmd module and pyreadline/GNU readline.
     * 1.0.0: Final bug-fixing, type checking, bounds checking, etc. Hopefully coinciding with (or following) a publication.
```

### Comparing `odb-plotter-0.6.2/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.6.3/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.2/src/odbp/cli.py` & `odb-plotter-0.6.3/src/odbp/cli.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.2/src/odbp/data/config.toml` & `odb-plotter-0.6.3/src/odbp/data/config.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.2/src/odbp/odb.py` & `odb-plotter-0.6.3/src/odbp/odb.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,31 +110,22 @@
         """
 
         self._odb_handler: Union[OdbLoader, OdbUnloader] = OdbLoader()
         self._odb: DataFrameType 
 
         self._odb_path: pathlib.Path
         self._odb_source_dir: Optional[pathlib.Path]
-        self._odb_source_dir = pathlib.Path(
-            pathlib.Path(__file__).parent,
-            "odbs",
-            ).absolute()
+        self._odb_source_dir = pathlib.Path.cwd().absolute() / "odbs"
 
         self._hdf_path: pathlib.Path
         self._hdf_source_dir: Optional[pathlib.Path]
-        self._hdf_source_dir = pathlib.Path(
-            pathlib.Path(__file__).parent,
-            "hdfs",
-            ).absolute()
+        self._hdf_source_dir = pathlib.Path.cwd().absolute() / "hdfs"
 
         self._result_dir: Optional[pathlib.Path]
-        self._result_dir = pathlib.Path(
-            pathlib.Path(__file__),
-            "results",
-        ).absolute()
+        self._result_dir = pathlib.Path.cwd().absolute() / "results"
 
         self._abaqus_executable: str = "abaqus"
 
         self._nodes: NullableNodeType = None
         self._nodesets: NullableStrList = None
         self._frames: NullableIntList = None
         self._parts: NullableStrList = None
@@ -1120,25 +1111,26 @@
                 label="Mean Temperature")
 
         if mean_max_both.lower() in ("max", "both"):
             temp_v_time.line(
                 time_data,
                 self._extracted_nodes["max"].values,
                 color="#FF0000",
-                label="Mean Temperature")
+                label="Max Temperature")
 
         if self.save:
+            if not self.result_dir.exists():
+                self.result_dir.mkdir()
+
             save_path: pathlib.Path = self.result_dir / f"{title}.png"
-            # Returns a numpy array of pixels
-            # But we don't need that.
-            _ = temp_v_time.show(
+            temp_v_time.show(
                 interactive=self.interactive,
                 off_screen=(not self.interactive),
-                screenshot=True,
-                filename=self.result_dir / f"{title}.png")
+                screenshot=self.result_dir / f"{title}.png"
+                )
 
             return save_path
 
         elif self.interactive:
             temp_v_time.show(
                 interactive=True,
                 off_screen=False,
@@ -1166,19 +1158,23 @@
 
         if target_nodes is None:
             if not hasattr(self, "odb"):
                 self.load_hdf()
 
             target_nodes = self.odb
 
+        if not self.result_dir.exists():
+            self.result_dir.mkdir()
+
         results: List[pathlib.Path] = list()
         frame: DataFrameType
         for frame in self:
             time: float = frame["Time"].values[0]
-            results.append(self._plot_3d_single(time, label, target_nodes))
+            if self.time_low <= time <= self.time_high:
+                results.append(self._plot_3d_single(time, label, target_nodes))
 
         return results
 
 
     def _plot_3d_single(
         self,
         time: float,
@@ -1194,43 +1190,65 @@
                 ' or odb-plotter["all"] rather than pip install odb-plotter'
                 " Or export the data from Odb.extract() to another tool,"
                 " such as matplotlib or bokeh.")
 
         dims_columns: set[str] = {"X", "Y", "Z"}
         combined_label: str = f"{label}-{round(time, 2):.2f}"
 
+        filtered_target_nodes: DataFrameType = target_nodes[
+            target_nodes["Time"] == time
+            ]
+        filtered_target_nodes = filtered_target_nodes[
+            filtered_target_nodes["X"] >= self.x_low
+            ]
+        filtered_target_nodes = filtered_target_nodes[
+            filtered_target_nodes["X"] <= self.x_high
+            ]
+        filtered_target_nodes = filtered_target_nodes[
+            filtered_target_nodes["Y"] >= self.y_low
+            ]
+        filtered_target_nodes = filtered_target_nodes[
+            filtered_target_nodes["Y"] <= self.y_high
+            ]
+        filtered_target_nodes = filtered_target_nodes[
+            filtered_target_nodes["Z"] >= self.z_low
+            ]
+        filtered_target_nodes = filtered_target_nodes[
+            filtered_target_nodes["Z"] <= self.z_high
+            ]
+
         plotter: pv.Plotter = pv.Plotter(
-            interactive=self.interactive,
             off_screen=(not self.interactive),
             window_size=(1920, 1080),
             lighting="three lights"
             )
 
         plotter.add_text(
             combined_label,
             position="upper_edge",
             color="#000000",
             font="courier"
         )
 
         points: pv.PolyData = pv.PolyData(
-            target_nodes.drop(
+            filtered_target_nodes.drop(
                 columns=list(
-                    set(target_nodes.columns.values.tolist())
+                    set(filtered_target_nodes.columns.values.tolist())
                     - dims_columns
                     )
                 ).to_numpy()
             )
 
-        points[self.temp_key] = target_nodes[self.temp_key].to_numpy()
+
+        points["Temp"] = filtered_target_nodes["Temp"].to_numpy()
         mesh: pv.PolyData = points.delaunay_3d()
 
         plotter.add_mesh(
             mesh,
-            scalars=self.temp_key,
+            scalars="Temp",
             cmap = pv.LookupTable(
                 cmap=self._colormap,
                 scalar_range=(
                     self.temp_low,
                     self.temp_high
                     ),
                 above_range_color=(
```

### Comparing `odb-plotter-0.6.2/src/odbp/odb_visualizer.py` & `odb-plotter-0.6.3/src/odbp/odb_visualizer.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.2/src/odbp/py2_scripts/converter.py` & `odb-plotter-0.6.3/src/odbp/py2_scripts/converter.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.2/src/odbp/py2_scripts/extractor.py` & `odb-plotter-0.6.3/src/odbp/py2_scripts/extractor.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.2/src/odbp/py2_scripts/state_collector.py` & `odb-plotter-0.6.3/src/odbp/py2_scripts/state_collector.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.2/src/odbp/reader.py` & `odb-plotter-0.6.3/src/odbp/reader.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.2/src/odbp/state.py` & `odb-plotter-0.6.3/src/odbp/state.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.2/src/odbp/util.py` & `odb-plotter-0.6.3/src/odbp/util.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.6.2/src/odbp/writer.py` & `odb-plotter-0.6.3/src/odbp/writer.py`

 * *Files identical despite different names*

