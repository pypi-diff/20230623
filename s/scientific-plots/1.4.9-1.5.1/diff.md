# Comparing `tmp/scientific_plots-1.4.9.tar.gz` & `tmp/scientific_plots-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientific_plots-1.4.9.tar", last modified: Tue Apr  4 10:52:24 2023, max compression
+gzip compressed data, was "scientific_plots-1.5.1.tar", last modified: Fri Jun 23 10:16:20 2023, max compression
```

## Comparing `scientific_plots-1.4.9.tar` & `scientific_plots-1.5.1.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.814645 scientific_plots-1.4.9/
--rw-r--r--   0 root         (0) root         (0)     2408 2023-04-04 10:52:24.814645 scientific_plots-1.4.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1356 2023-04-03 13:24:41.000000 scientific_plots-1.4.9/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1925 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/readme.md
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-04-04 10:52:24.814645 scientific_plots-1.4.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/cycler-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/cycler-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/hurst-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/hurst-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/matplotlib-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1526 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/animation.pyi
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/cm.pyi
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/colors.pyi
--rw-rw-rw-   0 root         (0) root         (0)      773 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/figure.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/matplotlib-stubs/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     5979 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/src/matplotlib-stubs/pyplot/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/pyplot/style.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/src/matplotlib-stubs/ticker.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/numba-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/numba-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/python_translator-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/python_translator-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.810645 scientific_plots-1.4.9/src/scientific_plots/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/src/scientific_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scientific_plots/data_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18014 2023-04-03 13:24:41.000000 scientific_plots-1.4.9/src/scientific_plots/default_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    15134 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/src/scientific_plots/plot_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 10:51:59.000000 scientific_plots-1.4.9/src/scientific_plots/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scientific_plots/two_d_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scientific_plots/types_.py
--rw-rw-rw-   0 root         (0) root         (0)     9674 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/src/scientific_plots/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.810645 scientific_plots-1.4.9/src/scientific_plots.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2408 2023-04-04 10:52:24.000000 scientific_plots-1.4.9/src/scientific_plots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1289 2023-04-04 10:52:24.000000 scientific_plots-1.4.9/src/scientific_plots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 10:52:24.000000 scientific_plots-1.4.9/src/scientific_plots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-04-04 10:52:24.000000 scientific_plots-1.4.9/src/scientific_plots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-04 10:52:24.000000 scientific_plots-1.4.9/src/scientific_plots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.810645 scientific_plots-1.4.9/src/scipy-stubs/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/fft.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/integrate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/interpolate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/optimize.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.810645 scientific_plots-1.4.9/src/scipy-stubs/signal/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/signal/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/signal/windows.pyi
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/special.pyi
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/stats.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.814645 scientific_plots-1.4.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1765 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/tests/test_plot_manual.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/tests/test_plots.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/tests/test_utilties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-06-23 10:08:16.000000 scientific_plots-1.5.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2023-06-23 08:33:51.000000 scientific_plots-1.5.1/readme.md
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.602146 scientific_plots-1.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.602146 scientific_plots-1.5.1/src/cycler-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/cycler-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.602146 scientific_plots-1.5.1/src/hurst-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/hurst-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.602146 scientific_plots-1.5.1/src/matplotlib-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2023-06-23 09:07:22.000000 scientific_plots-1.5.1/src/matplotlib-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/matplotlib-stubs/animation.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-23 09:07:22.000000 scientific_plots-1.5.1/src/matplotlib-stubs/cm.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/matplotlib-stubs/colors.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-06-22 22:33:58.000000 scientific_plots-1.5.1/src/matplotlib-stubs/figure.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.602146 scientific_plots-1.5.1/src/matplotlib-stubs/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     6787 2023-06-23 08:33:51.000000 scientific_plots-1.5.1/src/matplotlib-stubs/pyplot/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/matplotlib-stubs/pyplot/style.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-04 10:41:15.000000 scientific_plots-1.5.1/src/matplotlib-stubs/ticker.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.606146 scientific_plots-1.5.1/src/mpl_toolkits-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-23 09:07:22.000000 scientific_plots-1.5.1/src/mpl_toolkits-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-06-23 09:07:22.000000 scientific_plots-1.5.1/src/mpl_toolkits-stubs/mplot.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.606146 scientific_plots-1.5.1/src/numba-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/numba-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.606146 scientific_plots-1.5.1/src/python_translator-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/python_translator-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.606146 scientific_plots-1.5.1/src/scientific_plots/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-23 10:06:10.000000 scientific_plots-1.5.1/src/scientific_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scientific_plots/data_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18732 2023-06-23 08:33:51.000000 scientific_plots-1.5.1/src/scientific_plots/default_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    17677 2023-06-23 08:33:51.000000 scientific_plots-1.5.1/src/scientific_plots/plot_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 10:15:54.000000 scientific_plots-1.5.1/src/scientific_plots/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scientific_plots/two_d_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scientific_plots/types_.py
+-rw-rw-rw-   0 root         (0) root         (0)     8875 2023-04-05 14:09:05.000000 scientific_plots-1.5.1/src/scientific_plots/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.606146 scientific_plots-1.5.1/src/scientific_plots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-06-23 10:16:20.000000 scientific_plots-1.5.1/src/scientific_plots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-23 10:16:20.000000 scientific_plots-1.5.1/src/scientific_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 10:16:20.000000 scientific_plots-1.5.1/src/scientific_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-23 10:16:20.000000 scientific_plots-1.5.1/src/scientific_plots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-23 10:16:20.000000 scientific_plots-1.5.1/src/scientific_plots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/src/scipy-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/fft.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/integrate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/interpolate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/optimize.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/src/scipy-stubs/signal/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/signal/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/signal/windows.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/special.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/src/scipy-stubs/stats.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 10:16:20.610146 scientific_plots-1.5.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2023-06-22 14:06:06.000000 scientific_plots-1.5.1/tests/test_plot_manual.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/tests/test_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.5.1/tests/test_utilties.py
```

### Comparing `scientific_plots-1.4.9/PKG-INFO` & `scientific_plots-1.5.1/src/scientific_plots.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scientific_plots
-Version: 1.4.9
+Name: scientific-plots
+Version: 1.5.1
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 Keywords: Plotting,science,library,utilities,styling
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -45,14 +45,22 @@
     plt.savefig("subfolder/your_plot_name.pdf")
 ```
 
 The script will create a bunch of plots and place them in the given location
 next to your given path. Thus, it is advisable to create a different subfolder
 for new plots.
 
+For three-dimensional plots, it is recommended to set the optional argument
+*three_d* of the decorator to true:
+```
+@apply_styles(three_d=True)
+def plot_function():
+    ...
+```
+
 Alternatively, this package provides default plot settings in the submodule
 *default_plots*. The provided function apply a default design, which should
 look good in most situations.
 
 ```
 from scientific_plots.default_plots import plot
```

### Comparing `scientific_plots-1.4.9/pyproject.toml` & `scientific_plots-1.5.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -10,30 +10,32 @@
     "Programming Language :: Python :: 3"
 ]
 keywords = ["Plotting", "science", "library", "utilities", "styling"]
 
 dependencies = [
     "scipy",
     "numpy>=1.21",
-    "matplotlib",
+    "matplotlib>=3.7",
     "SciencePlots",
     "python_translator",
     "requests",
     "beautifulsoup4",
-    "urllib3"
+    "urllib3>=2.0.0"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "pylint",
     "flake8",
     "pytest",
-    "types-urllib3"
+    "types-urllib3",
+    "twine>=4.0.0",
+    "requests-toolbelt>=1.0.0"
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "scientific_plots.__version__"}
 
 [tool.mypy]
 python_version = "3.9"
```

### Comparing `scientific_plots-1.4.9/readme.md` & `scientific_plots-1.5.1/readme.md`

 * *Files 21% similar despite different names*

```diff
@@ -32,14 +32,22 @@
     plt.savefig("subfolder/your_plot_name.pdf")
 ```
 
 The script will create a bunch of plots and place them in the given location
 next to your given path. Thus, it is advisable to create a different subfolder
 for new plots.
 
+For three-dimensional plots, it is recommended to set the optional argument
+*three_d* of the decorator to true:
+```
+@apply_styles(three_d=True)
+def plot_function():
+    ...
+```
+
 Alternatively, this package provides default plot settings in the submodule
 *default_plots*. The provided function apply a default design, which should
 look good in most situations.
 
 ```
 from scientific_plots.default_plots import plot
```

### Comparing `scientific_plots-1.4.9/src/cycler-stubs/__init__.pyi` & `scientific_plots-1.5.1/src/cycler-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/src/matplotlib-stubs/__init__.pyi` & `scientific_plots-1.5.1/src/matplotlib-stubs/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 or modules, which use matplot-lib. No function is implemented in this folder.
 """
 from __future__ import annotations
 from typing import Union, overload, Literal, TypedDict
 
 from cycler import cycler
 
+from .cm import ColormapRegistry
+
 def use(backend: str) -> None: ...
 
 
 def rc(object_: str, **kwargs: Union[
         str,
         bool,
         dict[str, int],
@@ -43,7 +45,9 @@
     def __getitem__(self, key: str) -> Union[list[str], cycler]: ...
 
 
 rcParams: RCParams
 
 
 rcParamsDefault: RCParams
+
+colormaps: ColormapRegistry
```

### Comparing `scientific_plots-1.4.9/src/matplotlib-stubs/colors.pyi` & `scientific_plots-1.5.1/src/matplotlib-stubs/colors.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/src/matplotlib-stubs/figure.pyi` & `scientific_plots-1.5.1/src/matplotlib-stubs/figure.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -23,11 +23,14 @@
         self, figsize: Optional[Tuple[float, float]] = None) -> None: ...
 
     def gca(self) -> Axes: ...
 
     def set_size_inches(self, x: float, y: float) -> None: ...
 
     def subplots_adjust(self, bottom: Optional[float] = None,
-                        right: Optional[float] = None) -> None: ...
+                        right: Optional[float] = None,
+                        left: Optional[float] = None,
+                        top: Optional[float] = None,
+                        ) -> None: ...
 
     def add_subplot(self, position: int = 111,
                     projection: str = "2d") -> Axes: ...
```

### Comparing `scientific_plots-1.4.9/src/matplotlib-stubs/pyplot/__init__.pyi` & `scientific_plots-1.5.1/src/matplotlib-stubs/pyplot/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -62,20 +62,29 @@
     def get_color(self) -> str: ...
 
 
 class Legend:
     texts: Tuple[Label, ...]
 
 
+class Pane:
+    def set_alpha(
+        self,
+        input_: float) -> None: ...
+
+
 class Axis:
     label: Label
+    labelpad: float
+    pane: Pane
 
     def set_ticks_position(self, position: str) -> None: ...
 
-    def set_tick_params(self, direction: str = "", color: str = "")\
+    def set_tick_params(self, pad: Optional[float] = None,
+                        direction: str = "", color: str = "")\
         -> None: ...
 
     def set_major_formatter(self, format_str: str) -> None: ...
 
 
 class Spine:
     """Spine-class of axes."""
@@ -118,19 +127,28 @@
 
     def get_zticklabels(self) -> Iterable[Label]: ...
 
     def get_lines(self) -> Iterable[Line]: ...
 
     def get_legend(self) -> Legend: ...
 
-    def set_xlabel(self, label: str) -> None: ...
-
-    def set_ylabel(self, label: str) -> None: ...
-
-    def set_zlabel(self, label: str) -> None: ...
+    def set_xlabel(self, label: str,
+                   linespacing: Optional[float] = None,
+                   rotation: Optional[float] = None,
+                   labelpad: Optional[float] = None) -> None: ...
+
+    def set_ylabel(self, label: str,
+                   linespacing: Optional[float] = None,
+                   rotation: Optional[float] = None,
+                   labelpad: Optional[float] = None) -> None: ...
+
+    def set_zlabel(self, label: str,
+                   linespacing: Optional[float] = None,
+                   rotation: Optional[float] = None,
+                   labelpad: Optional[float] = None) -> None: ...
 
     def set_xlim(self, min_: float, max_: float) -> None: ...
 
     def set_ylim(self, min_: float, max_: float) -> None: ...
 
     def set_zlim(self, min_: float, max_: float) -> None: ...
 
@@ -165,14 +183,19 @@
     def tick_params(self, axis: str = "x",
                     colors: str = "") -> None: ...
 
     def ticklabel_format(
         self,
         useLocale: bool = False, useMathText: bool = False) -> None: ...
 
+    def set_box_aspect(
+        cself,
+        aspect: Optional[str] = None, zoom: float = 1.)\
+        -> None: ...
+
 
 def figure(figsize: Optional[Tuple[float, float]] = None) -> Figure: ...
 
 
 def close(fig: Union[Figure, str, None] = None) -> None: ...
 
 
@@ -246,15 +269,18 @@
 def clf() -> None: ...
 
 
 def imshow(frame: int, cmap: Union[colors.ColorMap, str] = "default")\
         -> None: ...
 
 
-def locator_params(nbins: int = 1) -> None: ...
+def locator_params(
+    *,
+    nbins: int = 1,
+    axis: str = "x") -> None: ...
 
 
 rcParams: RCParams
 
 
 class _ArrowProps(TypedDict):
     """Properties of an arrow."""
```

### Comparing `scientific_plots-1.4.9/src/numba-stubs/__init__.pyi` & `scientific_plots-1.5.1/src/numba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/src/scientific_plots/data_analysis.py` & `scientific_plots-1.5.1/src/scientific_plots/data_analysis.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/src/scientific_plots/default_plots.py` & `scientific_plots-1.5.1/src/scientific_plots/default_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,32 +156,45 @@
     plt.xlabel(xlabel)
     plt.legend()
     plt.tight_layout()
     plt.savefig(filename)
     plt.close()
 
 
-@apply_styles
+@apply_styles(three_d=True)
 def plot_surface(X: In2d, Y: In2d, Z: In2d,
                  xlabel: str, ylabel: str, zlabel: str,
                  filename: Union[str, Path], *,
                  log_scale: bool = False,
-                 set_z_lim: bool = True) -> None:
+                 set_z_lim: bool = True,
+                 colorscheme: str = "rwth_gradient",
+                 figsize: tuple[float, float] = (4.33, 3.5),
+                 labelpad: Optional[float] = None,
+                 nbins: Optional[int] = None) -> None:
     """create a 2D surface plot of meshgrid-like valued Xs, Ys and Zs"""
     if not check_inputs(
-            X[0], Z[0], xlabel, zlabel):
+            np.array(X).flatten(),
+            np.array(Z).flatten(), xlabel, zlabel):
         return
-    plt.set_cmap("rwth_gradient")
     fig = plt.figure()
     ax = fig.add_subplot(projection="3d")
-    ax.plot_surface(X, Y, Z, cmap="rwth_gradient")
+    fig.subplots_adjust(left=-0.02, right=0.75, bottom=0.15, top=0.98)
+    ax.plot_surface(X, Y, Z, cmap=colorscheme)
+    ax.set_box_aspect(aspect=None, zoom=.8)
+
+    if labelpad is None:
+        ax.set_xlabel(xlabel)
+        ax.set_ylabel(ylabel)
+        ax.set_zlabel(zlabel, rotation=90)
+    else:
+        ax.set_xlabel(xlabel, labelpad=labelpad)
+        ax.set_ylabel(ylabel, labelpad=labelpad)
+        ax.set_zlabel(zlabel, rotation=90, labelpad=labelpad)
 
-    ax.set_xlabel(xlabel)
-    ax.set_ylabel(ylabel)
-    ax.set_zlabel(zlabel)
+    assert ax.zaxis is not None
 
     ax.set_xlim(amin(X), amax(X))  # type: ignore
     ax.set_ylim(amin(Y), amax(Y))  # type: ignore
 
     if set_z_lim:
         if not log_scale:
             ax.set_zlim(
@@ -195,23 +208,29 @@
     if log_scale:
         ax.set_yscale("log")
         ax.set_xscale("log")
         ax.set_zscale("log")
 
     for spine in ax.spines.values():
         spine.set_visible(False)
-    # plt.tight_layout()
 
-    def empty_function() -> None:
-        """dummy function"""
+    ax.xaxis.pane.set_alpha(0.3)
+    ax.yaxis.pane.set_alpha(0.3)
+    ax.zaxis.pane.set_alpha(0.3)
+
+    if nbins is not None:
+        plt.locator_params(
+            nbins=nbins,
+            axis="x")
+        plt.locator_params(
+            nbins=nbins,
+            axis="y")
 
-    plt.tight_layout = empty_function
-    fig.subplots_adjust(bottom=0.18)
-    fig.subplots_adjust(right=0.85)
-    ax.dist = 13
+    fig.set_size_inches(*figsize)
+    plt.tight_layout()
     plt.savefig(filename)
     plt.close()
 
 
 @apply_styles
 def plot(X: In, Y: In, xlabel: str, ylabel: str,
          filename: Union[Path, str], *, logscale: bool = False,
@@ -338,15 +357,15 @@
                 logscale: bool = False,
                 xmin: Optional[float] = None,
                 xmax: Optional[float] = None) -> None:
     """Create a simple 1D plot with three different graphs inside of a single
     plot and a single y-axis."""
     x1, y1 = fix_inputs(x1, y1)  # type: ignore
     x2, y2 = fix_inputs(x2, y2)  # type: ignore
-    x2, y3 = fix_inputs(x3, y3)  # type: ignore
+    x3, y3 = fix_inputs(x3, y3)  # type: ignore
     if not (
             check_inputs(x1, y1, xlabel, label1)
             or check_inputs(x2, y3, xlabel, label1)
             or check_inputs(x3, y3, xlabel, label3)):
         return
 
     if any(len(x) <= 1 for x in (x1, x2, y1, y2, x3, y3)):
```

### Comparing `scientific_plots-1.4.9/src/scientific_plots/plot_settings.py` & `scientific_plots-1.5.1/src/scientific_plots/plot_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 import csv
 import locale
 from contextlib import contextmanager
 from math import sqrt
 from copy import copy
 from functools import wraps
 from typing import (
-    Generator, Optional, Union, Callable, Any)
+    Generator, Optional, Union, Callable, Any, overload)
 from pathlib import Path
 from warnings import warn
 from textwrap import dedent
 
+import mpl_toolkits
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.pyplot import Axes
 from matplotlib import colors
-from matplotlib import cm
 from cycler import cycler
 import numpy as np
 
 from .utilities import translate
 from .types_ import Vector
 
 mpl.use("Agg")
@@ -45,15 +45,15 @@
     yield "--"
     yield "-."
 
 
 rwth_colorlist: list[tuple[int, int, int]] = [(0, 84, 159), (246, 168, 0),
                                               (161, 16, 53), (0, 97, 101)]
 rwth_cmap = colors.ListedColormap(rwth_colorlist, name="rwth_list")
-cm.register_cmap(name="rwth_list", cmap=rwth_cmap)
+mpl.colormaps.register(rwth_cmap)
 
 rwth_hex_colors = ["#00549F", "#F6A800", "#A11035", "#006165",
                    "#57AB27", "#E30066"]
 
 rwth_cycle = (
     cycler(color=rwth_hex_colors)
     + cycler(linestyle=["-", "--", "-.", "dotted",
@@ -111,15 +111,15 @@
     [
         ((None, None, None), 0., hks_44),
         (hks_44_75, 0.33, hks_44_75),
         (rwth_orange_75, 0.66, rwth_orange),
         (rwth_bordeux, 1., (None, None, None))
     ]
 )
-cm.register_cmap(name="rwth_gradient", cmap=rwth_gradient_map)
+mpl.colormaps.register(rwth_gradient_map)
 
 
 def _germanify(ax: Axes, reverse: bool = False) -> None:
     """
     translate a figure from english to german.
     The direction can be reversed, if reverse it set to True
     Use the decorator instead
@@ -133,22 +133,27 @@
             pass
         items = [
             axi.xaxis.label,
             axi.yaxis.label,
             *axi.get_xticklabels(),
             *axi.get_yticklabels(),
         ]
+        try:
+            if axi.zaxis is not None:
+                items.append(axi.zaxis.label)
+                items += [*axi.get_zticklabels()]
+        except AttributeError:
+            pass
         if axi.get_legend():
             items += [*axi.get_legend().texts]
         for item in items:
             item.set_text(translate(item.get_text(),
                                     reverse=reverse))
     try:
-        if not hasattr(ax, "zaxis"):
-            plt.tight_layout()
+        plt.tight_layout()
     except IndexError:
         pass
 
 
 @contextmanager
 def germanify(ax: Axes,
               reverse: bool = False) -> Generator[None, None, None]:
@@ -313,16 +318,15 @@
         data_path = filename.parent / (
             filename.stem + ".dat")
 
         if not data_path.exists():
             data_plot(data_path)
 
         try:
-            if not hasattr(plt.gca(), "zaxis"):
-                plt.tight_layout()
+            plt.tight_layout()
         except IndexError:
             pass
         # save the figure
         try_save(new_path_pdf, bbox_inches=bbox_inches)
         try_save(new_path_png, bbox_inches=bbox_inches,
                  dpi=dpi)
 
@@ -353,19 +357,22 @@
     mpl.rcParams["ytick.labelsize"] = 18
     mpl.rcParams["figure.figsize"] = (10, 6)
     mpl.rcParams["figure.titlesize"] = 24
 
     mpl.rcParams["font.family"] = "sans-serif"
 
 
-def set_rwth_colors() -> None:
+def set_rwth_colors(three_d: bool = False) -> None:
     """Apply the RWTH CD colors to matplotlib."""
     mpl.rcParams["text.usetex"] = False
-    plt.set_cmap("rwth_list")
     mpl.rcParams["axes.prop_cycle"] = rwth_cycle
+    if three_d:
+        plt.set_cmap("rwth_gradient")
+    else:
+        plt.set_cmap("rwth_list")
 
 
 def set_serif() -> None:
     """Set the plot to use a style with serifs."""
     mpl.rcParams["font.family"] = "serif"
     mpl.rcParams["font.serif"] = [
         "cmr10", "stix", "Times New Roman"]
@@ -374,82 +381,150 @@
 def set_sans_serif() -> None:
     """Set matplotlib to use a sans-serif font."""
     mpl.rcParams["font.family"] = "sans-serif"
     mpl.rcParams["font.sans-serif"] = [
         "Arial", "Helvetica", "DejaVu Sans"]
 
 
-def apply_styles(plot_function: Callable[..., None]) -> Callable[..., None]:
-    """Apply the newly defined styles to a function, which creates a plot."""
-    # pylint: disable=too-many-statements
+class ThreeDPlotException(Exception):
+    """This exception is called when a 3D plot is drawn. This is used to exit
+    the plotting function with the science-style."""
 
-    @wraps(plot_function)
-    def new_plot_function(*args: Any, **kwargs: Any) -> None:
-        """
-        New plotting function, with applied styles.
-        """
-        # default plot
-        plt.set_cmap("rwth_list")
-        plt.savefig = new_save_simple()
-        plot_function(*args, **kwargs)
 
-        errors = (OSError, FileNotFoundError)
+def check_3d(three_d: bool) -> None:
+    """This function checks if the current plot is a 3d plot. In that case, an
+    exception is thrown, which can be used to stop the creation of the default
+    plot."""
+    if three_d:
+        raise ThreeDPlotException
+    if isinstance(plt.gca(), mpl_toolkits.mplot3d.axes3d.Axes3D):
+        raise ThreeDPlotException
 
-        try:
-            with plt.style.context(["science", "ieee"]):
-                set_rwth_colors()
-                set_serif()
-                plt.savefig = new_save_simple("journal")
-                plot_function(*args, **kwargs)
-        except errors:
-            with plt.style.context("fast"):
-                warn(dedent(""""Could not found style 'science'.
-                            Using a fallback-style."""), RuntimeWarning)
-                set_rwth_colors()
-                set_serif()
-                plt.savefig = new_save_simple("journal")
-                plot_function(*args, **kwargs)
 
-        try:
-            with plt.style.context(["science", "ieee", "nature"]):
-                set_rwth_colors()
-                set_sans_serif()
-                plt.savefig = new_save_simple("sans_serif", german=True)
-                plot_function(*args, **kwargs)
-        except errors:
-            with plt.style.context("fast"):
-                set_rwth_colors()
-                set_sans_serif()
-                plt.savefig = new_save_simple("sans_serif")
-                plot_function(*args, **kwargs)
+PlotFunction = Callable[..., None]
 
-        try:
-            with plt.style.context(["science", "ieee", "grayscale"]):
-                mpl.rcParams["text.usetex"] = False
-                set_serif()
-                plt.savefig = new_save_simple("grayscale")
-                plot_function(*args, **kwargs)
-        except errors:
-            with plt.style.context("grayscale"):
-                mpl.rcParams["text.usetex"] = False
-                set_serif()
-                plt.savefig = new_save_simple("grayscale")
-                plot_function(*args, **kwargs)
 
-        try:
-            with plt.style.context(["science", "ieee"]):
-                set_rwth_colors()
-                presentation_settings()
-                set_sans_serif()
-                plt.savefig = new_save_simple("presentation", german=True)
-                plot_function(*args, **kwargs)
-        except errors:
-            with plt.style.context("fast"):
-                set_rwth_colors()
-                presentation_settings()
-                set_sans_serif()
-                plt.savefig = new_save_simple("presentation", german=True)
-                plot_function(*args, **kwargs)
+@overload
+def apply_styles(plot_function: PlotFunction, *,
+                 three_d: bool = False) -> PlotFunction:
+    ...
+
+
+@overload
+def apply_styles(plot_function: None, *, three_d: bool = False)\
+        -> Callable[[PlotFunction], PlotFunction]:
+    ...
+
+
+@overload
+def apply_styles(*, three_d: bool = False)\
+        -> Callable[[PlotFunction], PlotFunction]:
+    ...
+
+
+def apply_styles(plot_function: Optional[PlotFunction] = None, *,
+                 three_d: bool = False)\
+        -> Union[Callable[[PlotFunction], PlotFunction], PlotFunction]:
+    """Apply the newly defined styles to a function, which creates a plot."""
+    # pylint: disable=too-many-statements
+
+    def _decorator(_plot_function: PlotFunction) -> PlotFunction:
+        """This is the  actual decorator. Thus, the outer function
+        'apply_styles' is acutally a decorator-factory."""
+
+        @wraps(_plot_function)
+        def new_plot_function(*args: Any, **kwargs: Any) -> None:
+            """
+            New plotting function, with applied styles.
+            """
+            # default plot
+            plt.set_cmap("rwth_list")
+            plt.savefig = new_save_simple()
+            _plot_function(*args, **kwargs)
+
+            errors = (OSError, FileNotFoundError, ThreeDPlotException)
+
+            try:
+                check_3d(three_d)
+                # journal
+                with plt.style.context(["science", "ieee"]):
+                    set_rwth_colors()
+                    set_serif()
+                    plt.savefig = new_save_simple("journal")
+                    _plot_function(*args, **kwargs)
+
+                # sans-serif
+                with plt.style.context(["science", "ieee", "nature"]):
+                    set_rwth_colors()
+                    set_sans_serif()
+                    plt.savefig = new_save_simple("sans_serif", german=True)
+                    _plot_function(*args, **kwargs)
+
+                # grayscale
+                with plt.style.context(["science", "ieee", "grayscale"]):
+                    mpl.rcParams["text.usetex"] = False
+                    set_serif()
+                    plt.savefig = new_save_simple("grayscale")
+                    _plot_function(*args, **kwargs)
+
+                # presentation
+                with plt.style.context(["science", "ieee"]):
+                    set_rwth_colors()
+                    presentation_settings()
+                    set_sans_serif()
+                    plt.savefig = new_save_simple("presentation", german=True)
+                    _plot_function(*args, **kwargs)
+
+            except errors:
+                if not three_d:
+                    warn(dedent(""""Could not found style 'science'.
+                                Using a fallback-style."""), RuntimeWarning)
+                # journal
+                with plt.style.context("fast"):
+                    set_rwth_colors(three_d)
+                    set_serif()
+                    plt.savefig = new_save_simple("journal")
+                    _plot_function(*args, **kwargs)
+
+                # sans-serif
+                with plt.style.context("fast"):
+                    set_rwth_colors(three_d)
+                    set_sans_serif()
+                    plt.savefig = new_save_simple("sans_serif")
+                    _plot_function(*args, **kwargs)
+
+                # grayscale
+                with plt.style.context("grayscale"):
+                    if three_d:
+                        plt.set_cmap("Greys")
+                        new_kwargs = copy(kwargs)
+                        new_kwargs["colorscheme"] = "Greys"
+                    else:
+                        new_kwargs = kwargs
+                    mpl.rcParams["text.usetex"] = False
+                    set_serif()
+                    plt.savefig = new_save_simple("grayscale")
+                    _plot_function(*args, **new_kwargs)
+
+                # presentation
+                with plt.style.context("fast"):
+                    if three_d:
+                        new_kwargs = copy(kwargs)
+                        new_kwargs["figsize"] = (9, 7)
+                        new_kwargs["labelpad"] = 20
+                        new_kwargs["nbins"] = 5
+                    else:
+                        new_kwargs = kwargs
+                    set_rwth_colors(three_d)
+                    presentation_settings()
+                    set_sans_serif()
+                    plt.savefig = new_save_simple("presentation", german=True)
+                    _plot_function(*args, **new_kwargs)
+
+            plt.savefig = old_save
+
+        return new_plot_function
 
-        plt.savefig = old_save
+    if plot_function is not None:
+        return _decorator(plot_function)
 
-    return new_plot_function
+    return _decorator
```

### Comparing `scientific_plots-1.4.9/src/scientific_plots/two_d_plot.py` & `scientific_plots-1.5.1/src/scientific_plots/two_d_plot.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/src/scientific_plots/types_.py` & `scientific_plots-1.5.1/src/scientific_plots/types_.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/src/scientific_plots/utilities.py` & `scientific_plots-1.5.1/src/scientific_plots/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -207,95 +207,71 @@
     if reverse:
         string = re.sub(r'(\d+),(\d+)', r'\1\.\2', string)
     else:
         string = re.sub(r'(\d+)\.(\d+)', r'\1,\2', string)
 
     _dict: dict[str, str] = OrderedDict({
         "leakage": "Leckage",
-        "Leakage": "Leckage",
         "contact pressure": "Kontaktdruck",
-        "Contact Pressure": "Kontaktdruck",
-        "Contact pressure": "Kontaktdruck",
         "fluid pressure": "Fluiddruck",
-        "Fluid pressure": "Fluiddruck",
-        "Fluid Pressure": "Fluiddruck",
         "pressure": "Druck",
-        "Pressure": "Druck",
         "density": "Dichte",
-        "Density": "Dichte",
         "roundness": "Rundheit",
-        "Roundness": "Rundheit",
         "eccentricity": r"Exzentrizit\"at",
-        "Eccentricity": r"Exzentrizit\"at",
         "contact area": r"Kontaktoberfl\"ache",
-        "Contact Area": r"Kontaktoberfl\"ache",
-        "Contact area": r"Kontaktoberfl\"ache",
         "area": r"Fl\"ache",
-        "Area": r"fl\"ache", "maximal": "maximale",
-        "Maximal": "Maximale",
-        "Time": "Zeit",
+        "maximal": "Maximale",
         "time": "Zeit",
         "normal-force": "Normalkraft",
-        "Normal-force": "Normalkraft",
         "normal force": "Normalkraft",
-        "Normal force": "Normalkraft",
         "total force": "Gesamtkraft",
-        "Total force": "Gesamtkraft",
         "force": "Kraft",
-        "Force": "Kraft",
         "distance": "Abstand",
-        "Distance": "Abstand",
         "position": "Position",
         "contact broadness": "Kontaktbreite",
-        "Contact broadness": "Kontaktbreite",
         "broadness": "Breite",
-        "Broadness": "Breite",
-        "Contact": "Kontakt-",
         "contact": "Kontakt-",
         "seat": "Sitz",
         "ball": "Kugel",
         "high": "hoch",
         "low": "tief",
         "elastic": "elastisch",
         "plastic": "plastisch",
         "angle": "Winkel",
-        "Angle": "Winkel",
         "degree": "Grad",
         "deg": "Grad",
         "hard": "hart",
         "soft": "weich",
-        "Hard": "Hart",
-        "Soft": "Weich",
         "fit": "Fit",
         "data": "Messwerte",
         "velocity": "Geschwindigkeit",
         "measurement": "Messung",
-        "Measurement": "Messung",
         "experiment": "Experiment",
         "simulation": "Simulation",
-        "Simulation": "Simulation",
         "analytical": "analytisch",
-        "Analytical": "Analytisch",
         "signal": "Signal",
+        "valve control": "Ventilansteuerung",
         "off": "zu",
         "on": "auf",
+        "status": "Zustand",
         "valve": "Ventil",
         "relative pressure": "Relativdruck",
         "absolute pressure": "Absolutdruck",
         "relative": "relativ",
-        "absolute": "absolut"
+        "absolute": "absolut",
+        "plot": "Graph"
     })
     if not reverse:
         for key, value in _dict.items():
-            if key in string:
-                string = string.replace(key, value)
+            if key in string.lower():
+                string = re.sub(key, value, string, flags=re.IGNORECASE)
                 break
         else:
             string = use_translator(string, "german", "english")
     else:
         for key, value in _dict.items():
-            if value in string:
-                string = string.replace(value, key)
+            if value.lower() in string.lower():
+                string = string.lower().replace(value.lower(), key.lower())
                 break
         else:
             string = use_translator(string, "english", "german")
     return string
```

### Comparing `scientific_plots-1.4.9/src/scientific_plots.egg-info/PKG-INFO` & `scientific_plots-1.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scientific-plots
-Version: 1.4.9
+Name: scientific_plots
+Version: 1.5.1
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 Keywords: Plotting,science,library,utilities,styling
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -45,14 +45,22 @@
     plt.savefig("subfolder/your_plot_name.pdf")
 ```
 
 The script will create a bunch of plots and place them in the given location
 next to your given path. Thus, it is advisable to create a different subfolder
 for new plots.
 
+For three-dimensional plots, it is recommended to set the optional argument
+*three_d* of the decorator to true:
+```
+@apply_styles(three_d=True)
+def plot_function():
+    ...
+```
+
 Alternatively, this package provides default plot settings in the submodule
 *default_plots*. The provided function apply a default design, which should
 look good in most situations.
 
 ```
 from scientific_plots.default_plots import plot
```

### Comparing `scientific_plots-1.4.9/src/scientific_plots.egg-info/SOURCES.txt` & `scientific_plots-1.5.1/src/scientific_plots.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 src/matplotlib-stubs/animation.pyi
 src/matplotlib-stubs/cm.pyi
 src/matplotlib-stubs/colors.pyi
 src/matplotlib-stubs/figure.pyi
 src/matplotlib-stubs/ticker.pyi
 src/matplotlib-stubs/pyplot/__init__.pyi
 src/matplotlib-stubs/pyplot/style.pyi
+src/mpl_toolkits-stubs/__init__.pyi
+src/mpl_toolkits-stubs/mplot.pyi
 src/numba-stubs/__init__.pyi
 src/python_translator-stubs/__init__.pyi
 src/scientific_plots/__init__.py
 src/scientific_plots/data_analysis.py
 src/scientific_plots/default_plots.py
 src/scientific_plots/plot_settings.py
 src/scientific_plots/py.typed
```

### Comparing `scientific_plots-1.4.9/src/scipy-stubs/fft.pyi` & `scientific_plots-1.5.1/src/scipy-stubs/fft.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/src/scipy-stubs/integrate.pyi` & `scientific_plots-1.5.1/src/scipy-stubs/integrate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/src/scipy-stubs/interpolate.pyi` & `scientific_plots-1.5.1/src/scipy-stubs/interpolate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/src/scipy-stubs/optimize.pyi` & `scientific_plots-1.5.1/src/scipy-stubs/optimize.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/src/scipy-stubs/signal/__init__.pyi` & `scientific_plots-1.5.1/src/scipy-stubs/signal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/tests/test_plot_manual.py` & `scientific_plots-1.5.1/tests/test_plot_manual.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 """
 Test the design of the created plots by eye and by hand. For this, the plots
 are placed in a persistent directory.
 """
 from pathlib import Path
 
 from pytest import mark
-from numpy import linspace
-from scientific_plots.default_plots import two_plots, three_axis_plots, plot
+from numpy import linspace, meshgrid
+from scientific_plots.default_plots import (
+    two_plots, three_axis_plots, plot, plot_surface)
 from scientific_plots.types_ import Vector
 
 
 LOCATION = Path("tests/plots/test_plot.pdf")
 LOCATION2 = Path("tests/plots/test_plot2.pdf")
 LOCATION3 = Path("tests/plots/test_plot3.pdf")
+LOCATION4 = Path("tests/plots/test_plot_surface.pdf")
 
 
 @mark.use_style
 def test_two_plots() -> None:
     """Test the creation of a twin-plot."""
     x_test: Vector = linspace(1., 100., 100)
     y_test1: Vector = x_test**2
@@ -54,7 +56,24 @@
     """Test the skipping of a color in the cycle."""
     x_test: Vector = linspace(1., 2., 100)
     y_test1: Vector = x_test**2
     filename = LOCATION3
     filename.parent.mkdir(exist_ok=True)
     plot(x_test, y_test1, "x", "y", filename, cycler=1)
     assert filename.exists()
+
+
+@mark.use_style
+def test_two_d_plot() -> None:
+    """Test the creation of a two dimensional surface plot."""
+    x_test: Vector = linspace(-10, 10, 100)
+    y_test: Vector = linspace(-10, 10, 100)
+    x_test_grid, y_test_grid = meshgrid(
+        x_test, y_test)
+    z_grid = x_test_grid**2 - y_test_grid
+    filename = LOCATION4
+    filename.parent.mkdir(exist_ok=True)
+    plot_surface(
+        x_test_grid, y_test_grid, z_grid,
+        "x-label", "y-label", "z-label",
+        LOCATION4)
+    assert filename.exists()
```

### Comparing `scientific_plots-1.4.9/tests/test_plots.py` & `scientific_plots-1.5.1/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/tests/test_types.py` & `scientific_plots-1.5.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.9/tests/test_utilties.py` & `scientific_plots-1.5.1/tests/test_utilties.py`

 * *Files identical despite different names*

