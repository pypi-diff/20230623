# Comparing `tmp/timescoring-0.0.3.tar.gz` & `tmp/timescoring-0.0.4.tar.gz`

## Comparing `timescoring-0.0.3.tar` & `timescoring-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 timescoring-0.0.3/requirements.txt
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 timescoring-0.0.3/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 timescoring-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timescoring-0.0.3/src/timescoring/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 timescoring-0.0.3/src/timescoring/annotations.py
--rw-r--r--   0        0        0     9221 2020-02-02 00:00:00.000000 timescoring-0.0.3/src/timescoring/scoring.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 timescoring-0.0.3/src/timescoring/visualization.py
--rw-r--r--   0        0        0    12973 2020-02-02 00:00:00.000000 timescoring-0.0.3/tests/test.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 timescoring-0.0.3/LICENSE
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 timescoring-0.0.3/README.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 timescoring-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 timescoring-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 timescoring-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 timescoring-0.0.4/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 timescoring-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timescoring-0.0.4/src/timescoring/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 timescoring-0.0.4/src/timescoring/annotations.py
+-rw-r--r--   0        0        0     9221 2020-02-02 00:00:00.000000 timescoring-0.0.4/src/timescoring/scoring.py
+-rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 timescoring-0.0.4/src/timescoring/visualization.py
+-rw-r--r--   0        0        0    12973 2020-02-02 00:00:00.000000 timescoring-0.0.4/tests/test.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 timescoring-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 timescoring-0.0.4/README.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 timescoring-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 timescoring-0.0.4/PKG-INFO
```

### Comparing `timescoring-0.0.3/.github/workflows/python-app.yml` & `timescoring-0.0.4/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.3/.github/workflows/python-publish.yml` & `timescoring-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.3/src/timescoring/annotations.py` & `timescoring-0.0.4/src/timescoring/annotations.py`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.3/src/timescoring/scoring.py` & `timescoring-0.0.4/src/timescoring/scoring.py`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.3/src/timescoring/visualization.py` & `timescoring-0.0.4/src/timescoring/visualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
+import matplotlib.colors as mc
+import colorsys
 import numpy as np
 
 from .annotations import Annotation
 from . import scoring
 
 
 def plotSampleScoring(ref: Annotation, hyp: Annotation, fs: int = 1, showLegend: bool = True, ax: Axes = None) -> plt.figure:
@@ -76,59 +78,58 @@
             Defaults to default values.
         showLegend (bool): Whether to show the legend. Default True.
         ax (Axes): If provided figure is plotted on that axes. Else a new figure is created. Default None (new figure).
 
     Returns:
         plt.figure: Output matplotlib figure
     """
-    def _plotEvent(x, y, color, ax):
-        ax.axvspan(x[0], x[1], alpha=0.2, color=color)
-        if x[1] - x[0] > 0:
-            ax.plot(x, y, color=color, linewidth=5, solid_capstyle='butt')
-        else:
-            ax.scatter(x[0], y[0], color=color)
-
     score = scoring.EventScoring(ref, hyp, param)
     time = np.arange(len(ref.mask)) / ref.fs
 
     if ax is None:
         plt.figure(figsize=(16, 3))
         ax = plt.axes()
 
     # Plot Labels
     ax.plot(time, ref.mask * 0.4 + 0.6, 'k')
     ax.plot(time, hyp.mask * 0.4 + 0.1, 'k')
+    # Plot splitting of events
+    for event in ref.events:
+        _plotSplitLongEvents(event, param.maxEventDuration, [0.6, 1])
+    for event in hyp.events:
+        _plotSplitLongEvents(event, param.maxEventDuration, [0.1, 0.5])
 
     # Initialize lines for legend
     lineTp, = ax.plot([], [], color='tab:green', linewidth=5)
     lineFn, = ax.plot([], [], color='tab:purple', linewidth=5)
     lineFp, = ax.plot([], [], color='tab:red', linewidth=5)
 
     # Plot REF TP & FN
-    for event in ref.events:
+    for event in score.ref.events:
         # TP
         if np.any(score.tpMask[round(event[0] * score.fs):round(event[1] * score.fs)]):
-            _plotEvent([event[0], event[1] - (1 / ref.fs)], [1, 1], 'tab:green', ax)
-            score.tpMask[round(event[0] * score.fs):round(event[1] * score.fs)] = 1
+            color = 'tab:green'
         else:
-            _plotEvent([event[0], event[1] - (1 / ref.fs)], [1, 1], 'tab:purple', ax)
+            color = 'tab:purple'
+        _plotEvent([event[0], event[1] - (1 / score.fs)], [1, 1], color, ax,
+                   [max(0, event[0] - param.toleranceStart), min(time[-1], event[1] + param.toleranceEnd - (1 / ref.fs))])
 
     # Plot HYP TP & FP
-    for event in hyp.events:
+    for event in score.hyp.events:
         # FP
         if np.all(~score.tpMask[round(event[0] * score.fs):round(event[1] * score.fs)]):
-            _plotEvent([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5], 'tab:red', ax)
+            _plotEvent([event[0], event[1] - (1 / score.fs)], [0.5, 0.5], 'tab:red', ax)
         # TP
         elif np.all(score.tpMask[round(event[0] * score.fs):round(event[1] * score.fs)]):
-            ax.plot([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5],
+            ax.plot([event[0], event[1] - (1 / score.fs)], [0.5, 0.5],
                     color='tab:green', linewidth=5, solid_capstyle='butt', linestyle='solid')
         # Mix TP, FP
         else:
-            _plotEvent([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5], 'tab:red', ax)
-            ax.plot([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5],
+            _plotEvent([event[0], event[1] - (1 / score.fs)], [0.5, 0.5], 'tab:red', ax, zorder=1.7)
+            ax.plot([event[0], event[1] - (1 / score.fs)], [0.5, 0.5],
                     color='tab:green', linewidth=5, solid_capstyle='butt', linestyle=(0, (2, 2)))
 
     # Text
     plt.title('Event Scoring')
 
     ax.set_yticks([0.3, 0.8], ['HYP', 'REF'])
     _scale_time_xaxis(ax)
@@ -221,7 +222,34 @@
     textstr += "• F1 - score   : {:.2f}".format(score.f1)
     ax.text(1.02, 0.05, textstr, fontsize=12, transform=ax.transAxes)
 
     # Adjust spacing
     ax.margins(x=0)  # No margin on X data
     plt.tight_layout()
     plt.subplots_adjust(right=0.86)  # Allow space for scoring text
+
+
+def _plotEvent(x, y, color, ax, bckg=None, zorder=1.8):
+    if bckg is None:
+        bckg = x
+    ax.axvspan(bckg[0], bckg[1], color=adjust_lightness(color, 0.2), zorder=zorder)
+    if x[1] - x[0] > 0:
+        ax.plot(x, y, color=color, linewidth=5, solid_capstyle='butt')
+    else:
+        ax.scatter(x[0], y[0], color=color)
+
+
+def _plotSplitLongEvents(event, maxEventDuration, y):
+    """ Visualize split of long events """
+    t = event[0] + maxEventDuration
+    while t < event[1]:
+        plt.plot([t, t], y, '--k', zorder=1.9)
+        t += maxEventDuration
+
+
+def adjust_lightness(color, amount=0.5):
+    try:
+        c = mc.cnames[color]
+    except KeyError:
+        c = color
+    c = colorsys.rgb_to_hls(*mc.to_rgb(c))
+    return colorsys.hls_to_rgb(c[0], 1 - amount * (1 - c[1]), c[2])
```

### Comparing `timescoring-0.0.3/tests/test.py` & `timescoring-0.0.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.3/LICENSE` & `timescoring-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.3/README.md` & `timescoring-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 In more details, we measures performance on the level of:
 
 - Sample : Performance metric that threats every label sample independently.
 - Events (e.g. epileptic seizure) : Classifies each event in both reference and hypothesis based on overlap of both.
 
 Both methods are illustrated in the following figures :
 
-![Illustration of sample based scoring.](https://user-images.githubusercontent.com/747240/244666630-cdfe12cc-22a2-4b23-be15-3e60dbedb437.png)
-![Illustration of event based scoring.](https://user-images.githubusercontent.com/747240/244666619-8dd90008-79af-4836-8769-daa204bbe16c.png)
+![Illustration of sample based scoring.](https://user-images.githubusercontent.com/747240/248309097-b7f76fde-c87a-41df-812d-9821375b640e.png)
+![Illustration of event based scoring.](https://user-images.githubusercontent.com/747240/248308898-64b4ae39-d02f-4f06-9b10-f07aaf6110d1.png)
 
 ## Installation
 
 The package can be installed through pip using the following command :
 
 `pip install timescoring`
```

### Comparing `timescoring-0.0.3/pyproject.toml` & `timescoring-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "timescoring"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Jonathan Dan", email="jonathan.dan@epfl.ch" },
   { name="Una Pale", email="una.pale@epfl.ch" },
   { name="PEDESITE" }
 ]
 description = "Library for measuring performance of time series classification"
 readme = "README.md"
```

### Comparing `timescoring-0.0.3/PKG-INFO` & `timescoring-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timescoring
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library for measuring performance of time series classification
 Project-URL: Homepage, https://github.com/esl-epfl/epilepsy_performance_metrics
 Project-URL: Bug Tracker, https://github.com/esl-epfl/epilepsy_performance_metrics/issues
 Author: PEDESITE
 Author-email: Jonathan Dan <jonathan.dan@epfl.ch>, Una Pale <una.pale@epfl.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -34,16 +34,16 @@
 In more details, we measures performance on the level of:
 
 - Sample : Performance metric that threats every label sample independently.
 - Events (e.g. epileptic seizure) : Classifies each event in both reference and hypothesis based on overlap of both.
 
 Both methods are illustrated in the following figures :
 
-![Illustration of sample based scoring.](https://user-images.githubusercontent.com/747240/244666630-cdfe12cc-22a2-4b23-be15-3e60dbedb437.png)
-![Illustration of event based scoring.](https://user-images.githubusercontent.com/747240/244666619-8dd90008-79af-4836-8769-daa204bbe16c.png)
+![Illustration of sample based scoring.](https://user-images.githubusercontent.com/747240/248309097-b7f76fde-c87a-41df-812d-9821375b640e.png)
+![Illustration of event based scoring.](https://user-images.githubusercontent.com/747240/248308898-64b4ae39-d02f-4f06-9b10-f07aaf6110d1.png)
 
 ## Installation
 
 The package can be installed through pip using the following command :
 
 `pip install timescoring`
```

