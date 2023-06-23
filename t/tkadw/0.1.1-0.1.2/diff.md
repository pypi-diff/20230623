# Comparing `tmp/tkadw-0.1.1.tar.gz` & `tmp/tkadw-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkadw-0.1.1.tar", max compression
+gzip compressed data, was "tkadw-0.1.2.tar", max compression
```

## Comparing `tkadw-0.1.1.tar` & `tkadw-0.1.2.tar`

### file list

```diff
@@ -1,206 +1,218 @@
--rw-r--r--   0        0        0      274 2023-06-23 03:45:25.506683 tkadw-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      101 2023-04-15 23:36:06.262325 tkadw-0.1.1/README.md
--rw-r--r--   0        0        0      112 2023-06-23 03:45:25.577456 tkadw-0.1.1/tkadw/__init__.py
--rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.1.1/tkadw/app.config
--rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.1.1/tkadw/appconfig.py
--rw-r--r--   0        0        0      586 2023-06-23 03:34:48.929456 tkadw-0.1.1/tkadw/canvas/__init__.py
--rw-r--r--   0        0        0     1141 2023-06-23 03:34:49.176813 tkadw-0.1.1/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.1.1/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    22027 2023-06-23 03:25:42.297840 tkadw-0.1.1/tkadw/canvas/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.1.1/tkadw/canvas/__pycache__/button.cpython-38.pyc
--rw-r--r--   0        0        0    22937 2023-06-10 11:13:04.365819 tkadw-0.1.1/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
--rw-r--r--   0        0        0    25637 2023-06-23 03:40:57.567704 tkadw-0.1.1/tkadw/canvas/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.1.1/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0        0 2023-06-10 10:53:44.353940 tkadw-0.1.1/tkadw/canvas/adwite/__init__.py
--rw-r--r--   0        0        0     1363 2023-06-10 11:23:03.996035 tkadw-0.1.1/tkadw/canvas/adwite/button.py
--rw-r--r--   0        0        0       80 2023-06-09 13:54:04.880107 tkadw-0.1.1/tkadw/canvas/atomize/__init__.py
--rw-r--r--   0        0        0     2520 2023-06-10 04:30:03.863844 tkadw-0.1.1/tkadw/canvas/atomize/button.py
--rw-r--r--   0        0        0    16899 2023-06-23 03:25:41.953997 tkadw-0.1.1/tkadw/canvas/button.py
--rw-r--r--   0        0        0     3263 2023-06-10 03:45:43.121120 tkadw-0.1.1/tkadw/canvas/demo.tcl
--rw-r--r--   0        0        0    20295 2023-06-10 11:13:04.292305 tkadw-0.1.1/tkadw/canvas/drawengine.py
--rw-r--r--   0        0        0    22085 2023-06-23 03:40:57.248638 tkadw-0.1.1/tkadw/canvas/entry.py
--rw-r--r--   0        0        0      513 2023-06-09 23:26:21.009369 tkadw-0.1.1/tkadw/canvas/fluent/__init__.py
--rw-r--r--   0        0        0     2051 2023-06-10 01:20:40.907297 tkadw-0.1.1/tkadw/canvas/fun.py
--rw-r--r--   0        0        0    15490 2023-06-10 01:25:11.532315 tkadw-0.1.1/tkadw/canvas/fun2.py
--rw-r--r--   0        0        0     8108 2023-06-10 01:29:02.970946 tkadw-0.1.1/tkadw/canvas/fun3.py
--rw-r--r--   0        0        0     3202 2023-06-10 03:27:44.231516 tkadw-0.1.1/tkadw/canvas/fun4.py
--rw-r--r--   0        0        0      942 2023-06-10 03:50:17.322506 tkadw-0.1.1/tkadw/canvas/fun5.py
--rw-r--r--   0        0        0     9870 2023-06-10 07:36:40.103845 tkadw-0.1.1/tkadw/canvas/fun6.py
--rw-r--r--   0        0        0     5690 2023-06-10 03:45:21.292347 tkadw-0.1.1/tkadw/canvas/poly.tcl
--rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.1.1/tkadw/canvas/titlebar.py
--rw-r--r--   0        0        0       29 2023-06-23 03:45:25.647673 tkadw-0.1.1/tkadw/tkite/__init__.py
--rw-r--r--   0        0        0      130 2023-06-23 03:42:34.068346 tkadw-0.1.1/tkadw/tkite/gtk/__init__.py
--rw-r--r--   0        0        0     2859 2023-06-23 01:27:57.541720 tkadw-0.1.1/tkadw/tkite/gtk/button.py
--rw-r--r--   0        0        0     1163 2023-06-23 03:39:51.907174 tkadw-0.1.1/tkadw/tkite/gtk/entry.py
--rw-r--r--   0        0        0      500 2023-06-23 00:56:14.658098 tkadw-0.1.1/tkadw/tkite/gtk/notebook.py
--rw-r--r--   0        0        0        0 2023-06-09 14:28:28.424277 tkadw-0.1.1/tkadw/ttk/__init__.py
--rw-r--r--   0        0        0      139 2023-06-09 14:38:22.776399 tkadw-0.1.1/tkadw/ttk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1349 2023-06-09 14:41:39.497543 tkadw-0.1.1/tkadw/ttk/atomize_ttk/__init__.py
--rw-r--r--   0        0        0     2722 2023-06-09 14:43:18.298069 tkadw-0.1.1/tkadw/ttk/atomize_ttk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2961 2023-06-09 14:41:39.498543 tkadw-0.1.1/tkadw/ttk/atomize_ttk/sun-valley.tcl
--rw-r--r--   0        0        0     5150 2023-05-14 15:25:00.266570 tkadw-0.1.1/tkadw/ttk/atomize_ttk/sv.tcl
--rw-r--r--   0        0        0      270 2023-06-09 14:41:39.500545 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/arrow-down.png
--rw-r--r--   0        0        0      261 2023-06-09 14:41:39.501544 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/arrow-right.png
--rw-r--r--   0        0        0      274 2023-06-09 14:41:39.501544 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/arrow-up.png
--rw-r--r--   0        0        0      262 2023-06-09 14:41:39.502544 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-accent-disabled.png
--rw-r--r--   0        0        0      373 2023-06-09 14:41:39.503545 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-accent-hover.png
--rw-r--r--   0        0        0      363 2023-06-09 14:41:39.503545 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-accent-pressed.png
--rw-r--r--   0        0        0      377 2023-06-09 14:41:39.504545 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-accent-rest.png
--rw-r--r--   0        0        0      274 2023-06-09 14:41:39.505542 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-close-hover.png
--rw-r--r--   0        0        0      274 2023-06-09 14:41:39.505542 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-close-pressed.png
--rw-r--r--   0        0        0      301 2023-06-09 14:41:39.506544 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-disabled.png
--rw-r--r--   0        0        0      276 2023-06-09 14:41:39.506544 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-hover.png
--rw-r--r--   0        0        0      288 2023-06-09 14:41:39.507543 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-pressed.png
--rw-r--r--   0        0        0      301 2023-06-09 14:41:39.508543 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-rest.png
--rw-r--r--   0        0        0      245 2023-06-09 14:41:39.508543 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-titlebar-hover.png
--rw-r--r--   0        0        0      238 2023-06-09 14:41:39.509543 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/button-titlebar-pressed.png
--rw-r--r--   0        0        0      386 2023-06-09 14:41:39.509543 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/card.png
--rw-r--r--   0        0        0      383 2023-06-09 14:41:39.510542 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-disabled.png
--rw-r--r--   0        0        0      474 2023-06-09 14:41:39.511543 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-hover.png
--rw-r--r--   0        0        0      460 2023-06-09 14:41:39.511543 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-pressed.png
--rw-r--r--   0        0        0      475 2023-06-09 14:41:39.512544 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-rest.png
--rw-r--r--   0        0        0      294 2023-06-09 14:41:39.513547 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-tri-disabled.png
--rw-r--r--   0        0        0      362 2023-06-09 14:41:39.514132 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-tri-hover.png
--rw-r--r--   0        0        0      358 2023-06-09 14:41:39.515137 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-tri-pressed.png
--rw-r--r--   0        0        0      363 2023-06-09 14:41:39.515137 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-tri-rest.png
--rw-r--r--   0        0        0      312 2023-06-09 14:41:39.516139 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-disabled.png
--rw-r--r--   0        0        0      353 2023-06-09 14:41:39.517139 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-hover.png
--rw-r--r--   0        0        0      302 2023-06-09 14:41:39.517139 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-pressed.png
--rw-r--r--   0        0        0      353 2023-06-09 14:41:39.518137 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-rest.png
--rw-r--r--   0        0        0      129 2023-06-09 14:41:39.519137 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/empty.png
--rw-r--r--   0        0        0      273 2023-06-09 14:41:39.519137 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/entry-disabled.png
--rw-r--r--   0        0        0      335 2023-06-09 14:41:39.520136 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/entry-focus.png
--rw-r--r--   0        0        0      269 2023-06-09 14:41:39.521137 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/entry-hover.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.522140 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/entry-invalid.png
--rw-r--r--   0        0        0      297 2023-06-09 14:41:39.522140 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/entry-rest.png
--rw-r--r--   0        0        0      337 2023-06-09 14:41:39.523139 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/notebook-border.png
--rw-r--r--   0        0        0      186 2023-06-09 14:41:39.524139 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/notebook.png
--rw-r--r--   0        0        0      193 2023-06-09 14:41:39.524139 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/progress-pbar-hor.png
--rw-r--r--   0        0        0      214 2023-06-09 14:41:39.525137 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/progress-pbar-vert.png
--rw-r--r--   0        0        0      157 2023-06-09 14:41:39.526137 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/progress-trough-hor.png
--rw-r--r--   0        0        0      160 2023-06-09 14:41:39.526137 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/progress-trough-vert.png
--rw-r--r--   0        0        0      553 2023-06-09 14:41:39.527138 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-disabled.png
--rw-r--r--   0        0        0      853 2023-06-09 14:41:39.527138 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-hover.png
--rw-r--r--   0        0        0      786 2023-06-09 14:41:39.528137 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-pressed.png
--rw-r--r--   0        0        0      830 2023-06-09 14:41:39.528640 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-rest.png
--rw-r--r--   0        0        0      552 2023-06-09 14:41:39.529647 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-disabled.png
--rw-r--r--   0        0        0      602 2023-06-09 14:41:39.530644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-hover.png
--rw-r--r--   0        0        0      616 2023-06-09 14:41:39.530644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-pressed.png
--rw-r--r--   0        0        0      621 2023-06-09 14:41:39.531645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-rest.png
--rw-r--r--   0        0        0      724 2023-06-09 14:41:39.532645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-disabled.png
--rw-r--r--   0        0        0      808 2023-06-09 14:41:39.532645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-hover.png
--rw-r--r--   0        0        0      735 2023-06-09 14:41:39.533645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-pressed.png
--rw-r--r--   0        0        0      771 2023-06-09 14:41:39.533645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-rest.png
--rw-r--r--   0        0        0      216 2023-06-09 14:41:39.534644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scale-trough-hor.png
--rw-r--r--   0        0        0      215 2023-06-09 14:41:39.534644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scale-trough-vert.png
--rw-r--r--   0        0        0      226 2023-06-09 14:41:39.535644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scroll-down.png
--rw-r--r--   0        0        0      254 2023-06-09 14:41:39.536643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scroll-hor-thumb.png
--rw-r--r--   0        0        0      338 2023-06-09 14:41:39.537644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scroll-hor-trough.png
--rw-r--r--   0        0        0      233 2023-06-09 14:41:39.538644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scroll-left.png
--rw-r--r--   0        0        0      227 2023-06-09 14:41:39.538644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scroll-right.png
--rw-r--r--   0        0        0      236 2023-06-09 14:41:39.539644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scroll-up.png
--rw-r--r--   0        0        0      264 2023-06-09 14:41:39.539644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scroll-vert-thumb.png
--rw-r--r--   0        0        0      343 2023-06-09 14:41:39.540644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scroll-vert-trough.png
--rw-r--r--   0        0        0      128 2023-06-09 14:41:39.541644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/separator.png
--rw-r--r--   0        0        0      276 2023-06-09 14:41:39.542647 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/sizegrip.png
--rw-r--r--   0        0        0      733 2023-06-09 14:41:39.542647 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-off-disabled.png
--rw-r--r--   0        0        0      945 2023-06-09 14:41:39.543645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-off-hover.png
--rw-r--r--   0        0        0      963 2023-06-09 14:41:39.544643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-off-pressed.png
--rw-r--r--   0        0        0      895 2023-06-09 14:41:39.545645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-off-rest.png
--rw-r--r--   0        0        0      623 2023-06-09 14:41:39.545645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-on-disabled.png
--rw-r--r--   0        0        0      927 2023-06-09 14:41:39.546644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-on-hover.png
--rw-r--r--   0        0        0      936 2023-06-09 14:41:39.547644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-on-pressed.png
--rw-r--r--   0        0        0      859 2023-06-09 14:41:39.547644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-on-rest.png
--rw-r--r--   0        0        0      265 2023-06-09 14:41:39.548643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/tab-hover.png
--rw-r--r--   0        0        0      164 2023-06-09 14:41:39.549644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/tab-rest.png
--rw-r--r--   0        0        0      319 2023-06-09 14:41:39.549644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/tab-selected.png
--rw-r--r--   0        0        0      295 2023-06-09 14:41:39.550645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/treeheading-hover.png
--rw-r--r--   0        0        0      317 2023-06-09 14:41:39.551644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/treeheading-pressed.png
--rw-r--r--   0        0        0      321 2023-06-09 14:41:39.551644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/treeheading-rest.png
--rw-r--r--   0        0        0    20188 2023-06-09 14:41:39.499549 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark.tcl
--rw-r--r--   0        0        0      278 2023-06-09 14:41:39.552643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/arrow-down.png
--rw-r--r--   0        0        0      273 2023-06-09 14:41:39.552643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/arrow-right.png
--rw-r--r--   0        0        0      285 2023-06-09 14:41:39.553645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/arrow-up.png
--rw-r--r--   0        0        0      271 2023-06-09 14:41:39.554647 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-accent-disabled.png
--rw-r--r--   0        0        0      219 2023-06-09 14:48:51.766400 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-accent-hover.png
--rw-r--r--   0        0        0      255 2023-06-09 14:53:14.082428 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-accent-pressed.png
--rw-r--r--   0        0        0      217 2023-06-09 14:48:47.641380 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-accent-rest.png
--rw-r--r--   0        0        0      326 2023-06-09 14:41:39.556644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-close-hover.png
--rw-r--r--   0        0        0      316 2023-06-09 14:41:39.557644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-close-pressed.png
--rw-r--r--   0        0        0      307 2023-06-09 14:41:39.557644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-disabled.png
--rw-r--r--   0        0        0      306 2023-06-09 14:41:39.558645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-hover.png
--rw-r--r--   0        0        0      289 2023-06-09 14:41:39.559644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-pressed.png
--rw-r--r--   0        0        0      303 2023-06-09 14:41:39.559644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-rest.png
--rw-r--r--   0        0        0      238 2023-06-09 14:41:39.560643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-titlebar-hover.png
--rw-r--r--   0        0        0      225 2023-06-09 14:41:39.561643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/button-titlebar-pressed.png
--rw-r--r--   0        0        0      479 2023-06-09 14:43:10.460434 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/card.png
--rw-r--r--   0        0        0      381 2023-06-09 14:41:39.562646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-disabled.png
--rw-r--r--   0        0        0      476 2023-06-09 14:41:39.562646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-hover.png
--rw-r--r--   0        0        0      467 2023-06-09 14:41:39.563646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-pressed.png
--rw-r--r--   0        0        0      473 2023-06-09 14:41:39.564644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-rest.png
--rw-r--r--   0        0        0      299 2023-06-09 14:41:39.564644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-tri-disabled.png
--rw-r--r--   0        0        0      365 2023-06-09 14:41:39.565643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-tri-hover.png
--rw-r--r--   0        0        0      362 2023-06-09 14:41:39.566644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-tri-pressed.png
--rw-r--r--   0        0        0      367 2023-06-09 14:41:39.566644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-tri-rest.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.567644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-unsel-disabled.png
--rw-r--r--   0        0        0      334 2023-06-09 14:41:39.568643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-unsel-hover.png
--rw-r--r--   0        0        0      302 2023-06-09 14:41:39.568643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-unsel-pressed.png
--rw-r--r--   0        0        0      333 2023-06-09 14:41:39.569646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/check-unsel-rest.png
--rw-r--r--   0        0        0      129 2023-06-09 14:41:39.569646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/empty.png
--rw-r--r--   0        0        0      289 2023-06-09 14:41:39.570644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/entry-disabled.png
--rw-r--r--   0        0        0      331 2023-06-09 14:41:39.571647 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/entry-focus.png
--rw-r--r--   0        0        0      302 2023-06-09 14:41:39.572644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/entry-hover.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.572644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/entry-invalid.png
--rw-r--r--   0        0        0      308 2023-06-09 14:41:39.573646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/entry-rest.png
--rw-r--r--   0        0        0      298 2023-06-09 14:41:39.573646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/notebook-border.png
--rw-r--r--   0        0        0      185 2023-06-09 14:41:39.574643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/notebook.png
--rw-r--r--   0        0        0      192 2023-06-09 14:41:39.575643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/progress-pbar-hor.png
--rw-r--r--   0        0        0      216 2023-06-09 14:41:39.575643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/progress-pbar-vert.png
--rw-r--r--   0        0        0      158 2023-06-09 14:41:39.576643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/progress-trough-hor.png
--rw-r--r--   0        0        0      161 2023-06-09 14:41:39.577644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/progress-trough-vert.png
--rw-r--r--   0        0        0      523 2023-06-09 14:41:39.578645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-disabled.png
--rw-r--r--   0        0        0      837 2023-06-09 14:41:39.578645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-hover.png
--rw-r--r--   0        0        0      764 2023-06-09 14:41:39.579645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-pressed.png
--rw-r--r--   0        0        0      773 2023-06-09 14:41:39.580644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-rest.png
--rw-r--r--   0        0        0      521 2023-06-09 14:41:39.581644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-disabled.png
--rw-r--r--   0        0        0      573 2023-06-09 14:41:39.582644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-hover.png
--rw-r--r--   0        0        0      636 2023-06-09 14:41:39.582644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-pressed.png
--rw-r--r--   0        0        0      576 2023-06-09 14:41:39.583644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-rest.png
--rw-r--r--   0        0        0      658 2023-06-09 14:41:39.584643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-disabled.png
--rw-r--r--   0        0        0      749 2023-06-09 14:41:39.584643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-hover.png
--rw-r--r--   0        0        0      675 2023-06-09 14:41:39.585645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-pressed.png
--rw-r--r--   0        0        0      701 2023-06-09 14:41:39.586645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-rest.png
--rw-r--r--   0        0        0      208 2023-06-09 14:41:39.586645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scale-trough-hor.png
--rw-r--r--   0        0        0      214 2023-06-09 14:41:39.587646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scale-trough-vert.png
--rw-r--r--   0        0        0      229 2023-06-09 14:41:39.588644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scroll-down.png
--rw-r--r--   0        0        0      234 2023-06-09 14:41:39.589644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scroll-hor-thumb.png
--rw-r--r--   0        0        0      321 2023-06-09 14:41:39.589644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scroll-hor-trough.png
--rw-r--r--   0        0        0      232 2023-06-09 14:41:39.590644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scroll-left.png
--rw-r--r--   0        0        0      223 2023-06-09 14:41:39.590644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scroll-right.png
--rw-r--r--   0        0        0      237 2023-06-09 14:41:39.591643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scroll-up.png
--rw-r--r--   0        0        0      262 2023-06-09 14:41:39.592644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scroll-vert-thumb.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.593644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scroll-vert-trough.png
--rw-r--r--   0        0        0      128 2023-06-09 14:41:39.594646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/separator.png
--rw-r--r--   0        0        0      272 2023-06-09 14:41:39.594646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/sizegrip.png
--rw-r--r--   0        0        0      726 2023-06-09 14:41:39.595643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-off-disabled.png
--rw-r--r--   0        0        0      867 2023-06-09 14:41:39.596647 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-off-hover.png
--rw-r--r--   0        0        0      880 2023-06-09 14:41:39.597645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-off-pressed.png
--rw-r--r--   0        0        0      814 2023-06-09 14:41:39.597645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-off-rest.png
--rw-r--r--   0        0        0      590 2023-06-09 14:41:39.598645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-on-disabled.png
--rw-r--r--   0        0        0      906 2023-06-09 14:41:39.598645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-on-hover.png
--rw-r--r--   0        0        0      916 2023-06-09 14:41:39.599644 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-on-pressed.png
--rw-r--r--   0        0        0      857 2023-06-09 14:41:39.600643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-on-rest.png
--rw-r--r--   0        0        0      295 2023-06-09 14:41:39.600643 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/tab-hover.png
--rw-r--r--   0        0        0      164 2023-06-09 14:41:39.601645 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/tab-rest.png
--rw-r--r--   0        0        0      318 2023-06-09 14:41:39.602649 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/tab-selected.png
--rw-r--r--   0        0        0      338 2023-06-09 14:41:39.602649 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/treeheading-hover.png
--rw-r--r--   0        0        0      318 2023-06-09 14:41:39.603646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/treeheading-pressed.png
--rw-r--r--   0        0        0      330 2023-06-09 14:41:39.603646 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/treeheading-rest.png
--rw-r--r--   0        0        0    20371 2023-06-09 14:41:39.500545 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light.tcl
--rw-r--r--   0        0        0     3045 2023-05-14 15:25:00.269895 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/sprites_dark.tcl
--rw-r--r--   0        0        0     3092 2023-05-14 15:25:00.270897 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/sprites_light.tcl
--rw-r--r--   0        0        0    18371 2023-05-14 15:25:00.272896 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/spritesheet_dark.png
--rw-r--r--   0        0        0     2649 2023-06-09 14:36:51.668892 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/spritesheet_light.png
--rw-r--r--   0        0        0    18462 2023-05-14 15:25:00.272896 tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/spritesheet_light2.png
--rw-r--r--   0        0        0      372 2023-06-09 14:40:30.166428 tkadw-0.1.1/tkadw/ttk/test.py
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 tkadw-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      274 2023-06-23 07:49:33.316949 tkadw-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-04-15 23:36:06.262325 tkadw-0.1.2/README.md
+-rw-r--r--   0        0        0      112 2023-06-23 03:45:25.577456 tkadw-0.1.2/tkadw/__init__.py
+-rw-r--r--   0        0        0      948 2023-06-23 07:49:26.692233 tkadw-0.1.2/tkadw/__main__.py
+-rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.1.2/tkadw/app.config
+-rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.1.2/tkadw/appconfig.py
+-rw-r--r--   0        0        0      896 2023-06-23 07:36:10.506439 tkadw-0.1.2/tkadw/canvas/__init__.py
+-rw-r--r--   0        0        0     1701 2023-06-23 07:38:42.890718 tkadw-0.1.2/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.1.2/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    22885 2023-06-23 04:54:52.588047 tkadw-0.1.2/tkadw/canvas/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.1.2/tkadw/canvas/__pycache__/button.cpython-38.pyc
+-rw-r--r--   0        0        0    23239 2023-06-23 05:05:08.679421 tkadw-0.1.2/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
+-rw-r--r--   0        0        0    25982 2023-06-23 07:48:50.831965 tkadw-0.1.2/tkadw/canvas/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0    13288 2023-06-23 07:38:42.954769 tkadw-0.1.2/tkadw/canvas/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.1.2/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    27814 2023-06-23 07:48:50.836964 tkadw-0.1.2/tkadw/canvas/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-06-10 10:53:44.353940 tkadw-0.1.2/tkadw/canvas/adwite/__init__.py
+-rw-r--r--   0        0        0     1363 2023-06-10 11:23:03.996035 tkadw-0.1.2/tkadw/canvas/adwite/button.py
+-rw-r--r--   0        0        0       80 2023-06-09 13:54:04.880107 tkadw-0.1.2/tkadw/canvas/atomize/__init__.py
+-rw-r--r--   0        0        0     2520 2023-06-10 04:30:03.863844 tkadw-0.1.2/tkadw/canvas/atomize/button.py
+-rw-r--r--   0        0        0    17270 2023-06-23 04:54:52.447686 tkadw-0.1.2/tkadw/canvas/button.py
+-rw-r--r--   0        0        0    20382 2023-06-23 05:05:08.591410 tkadw-0.1.2/tkadw/canvas/drawengine.py
+-rw-r--r--   0        0        0    22377 2023-06-23 07:48:50.714445 tkadw-0.1.2/tkadw/canvas/entry.py
+-rw-r--r--   0        0        0      513 2023-06-09 23:26:21.009369 tkadw-0.1.2/tkadw/canvas/fluent/__init__.py
+-rw-r--r--   0        0        0     8629 2023-06-23 05:15:43.010231 tkadw-0.1.2/tkadw/canvas/frame.py
+-rw-r--r--   0        0        0     2051 2023-06-10 01:20:40.907297 tkadw-0.1.2/tkadw/canvas/fun.py
+-rw-r--r--   0        0        0    15490 2023-06-10 01:25:11.532315 tkadw-0.1.2/tkadw/canvas/fun2.py
+-rw-r--r--   0        0        0     8108 2023-06-10 01:29:02.970946 tkadw-0.1.2/tkadw/canvas/fun3.py
+-rw-r--r--   0        0        0     3202 2023-06-10 03:27:44.231516 tkadw-0.1.2/tkadw/canvas/fun4.py
+-rw-r--r--   0        0        0      942 2023-06-10 03:50:17.322506 tkadw-0.1.2/tkadw/canvas/fun5.py
+-rw-r--r--   0        0        0     9870 2023-06-10 07:36:40.103845 tkadw-0.1.2/tkadw/canvas/fun6.py
+-rw-r--r--   0        0        0     5690 2023-06-10 03:45:21.292347 tkadw-0.1.2/tkadw/canvas/poly.tcl
+-rw-r--r--   0        0        0    22421 2023-06-23 07:48:50.681445 tkadw-0.1.2/tkadw/canvas/textbox.py
+-rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.1.2/tkadw/canvas/titlebar.py
+-rw-r--r--   0        0        0       29 2023-06-23 03:52:51.957932 tkadw-0.1.2/tkadw/tkite/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-23 03:52:52.129145 tkadw-0.1.2/tkadw/tkite/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      283 2023-06-23 07:44:06.875178 tkadw-0.1.2/tkadw/tkite/gtk/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-23 07:44:06.983012 tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5020 2023-06-23 05:37:39.419391 tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     2902 2023-06-23 05:36:24.094777 tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     2457 2023-06-23 07:42:27.405172 tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0     3908 2023-06-23 07:45:23.356231 tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0     3898 2023-06-23 05:37:39.292931 tkadw-0.1.2/tkadw/tkite/gtk/button.py
+-rw-r--r--   0        0        0     2201 2023-06-23 05:36:23.978561 tkadw-0.1.2/tkadw/tkite/gtk/entry.py
+-rw-r--r--   0        0        0     1141 2023-06-23 07:40:36.374539 tkadw-0.1.2/tkadw/tkite/gtk/frame.py
+-rw-r--r--   0        0        0      500 2023-06-23 00:56:14.658098 tkadw-0.1.2/tkadw/tkite/gtk/notebook.py
+-rw-r--r--   0        0        0     2785 2023-06-23 07:45:23.240982 tkadw-0.1.2/tkadw/tkite/gtk/textbox.py
+-rw-r--r--   0        0        0        0 2023-06-09 14:28:28.424277 tkadw-0.1.2/tkadw/ttk/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-09 14:38:22.776399 tkadw-0.1.2/tkadw/ttk/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1349 2023-06-09 14:41:39.497543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/__init__.py
+-rw-r--r--   0        0        0     2722 2023-06-09 14:43:18.298069 tkadw-0.1.2/tkadw/ttk/atomize_ttk/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2961 2023-06-09 14:41:39.498543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/sun-valley.tcl
+-rw-r--r--   0        0        0     5150 2023-05-14 15:25:00.266570 tkadw-0.1.2/tkadw/ttk/atomize_ttk/sv.tcl
+-rw-r--r--   0        0        0      270 2023-06-09 14:41:39.500545 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/arrow-down.png
+-rw-r--r--   0        0        0      261 2023-06-09 14:41:39.501544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/arrow-right.png
+-rw-r--r--   0        0        0      274 2023-06-09 14:41:39.501544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/arrow-up.png
+-rw-r--r--   0        0        0      262 2023-06-09 14:41:39.502544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-accent-disabled.png
+-rw-r--r--   0        0        0      373 2023-06-09 14:41:39.503545 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-accent-hover.png
+-rw-r--r--   0        0        0      363 2023-06-09 14:41:39.503545 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-accent-pressed.png
+-rw-r--r--   0        0        0      377 2023-06-09 14:41:39.504545 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-accent-rest.png
+-rw-r--r--   0        0        0      274 2023-06-09 14:41:39.505542 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-close-hover.png
+-rw-r--r--   0        0        0      274 2023-06-09 14:41:39.505542 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-close-pressed.png
+-rw-r--r--   0        0        0      301 2023-06-09 14:41:39.506544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-disabled.png
+-rw-r--r--   0        0        0      276 2023-06-09 14:41:39.506544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-hover.png
+-rw-r--r--   0        0        0      288 2023-06-09 14:41:39.507543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-pressed.png
+-rw-r--r--   0        0        0      301 2023-06-09 14:41:39.508543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-rest.png
+-rw-r--r--   0        0        0      245 2023-06-09 14:41:39.508543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-titlebar-hover.png
+-rw-r--r--   0        0        0      238 2023-06-09 14:41:39.509543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-titlebar-pressed.png
+-rw-r--r--   0        0        0      386 2023-06-09 14:41:39.509543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/card.png
+-rw-r--r--   0        0        0      383 2023-06-09 14:41:39.510542 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-disabled.png
+-rw-r--r--   0        0        0      474 2023-06-09 14:41:39.511543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-hover.png
+-rw-r--r--   0        0        0      460 2023-06-09 14:41:39.511543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-pressed.png
+-rw-r--r--   0        0        0      475 2023-06-09 14:41:39.512544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-rest.png
+-rw-r--r--   0        0        0      294 2023-06-09 14:41:39.513547 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-tri-disabled.png
+-rw-r--r--   0        0        0      362 2023-06-09 14:41:39.514132 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-tri-hover.png
+-rw-r--r--   0        0        0      358 2023-06-09 14:41:39.515137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-tri-pressed.png
+-rw-r--r--   0        0        0      363 2023-06-09 14:41:39.515137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-tri-rest.png
+-rw-r--r--   0        0        0      312 2023-06-09 14:41:39.516139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-disabled.png
+-rw-r--r--   0        0        0      353 2023-06-09 14:41:39.517139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-hover.png
+-rw-r--r--   0        0        0      302 2023-06-09 14:41:39.517139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-pressed.png
+-rw-r--r--   0        0        0      353 2023-06-09 14:41:39.518137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-rest.png
+-rw-r--r--   0        0        0      129 2023-06-09 14:41:39.519137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/empty.png
+-rw-r--r--   0        0        0      273 2023-06-09 14:41:39.519137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/entry-disabled.png
+-rw-r--r--   0        0        0      335 2023-06-09 14:41:39.520136 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/entry-focus.png
+-rw-r--r--   0        0        0      269 2023-06-09 14:41:39.521137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/entry-hover.png
+-rw-r--r--   0        0        0      324 2023-06-09 14:41:39.522140 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/entry-invalid.png
+-rw-r--r--   0        0        0      297 2023-06-09 14:41:39.522140 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/entry-rest.png
+-rw-r--r--   0        0        0      337 2023-06-09 14:41:39.523139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/notebook-border.png
+-rw-r--r--   0        0        0      186 2023-06-09 14:41:39.524139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/notebook.png
+-rw-r--r--   0        0        0      193 2023-06-09 14:41:39.524139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/progress-pbar-hor.png
+-rw-r--r--   0        0        0      214 2023-06-09 14:41:39.525137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/progress-pbar-vert.png
+-rw-r--r--   0        0        0      157 2023-06-09 14:41:39.526137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/progress-trough-hor.png
+-rw-r--r--   0        0        0      160 2023-06-09 14:41:39.526137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/progress-trough-vert.png
+-rw-r--r--   0        0        0      553 2023-06-09 14:41:39.527138 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-disabled.png
+-rw-r--r--   0        0        0      853 2023-06-09 14:41:39.527138 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-hover.png
+-rw-r--r--   0        0        0      786 2023-06-09 14:41:39.528137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-pressed.png
+-rw-r--r--   0        0        0      830 2023-06-09 14:41:39.528640 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-rest.png
+-rw-r--r--   0        0        0      552 2023-06-09 14:41:39.529647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-disabled.png
+-rw-r--r--   0        0        0      602 2023-06-09 14:41:39.530644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-hover.png
+-rw-r--r--   0        0        0      616 2023-06-09 14:41:39.530644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-pressed.png
+-rw-r--r--   0        0        0      621 2023-06-09 14:41:39.531645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-rest.png
+-rw-r--r--   0        0        0      724 2023-06-09 14:41:39.532645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-disabled.png
+-rw-r--r--   0        0        0      808 2023-06-09 14:41:39.532645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-hover.png
+-rw-r--r--   0        0        0      735 2023-06-09 14:41:39.533645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-pressed.png
+-rw-r--r--   0        0        0      771 2023-06-09 14:41:39.533645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-rest.png
+-rw-r--r--   0        0        0      216 2023-06-09 14:41:39.534644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-trough-hor.png
+-rw-r--r--   0        0        0      215 2023-06-09 14:41:39.534644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-trough-vert.png
+-rw-r--r--   0        0        0      226 2023-06-09 14:41:39.535644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-down.png
+-rw-r--r--   0        0        0      254 2023-06-09 14:41:39.536643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-hor-thumb.png
+-rw-r--r--   0        0        0      338 2023-06-09 14:41:39.537644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-hor-trough.png
+-rw-r--r--   0        0        0      233 2023-06-09 14:41:39.538644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-left.png
+-rw-r--r--   0        0        0      227 2023-06-09 14:41:39.538644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-right.png
+-rw-r--r--   0        0        0      236 2023-06-09 14:41:39.539644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-up.png
+-rw-r--r--   0        0        0      264 2023-06-09 14:41:39.539644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-vert-thumb.png
+-rw-r--r--   0        0        0      343 2023-06-09 14:41:39.540644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-vert-trough.png
+-rw-r--r--   0        0        0      128 2023-06-09 14:41:39.541644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/separator.png
+-rw-r--r--   0        0        0      276 2023-06-09 14:41:39.542647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/sizegrip.png
+-rw-r--r--   0        0        0      733 2023-06-09 14:41:39.542647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-disabled.png
+-rw-r--r--   0        0        0      945 2023-06-09 14:41:39.543645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-hover.png
+-rw-r--r--   0        0        0      963 2023-06-09 14:41:39.544643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-pressed.png
+-rw-r--r--   0        0        0      895 2023-06-09 14:41:39.545645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-rest.png
+-rw-r--r--   0        0        0      623 2023-06-09 14:41:39.545645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-disabled.png
+-rw-r--r--   0        0        0      927 2023-06-09 14:41:39.546644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-hover.png
+-rw-r--r--   0        0        0      936 2023-06-09 14:41:39.547644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-pressed.png
+-rw-r--r--   0        0        0      859 2023-06-09 14:41:39.547644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-rest.png
+-rw-r--r--   0        0        0      265 2023-06-09 14:41:39.548643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/tab-hover.png
+-rw-r--r--   0        0        0      164 2023-06-09 14:41:39.549644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/tab-rest.png
+-rw-r--r--   0        0        0      319 2023-06-09 14:41:39.549644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/tab-selected.png
+-rw-r--r--   0        0        0      295 2023-06-09 14:41:39.550645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/treeheading-hover.png
+-rw-r--r--   0        0        0      317 2023-06-09 14:41:39.551644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/treeheading-pressed.png
+-rw-r--r--   0        0        0      321 2023-06-09 14:41:39.551644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/treeheading-rest.png
+-rw-r--r--   0        0        0    20188 2023-06-09 14:41:39.499549 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark.tcl
+-rw-r--r--   0        0        0      278 2023-06-09 14:41:39.552643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/arrow-down.png
+-rw-r--r--   0        0        0      273 2023-06-09 14:41:39.552643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/arrow-right.png
+-rw-r--r--   0        0        0      285 2023-06-09 14:41:39.553645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/arrow-up.png
+-rw-r--r--   0        0        0      271 2023-06-09 14:41:39.554647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-accent-disabled.png
+-rw-r--r--   0        0        0      219 2023-06-09 14:48:51.766400 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-accent-hover.png
+-rw-r--r--   0        0        0      255 2023-06-09 14:53:14.082428 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-accent-pressed.png
+-rw-r--r--   0        0        0      217 2023-06-09 14:48:47.641380 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-accent-rest.png
+-rw-r--r--   0        0        0      326 2023-06-09 14:41:39.556644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-close-hover.png
+-rw-r--r--   0        0        0      316 2023-06-09 14:41:39.557644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-close-pressed.png
+-rw-r--r--   0        0        0      307 2023-06-09 14:41:39.557644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-disabled.png
+-rw-r--r--   0        0        0      306 2023-06-09 14:41:39.558645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-hover.png
+-rw-r--r--   0        0        0      289 2023-06-09 14:41:39.559644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-pressed.png
+-rw-r--r--   0        0        0      303 2023-06-09 14:41:39.559644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-rest.png
+-rw-r--r--   0        0        0      238 2023-06-09 14:41:39.560643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-titlebar-hover.png
+-rw-r--r--   0        0        0      225 2023-06-09 14:41:39.561643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-titlebar-pressed.png
+-rw-r--r--   0        0        0      479 2023-06-09 14:43:10.460434 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/card.png
+-rw-r--r--   0        0        0      381 2023-06-09 14:41:39.562646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-disabled.png
+-rw-r--r--   0        0        0      476 2023-06-09 14:41:39.562646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-hover.png
+-rw-r--r--   0        0        0      467 2023-06-09 14:41:39.563646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-pressed.png
+-rw-r--r--   0        0        0      473 2023-06-09 14:41:39.564644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-rest.png
+-rw-r--r--   0        0        0      299 2023-06-09 14:41:39.564644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-tri-disabled.png
+-rw-r--r--   0        0        0      365 2023-06-09 14:41:39.565643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-tri-hover.png
+-rw-r--r--   0        0        0      362 2023-06-09 14:41:39.566644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-tri-pressed.png
+-rw-r--r--   0        0        0      367 2023-06-09 14:41:39.566644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-tri-rest.png
+-rw-r--r--   0        0        0      324 2023-06-09 14:41:39.567644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-unsel-disabled.png
+-rw-r--r--   0        0        0      334 2023-06-09 14:41:39.568643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-unsel-hover.png
+-rw-r--r--   0        0        0      302 2023-06-09 14:41:39.568643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-unsel-pressed.png
+-rw-r--r--   0        0        0      333 2023-06-09 14:41:39.569646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-unsel-rest.png
+-rw-r--r--   0        0        0      129 2023-06-09 14:41:39.569646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/empty.png
+-rw-r--r--   0        0        0      289 2023-06-09 14:41:39.570644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/entry-disabled.png
+-rw-r--r--   0        0        0      331 2023-06-09 14:41:39.571647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/entry-focus.png
+-rw-r--r--   0        0        0      302 2023-06-09 14:41:39.572644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/entry-hover.png
+-rw-r--r--   0        0        0      324 2023-06-09 14:41:39.572644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/entry-invalid.png
+-rw-r--r--   0        0        0      308 2023-06-09 14:41:39.573646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/entry-rest.png
+-rw-r--r--   0        0        0      298 2023-06-09 14:41:39.573646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/notebook-border.png
+-rw-r--r--   0        0        0      185 2023-06-09 14:41:39.574643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/notebook.png
+-rw-r--r--   0        0        0      192 2023-06-09 14:41:39.575643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/progress-pbar-hor.png
+-rw-r--r--   0        0        0      216 2023-06-09 14:41:39.575643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/progress-pbar-vert.png
+-rw-r--r--   0        0        0      158 2023-06-09 14:41:39.576643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/progress-trough-hor.png
+-rw-r--r--   0        0        0      161 2023-06-09 14:41:39.577644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/progress-trough-vert.png
+-rw-r--r--   0        0        0      523 2023-06-09 14:41:39.578645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-disabled.png
+-rw-r--r--   0        0        0      837 2023-06-09 14:41:39.578645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-hover.png
+-rw-r--r--   0        0        0      764 2023-06-09 14:41:39.579645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-pressed.png
+-rw-r--r--   0        0        0      773 2023-06-09 14:41:39.580644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-rest.png
+-rw-r--r--   0        0        0      521 2023-06-09 14:41:39.581644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-disabled.png
+-rw-r--r--   0        0        0      573 2023-06-09 14:41:39.582644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-hover.png
+-rw-r--r--   0        0        0      636 2023-06-09 14:41:39.582644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-pressed.png
+-rw-r--r--   0        0        0      576 2023-06-09 14:41:39.583644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-rest.png
+-rw-r--r--   0        0        0      658 2023-06-09 14:41:39.584643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-disabled.png
+-rw-r--r--   0        0        0      749 2023-06-09 14:41:39.584643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-hover.png
+-rw-r--r--   0        0        0      675 2023-06-09 14:41:39.585645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-pressed.png
+-rw-r--r--   0        0        0      701 2023-06-09 14:41:39.586645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-rest.png
+-rw-r--r--   0        0        0      208 2023-06-09 14:41:39.586645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-trough-hor.png
+-rw-r--r--   0        0        0      214 2023-06-09 14:41:39.587646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-trough-vert.png
+-rw-r--r--   0        0        0      229 2023-06-09 14:41:39.588644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-down.png
+-rw-r--r--   0        0        0      234 2023-06-09 14:41:39.589644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-hor-thumb.png
+-rw-r--r--   0        0        0      321 2023-06-09 14:41:39.589644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-hor-trough.png
+-rw-r--r--   0        0        0      232 2023-06-09 14:41:39.590644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-left.png
+-rw-r--r--   0        0        0      223 2023-06-09 14:41:39.590644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-right.png
+-rw-r--r--   0        0        0      237 2023-06-09 14:41:39.591643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-up.png
+-rw-r--r--   0        0        0      262 2023-06-09 14:41:39.592644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-vert-thumb.png
+-rw-r--r--   0        0        0      324 2023-06-09 14:41:39.593644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-vert-trough.png
+-rw-r--r--   0        0        0      128 2023-06-09 14:41:39.594646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/separator.png
+-rw-r--r--   0        0        0      272 2023-06-09 14:41:39.594646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/sizegrip.png
+-rw-r--r--   0        0        0      726 2023-06-09 14:41:39.595643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-disabled.png
+-rw-r--r--   0        0        0      867 2023-06-09 14:41:39.596647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-hover.png
+-rw-r--r--   0        0        0      880 2023-06-09 14:41:39.597645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-pressed.png
+-rw-r--r--   0        0        0      814 2023-06-09 14:41:39.597645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-rest.png
+-rw-r--r--   0        0        0      590 2023-06-09 14:41:39.598645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-disabled.png
+-rw-r--r--   0        0        0      906 2023-06-09 14:41:39.598645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-hover.png
+-rw-r--r--   0        0        0      916 2023-06-09 14:41:39.599644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-pressed.png
+-rw-r--r--   0        0        0      857 2023-06-09 14:41:39.600643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-rest.png
+-rw-r--r--   0        0        0      295 2023-06-09 14:41:39.600643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/tab-hover.png
+-rw-r--r--   0        0        0      164 2023-06-09 14:41:39.601645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/tab-rest.png
+-rw-r--r--   0        0        0      318 2023-06-09 14:41:39.602649 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/tab-selected.png
+-rw-r--r--   0        0        0      338 2023-06-09 14:41:39.602649 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/treeheading-hover.png
+-rw-r--r--   0        0        0      318 2023-06-09 14:41:39.603646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/treeheading-pressed.png
+-rw-r--r--   0        0        0      330 2023-06-09 14:41:39.603646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/treeheading-rest.png
+-rw-r--r--   0        0        0    20371 2023-06-09 14:41:39.500545 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light.tcl
+-rw-r--r--   0        0        0     3045 2023-05-14 15:25:00.269895 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/sprites_dark.tcl
+-rw-r--r--   0        0        0     3092 2023-05-14 15:25:00.270897 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/sprites_light.tcl
+-rw-r--r--   0        0        0    18371 2023-05-14 15:25:00.272896 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_dark.png
+-rw-r--r--   0        0        0     2649 2023-06-09 14:36:51.668892 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_light.png
+-rw-r--r--   0        0        0    18462 2023-05-14 15:25:00.272896 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_light2.png
+-rw-r--r--   0        0        0      372 2023-06-09 14:40:30.166428 tkadw-0.1.2/tkadw/ttk/test.py
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 tkadw-0.1.2/PKG-INFO
```

### Comparing `tkadw-0.1.1/tkadw/appconfig.py` & `tkadw-0.1.2/tkadw/appconfig.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/__init__.py` & `tkadw-0.1.2/tkadw/canvas/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 from tkadw.canvas.drawengine import AdwDrawEngine
+from tkadw.canvas.frame import AdwDrawFrame, AdwDrawDarkFrame, AdwDrawRoundFrame, AdwDrawDarkRoundFrame, \
+    AdwDrawRoundFrame3, AdwDrawDarkRoundFrame3
 from tkadw.canvas.button import AdwDrawButton, AdwDrawDarkButton, AdwDrawAccentButton, \
     AdwDrawRoundButton, AdwDrawRoundDarkButton, AdwDrawRoundAccentButton, \
     AdwDrawRoundButton2, AdwDrawRoundDarkButton2, AdwDrawRoundAccentButton2, \
     AdwDrawRoundButton3, AdwDrawRoundDarkButton3, AdwDrawRoundAccentButton3, \
     AdwDrawCircularButton, AdwDrawCircularDarkButton
 from tkadw.canvas.entry import AdwDrawEntry, AdwDrawDarkEntry, AdwDrawRoundEntry, AdwDrawRoundDarkEntry, \
-    AdwDrawRoundEntry3, AdwDrawRoundDarkEntry3
+    AdwDrawRoundEntry3, AdwDrawRoundDarkEntry3
+from tkadw.canvas.textbox import AdwDrawText, AdwDrawDarkText, AdwDrawRoundText, AdwDrawRoundDarkText, \
+    AdwDrawRoundText3, AdwDrawRoundDarkText3
```

### Comparing `tkadw-0.1.1/tkadw/canvas/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.1.2/tkadw/canvas/__pycache__/__init__.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,87 +1,125 @@
 magic:    0xa70d0d0a
-moddate:  0xd8129564 (Fri Jun 23 03:34:48 2023 UTC)
-files sz: 586
+moddate:  0x6a4b9564 (Fri Jun 23 07:36:10 2023 UTC)
+files sz: 896
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a036d045a046d
-      055a056d065a066d075a076d085a086d095a096d0a5a0a6d0b5a0b6d0c5a
-      0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a100100640064036c116d125a126d
-      135a136d145a146d155a156d165a166d175a17010064045300
+      055a056d065a066d075a076d085a080100640064036c096d0a5a0a6d0b5a
+      0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a106d115a116d125a126d
+      135a136d145a146d155a156d165a166d175a170100640064046c186d195a
+      196d1a5a1a6d1b5a1b6d1c5a1c6d1d5a1d6d1e5a1e0100640064056c1f6d
+      205a206d215a216d225a226d235a236d245a246d255a25010064065300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('AdwDrawEngine',))
                  6 IMPORT_NAME              0 (tkadw.canvas.drawengine)
                  8 IMPORT_FROM              1 (AdwDrawEngine)
                 10 STORE_NAME               1 (AdwDrawEngine)
                 12 POP_TOP
    
      2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawRoundButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton'))
-                18 IMPORT_NAME              2 (tkadw.canvas.button)
-                20 IMPORT_FROM              3 (AdwDrawButton)
-                22 STORE_NAME               3 (AdwDrawButton)
-                24 IMPORT_FROM              4 (AdwDrawDarkButton)
-                26 STORE_NAME               4 (AdwDrawDarkButton)
-                28 IMPORT_FROM              5 (AdwDrawAccentButton)
-                30 STORE_NAME               5 (AdwDrawAccentButton)
-                32 IMPORT_FROM              6 (AdwDrawRoundButton)
-                34 STORE_NAME               6 (AdwDrawRoundButton)
-                36 IMPORT_FROM              7 (AdwDrawRoundDarkButton)
-                38 STORE_NAME               7 (AdwDrawRoundDarkButton)
-                40 IMPORT_FROM              8 (AdwDrawRoundAccentButton)
-                42 STORE_NAME               8 (AdwDrawRoundAccentButton)
-                44 IMPORT_FROM              9 (AdwDrawRoundButton2)
-                46 STORE_NAME               9 (AdwDrawRoundButton2)
-                48 IMPORT_FROM             10 (AdwDrawRoundDarkButton2)
-                50 STORE_NAME              10 (AdwDrawRoundDarkButton2)
-                52 IMPORT_FROM             11 (AdwDrawRoundAccentButton2)
-                54 STORE_NAME              11 (AdwDrawRoundAccentButton2)
-                56 IMPORT_FROM             12 (AdwDrawRoundButton3)
-                58 STORE_NAME              12 (AdwDrawRoundButton3)
-                60 IMPORT_FROM             13 (AdwDrawRoundDarkButton3)
-                62 STORE_NAME              13 (AdwDrawRoundDarkButton3)
-                64 IMPORT_FROM             14 (AdwDrawRoundAccentButton3)
-                66 STORE_NAME              14 (AdwDrawRoundAccentButton3)
-                68 IMPORT_FROM             15 (AdwDrawCircularButton)
-                70 STORE_NAME              15 (AdwDrawCircularButton)
-                72 IMPORT_FROM             16 (AdwDrawCircularDarkButton)
-                74 STORE_NAME              16 (AdwDrawCircularDarkButton)
-                76 POP_TOP
+                16 LOAD_CONST               2 (('AdwDrawFrame', 'AdwDrawDarkFrame', 'AdwDrawRoundFrame', 'AdwDrawDarkRoundFrame', 'AdwDrawRoundFrame3', 'AdwDrawDarkRoundFrame3'))
+                18 IMPORT_NAME              2 (tkadw.canvas.frame)
+                20 IMPORT_FROM              3 (AdwDrawFrame)
+                22 STORE_NAME               3 (AdwDrawFrame)
+                24 IMPORT_FROM              4 (AdwDrawDarkFrame)
+                26 STORE_NAME               4 (AdwDrawDarkFrame)
+                28 IMPORT_FROM              5 (AdwDrawRoundFrame)
+                30 STORE_NAME               5 (AdwDrawRoundFrame)
+                32 IMPORT_FROM              6 (AdwDrawDarkRoundFrame)
+                34 STORE_NAME               6 (AdwDrawDarkRoundFrame)
+                36 IMPORT_FROM              7 (AdwDrawRoundFrame3)
+                38 STORE_NAME               7 (AdwDrawRoundFrame3)
+                40 IMPORT_FROM              8 (AdwDrawDarkRoundFrame3)
+                42 STORE_NAME               8 (AdwDrawDarkRoundFrame3)
+                44 POP_TOP
    
-     7          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               3 (('AdwDrawEntry', 'AdwDrawDarkEntry', 'AdwDrawRoundEntry', 'AdwDrawRoundDarkEntry', 'AdwDrawRoundEntry3', 'AdwDrawRoundDarkEntry3'))
-                82 IMPORT_NAME             17 (tkadw.canvas.entry)
-                84 IMPORT_FROM             18 (AdwDrawEntry)
-                86 STORE_NAME              18 (AdwDrawEntry)
-                88 IMPORT_FROM             19 (AdwDrawDarkEntry)
-                90 STORE_NAME              19 (AdwDrawDarkEntry)
-                92 IMPORT_FROM             20 (AdwDrawRoundEntry)
-                94 STORE_NAME              20 (AdwDrawRoundEntry)
-                96 IMPORT_FROM             21 (AdwDrawRoundDarkEntry)
-                98 STORE_NAME              21 (AdwDrawRoundDarkEntry)
-               100 IMPORT_FROM             22 (AdwDrawRoundEntry3)
-               102 STORE_NAME              22 (AdwDrawRoundEntry3)
-               104 IMPORT_FROM             23 (AdwDrawRoundDarkEntry3)
-               106 STORE_NAME              23 (AdwDrawRoundDarkEntry3)
+     4          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               3 (('AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawRoundButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton'))
+                50 IMPORT_NAME              9 (tkadw.canvas.button)
+                52 IMPORT_FROM             10 (AdwDrawButton)
+                54 STORE_NAME              10 (AdwDrawButton)
+                56 IMPORT_FROM             11 (AdwDrawDarkButton)
+                58 STORE_NAME              11 (AdwDrawDarkButton)
+                60 IMPORT_FROM             12 (AdwDrawAccentButton)
+                62 STORE_NAME              12 (AdwDrawAccentButton)
+                64 IMPORT_FROM             13 (AdwDrawRoundButton)
+                66 STORE_NAME              13 (AdwDrawRoundButton)
+                68 IMPORT_FROM             14 (AdwDrawRoundDarkButton)
+                70 STORE_NAME              14 (AdwDrawRoundDarkButton)
+                72 IMPORT_FROM             15 (AdwDrawRoundAccentButton)
+                74 STORE_NAME              15 (AdwDrawRoundAccentButton)
+                76 IMPORT_FROM             16 (AdwDrawRoundButton2)
+                78 STORE_NAME              16 (AdwDrawRoundButton2)
+                80 IMPORT_FROM             17 (AdwDrawRoundDarkButton2)
+                82 STORE_NAME              17 (AdwDrawRoundDarkButton2)
+                84 IMPORT_FROM             18 (AdwDrawRoundAccentButton2)
+                86 STORE_NAME              18 (AdwDrawRoundAccentButton2)
+                88 IMPORT_FROM             19 (AdwDrawRoundButton3)
+                90 STORE_NAME              19 (AdwDrawRoundButton3)
+                92 IMPORT_FROM             20 (AdwDrawRoundDarkButton3)
+                94 STORE_NAME              20 (AdwDrawRoundDarkButton3)
+                96 IMPORT_FROM             21 (AdwDrawRoundAccentButton3)
+                98 STORE_NAME              21 (AdwDrawRoundAccentButton3)
+               100 IMPORT_FROM             22 (AdwDrawCircularButton)
+               102 STORE_NAME              22 (AdwDrawCircularButton)
+               104 IMPORT_FROM             23 (AdwDrawCircularDarkButton)
+               106 STORE_NAME              23 (AdwDrawCircularDarkButton)
                108 POP_TOP
-               110 LOAD_CONST               4 (None)
-               112 RETURN_VALUE
+   
+     9         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               4 (('AdwDrawEntry', 'AdwDrawDarkEntry', 'AdwDrawRoundEntry', 'AdwDrawRoundDarkEntry', 'AdwDrawRoundEntry3', 'AdwDrawRoundDarkEntry3'))
+               114 IMPORT_NAME             24 (tkadw.canvas.entry)
+               116 IMPORT_FROM             25 (AdwDrawEntry)
+               118 STORE_NAME              25 (AdwDrawEntry)
+               120 IMPORT_FROM             26 (AdwDrawDarkEntry)
+               122 STORE_NAME              26 (AdwDrawDarkEntry)
+               124 IMPORT_FROM             27 (AdwDrawRoundEntry)
+               126 STORE_NAME              27 (AdwDrawRoundEntry)
+               128 IMPORT_FROM             28 (AdwDrawRoundDarkEntry)
+               130 STORE_NAME              28 (AdwDrawRoundDarkEntry)
+               132 IMPORT_FROM             29 (AdwDrawRoundEntry3)
+               134 STORE_NAME              29 (AdwDrawRoundEntry3)
+               136 IMPORT_FROM             30 (AdwDrawRoundDarkEntry3)
+               138 STORE_NAME              30 (AdwDrawRoundDarkEntry3)
+               140 POP_TOP
+   
+    11         142 LOAD_CONST               0 (0)
+               144 LOAD_CONST               5 (('AdwDrawText', 'AdwDrawDarkText', 'AdwDrawRoundText', 'AdwDrawRoundDarkText', 'AdwDrawRoundText3', 'AdwDrawRoundDarkText3'))
+               146 IMPORT_NAME             31 (tkadw.canvas.textbox)
+               148 IMPORT_FROM             32 (AdwDrawText)
+               150 STORE_NAME              32 (AdwDrawText)
+               152 IMPORT_FROM             33 (AdwDrawDarkText)
+               154 STORE_NAME              33 (AdwDrawDarkText)
+               156 IMPORT_FROM             34 (AdwDrawRoundText)
+               158 STORE_NAME              34 (AdwDrawRoundText)
+               160 IMPORT_FROM             35 (AdwDrawRoundDarkText)
+               162 STORE_NAME              35 (AdwDrawRoundDarkText)
+               164 IMPORT_FROM             36 (AdwDrawRoundText3)
+               166 STORE_NAME              36 (AdwDrawRoundText3)
+               168 IMPORT_FROM             37 (AdwDrawRoundDarkText3)
+               170 STORE_NAME              37 (AdwDrawRoundDarkText3)
+               172 POP_TOP
+               174 LOAD_CONST               6 (None)
+               176 RETURN_VALUE
    consts
       0
       ('AdwDrawEngine',)
+      ('AdwDrawFrame', 'AdwDrawDarkFrame', 'AdwDrawRoundFrame', 'AdwDrawDarkRoundFrame', 'AdwDrawRoundFrame3', 'AdwDrawDarkRoundFrame3')
       ('AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawRoundButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton')
       ('AdwDrawEntry', 'AdwDrawDarkEntry', 'AdwDrawRoundEntry', 'AdwDrawRoundDarkEntry', 'AdwDrawRoundEntry3', 'AdwDrawRoundDarkEntry3')
+      ('AdwDrawText', 'AdwDrawDarkText', 'AdwDrawRoundText', 'AdwDrawRoundDarkText', 'AdwDrawRoundText3', 'AdwDrawRoundDarkText3')
       None
-   names      ('tkadw.canvas.drawengine', 'AdwDrawEngine', 'tkadw.canvas.button', 'AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawRoundButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton', 'tkadw.canvas.entry', 'AdwDrawEntry', 'AdwDrawDarkEntry', 'AdwDrawRoundEntry', 'AdwDrawRoundDarkEntry', 'AdwDrawRoundEntry3', 'AdwDrawRoundDarkEntry3')
+   names      ('tkadw.canvas.drawengine', 'AdwDrawEngine', 'tkadw.canvas.frame', 'AdwDrawFrame', 'AdwDrawDarkFrame', 'AdwDrawRoundFrame', 'AdwDrawDarkRoundFrame', 'AdwDrawRoundFrame3', 'AdwDrawDarkRoundFrame3', 'tkadw.canvas.button', 'AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawRoundButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton', 'tkadw.canvas.entry', 'AdwDrawEntry', 'AdwDrawDarkEntry', 'AdwDrawRoundEntry', 'AdwDrawRoundDarkEntry', 'AdwDrawRoundEntry3', 'AdwDrawRoundDarkEntry3', 'tkadw.canvas.textbox', 'AdwDrawText', 'AdwDrawDarkText', 'AdwDrawRoundText', 'AdwDrawRoundDarkText', 'AdwDrawRoundText3', 'AdwDrawRoundDarkText3')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\canvas\\__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c014005
+   lnotab 0x00ff02010c01200240052002
```

### Comparing `tkadw-0.1.1/tkadw/canvas/__pycache__/button.cpython-311.pyc` & `tkadw-0.1.2/tkadw/canvas/__pycache__/button.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xb5109564 (Fri Jun 23 03:25:41 2023 UTC)
-files sz: 16899
+moddate:  0x9c259564 (Fri Jun 23 04:54:52 2023 UTC)
+files sz: 17270
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -71,353 +71,353 @@
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               4 ('AdwDrawBasicButton')
                 40 LOAD_NAME                4 (AdwDrawEngine)
                 42 PRECALL                  3
                 46 CALL                     3
                 56 STORE_NAME               5 (AdwDrawBasicButton)
    
-   179          58 PUSH_NULL
+   189          58 PUSH_NULL
                 60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               5 (<code object AdwDrawButton, file "D:\tkadw\tkadw\canvas\button.py", line 179>)
+                62 LOAD_CONST               5 (<code object AdwDrawButton, file "D:\tkadw\tkadw\canvas\button.py", line 189>)
                 64 MAKE_FUNCTION            0
                 66 LOAD_CONST               6 ('AdwDrawButton')
                 68 LOAD_NAME                5 (AdwDrawBasicButton)
                 70 PRECALL                  3
                 74 CALL                     3
                 84 STORE_NAME               6 (AdwDrawButton)
    
-   184          86 PUSH_NULL
+   194          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object AdwDrawDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 184>)
+                90 LOAD_CONST               7 (<code object AdwDrawDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 194>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('AdwDrawDarkButton')
                 96 LOAD_NAME                5 (AdwDrawBasicButton)
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME               7 (AdwDrawDarkButton)
    
-   189         114 PUSH_NULL
+   199         114 PUSH_NULL
                116 LOAD_BUILD_CLASS
-               118 LOAD_CONST               9 (<code object AdwDrawAccentButton, file "D:\tkadw\tkadw\canvas\button.py", line 189>)
+               118 LOAD_CONST               9 (<code object AdwDrawAccentButton, file "D:\tkadw\tkadw\canvas\button.py", line 199>)
                120 MAKE_FUNCTION            0
                122 LOAD_CONST              10 ('AdwDrawAccentButton')
                124 LOAD_NAME                5 (AdwDrawBasicButton)
                126 PRECALL                  3
                130 CALL                     3
                140 STORE_NAME               8 (AdwDrawAccentButton)
    
-   213         142 PUSH_NULL
+   223         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object AdwDrawBasicRoundButton, file "D:\tkadw\tkadw\canvas\button.py", line 213>)
+               146 LOAD_CONST              11 (<code object AdwDrawBasicRoundButton, file "D:\tkadw\tkadw\canvas\button.py", line 223>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('AdwDrawBasicRoundButton')
                152 LOAD_NAME                5 (AdwDrawBasicButton)
                154 PRECALL                  3
                158 CALL                     3
                168 STORE_NAME               9 (AdwDrawBasicRoundButton)
    
-   328         170 PUSH_NULL
+   338         170 PUSH_NULL
                172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              13 (<code object AdwDrawRoundButton, file "D:\tkadw\tkadw\canvas\button.py", line 328>)
+               174 LOAD_CONST              13 (<code object AdwDrawRoundButton, file "D:\tkadw\tkadw\canvas\button.py", line 338>)
                176 MAKE_FUNCTION            0
                178 LOAD_CONST              14 ('AdwDrawRoundButton')
                180 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                182 PRECALL                  3
                186 CALL                     3
                196 STORE_NAME              10 (AdwDrawRoundButton)
    
-   333         198 PUSH_NULL
+   343         198 PUSH_NULL
                200 LOAD_BUILD_CLASS
-               202 LOAD_CONST              15 (<code object AdwDrawRoundAccentButton, file "D:\tkadw\tkadw\canvas\button.py", line 333>)
+               202 LOAD_CONST              15 (<code object AdwDrawRoundAccentButton, file "D:\tkadw\tkadw\canvas\button.py", line 343>)
                204 MAKE_FUNCTION            0
                206 LOAD_CONST              16 ('AdwDrawRoundAccentButton')
                208 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                210 PRECALL                  3
                214 CALL                     3
                224 STORE_NAME              11 (AdwDrawRoundAccentButton)
    
-   356         226 PUSH_NULL
+   366         226 PUSH_NULL
                228 LOAD_BUILD_CLASS
-               230 LOAD_CONST              17 (<code object AdwDrawRoundDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 356>)
+               230 LOAD_CONST              17 (<code object AdwDrawRoundDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 366>)
                232 MAKE_FUNCTION            0
                234 LOAD_CONST              18 ('AdwDrawRoundDarkButton')
                236 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                238 PRECALL                  3
                242 CALL                     3
                252 STORE_NAME              12 (AdwDrawRoundDarkButton)
    
-   361         254 PUSH_NULL
+   371         254 PUSH_NULL
                256 LOAD_BUILD_CLASS
-               258 LOAD_CONST              19 (<code object AdwDrawRoundButton2, file "D:\tkadw\tkadw\canvas\button.py", line 361>)
+               258 LOAD_CONST              19 (<code object AdwDrawRoundButton2, file "D:\tkadw\tkadw\canvas\button.py", line 371>)
                260 MAKE_FUNCTION            0
                262 LOAD_CONST              20 ('AdwDrawRoundButton2')
                264 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                266 PRECALL                  3
                270 CALL                     3
                280 STORE_NAME              13 (AdwDrawRoundButton2)
    
-   383         282 PUSH_NULL
+   393         282 PUSH_NULL
                284 LOAD_BUILD_CLASS
-               286 LOAD_CONST              21 (<code object AdwDrawRoundAccentButton2, file "D:\tkadw\tkadw\canvas\button.py", line 383>)
+               286 LOAD_CONST              21 (<code object AdwDrawRoundAccentButton2, file "D:\tkadw\tkadw\canvas\button.py", line 393>)
                288 MAKE_FUNCTION            0
                290 LOAD_CONST              22 ('AdwDrawRoundAccentButton2')
                292 LOAD_NAME               13 (AdwDrawRoundButton2)
                294 PRECALL                  3
                298 CALL                     3
                308 STORE_NAME              14 (AdwDrawRoundAccentButton2)
    
-   406         310 PUSH_NULL
+   416         310 PUSH_NULL
                312 LOAD_BUILD_CLASS
-               314 LOAD_CONST              23 (<code object AdwDrawRoundDarkButton2, file "D:\tkadw\tkadw\canvas\button.py", line 406>)
+               314 LOAD_CONST              23 (<code object AdwDrawRoundDarkButton2, file "D:\tkadw\tkadw\canvas\button.py", line 416>)
                316 MAKE_FUNCTION            0
                318 LOAD_CONST              24 ('AdwDrawRoundDarkButton2')
                320 LOAD_NAME               13 (AdwDrawRoundButton2)
                322 PRECALL                  3
                326 CALL                     3
                336 STORE_NAME              15 (AdwDrawRoundDarkButton2)
    
-   411         338 PUSH_NULL
+   421         338 PUSH_NULL
                340 LOAD_BUILD_CLASS
-               342 LOAD_CONST              25 (<code object AdwDrawRoundButton3, file "D:\tkadw\tkadw\canvas\button.py", line 411>)
+               342 LOAD_CONST              25 (<code object AdwDrawRoundButton3, file "D:\tkadw\tkadw\canvas\button.py", line 421>)
                344 MAKE_FUNCTION            0
                346 LOAD_CONST              26 ('AdwDrawRoundButton3')
                348 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                350 PRECALL                  3
                354 CALL                     3
                364 STORE_NAME              16 (AdwDrawRoundButton3)
    
-   433         366 PUSH_NULL
+   443         366 PUSH_NULL
                368 LOAD_BUILD_CLASS
-               370 LOAD_CONST              27 (<code object AdwDrawRoundAccentButton3, file "D:\tkadw\tkadw\canvas\button.py", line 433>)
+               370 LOAD_CONST              27 (<code object AdwDrawRoundAccentButton3, file "D:\tkadw\tkadw\canvas\button.py", line 443>)
                372 MAKE_FUNCTION            0
                374 LOAD_CONST              28 ('AdwDrawRoundAccentButton3')
                376 LOAD_NAME               16 (AdwDrawRoundButton3)
                378 PRECALL                  3
                382 CALL                     3
                392 STORE_NAME              17 (AdwDrawRoundAccentButton3)
    
-   456         394 PUSH_NULL
+   466         394 PUSH_NULL
                396 LOAD_BUILD_CLASS
-               398 LOAD_CONST              29 (<code object AdwDrawRoundDarkButton3, file "D:\tkadw\tkadw\canvas\button.py", line 456>)
+               398 LOAD_CONST              29 (<code object AdwDrawRoundDarkButton3, file "D:\tkadw\tkadw\canvas\button.py", line 466>)
                400 MAKE_FUNCTION            0
                402 LOAD_CONST              30 ('AdwDrawRoundDarkButton3')
                404 LOAD_NAME               16 (AdwDrawRoundButton3)
                406 PRECALL                  3
                410 CALL                     3
                420 STORE_NAME              18 (AdwDrawRoundDarkButton3)
    
-   462         422 PUSH_NULL
+   472         422 PUSH_NULL
                424 LOAD_BUILD_CLASS
-               426 LOAD_CONST              31 (<code object AdwDrawBasicCircularButton, file "D:\tkadw\tkadw\canvas\button.py", line 462>)
+               426 LOAD_CONST              31 (<code object AdwDrawBasicCircularButton, file "D:\tkadw\tkadw\canvas\button.py", line 472>)
                428 MAKE_FUNCTION            0
                430 LOAD_CONST              32 ('AdwDrawBasicCircularButton')
                432 LOAD_NAME                5 (AdwDrawBasicButton)
                434 PRECALL                  3
                438 CALL                     3
                448 STORE_NAME              19 (AdwDrawBasicCircularButton)
    
-   482         450 PUSH_NULL
+   492         450 PUSH_NULL
                452 LOAD_BUILD_CLASS
-               454 LOAD_CONST              33 (<code object AdwDrawCircularButton, file "D:\tkadw\tkadw\canvas\button.py", line 482>)
+               454 LOAD_CONST              33 (<code object AdwDrawCircularButton, file "D:\tkadw\tkadw\canvas\button.py", line 492>)
                456 MAKE_FUNCTION            0
                458 LOAD_CONST              34 ('AdwDrawCircularButton')
                460 LOAD_NAME               19 (AdwDrawBasicCircularButton)
                462 PRECALL                  3
                466 CALL                     3
                476 STORE_NAME              20 (AdwDrawCircularButton)
    
-   487         478 PUSH_NULL
+   497         478 PUSH_NULL
                480 LOAD_BUILD_CLASS
-               482 LOAD_CONST              35 (<code object AdwDrawCircularDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 487>)
+               482 LOAD_CONST              35 (<code object AdwDrawCircularDarkButton, file "D:\tkadw\tkadw\canvas\button.py", line 497>)
                484 MAKE_FUNCTION            0
                486 LOAD_CONST              36 ('AdwDrawCircularDarkButton')
                488 LOAD_NAME               19 (AdwDrawBasicCircularButton)
                490 PRECALL                  3
                494 CALL                     3
                504 STORE_NAME              21 (AdwDrawCircularDarkButton)
    
-   492         506 LOAD_NAME               22 (__name__)
+   502         506 LOAD_NAME               22 (__name__)
                508 LOAD_CONST              37 ('__main__')
                510 COMPARE_OP               2 (==)
                516 EXTENDED_ARG             1
                518 POP_JUMP_FORWARD_IF_FALSE   333 (to 1186)
    
-   493         520 LOAD_CONST               0 (0)
+   503         520 LOAD_CONST               0 (0)
                522 LOAD_CONST              38 (('Tk',))
                524 IMPORT_NAME             23 (tkinter)
                526 IMPORT_FROM             24 (Tk)
                528 STORE_NAME              24 (Tk)
                530 POP_TOP
    
-   495         532 PUSH_NULL
+   505         532 PUSH_NULL
                534 LOAD_NAME               24 (Tk)
                536 PRECALL                  0
                540 CALL                     0
                550 STORE_NAME              25 (root)
    
-   497         552 PUSH_NULL
+   507         552 PUSH_NULL
                554 LOAD_NAME                6 (AdwDrawButton)
                556 LOAD_CONST              39 ('Hello')
                558 KW_NAMES                40
                560 PRECALL                  1
                564 CALL                     1
                574 STORE_NAME              26 (button)
    
-   498         576 LOAD_NAME               26 (button)
+   508         576 LOAD_NAME               26 (button)
                578 LOAD_METHOD             27 (bind)
                600 LOAD_CONST              41 ('<<Click>>')
-               602 LOAD_CONST              42 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 498>)
+               602 LOAD_CONST              42 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 508>)
                604 MAKE_FUNCTION            0
                606 PRECALL                  2
                610 CALL                     2
                620 POP_TOP
    
-   499         622 LOAD_NAME               26 (button)
+   509         622 LOAD_NAME               26 (button)
                624 LOAD_METHOD             28 (pack)
                646 LOAD_CONST              43 ('x')
                648 LOAD_CONST              44 (5)
                650 LOAD_CONST              44 (5)
                652 KW_NAMES                45
                654 PRECALL                  3
                658 CALL                     3
                668 POP_TOP
    
-   501         670 PUSH_NULL
+   511         670 PUSH_NULL
                672 LOAD_NAME               10 (AdwDrawRoundButton)
                674 LOAD_CONST              39 ('Hello')
                676 KW_NAMES                40
                678 PRECALL                  1
                682 CALL                     1
                692 STORE_NAME              29 (button4)
    
-   502         694 LOAD_NAME               29 (button4)
+   512         694 LOAD_NAME               29 (button4)
                696 LOAD_METHOD             27 (bind)
                718 LOAD_CONST              41 ('<<Click>>')
-               720 LOAD_CONST              46 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 502>)
+               720 LOAD_CONST              46 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 512>)
                722 MAKE_FUNCTION            0
                724 PRECALL                  2
                728 CALL                     2
                738 POP_TOP
    
-   503         740 LOAD_NAME               29 (button4)
+   513         740 LOAD_NAME               29 (button4)
                742 LOAD_METHOD             28 (pack)
                764 LOAD_CONST              43 ('x')
                766 LOAD_CONST              44 (5)
                768 LOAD_CONST              44 (5)
                770 KW_NAMES                45
                772 PRECALL                  3
                776 CALL                     3
                786 POP_TOP
    
-   505         788 PUSH_NULL
+   515         788 PUSH_NULL
                790 LOAD_NAME               13 (AdwDrawRoundButton2)
                792 LOAD_CONST              39 ('Hello')
                794 KW_NAMES                40
                796 PRECALL                  1
                800 CALL                     1
                810 STORE_NAME              30 (button7)
    
-   506         812 LOAD_NAME               30 (button7)
+   516         812 LOAD_NAME               30 (button7)
                814 LOAD_METHOD             27 (bind)
                836 LOAD_CONST              41 ('<<Click>>')
-               838 LOAD_CONST              47 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 506>)
+               838 LOAD_CONST              47 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 516>)
                840 MAKE_FUNCTION            0
                842 PRECALL                  2
                846 CALL                     2
                856 POP_TOP
    
-   507         858 LOAD_NAME               30 (button7)
+   517         858 LOAD_NAME               30 (button7)
                860 LOAD_METHOD             28 (pack)
                882 LOAD_CONST              43 ('x')
                884 LOAD_CONST              44 (5)
                886 LOAD_CONST              44 (5)
                888 KW_NAMES                45
                890 PRECALL                  3
                894 CALL                     3
                904 POP_TOP
    
-   509         906 PUSH_NULL
+   519         906 PUSH_NULL
                908 LOAD_NAME               16 (AdwDrawRoundButton3)
                910 LOAD_CONST              39 ('Hello')
                912 KW_NAMES                40
                914 PRECALL                  1
                918 CALL                     1
                928 STORE_NAME              31 (button10)
    
-   510         930 LOAD_NAME               31 (button10)
+   520         930 LOAD_NAME               31 (button10)
                932 LOAD_METHOD             27 (bind)
                954 LOAD_CONST              41 ('<<Click>>')
-               956 LOAD_CONST              48 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 510>)
+               956 LOAD_CONST              48 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 520>)
                958 MAKE_FUNCTION            0
                960 PRECALL                  2
                964 CALL                     2
                974 POP_TOP
    
-   511         976 LOAD_NAME               31 (button10)
+   521         976 LOAD_NAME               31 (button10)
                978 LOAD_METHOD             28 (pack)
               1000 LOAD_CONST              43 ('x')
               1002 LOAD_CONST              44 (5)
               1004 LOAD_CONST              44 (5)
               1006 KW_NAMES                45
               1008 PRECALL                  3
               1012 CALL                     3
               1022 POP_TOP
    
-   513        1024 PUSH_NULL
+   523        1024 PUSH_NULL
               1026 LOAD_NAME               20 (AdwDrawCircularButton)
               1028 LOAD_CONST              39 ('Hello')
               1030 KW_NAMES                40
               1032 PRECALL                  1
               1036 CALL                     1
               1046 STORE_NAME              32 (button13)
    
-   514        1048 LOAD_NAME               32 (button13)
+   524        1048 LOAD_NAME               32 (button13)
               1050 LOAD_METHOD             27 (bind)
               1072 LOAD_CONST              41 ('<<Click>>')
-              1074 LOAD_CONST              49 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 514>)
+              1074 LOAD_CONST              49 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 524>)
               1076 MAKE_FUNCTION            0
               1078 PRECALL                  2
               1082 CALL                     2
               1092 POP_TOP
    
-   515        1094 LOAD_NAME               32 (button13)
+   525        1094 LOAD_NAME               32 (button13)
               1096 LOAD_METHOD             28 (pack)
               1118 LOAD_CONST              43 ('x')
               1120 LOAD_CONST              44 (5)
               1122 LOAD_CONST              44 (5)
               1124 KW_NAMES                45
               1126 PRECALL                  3
               1130 CALL                     3
               1140 POP_TOP
    
-   517        1142 LOAD_NAME               25 (root)
+   527        1142 LOAD_NAME               25 (root)
               1144 LOAD_METHOD             33 (mainloop)
               1166 PRECALL                  0
               1170 CALL                     0
               1180 POP_TOP
               1182 LOAD_CONST              50 (None)
               1184 RETURN_VALUE
    
-   492     >> 1186 LOAD_CONST              50 (None)
+   502     >> 1186 LOAD_CONST              50 (None)
               1188 RETURN_VALUE
    consts
       0
       ('Font', 'nametofont')
       ('AdwDrawEngine',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x8700970065005a0164005a02640164026403640464059c046406650366
-            02880066016407840e5a04640884005a05640984005a066414640a84015a
-            076414640b84015a086414640c84015a096414640d84015a0a6414640e65
-            0b6602640f84055a0c641084005a0d641184005a0e641284005a0f641464
-            1384015a10880078015a115300
+            02880066016407840e5a0488006601640884085a05640984005a06640a84
+            005a076415640b84015a086415640c84015a096415640d84015a0a641564
+            0e84015a0b6415640f650c6602641084055a0d641184005a0e641284005a
+            0f641384005a106415641484015a11880078015a125300
                        0 MAKE_CELL                0 (__class__)
          
            6           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicButton')
                       10 STORE_NAME               2 (__qualname__)
@@ -433,247 +433,254 @@
                       28 BUILD_TUPLE              2
                       30 LOAD_CLOSURE             0 (__class__)
                       32 BUILD_TUPLE              1
                       34 LOAD_CONST               7 (<code object __init__, file "D:\tkadw\tkadw\canvas\button.py", line 7>)
                       36 MAKE_FUNCTION           14 (kwdefaults, annotations, closure)
                       38 STORE_NAME               4 (__init__)
          
-          33          40 LOAD_CONST               8 (<code object _other, file "D:\tkadw\tkadw\canvas\button.py", line 33>)
-                      42 MAKE_FUNCTION            0
-                      44 STORE_NAME               5 (_other)
-         
-          37          46 LOAD_CONST               9 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 37>)
-                      48 MAKE_FUNCTION            0
-                      50 STORE_NAME               6 (_draw)
-         
-          52          52 LOAD_CONST              20 ((None,))
-                      54 LOAD_CONST              10 (<code object _click, file "D:\tkadw\tkadw\canvas\button.py", line 52>)
-                      56 MAKE_FUNCTION            1 (defaults)
-                      58 STORE_NAME               7 (_click)
-         
-          62          60 LOAD_CONST              20 ((None,))
-                      62 LOAD_CONST              11 (<code object _unclick, file "D:\tkadw\tkadw\canvas\button.py", line 62>)
-                      64 MAKE_FUNCTION            1 (defaults)
-                      66 STORE_NAME               8 (_unclick)
-         
-          72          68 LOAD_CONST              20 ((None,))
-                      70 LOAD_CONST              12 (<code object _hover, file "D:\tkadw\tkadw\canvas\button.py", line 72>)
-                      72 MAKE_FUNCTION            1 (defaults)
-                      74 STORE_NAME               9 (_hover)
-         
-          80          76 LOAD_CONST              20 ((None,))
-                      78 LOAD_CONST              13 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\button.py", line 80>)
-                      80 MAKE_FUNCTION            1 (defaults)
-                      82 STORE_NAME              10 (_hover_release)
-         
-          88          84 LOAD_CONST              20 ((None,))
-                      86 LOAD_CONST              14 ('font')
-                      88 LOAD_NAME               11 (Font)
-                      90 BUILD_TUPLE              2
-                      92 LOAD_CONST              15 (<code object font, file "D:\tkadw\tkadw\canvas\button.py", line 88>)
-                      94 MAKE_FUNCTION            5 (defaults, annotations)
-                      96 STORE_NAME              12 (font)
-         
-          94          98 LOAD_CONST              16 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 94>)
-                     100 MAKE_FUNCTION            0
-                     102 STORE_NAME              13 (default_palette)
-         
-          97         104 LOAD_CONST              17 (<code object palette_light, file "D:\tkadw\tkadw\canvas\button.py", line 97>)
-                     106 MAKE_FUNCTION            0
-                     108 STORE_NAME              14 (palette_light)
-         
-         118         110 LOAD_CONST              18 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\button.py", line 118>)
-                     112 MAKE_FUNCTION            0
-                     114 STORE_NAME              15 (palette_dark)
-         
-         139         116 LOAD_CONST              20 ((None,))
-                     118 LOAD_CONST              19 (<code object palette, file "D:\tkadw\tkadw\canvas\button.py", line 139>)
-                     120 MAKE_FUNCTION            1 (defaults)
-                     122 STORE_NAME              16 (palette)
-                     124 LOAD_CLOSURE             0 (__class__)
-                     126 COPY                     1
-                     128 STORE_NAME              17 (__classcell__)
-                     130 RETURN_VALUE
+          33          40 LOAD_CLOSURE             0 (__class__)
+                      42 BUILD_TUPLE              1
+                      44 LOAD_CONST               8 (<code object configure, file "D:\tkadw\tkadw\canvas\button.py", line 33>)
+                      46 MAKE_FUNCTION            8 (closure)
+                      48 STORE_NAME               5 (configure)
+         
+          43          50 LOAD_CONST               9 (<code object _other, file "D:\tkadw\tkadw\canvas\button.py", line 43>)
+                      52 MAKE_FUNCTION            0
+                      54 STORE_NAME               6 (_other)
+         
+          47          56 LOAD_CONST              10 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 47>)
+                      58 MAKE_FUNCTION            0
+                      60 STORE_NAME               7 (_draw)
+         
+          62          62 LOAD_CONST              21 ((None,))
+                      64 LOAD_CONST              11 (<code object _click, file "D:\tkadw\tkadw\canvas\button.py", line 62>)
+                      66 MAKE_FUNCTION            1 (defaults)
+                      68 STORE_NAME               8 (_click)
+         
+          72          70 LOAD_CONST              21 ((None,))
+                      72 LOAD_CONST              12 (<code object _unclick, file "D:\tkadw\tkadw\canvas\button.py", line 72>)
+                      74 MAKE_FUNCTION            1 (defaults)
+                      76 STORE_NAME               9 (_unclick)
+         
+          82          78 LOAD_CONST              21 ((None,))
+                      80 LOAD_CONST              13 (<code object _hover, file "D:\tkadw\tkadw\canvas\button.py", line 82>)
+                      82 MAKE_FUNCTION            1 (defaults)
+                      84 STORE_NAME              10 (_hover)
+         
+          90          86 LOAD_CONST              21 ((None,))
+                      88 LOAD_CONST              14 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\button.py", line 90>)
+                      90 MAKE_FUNCTION            1 (defaults)
+                      92 STORE_NAME              11 (_hover_release)
+         
+          98          94 LOAD_CONST              21 ((None,))
+                      96 LOAD_CONST              15 ('font')
+                      98 LOAD_NAME               12 (Font)
+                     100 BUILD_TUPLE              2
+                     102 LOAD_CONST              16 (<code object font, file "D:\tkadw\tkadw\canvas\button.py", line 98>)
+                     104 MAKE_FUNCTION            5 (defaults, annotations)
+                     106 STORE_NAME              13 (font)
+         
+         104         108 LOAD_CONST              17 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 104>)
+                     110 MAKE_FUNCTION            0
+                     112 STORE_NAME              14 (default_palette)
+         
+         107         114 LOAD_CONST              18 (<code object palette_light, file "D:\tkadw\tkadw\canvas\button.py", line 107>)
+                     116 MAKE_FUNCTION            0
+                     118 STORE_NAME              15 (palette_light)
+         
+         128         120 LOAD_CONST              19 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\button.py", line 128>)
+                     122 MAKE_FUNCTION            0
+                     124 STORE_NAME              16 (palette_dark)
+         
+         149         126 LOAD_CONST              21 ((None,))
+                     128 LOAD_CONST              20 (<code object palette, file "D:\tkadw\tkadw\canvas\button.py", line 149>)
+                     130 MAKE_FUNCTION            1 (defaults)
+                     132 STORE_NAME              17 (palette)
+                     134 LOAD_CLOSURE             0 (__class__)
+                     136 COPY                     1
+                     138 STORE_NAME              18 (__classcell__)
+                     140 RETURN_VALUE
          consts
             'AdwDrawBasicButton'
             120
             40
             ''
             None
             ('width', 'height', 'text', 'command')
             'text'
             code
                argcount  : 1
                nlocals   : 7
-               stacksize : 7
+               stacksize : 8
                flags     : 15
                code
                   0x9501870497000200740100000000000000000000a6000000ab00000000
-                  00000000006a0100000000000000007c057c017c02640164029c037c06a4
-                  018e0101007c00a0020000000000000000000000000000000000000000a6
-                  000000ab00000000000000000001007c00a0030000000000000000000000
-                  000000000000000000a6000000ab00000000000000000001007c037c005f
-                  0400000000000000007c006a0500000000000000007c005f060000000000
-                  0000007c006a0700000000000000007c005f0800000000000000007c006a
-                  0900000000000000007c005f0a0000000000000000741700000000000000
-                  0000006403a6010000ab0100000000000000007c005f0c00000000000000
-                  007c00a00d000000000000000000000000000000000000000064047c006a
-                  0e00000000000000006405ac06a6030000ab03000000000000000001007c
-                  00a00d000000000000000000000000000000000000000064077c006a0f00
+                  00000000006a0100000000000000007c057c017c026401640164029c047c
+                  06a4018e0101007c00a00200000000000000000000000000000000000000
+                  00a6000000ab00000000000000000001007c00a003000000000000000000
+                  0000000000000000000000a6000000ab00000000000000000001007c037c
+                  005f0400000000000000007c006a0500000000000000007c005f06000000
+                  00000000007c006a0700000000000000007c005f0800000000000000007c
+                  006a0900000000000000007c005f0a000000000000000074170000000000
+                  00000000006403a6010000ab0100000000000000007c005f0c0000000000
+                  0000007c00a00d000000000000000000000000000000000000000064047c
+                  006a0e00000000000000006405ac06a6030000ab03000000000000000001
+                  007c00a00d000000000000000000000000000000000000000064077c006a
+                  0f00000000000000006405ac06a6030000ab03000000000000000001007c
+                  00a00d000000000000000000000000000000000000000064087c006a1000
                   000000000000006405ac06a6030000ab03000000000000000001007c00a0
-                  0d000000000000000000000000000000000000000064087c006a10000000
+                  0d000000000000000000000000000000000000000064097c006a11000000
                   00000000006405ac06a6030000ab03000000000000000001007c00a00d00
-                  0000000000000000000000000000000000000064097c006a110000000000
-                  0000006405ac06a6030000ab03000000000000000001007c00a00d000000
-                  0000000000000000000000000000000000640a7c006a1200000000000000
-                  006405ac06a6030000ab0300000000000000000100890481197c00a00d00
-                  00000000000000000000000000000000000000640b88046601640c8408a6
-                  020000ab02000000000000000001007c00a00e0000000000000000000000
-                  0000000000000000006400a6010000ab0100000000000000000100640053
-                  00
+                  00000000000000000000000000000000000000640a7c006a120000000000
+                  0000006405ac06a6030000ab0300000000000000000100890481197c00a0
+                  0d0000000000000000000000000000000000000000640b88046601640c84
+                  08a6020000ab02000000000000000001007c00a00e000000000000000000
+                  00000000000000000000006400a6010000ab010000000000000000010064
+                  005300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                4 (command)
                
                  7           4 RESUME                   0
                
                  8           6 PUSH_NULL
                              8 LOAD_GLOBAL              1 (NULL + super)
                             20 PRECALL                  0
                             24 CALL                     0
                             34 LOAD_ATTR                1 (__init__)
                             44 LOAD_FAST                5 (args)
                             46 LOAD_FAST                1 (width)
                             48 LOAD_FAST                2 (height)
                             50 LOAD_CONST               1 (0)
-                            52 LOAD_CONST               2 (('width', 'height', 'bd'))
-                            54 BUILD_CONST_KEY_MAP      3
-                            56 LOAD_FAST                6 (kwargs)
-                            58 DICT_MERGE               1
-                            60 CALL_FUNCTION_EX         1
-                            62 POP_TOP
-               
-                10          64 LOAD_FAST                0 (self)
-                            66 LOAD_METHOD              2 (_other)
-                            88 PRECALL                  0
-                            92 CALL                     0
-                           102 POP_TOP
+                            52 LOAD_CONST               1 (0)
+                            54 LOAD_CONST               2 (('width', 'height', 'bd', 'highlightthickness'))
+                            56 BUILD_CONST_KEY_MAP      4
+                            58 LOAD_FAST                6 (kwargs)
+                            60 DICT_MERGE               1
+                            62 CALL_FUNCTION_EX         1
+                            64 POP_TOP
+               
+                10          66 LOAD_FAST                0 (self)
+                            68 LOAD_METHOD              2 (_other)
+                            90 PRECALL                  0
+                            94 CALL                     0
+                           104 POP_TOP
+               
+                12         106 LOAD_FAST                0 (self)
+                           108 LOAD_METHOD              3 (default_palette)
+                           130 PRECALL                  0
+                           134 CALL                     0
+                           144 POP_TOP
+               
+                14         146 LOAD_FAST                3 (text)
+                           148 LOAD_FAST                0 (self)
+                           150 STORE_ATTR               4 (text)
+               
+                16         160 LOAD_FAST                0 (self)
+                           162 LOAD_ATTR                5 (button_back)
+                           172 LOAD_FAST                0 (self)
+                           174 STORE_ATTR               6 (_button_back)
                
-                12         104 LOAD_FAST                0 (self)
-                           106 LOAD_METHOD              3 (default_palette)
-                           128 PRECALL                  0
-                           132 CALL                     0
-                           142 POP_TOP
-               
-                14         144 LOAD_FAST                3 (text)
-                           146 LOAD_FAST                0 (self)
-                           148 STORE_ATTR               4 (text)
-               
-                16         158 LOAD_FAST                0 (self)
-                           160 LOAD_ATTR                5 (button_back)
-                           170 LOAD_FAST                0 (self)
-                           172 STORE_ATTR               6 (_button_back)
-               
-                17         182 LOAD_FAST                0 (self)
-                           184 LOAD_ATTR                7 (button_border)
-                           194 LOAD_FAST                0 (self)
-                           196 STORE_ATTR               8 (_button_border)
+                17         184 LOAD_FAST                0 (self)
+                           186 LOAD_ATTR                7 (button_border)
+                           196 LOAD_FAST                0 (self)
+                           198 STORE_ATTR               8 (_button_border)
                
-                18         206 LOAD_FAST                0 (self)
-                           208 LOAD_ATTR                9 (button_text_back)
-                           218 LOAD_FAST                0 (self)
-                           220 STORE_ATTR              10 (_button_text_back)
+                18         208 LOAD_FAST                0 (self)
+                           210 LOAD_ATTR                9 (button_text_back)
+                           220 LOAD_FAST                0 (self)
+                           222 STORE_ATTR              10 (_button_text_back)
+               
+                20         232 LOAD_GLOBAL             23 (NULL + nametofont)
+                           244 LOAD_CONST               3 ('TkDefaultFont')
+                           246 PRECALL                  1
+                           250 CALL                     1
+                           260 LOAD_FAST                0 (self)
+                           262 STORE_ATTR              12 (button_text_font)
                
-                20         230 LOAD_GLOBAL             23 (NULL + nametofont)
-                           242 LOAD_CONST               3 ('TkDefaultFont')
-                           244 PRECALL                  1
-                           248 CALL                     1
-                           258 LOAD_FAST                0 (self)
-                           260 STORE_ATTR              12 (button_text_font)
-               
-                22         270 LOAD_FAST                0 (self)
-                           272 LOAD_METHOD             13 (bind)
-                           294 LOAD_CONST               4 ('<Configure>')
-                           296 LOAD_FAST                0 (self)
-                           298 LOAD_ATTR               14 (_draw)
-                           308 LOAD_CONST               5 ('+')
-                           310 KW_NAMES                 6
-                           312 PRECALL                  3
-                           316 CALL                     3
-                           326 POP_TOP
-               
-                23         328 LOAD_FAST                0 (self)
-                           330 LOAD_METHOD             13 (bind)
-                           352 LOAD_CONST               7 ('<Button>')
-                           354 LOAD_FAST                0 (self)
-                           356 LOAD_ATTR               15 (_click)
-                           366 LOAD_CONST               5 ('+')
-                           368 KW_NAMES                 6
-                           370 PRECALL                  3
-                           374 CALL                     3
-                           384 POP_TOP
-               
-                24         386 LOAD_FAST                0 (self)
-                           388 LOAD_METHOD             13 (bind)
-                           410 LOAD_CONST               8 ('<ButtonRelease>')
-                           412 LOAD_FAST                0 (self)
-                           414 LOAD_ATTR               16 (_unclick)
-                           424 LOAD_CONST               5 ('+')
-                           426 KW_NAMES                 6
-                           428 PRECALL                  3
-                           432 CALL                     3
-                           442 POP_TOP
-               
-                25         444 LOAD_FAST                0 (self)
-                           446 LOAD_METHOD             13 (bind)
-                           468 LOAD_CONST               9 ('<Enter>')
-                           470 LOAD_FAST                0 (self)
-                           472 LOAD_ATTR               17 (_hover)
-                           482 LOAD_CONST               5 ('+')
-                           484 KW_NAMES                 6
-                           486 PRECALL                  3
-                           490 CALL                     3
-                           500 POP_TOP
-               
-                26         502 LOAD_FAST                0 (self)
-                           504 LOAD_METHOD             13 (bind)
-                           526 LOAD_CONST              10 ('<Leave>')
-                           528 LOAD_FAST                0 (self)
-                           530 LOAD_ATTR               18 (_hover_release)
-                           540 LOAD_CONST               5 ('+')
-                           542 KW_NAMES                 6
-                           544 PRECALL                  3
-                           548 CALL                     3
-                           558 POP_TOP
-               
-                28         560 LOAD_DEREF               4 (command)
-                           562 POP_JUMP_FORWARD_IF_NONE    25 (to 614)
-               
-                29         564 LOAD_FAST                0 (self)
-                           566 LOAD_METHOD             13 (bind)
-                           588 LOAD_CONST              11 ('<<Click>>')
-                           590 LOAD_CLOSURE             4 (command)
-                           592 BUILD_TUPLE              1
-                           594 LOAD_CONST              12 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 29>)
-                           596 MAKE_FUNCTION            8 (closure)
-                           598 PRECALL                  2
-                           602 CALL                     2
-                           612 POP_TOP
-               
-                31     >>  614 LOAD_FAST                0 (self)
-                           616 LOAD_METHOD             14 (_draw)
-                           638 LOAD_CONST               0 (None)
-                           640 PRECALL                  1
-                           644 CALL                     1
-                           654 POP_TOP
-                           656 LOAD_CONST               0 (None)
-                           658 RETURN_VALUE
+                22         272 LOAD_FAST                0 (self)
+                           274 LOAD_METHOD             13 (bind)
+                           296 LOAD_CONST               4 ('<Configure>')
+                           298 LOAD_FAST                0 (self)
+                           300 LOAD_ATTR               14 (_draw)
+                           310 LOAD_CONST               5 ('+')
+                           312 KW_NAMES                 6
+                           314 PRECALL                  3
+                           318 CALL                     3
+                           328 POP_TOP
+               
+                23         330 LOAD_FAST                0 (self)
+                           332 LOAD_METHOD             13 (bind)
+                           354 LOAD_CONST               7 ('<Button>')
+                           356 LOAD_FAST                0 (self)
+                           358 LOAD_ATTR               15 (_click)
+                           368 LOAD_CONST               5 ('+')
+                           370 KW_NAMES                 6
+                           372 PRECALL                  3
+                           376 CALL                     3
+                           386 POP_TOP
+               
+                24         388 LOAD_FAST                0 (self)
+                           390 LOAD_METHOD             13 (bind)
+                           412 LOAD_CONST               8 ('<ButtonRelease>')
+                           414 LOAD_FAST                0 (self)
+                           416 LOAD_ATTR               16 (_unclick)
+                           426 LOAD_CONST               5 ('+')
+                           428 KW_NAMES                 6
+                           430 PRECALL                  3
+                           434 CALL                     3
+                           444 POP_TOP
+               
+                25         446 LOAD_FAST                0 (self)
+                           448 LOAD_METHOD             13 (bind)
+                           470 LOAD_CONST               9 ('<Enter>')
+                           472 LOAD_FAST                0 (self)
+                           474 LOAD_ATTR               17 (_hover)
+                           484 LOAD_CONST               5 ('+')
+                           486 KW_NAMES                 6
+                           488 PRECALL                  3
+                           492 CALL                     3
+                           502 POP_TOP
+               
+                26         504 LOAD_FAST                0 (self)
+                           506 LOAD_METHOD             13 (bind)
+                           528 LOAD_CONST              10 ('<Leave>')
+                           530 LOAD_FAST                0 (self)
+                           532 LOAD_ATTR               18 (_hover_release)
+                           542 LOAD_CONST               5 ('+')
+                           544 KW_NAMES                 6
+                           546 PRECALL                  3
+                           550 CALL                     3
+                           560 POP_TOP
+               
+                28         562 LOAD_DEREF               4 (command)
+                           564 POP_JUMP_FORWARD_IF_NONE    25 (to 616)
+               
+                29         566 LOAD_FAST                0 (self)
+                           568 LOAD_METHOD             13 (bind)
+                           590 LOAD_CONST              11 ('<<Click>>')
+                           592 LOAD_CLOSURE             4 (command)
+                           594 BUILD_TUPLE              1
+                           596 LOAD_CONST              12 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 29>)
+                           598 MAKE_FUNCTION            8 (closure)
+                           600 PRECALL                  2
+                           604 CALL                     2
+                           614 POP_TOP
+               
+                31     >>  616 LOAD_FAST                0 (self)
+                           618 LOAD_METHOD             14 (_draw)
+                           640 LOAD_CONST               0 (None)
+                           642 PRECALL                  1
+                           646 CALL                     1
+                           656 POP_TOP
+                           658 LOAD_CONST               0 (None)
+                           660 RETURN_VALUE
                consts
                   None
                   0
-                  ('width', 'height', 'bd')
+                  ('width', 'height', 'bd', 'highlightthickness')
                   'TkDefaultFont'
                   '<Configure>'
                   '+'
                   ('add',)
                   '<Button>'
                   '<ButtonRelease>'
                   '<Enter>'
@@ -707,61 +714,183 @@
                varnames   ('self', 'width', 'height', 'text', 'command', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ('command',)
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '__init__'
                firstlineno 7
                lnotab
-                  0x06013a02280228020e0218011801180228023a013a013a013a013a0204
+                  0x06013c02280228020e0218011801180228023a013a013a013a013a0204
                   013202
             code
                argcount  : 1
+               nlocals   : 2
+               stacksize : 5
+               flags     : 11
+               code
+                  0x95018700970064017c01760072357c01a0000000000000000000000000
+                  0000000000000000006401a6010000ab01000000000000000089005f0100
+                  000000000000008900a00200000000000000000000000000000000000000
+                  0064028800660164038408a6020000ab0200000000000000000100640053
+                  0064047c01760072317c01a0000000000000000000000000000000000000
+                  0000006404a6010000ab01000000000000000089005f0300000000000000
+                  008900a00400000000000000000000000000000000000000006400a60100
+                  00ab0100000000000000000100640053000200740b000000000000000000
+                  00a6000000ab0000000000000000006a060000000000000000640569007c
+                  01a4018e01010064005300
+                             0 COPY_FREE_VARS           1
+                             2 MAKE_CELL                0 (self)
+               
+                33           4 RESUME                   0
+               
+                34           6 LOAD_CONST               1 ('command')
+                             8 LOAD_FAST                1 (kwargs)
+                            10 CONTAINS_OP              0
+                            12 POP_JUMP_FORWARD_IF_FALSE    53 (to 120)
+               
+                35          14 LOAD_FAST                1 (kwargs)
+                            16 LOAD_METHOD              0 (pop)
+                            38 LOAD_CONST               1 ('command')
+                            40 PRECALL                  1
+                            44 CALL                     1
+                            54 LOAD_DEREF               0 (self)
+                            56 STORE_ATTR               1 (command)
+               
+                36          66 LOAD_DEREF               0 (self)
+                            68 LOAD_METHOD              2 (bind)
+                            90 LOAD_CONST               2 ('<<Click>>')
+                            92 LOAD_CLOSURE             0 (self)
+                            94 BUILD_TUPLE              1
+                            96 LOAD_CONST               3 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\button.py", line 36>)
+                            98 MAKE_FUNCTION            8 (closure)
+                           100 PRECALL                  2
+                           104 CALL                     2
+                           114 POP_TOP
+                           116 LOAD_CONST               0 (None)
+                           118 RETURN_VALUE
+               
+                37     >>  120 LOAD_CONST               4 ('text')
+                           122 LOAD_FAST                1 (kwargs)
+                           124 CONTAINS_OP              0
+                           126 POP_JUMP_FORWARD_IF_FALSE    49 (to 226)
+               
+                38         128 LOAD_FAST                1 (kwargs)
+                           130 LOAD_METHOD              0 (pop)
+                           152 LOAD_CONST               4 ('text')
+                           154 PRECALL                  1
+                           158 CALL                     1
+                           168 LOAD_DEREF               0 (self)
+                           170 STORE_ATTR               3 (text)
+               
+                39         180 LOAD_DEREF               0 (self)
+                           182 LOAD_METHOD              4 (_draw)
+                           204 LOAD_CONST               0 (None)
+                           206 PRECALL                  1
+                           210 CALL                     1
+                           220 POP_TOP
+                           222 LOAD_CONST               0 (None)
+                           224 RETURN_VALUE
+               
+                41     >>  226 PUSH_NULL
+                           228 LOAD_GLOBAL             11 (NULL + super)
+                           240 PRECALL                  0
+                           244 CALL                     0
+                           254 LOAD_ATTR                6 (configure)
+                           264 LOAD_CONST               5 (())
+                           266 BUILD_MAP                0
+                           268 LOAD_FAST                1 (kwargs)
+                           270 DICT_MERGE               1
+                           272 CALL_FUNCTION_EX         1
+                           274 POP_TOP
+                           276 LOAD_CONST               0 (None)
+                           278 RETURN_VALUE
+               consts
+                  None
+                  'command'
+                  '<<Click>>'
+                  code
+                     argcount  : 1
+                     nlocals   : 1
+                     stacksize : 2
+                     flags     : 19
+                     code
+                        0x950197008901a0000000000000000000000000000000000000000000a6
+                        000000ab0000000000000000005300
+                                   0 COPY_FREE_VARS           1
+                     
+                      36           2 RESUME                   0
+                                   4 LOAD_DEREF               1 (self)
+                                   6 LOAD_METHOD              0 (command)
+                                  28 PRECALL                  0
+                                  32 CALL                     0
+                                  42 RETURN_VALUE
+                     consts
+                        None
+                     names      ('command',)
+                     varnames   ('event',)
+                     freevars   ('self',)
+                     cellvars   ()
+                     filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
+                     name       '<lambda>'
+                     firstlineno 36
+                     lnotab 0x
+                  'text'
+                  ()
+               names      ('pop', 'command', 'bind', 'text', '_draw', 'super', 'configure')
+               varnames   ('self', 'kwargs')
+               freevars   ('__class__',)
+               cellvars   ('self',)
+               filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
+               name       'configure'
+               firstlineno 33
+               lnotab 0x0601080134013601080134012e02
+            code
+               argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006401a6020000ab020000000000
                   000000721e7c00a00100000000000000000000000000000000000000007c
                   006a0200000000000000006402ac03a6020000ab02000000000000000001
                   006400530064005300
-                33           0 RESUME                   0
+                43           0 RESUME                   0
                
-                34           2 LOAD_GLOBAL              1 (NULL + hasattr)
+                44           2 LOAD_GLOBAL              1 (NULL + hasattr)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_CONST               1 ('button_frame_back')
                             18 PRECALL                  2
                             22 CALL                     2
                             32 POP_JUMP_FORWARD_IF_FALSE    30 (to 94)
                
-                35          34 LOAD_FAST                0 (self)
+                45          34 LOAD_FAST                0 (self)
                             36 LOAD_METHOD              1 (configure)
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                2 (button_frame_back)
                             70 LOAD_CONST               2 (0)
                             72 KW_NAMES                 3
                             74 PRECALL                  2
                             78 CALL                     2
                             88 POP_TOP
                             90 LOAD_CONST               0 (None)
                             92 RETURN_VALUE
                
-                34     >>   94 LOAD_CONST               0 (None)
+                44     >>   94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                consts
                   None
                   'button_frame_back'
                   0
                   ('background', 'borderwidth')
                names      ('hasattr', 'configure', 'button_frame_back')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_other'
-               firstlineno 33
+               firstlineno 43
                lnotab 0x020120013cff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 9
                flags     : 3
                code
@@ -775,80 +904,80 @@
                   0000007c005f0700000000000000007c00a0080000000000000000000000
                   0000000000000000007c00a0020000000000000000000000000000000000
                   000000a6000000ab00000000000000000064057a0b00007c00a003000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0064057a0b00007c006a0900000000000000007c006a0a00000000000000
                   007c006a0b0000000000000000ac06a6050000ab0500000000000000007c
                   005f0c000000000000000064005300
-                37           0 RESUME                   0
+                47           0 RESUME                   0
                
-                38           2 LOAD_FAST                0 (self)
+                48           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-                40          44 LOAD_FAST                0 (self)
+                50          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_rectangle)
                
-                41          68 LOAD_CONST               2 (1.5)
+                51          68 LOAD_CONST               2 (1.5)
                             70 LOAD_CONST               2 (1.5)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
                            116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                
-                42         160 LOAD_FAST                0 (self)
+                52         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (button_border_width)
                
-                43         172 LOAD_FAST                0 (self)
+                53         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (_button_border)
                            184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_button_back)
                
-                40         196 KW_NAMES                 4
+                50         196 KW_NAMES                 4
                            198 PRECALL                  7
                            202 CALL                     7
                            212 LOAD_FAST                0 (self)
                            214 STORE_ATTR               7 (button_frame)
                
-                46         224 LOAD_FAST                0 (self)
+                56         224 LOAD_FAST                0 (self)
                            226 LOAD_METHOD              8 (create_text)
                
-                47         248 LOAD_FAST                0 (self)
+                57         248 LOAD_FAST                0 (self)
                            250 LOAD_METHOD              2 (winfo_width)
                            272 PRECALL                  0
                            276 CALL                     0
                            286 LOAD_CONST               5 (2)
                            288 BINARY_OP               11 (/)
                            292 LOAD_FAST                0 (self)
                            294 LOAD_METHOD              3 (winfo_height)
                            316 PRECALL                  0
                            320 CALL                     0
                            330 LOAD_CONST               5 (2)
                            332 BINARY_OP               11 (/)
                
-                48         336 LOAD_FAST                0 (self)
+                58         336 LOAD_FAST                0 (self)
                            338 LOAD_ATTR                9 (text)
                            348 LOAD_FAST                0 (self)
                            350 LOAD_ATTR               10 (_button_text_back)
                
-                49         360 LOAD_FAST                0 (self)
+                59         360 LOAD_FAST                0 (self)
                            362 LOAD_ATTR               11 (button_text_font)
                
-                46         372 KW_NAMES                 6
+                56         372 KW_NAMES                 6
                            374 PRECALL                  5
                            378 CALL                     5
                            388 LOAD_FAST                0 (self)
                            390 STORE_ATTR              12 (button_text)
                            400 LOAD_CONST               0 (None)
                            402 RETURN_VALUE
                consts
@@ -861,56 +990,56 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_rectangle', 'winfo_width', 'winfo_height', 'button_border_width', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_draw'
-               firstlineno 37
+               firstlineno 47
                lnotab 0x02012a0218015c010c0118fd1c061801580118010cfd
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x970064017c005f0000000000000000007c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
                   00a0070000000000000000000000000000000000000000a6000000ab0000
                   0000000000000001007c00a0080000000000000000000000000000000000
                   0000006400a6010000ab010000000000000000010064005300
-                52           0 RESUME                   0
+                62           0 RESUME                   0
                
-                53           2 LOAD_CONST               1 (True)
+                63           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                
-                54          16 LOAD_FAST                0 (self)
+                64          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_pressed_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                55          40 LOAD_FAST                0 (self)
+                65          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_pressed_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                56          64 LOAD_FAST                0 (self)
+                66          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                5 (button_pressed_text_back)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               6 (_button_text_back)
                
-                58          88 LOAD_FAST                0 (self)
+                68          88 LOAD_FAST                0 (self)
                             90 LOAD_METHOD              7 (focus_set)
                            112 PRECALL                  0
                            116 CALL                     0
                            126 POP_TOP
                
-                60         128 LOAD_FAST                0 (self)
+                70         128 LOAD_FAST                0 (self)
                            130 LOAD_METHOD              8 (_draw)
                            152 LOAD_CONST               0 (None)
                            154 PRECALL                  1
                            158 CALL                     1
                            168 POP_TOP
                            170 LOAD_CONST               0 (None)
                            172 RETURN_VALUE
@@ -919,112 +1048,112 @@
                   True
                names      ('hover', 'button_pressed_back', '_button_back', 'button_pressed_border', '_button_border', 'button_pressed_text_back', '_button_text_back', 'focus_set', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_click'
-               firstlineno 52
+               firstlineno 62
                lnotab 0x02010e011801180118022802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a00000000000000000072507c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
                   00a00700000000000000000000000000000000000000006400a6010000ab
                   01000000000000000001007c00a008000000000000000000000000000000
                   00000000006401a6010000ab010000000000000000010064005300640053
                   00
-                62           0 RESUME                   0
+                72           0 RESUME                   0
                
-                63           2 LOAD_FAST                0 (self)
+                73           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (hover)
                             14 POP_JUMP_FORWARD_IF_FALSE    80 (to 176)
                
-                64          16 LOAD_FAST                0 (self)
+                74          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_active_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                65          40 LOAD_FAST                0 (self)
+                75          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_active_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                66          64 LOAD_FAST                0 (self)
+                76          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                5 (button_active_text_back)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               6 (_button_text_back)
                
-                68          88 LOAD_FAST                0 (self)
+                78          88 LOAD_FAST                0 (self)
                             90 LOAD_METHOD              7 (_draw)
                            112 LOAD_CONST               0 (None)
                            114 PRECALL                  1
                            118 CALL                     1
                            128 POP_TOP
                
-                70         130 LOAD_FAST                0 (self)
+                80         130 LOAD_FAST                0 (self)
                            132 LOAD_METHOD              8 (event_generate)
                            154 LOAD_CONST               1 ('<<Click>>')
                            156 PRECALL                  1
                            160 CALL                     1
                            170 POP_TOP
                            172 LOAD_CONST               0 (None)
                            174 RETURN_VALUE
                
-                63     >>  176 LOAD_CONST               0 (None)
+                73     >>  176 LOAD_CONST               0 (None)
                            178 RETURN_VALUE
                consts
                   None
                   '<<Click>>'
                names      ('hover', 'button_active_back', '_button_back', 'button_active_border', '_button_border', 'button_active_text_back', '_button_text_back', '_draw', 'event_generate')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_unclick'
-               firstlineno 62
+               firstlineno 72
                lnotab 0x02010e011801180118022a022ef9
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x970064017c005f0000000000000000007c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
                   00a00700000000000000000000000000000000000000006400a6010000ab
                   010000000000000000010064005300
-                72           0 RESUME                   0
+                82           0 RESUME                   0
                
-                73           2 LOAD_CONST               1 (True)
+                83           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                
-                74          16 LOAD_FAST                0 (self)
+                84          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_active_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                75          40 LOAD_FAST                0 (self)
+                85          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_active_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                76          64 LOAD_FAST                0 (self)
+                86          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                5 (button_active_text_back)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               6 (_button_text_back)
                
-                78          88 LOAD_FAST                0 (self)
+                88          88 LOAD_FAST                0 (self)
                             90 LOAD_METHOD              7 (_draw)
                            112 LOAD_CONST               0 (None)
                            114 PRECALL                  1
                            118 CALL                     1
                            128 POP_TOP
                            130 LOAD_CONST               0 (None)
                            132 RETURN_VALUE
@@ -1033,49 +1162,49 @@
                   True
                names      ('hover', 'button_active_back', '_button_back', 'button_active_border', '_button_border', 'button_active_text_back', '_button_text_back', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_hover'
-               firstlineno 72
+               firstlineno 82
                lnotab 0x02010e01180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x970064017c005f0000000000000000007c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
                   00a00700000000000000000000000000000000000000006400a6010000ab
                   010000000000000000010064005300
-                80           0 RESUME                   0
+                90           0 RESUME                   0
                
-                81           2 LOAD_CONST               1 (False)
+                91           2 LOAD_CONST               1 (False)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                
-                82          16 LOAD_FAST                0 (self)
+                92          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                83          40 LOAD_FAST                0 (self)
+                93          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                84          64 LOAD_FAST                0 (self)
+                94          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                5 (button_text_back)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               6 (_button_text_back)
                
-                86          88 LOAD_FAST                0 (self)
+                96          88 LOAD_FAST                0 (self)
                             90 LOAD_METHOD              7 (_draw)
                            112 LOAD_CONST               0 (None)
                            114 PRECALL                  1
                            118 CALL                     1
                            128 POP_TOP
                            130 LOAD_CONST               0 (None)
                            132 RETURN_VALUE
@@ -1084,116 +1213,116 @@
                   False
                names      ('hover', 'button_back', '_button_back', 'button_border', '_button_border', 'button_text_back', '_button_text_back', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_hover_release'
-               firstlineno 80
+               firstlineno 90
                lnotab 0x02010e01180118011802
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-                88           0 RESUME                   0
+                98           0 RESUME                   0
                
-                89           2 LOAD_FAST                1 (font)
+                99           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-                90           6 LOAD_FAST                0 (self)
+               100           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_text_font)
                             18 RETURN_VALUE
                
-                92     >>   20 LOAD_FAST                1 (font)
+               102     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'font'
-               firstlineno 88
+               firstlineno 98
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                94           0 RESUME                   0
+               104           0 RESUME                   0
                
-                95           2 LOAD_FAST                0 (self)
+               105           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 94
+               firstlineno 104
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02640364046405640664076408640664076409640a9c0ba6010000ab0100
                   00000000000000010064005300
-                97           0 RESUME                   0
+               107           0 RESUME                   0
                
-                98           2 LOAD_FAST                0 (self)
+               108           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               100          26 LOAD_CONST               1 ('#f3f3f3')
+               110          26 LOAD_CONST               1 ('#f3f3f3')
                
-               102          28 LOAD_CONST               2 (1)
+               112          28 LOAD_CONST               2 (1)
                
-               104          30 LOAD_CONST               3 ('#eaeaea')
+               114          30 LOAD_CONST               3 ('#eaeaea')
                
-               105          32 LOAD_CONST               4 ('#fdfdfd')
+               115          32 LOAD_CONST               4 ('#fdfdfd')
                
-               106          34 LOAD_CONST               5 ('#1a1a1a')
+               116          34 LOAD_CONST               5 ('#1a1a1a')
                
-               108          36 LOAD_CONST               6 ('#e2e2e2')
+               118          36 LOAD_CONST               6 ('#e2e2e2')
                
-               109          38 LOAD_CONST               7 ('#f9f9f9')
+               119          38 LOAD_CONST               7 ('#f9f9f9')
                
-               110          40 LOAD_CONST               8 ('#5f5f5f')
+               120          40 LOAD_CONST               8 ('#5f5f5f')
                
-               112          42 LOAD_CONST               6 ('#e2e2e2')
+               122          42 LOAD_CONST               6 ('#e2e2e2')
                
-               113          44 LOAD_CONST               7 ('#f9f9f9')
+               123          44 LOAD_CONST               7 ('#f9f9f9')
                
-               114          46 LOAD_CONST               9 ('#8a8a8a')
+               124          46 LOAD_CONST               9 ('#8a8a8a')
                
-                99          48 LOAD_CONST              10 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
+               109          48 LOAD_CONST              10 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
                             50 BUILD_CONST_KEY_MAP     11
                
-                98          52 PRECALL                  1
+               108          52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
                             68 LOAD_CONST               0 (None)
                             70 RETURN_VALUE
                consts
                   None
                   '#f3f3f3'
@@ -1208,56 +1337,56 @@
                   ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette_light'
-               firstlineno 97
+               firstlineno 107
                lnotab 0x02011802020202020201020102020201020102020201020102f104ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02640364046405640364066407640364086409640a9c0ba6010000ab0100
                   00000000000000010064005300
-               118           0 RESUME                   0
+               128           0 RESUME                   0
                
-               119           2 LOAD_FAST                0 (self)
+               129           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               121          26 LOAD_CONST               1 ('#202020')
+               131          26 LOAD_CONST               1 ('#202020')
                
-               123          28 LOAD_CONST               2 (1)
+               133          28 LOAD_CONST               2 (1)
                
-               125          30 LOAD_CONST               3 ('#454545')
+               135          30 LOAD_CONST               3 ('#454545')
                
-               126          32 LOAD_CONST               4 ('#353535')
+               136          32 LOAD_CONST               4 ('#353535')
                
-               127          34 LOAD_CONST               5 ('#ffffff')
+               137          34 LOAD_CONST               5 ('#ffffff')
                
-               129          36 LOAD_CONST               3 ('#454545')
+               139          36 LOAD_CONST               3 ('#454545')
                
-               130          38 LOAD_CONST               6 ('#3a3a3a')
+               140          38 LOAD_CONST               6 ('#3a3a3a')
                
-               131          40 LOAD_CONST               7 ('#cecece')
+               141          40 LOAD_CONST               7 ('#cecece')
                
-               133          42 LOAD_CONST               3 ('#454545')
+               143          42 LOAD_CONST               3 ('#454545')
                
-               134          44 LOAD_CONST               8 ('#2f2f2f')
+               144          44 LOAD_CONST               8 ('#2f2f2f')
                
-               135          46 LOAD_CONST               9 ('#9a9a9a')
+               145          46 LOAD_CONST               9 ('#9a9a9a')
                
-               120          48 LOAD_CONST              10 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
+               130          48 LOAD_CONST              10 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
                             50 BUILD_CONST_KEY_MAP     11
                
-               119          52 PRECALL                  1
+               129          52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
                             68 LOAD_CONST               0 (None)
                             70 RETURN_VALUE
                consts
                   None
                   '#202020'
@@ -1272,15 +1401,15 @@
                   ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette_dark'
-               firstlineno 118
+               firstlineno 128
                lnotab 0x02011802020202020201020102020201020102020201020102f104ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 12
                flags     : 3
                code
@@ -1298,145 +1427,145 @@
                   000000000001006400530023007418000000000000000000002400720401
                   0059006400530077007803590077017c006a0000000000000000007c006a
                   0100000000000000007c006a0200000000000000007c006a030000000000
                   0000007c006a0400000000000000007c006a0500000000000000007c006a
                   0600000000000000007c006a0700000000000000007c006a080000000000
                   0000007c006a0900000000000000007c006a0a0000000000000000640c9c
                   0b5300
-               139           0 RESUME                   0
+               149           0 RESUME                   0
                
-               140           2 LOAD_FAST                1 (dict)
+               150           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE   184 (to 374)
                
-               141           6 LOAD_FAST                1 (dict)
+               151           6 LOAD_FAST                1 (dict)
                              8 LOAD_CONST               1 ('button_frame_back')
                             10 BINARY_SUBSCR
                             20 LOAD_FAST                0 (self)
                             22 STORE_ATTR               0 (button_frame_back)
                
-               142          32 LOAD_FAST                1 (dict)
+               152          32 LOAD_FAST                1 (dict)
                             34 LOAD_CONST               2 ('button_border_width')
                             36 BINARY_SUBSCR
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               1 (button_border_width)
                
-               144          58 LOAD_FAST                1 (dict)
+               154          58 LOAD_FAST                1 (dict)
                             60 LOAD_CONST               3 ('button_border')
                             62 BINARY_SUBSCR
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (button_border)
                
-               145          84 LOAD_FAST                1 (dict)
+               155          84 LOAD_FAST                1 (dict)
                             86 LOAD_CONST               4 ('button_back')
                             88 BINARY_SUBSCR
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               3 (button_back)
                
-               146         110 LOAD_FAST                1 (dict)
+               156         110 LOAD_FAST                1 (dict)
                            112 LOAD_CONST               5 ('button_text_back')
                            114 BINARY_SUBSCR
                            124 LOAD_FAST                0 (self)
                            126 STORE_ATTR               4 (button_text_back)
                
-               148         136 LOAD_FAST                1 (dict)
+               158         136 LOAD_FAST                1 (dict)
                            138 LOAD_CONST               6 ('button_active_border')
                            140 BINARY_SUBSCR
                            150 LOAD_FAST                0 (self)
                            152 STORE_ATTR               5 (button_active_border)
                
-               149         162 LOAD_FAST                1 (dict)
+               159         162 LOAD_FAST                1 (dict)
                            164 LOAD_CONST               7 ('button_active_back')
                            166 BINARY_SUBSCR
                            176 LOAD_FAST                0 (self)
                            178 STORE_ATTR               6 (button_active_back)
                
-               150         188 LOAD_FAST                1 (dict)
+               160         188 LOAD_FAST                1 (dict)
                            190 LOAD_CONST               8 ('button_active_text_back')
                            192 BINARY_SUBSCR
                            202 LOAD_FAST                0 (self)
                            204 STORE_ATTR               7 (button_active_text_back)
                
-               152         214 LOAD_FAST                1 (dict)
+               162         214 LOAD_FAST                1 (dict)
                            216 LOAD_CONST               9 ('button_pressed_border')
                            218 BINARY_SUBSCR
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (button_pressed_border)
                
-               153         240 LOAD_FAST                1 (dict)
+               163         240 LOAD_FAST                1 (dict)
                            242 LOAD_CONST              10 ('button_pressed_back')
                            244 BINARY_SUBSCR
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (button_pressed_back)
                
-               154         266 LOAD_FAST                1 (dict)
+               164         266 LOAD_FAST                1 (dict)
                            268 LOAD_CONST              11 ('button_pressed_text_back')
                            270 BINARY_SUBSCR
                            280 LOAD_FAST                0 (self)
                            282 STORE_ATTR              10 (button_pressed_text_back)
                
-               156         292 NOP
+               166         292 NOP
                
-               157         294 LOAD_FAST                0 (self)
+               167         294 LOAD_FAST                0 (self)
                            296 LOAD_METHOD             11 (_draw)
                            318 LOAD_CONST               0 (None)
                            320 PRECALL                  1
                            324 CALL                     1
                            334 POP_TOP
                            336 LOAD_CONST               0 (None)
                            338 RETURN_VALUE
                        >>  340 PUSH_EXC_INFO
                
-               158         342 LOAD_GLOBAL             24 (AttributeError)
+               168         342 LOAD_GLOBAL             24 (AttributeError)
                            354 CHECK_EXC_MATCH
                            356 POP_JUMP_FORWARD_IF_FALSE     4 (to 366)
                            358 POP_TOP
                
-               159         360 POP_EXCEPT
+               169         360 POP_EXCEPT
                            362 LOAD_CONST               0 (None)
                            364 RETURN_VALUE
                
-               158     >>  366 RERAISE                  0
+               168     >>  366 RERAISE                  0
                        >>  368 COPY                     3
                            370 POP_EXCEPT
                            372 RERAISE                  1
                
-               162     >>  374 LOAD_FAST                0 (self)
+               172     >>  374 LOAD_FAST                0 (self)
                            376 LOAD_ATTR                0 (button_frame_back)
                
-               163         386 LOAD_FAST                0 (self)
+               173         386 LOAD_FAST                0 (self)
                            388 LOAD_ATTR                1 (button_border_width)
                
-               165         398 LOAD_FAST                0 (self)
+               175         398 LOAD_FAST                0 (self)
                            400 LOAD_ATTR                2 (button_border)
                
-               166         410 LOAD_FAST                0 (self)
+               176         410 LOAD_FAST                0 (self)
                            412 LOAD_ATTR                3 (button_back)
                
-               167         422 LOAD_FAST                0 (self)
+               177         422 LOAD_FAST                0 (self)
                            424 LOAD_ATTR                4 (button_text_back)
                
-               169         434 LOAD_FAST                0 (self)
+               179         434 LOAD_FAST                0 (self)
                            436 LOAD_ATTR                5 (button_active_border)
                
-               170         446 LOAD_FAST                0 (self)
+               180         446 LOAD_FAST                0 (self)
                            448 LOAD_ATTR                6 (button_active_back)
                
-               171         458 LOAD_FAST                0 (self)
+               181         458 LOAD_FAST                0 (self)
                            460 LOAD_ATTR                7 (button_active_text_back)
                
-               173         470 LOAD_FAST                0 (self)
+               183         470 LOAD_FAST                0 (self)
                            472 LOAD_ATTR                8 (button_pressed_border)
                
-               174         482 LOAD_FAST                0 (self)
+               184         482 LOAD_FAST                0 (self)
                            484 LOAD_ATTR                9 (button_pressed_back)
                
-               175         494 LOAD_FAST                0 (self)
+               185         494 LOAD_FAST                0 (self)
                            496 LOAD_ATTR               10 (button_pressed_text_back)
                
-               161         506 LOAD_CONST              12 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
+               171         506 LOAD_CONST              12 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
                            508 BUILD_CONST_KEY_MAP     11
                            510 RETURN_VALUE
                ExceptionTable:
                  294 to 334 -> 340 [0]
                  340 to 358 -> 368 [1] lasti
                  366 to 366 -> 368 [1] lasti
                consts
@@ -1455,153 +1584,153 @@
                   ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
                names      ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette'
-               firstlineno 139
+               firstlineno 149
                lnotab
                   0x020104011a011a021a011a011a021a011a011a021a011a011a02020130
                   01120106ff08040c010c020c010c010c020c010c010c020c010c010cf2
             (None,)
-         names      ('__name__', '__module__', '__qualname__', 'str', '__init__', '_other', '_draw', '_click', '_unclick', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'configure', '_other', '_draw', '_click', '_unclick', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawBasicButton'
          firstlineno 6
-         lnotab 0x0c011c1a0604060f080a080a080808080e06060306150615
+         lnotab 0x0c011c1a0a0a0604060f080a080a080808080e06060306150615
       'AdwDrawBasicButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         179           0 RESUME                   0
+         189           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         180          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 180>)
+         190          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 190>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               180           0 RESUME                   0
+               190           0 RESUME                   0
                
-               181           2 LOAD_FAST                0 (self)
+               191           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 180
+               firstlineno 190
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawButton'
-         firstlineno 179
+         firstlineno 189
          lnotab 0x0a01
       'AdwDrawButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         184           0 RESUME                   0
+         194           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         185          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 185>)
+         195          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 195>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               185           0 RESUME                   0
+               195           0 RESUME                   0
                
-               186           2 LOAD_FAST                0 (self)
+               196           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 185
+               firstlineno 195
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawDarkButton'
-         firstlineno 184
+         firstlineno 194
          lnotab 0x0a01
       'AdwDrawDarkButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         189           0 RESUME                   0
+         199           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawAccentButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         190          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 190>)
+         200          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 200>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawAccentButton'
             code
@@ -1609,45 +1738,45 @@
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036401640464036405640464066406640764089c0ba6010000ab0100
                   00000000000000010064005300
-               190           0 RESUME                   0
+               200           0 RESUME                   0
                
-               191           2 LOAD_FAST                0 (self)
+               201           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               193          26 LOAD_CONST               1 ('#0067c0')
+               203          26 LOAD_CONST               1 ('#0067c0')
                
-               195          28 LOAD_CONST               2 (1)
+               205          28 LOAD_CONST               2 (1)
                
-               197          30 LOAD_CONST               3 ('#1473c5')
+               207          30 LOAD_CONST               3 ('#1473c5')
                
-               198          32 LOAD_CONST               1 ('#0067c0')
+               208          32 LOAD_CONST               1 ('#0067c0')
                
-               199          34 LOAD_CONST               4 ('#ffffff')
+               209          34 LOAD_CONST               4 ('#ffffff')
                
-               201          36 LOAD_CONST               3 ('#1473c5')
+               211          36 LOAD_CONST               3 ('#1473c5')
                
-               202          38 LOAD_CONST               5 ('#1975c5')
+               212          38 LOAD_CONST               5 ('#1975c5')
                
-               203          40 LOAD_CONST               4 ('#ffffff')
+               213          40 LOAD_CONST               4 ('#ffffff')
                
-               205          42 LOAD_CONST               6 ('#3284cb')
+               215          42 LOAD_CONST               6 ('#3284cb')
                
-               206          44 LOAD_CONST               6 ('#3284cb')
+               216          44 LOAD_CONST               6 ('#3284cb')
                
-               207          46 LOAD_CONST               7 ('#fdfdfd')
+               217          46 LOAD_CONST               7 ('#fdfdfd')
                
-               192          48 LOAD_CONST               8 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
+               202          48 LOAD_CONST               8 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
                             50 BUILD_CONST_KEY_MAP     11
                
-               191          52 PRECALL                  1
+               201          52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
                             68 LOAD_CONST               0 (None)
                             70 RETURN_VALUE
                consts
                   None
                   '#0067c0'
@@ -1660,81 +1789,81 @@
                   ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 190
+               firstlineno 200
                lnotab 0x02011802020202020201020102020201020102020201020102f104ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawAccentButton'
-         firstlineno 189
+         firstlineno 199
          lnotab 0x0a01
       'AdwDrawAccentButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             0b6404650565067a0700006602640584055a07640684005a08640784005a
             09640884005a0a640984005a0b640b640a84015a0c880078015a0d5300
                        0 MAKE_CELL                0 (__class__)
          
-         213           2 RESUME                   0
+         223           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundButton')
                       10 STORE_NAME               2 (__qualname__)
          
-         214          12 LOAD_CLOSURE             0 (__class__)
+         224          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\button.py", line 214>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\button.py", line 224>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         217          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\button.py", line 217>)
+         227          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\button.py", line 227>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         220          28 LOAD_CONST              11 ((None,))
+         230          28 LOAD_CONST              11 ((None,))
                       30 LOAD_CONST               4 ('radius')
                       32 LOAD_NAME                5 (float)
                       34 LOAD_NAME                6 (int)
                       36 BINARY_OP                7 (|)
                       40 BUILD_TUPLE              2
-                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\button.py", line 220>)
+                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\button.py", line 230>)
                       44 MAKE_FUNCTION            5 (defaults, annotations)
                       46 STORE_NAME               7 (border_radius)
          
-         226          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 226>)
+         236          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 236>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               8 (_draw)
          
-         241          54 LOAD_CONST               7 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 241>)
+         251          54 LOAD_CONST               7 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 251>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               9 (default_palette)
          
-         244          60 LOAD_CONST               8 (<code object palette_light, file "D:\tkadw\tkadw\canvas\button.py", line 244>)
+         254          60 LOAD_CONST               8 (<code object palette_light, file "D:\tkadw\tkadw\canvas\button.py", line 254>)
                       62 MAKE_FUNCTION            0
                       64 STORE_NAME              10 (palette_light)
          
-         265          66 LOAD_CONST               9 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\button.py", line 265>)
+         275          66 LOAD_CONST               9 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\button.py", line 275>)
                       68 MAKE_FUNCTION            0
                       70 STORE_NAME              11 (palette_dark)
          
-         286          72 LOAD_CONST              11 ((None,))
-                      74 LOAD_CONST              10 (<code object palette, file "D:\tkadw\tkadw\canvas\button.py", line 286>)
+         296          72 LOAD_CONST              11 ((None,))
+                      74 LOAD_CONST              10 (<code object palette, file "D:\tkadw\tkadw\canvas\button.py", line 296>)
                       76 MAKE_FUNCTION            1 (defaults)
                       78 STORE_NAME              12 (palette)
                       80 LOAD_CLOSURE             0 (__class__)
                       82 COPY                     1
                       84 STORE_NAME              13 (__classcell__)
                       86 RETURN_VALUE
          consts
@@ -1745,17 +1874,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               214           2 RESUME                   0
+               224           2 RESUME                   0
                
-               215           4 PUSH_NULL
+               225           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -1768,29 +1897,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '__init__'
-               firstlineno 214
+               firstlineno 224
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               217           0 RESUME                   0
+               227           0 RESUME                   0
                
-               218           2 LOAD_FAST                0 (self)
+               228           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -1808,49 +1937,49 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_other'
-               firstlineno 217
+               firstlineno 227
                lnotab 0x0201
             None
             'radius'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               220           0 RESUME                   0
+               230           0 RESUME                   0
                
-               221           2 LOAD_FAST                1 (radius)
+               231           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               222           6 LOAD_FAST                0 (self)
+               232           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               224     >>   20 LOAD_FAST                1 (radius)
+               234     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'border_radius'
-               firstlineno 220
+               firstlineno 230
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -1864,27 +1993,27 @@
                   04a6080000ab0800000000000000007c005f0800000000000000007c00a0
                   0900000000000000000000000000000000000000007c00a0020000000000
                   000000000000000000000000000000a6000000ab00000000000000000064
                   027a0b00007c00a0030000000000000000000000000000000000000000a6
                   000000ab00000000000000000064027a0b00007c006a0a00000000000000
                   007c006a0b00000000000000007c006a0c0000000000000000ac05a60500
                   00ab0500000000000000007c005f0d000000000000000064005300
-               226           0 RESUME                   0
+               236           0 RESUME                   0
                
-               227           2 LOAD_FAST                0 (self)
+               237           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               229          44 LOAD_FAST                0 (self)
+               239          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect2)
                
-               230          68 LOAD_CONST               2 (2)
+               240          68 LOAD_CONST               2 (2)
                             70 LOAD_CONST               2 (2)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
@@ -1893,53 +2022,53 @@
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                            160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (button_radius)
                
-               231         172 LOAD_FAST                0 (self)
+               241         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (button_border_width)
                
-               232         184 LOAD_FAST                0 (self)
+               242         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_button_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_button_back)
                
-               229         208 KW_NAMES                 4
+               239         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 LOAD_FAST                0 (self)
                            226 STORE_ATTR               8 (button_frame)
                
-               235         236 LOAD_FAST                0 (self)
+               245         236 LOAD_FAST                0 (self)
                            238 LOAD_METHOD              9 (create_text)
                
-               236         260 LOAD_FAST                0 (self)
+               246         260 LOAD_FAST                0 (self)
                            262 LOAD_METHOD              2 (winfo_width)
                            284 PRECALL                  0
                            288 CALL                     0
                            298 LOAD_CONST               2 (2)
                            300 BINARY_OP               11 (/)
                            304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              3 (winfo_height)
                            328 PRECALL                  0
                            332 CALL                     0
                            342 LOAD_CONST               2 (2)
                            344 BINARY_OP               11 (/)
                
-               237         348 LOAD_FAST                0 (self)
+               247         348 LOAD_FAST                0 (self)
                            350 LOAD_ATTR               10 (text)
                            360 LOAD_FAST                0 (self)
                            362 LOAD_ATTR               11 (_button_text_back)
                
-               238         372 LOAD_FAST                0 (self)
+               248         372 LOAD_FAST                0 (self)
                            374 LOAD_ATTR               12 (button_text_font)
                
-               235         384 KW_NAMES                 5
+               245         384 KW_NAMES                 5
                            386 PRECALL                  5
                            390 CALL                     5
                            400 LOAD_FAST                0 (self)
                            402 STORE_ATTR              13 (button_text)
                            412 LOAD_CONST               0 (None)
                            414 RETURN_VALUE
                consts
@@ -1951,83 +2080,83 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_round_rect2', 'winfo_width', 'winfo_height', 'button_radius', 'button_border_width', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_draw'
-               firstlineno 226
+               firstlineno 236
                lnotab 0x02012a02180168010c0118fd1c061801580118010cfd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               241           0 RESUME                   0
+               251           0 RESUME                   0
                
-               242           2 LOAD_FAST                0 (self)
+               252           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 241
+               firstlineno 251
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02640364046405640664076408640664076409640a9c0ba6010000ab0100
                   00000000000000010064005300
-               244           0 RESUME                   0
+               254           0 RESUME                   0
                
-               245           2 LOAD_FAST                0 (self)
+               255           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               247          26 LOAD_CONST               1 (8)
+               257          26 LOAD_CONST               1 (8)
                
-               249          28 LOAD_CONST               2 (1)
+               259          28 LOAD_CONST               2 (1)
                
-               251          30 LOAD_CONST               3 ('#eaeaea')
+               261          30 LOAD_CONST               3 ('#eaeaea')
                
-               252          32 LOAD_CONST               4 ('#fdfdfd')
+               262          32 LOAD_CONST               4 ('#fdfdfd')
                
-               253          34 LOAD_CONST               5 ('#1a1a1a')
+               263          34 LOAD_CONST               5 ('#1a1a1a')
                
-               255          36 LOAD_CONST               6 ('#e2e2e2')
+               265          36 LOAD_CONST               6 ('#e2e2e2')
                
-               256          38 LOAD_CONST               7 ('#f9f9f9')
+               266          38 LOAD_CONST               7 ('#f9f9f9')
                
-               257          40 LOAD_CONST               8 ('#5f5f5f')
+               267          40 LOAD_CONST               8 ('#5f5f5f')
                
-               259          42 LOAD_CONST               6 ('#e2e2e2')
+               269          42 LOAD_CONST               6 ('#e2e2e2')
                
-               260          44 LOAD_CONST               7 ('#f9f9f9')
+               270          44 LOAD_CONST               7 ('#f9f9f9')
                
-               261          46 LOAD_CONST               9 ('#8a8a8a')
+               271          46 LOAD_CONST               9 ('#8a8a8a')
                
-               246          48 LOAD_CONST              10 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
+               256          48 LOAD_CONST              10 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
                             50 BUILD_CONST_KEY_MAP     11
                
-               245          52 PRECALL                  1
+               255          52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
                             68 LOAD_CONST               0 (None)
                             70 RETURN_VALUE
                consts
                   None
                   8
@@ -2042,56 +2171,56 @@
                   ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette_light'
-               firstlineno 244
+               firstlineno 254
                lnotab 0x02011802020202020201020102020201020102020201020102f104ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02640364046405640364066407640364086409640a9c0ba6010000ab0100
                   00000000000000010064005300
-               265           0 RESUME                   0
+               275           0 RESUME                   0
                
-               266           2 LOAD_FAST                0 (self)
+               276           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               268          26 LOAD_CONST               1 (8)
+               278          26 LOAD_CONST               1 (8)
                
-               270          28 LOAD_CONST               2 (1)
+               280          28 LOAD_CONST               2 (1)
                
-               272          30 LOAD_CONST               3 ('#454545')
+               282          30 LOAD_CONST               3 ('#454545')
                
-               273          32 LOAD_CONST               4 ('#353535')
+               283          32 LOAD_CONST               4 ('#353535')
                
-               274          34 LOAD_CONST               5 ('#ffffff')
+               284          34 LOAD_CONST               5 ('#ffffff')
                
-               276          36 LOAD_CONST               3 ('#454545')
+               286          36 LOAD_CONST               3 ('#454545')
                
-               277          38 LOAD_CONST               6 ('#3a3a3a')
+               287          38 LOAD_CONST               6 ('#3a3a3a')
                
-               278          40 LOAD_CONST               7 ('#cecece')
+               288          40 LOAD_CONST               7 ('#cecece')
                
-               280          42 LOAD_CONST               3 ('#454545')
+               290          42 LOAD_CONST               3 ('#454545')
                
-               281          44 LOAD_CONST               8 ('#2f2f2f')
+               291          44 LOAD_CONST               8 ('#2f2f2f')
                
-               282          46 LOAD_CONST               9 ('#9a9a9a')
+               292          46 LOAD_CONST               9 ('#9a9a9a')
                
-               267          48 LOAD_CONST              10 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
+               277          48 LOAD_CONST              10 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
                             50 BUILD_CONST_KEY_MAP     11
                
-               266          52 PRECALL                  1
+               276          52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
                             68 LOAD_CONST               0 (None)
                             70 RETURN_VALUE
                consts
                   None
                   8
@@ -2106,15 +2235,15 @@
                   ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette_dark'
-               firstlineno 265
+               firstlineno 275
                lnotab 0x02011802020202020201020102020201020102020201020102f104ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 12
                flags     : 3
                code
@@ -2132,145 +2261,145 @@
                   000000000001006400530023007418000000000000000000002400720401
                   0059006400530077007803590077017c006a0d00000000000000007c006a
                   0100000000000000007c006a0200000000000000007c006a030000000000
                   0000007c006a0400000000000000007c006a0500000000000000007c006a
                   0600000000000000007c006a0700000000000000007c006a080000000000
                   0000007c006a0900000000000000007c006a0a0000000000000000640c9c
                   0b5300
-               286           0 RESUME                   0
+               296           0 RESUME                   0
                
-               287           2 LOAD_FAST                1 (dict)
+               297           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE   184 (to 374)
                
-               288           6 LOAD_FAST                1 (dict)
+               298           6 LOAD_FAST                1 (dict)
                              8 LOAD_CONST               1 ('button_radius')
                             10 BINARY_SUBSCR
                             20 LOAD_FAST                0 (self)
                             22 STORE_ATTR               0 (button_radius)
                
-               290          32 LOAD_FAST                1 (dict)
+               300          32 LOAD_FAST                1 (dict)
                             34 LOAD_CONST               2 ('button_border_width')
                             36 BINARY_SUBSCR
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               1 (button_border_width)
                
-               292          58 LOAD_FAST                1 (dict)
+               302          58 LOAD_FAST                1 (dict)
                             60 LOAD_CONST               3 ('button_border')
                             62 BINARY_SUBSCR
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (button_border)
                
-               293          84 LOAD_FAST                1 (dict)
+               303          84 LOAD_FAST                1 (dict)
                             86 LOAD_CONST               4 ('button_back')
                             88 BINARY_SUBSCR
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               3 (button_back)
                
-               294         110 LOAD_FAST                1 (dict)
+               304         110 LOAD_FAST                1 (dict)
                            112 LOAD_CONST               5 ('button_text_back')
                            114 BINARY_SUBSCR
                            124 LOAD_FAST                0 (self)
                            126 STORE_ATTR               4 (button_text_back)
                
-               296         136 LOAD_FAST                1 (dict)
+               306         136 LOAD_FAST                1 (dict)
                            138 LOAD_CONST               6 ('button_active_border')
                            140 BINARY_SUBSCR
                            150 LOAD_FAST                0 (self)
                            152 STORE_ATTR               5 (button_active_border)
                
-               297         162 LOAD_FAST                1 (dict)
+               307         162 LOAD_FAST                1 (dict)
                            164 LOAD_CONST               7 ('button_active_back')
                            166 BINARY_SUBSCR
                            176 LOAD_FAST                0 (self)
                            178 STORE_ATTR               6 (button_active_back)
                
-               298         188 LOAD_FAST                1 (dict)
+               308         188 LOAD_FAST                1 (dict)
                            190 LOAD_CONST               8 ('button_active_text_back')
                            192 BINARY_SUBSCR
                            202 LOAD_FAST                0 (self)
                            204 STORE_ATTR               7 (button_active_text_back)
                
-               300         214 LOAD_FAST                1 (dict)
+               310         214 LOAD_FAST                1 (dict)
                            216 LOAD_CONST               9 ('button_pressed_border')
                            218 BINARY_SUBSCR
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (button_pressed_border)
                
-               301         240 LOAD_FAST                1 (dict)
+               311         240 LOAD_FAST                1 (dict)
                            242 LOAD_CONST              10 ('button_pressed_back')
                            244 BINARY_SUBSCR
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (button_pressed_back)
                
-               302         266 LOAD_FAST                1 (dict)
+               312         266 LOAD_FAST                1 (dict)
                            268 LOAD_CONST              11 ('button_pressed_text_back')
                            270 BINARY_SUBSCR
                            280 LOAD_FAST                0 (self)
                            282 STORE_ATTR              10 (button_pressed_text_back)
                
-               304         292 NOP
+               314         292 NOP
                
-               305         294 LOAD_FAST                0 (self)
+               315         294 LOAD_FAST                0 (self)
                            296 LOAD_METHOD             11 (_draw)
                            318 LOAD_CONST               0 (None)
                            320 PRECALL                  1
                            324 CALL                     1
                            334 POP_TOP
                            336 LOAD_CONST               0 (None)
                            338 RETURN_VALUE
                        >>  340 PUSH_EXC_INFO
                
-               306         342 LOAD_GLOBAL             24 (AttributeError)
+               316         342 LOAD_GLOBAL             24 (AttributeError)
                            354 CHECK_EXC_MATCH
                            356 POP_JUMP_FORWARD_IF_FALSE     4 (to 366)
                            358 POP_TOP
                
-               307         360 POP_EXCEPT
+               317         360 POP_EXCEPT
                            362 LOAD_CONST               0 (None)
                            364 RETURN_VALUE
                
-               306     >>  366 RERAISE                  0
+               316     >>  366 RERAISE                  0
                        >>  368 COPY                     3
                            370 POP_EXCEPT
                            372 RERAISE                  1
                
-               310     >>  374 LOAD_FAST                0 (self)
+               320     >>  374 LOAD_FAST                0 (self)
                            376 LOAD_ATTR               13 (button_frame_back)
                
-               312         386 LOAD_FAST                0 (self)
+               322         386 LOAD_FAST                0 (self)
                            388 LOAD_ATTR                1 (button_border_width)
                
-               314         398 LOAD_FAST                0 (self)
+               324         398 LOAD_FAST                0 (self)
                            400 LOAD_ATTR                2 (button_border)
                
-               315         410 LOAD_FAST                0 (self)
+               325         410 LOAD_FAST                0 (self)
                            412 LOAD_ATTR                3 (button_back)
                
-               316         422 LOAD_FAST                0 (self)
+               326         422 LOAD_FAST                0 (self)
                            424 LOAD_ATTR                4 (button_text_back)
                
-               318         434 LOAD_FAST                0 (self)
+               328         434 LOAD_FAST                0 (self)
                            436 LOAD_ATTR                5 (button_active_border)
                
-               319         446 LOAD_FAST                0 (self)
+               329         446 LOAD_FAST                0 (self)
                            448 LOAD_ATTR                6 (button_active_back)
                
-               320         458 LOAD_FAST                0 (self)
+               330         458 LOAD_FAST                0 (self)
                            460 LOAD_ATTR                7 (button_active_text_back)
                
-               322         470 LOAD_FAST                0 (self)
+               332         470 LOAD_FAST                0 (self)
                            472 LOAD_ATTR                8 (button_pressed_border)
                
-               323         482 LOAD_FAST                0 (self)
+               333         482 LOAD_FAST                0 (self)
                            484 LOAD_ATTR                9 (button_pressed_back)
                
-               324         494 LOAD_FAST                0 (self)
+               334         494 LOAD_FAST                0 (self)
                            496 LOAD_ATTR               10 (button_pressed_text_back)
                
-               309         506 LOAD_CONST              12 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
+               319         506 LOAD_CONST              12 (('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
                            508 BUILD_CONST_KEY_MAP     11
                            510 RETURN_VALUE
                ExceptionTable:
                  294 to 334 -> 340 [0]
                  340 to 358 -> 368 [1] lasti
                  366 to 366 -> 368 [1] lasti
                consts
@@ -2289,97 +2418,97 @@
                   ('button_frame_back', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
                names      ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back', '_draw', 'AttributeError', 'button_frame_back')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'palette'
-               firstlineno 286
+               firstlineno 296
                lnotab
                   0x020104011a021a021a011a011a021a011a011a021a011a011a02020130
                   01120106ff08040c020c020c010c010c020c010c010c020c010c010cf1
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'float', 'int', 'border_radius', '_draw', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawBasicRoundButton'
-         firstlineno 213
+         firstlineno 223
          lnotab 0x0c010a0306031406060f060306150615
       'AdwDrawBasicRoundButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         328           0 RESUME                   0
+         338           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         329          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 329>)
+         339          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 339>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               329           0 RESUME                   0
+               339           0 RESUME                   0
                
-               330           2 LOAD_FAST                0 (self)
+               340           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 329
+               firstlineno 339
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundButton'
-         firstlineno 328
+         firstlineno 338
          lnotab 0x0a01
       'AdwDrawRoundButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         333           0 RESUME                   0
+         343           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundAccentButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         334          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 334>)
+         344          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 344>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundAccentButton'
             code
@@ -2387,45 +2516,45 @@
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564036406640564076407640864099c0ba6010000ab0100
                   00000000000000010064005300
-               334           0 RESUME                   0
+               344           0 RESUME                   0
                
-               335           2 LOAD_FAST                0 (self)
+               345           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               337          26 LOAD_CONST               1 (8)
+               347          26 LOAD_CONST               1 (8)
                
-               339          28 LOAD_CONST               2 (1)
+               349          28 LOAD_CONST               2 (1)
                
-               341          30 LOAD_CONST               3 ('#1473c5')
+               351          30 LOAD_CONST               3 ('#1473c5')
                
-               342          32 LOAD_CONST               4 ('#0067c0')
+               352          32 LOAD_CONST               4 ('#0067c0')
                
-               343          34 LOAD_CONST               5 ('#ffffff')
+               353          34 LOAD_CONST               5 ('#ffffff')
                
-               345          36 LOAD_CONST               3 ('#1473c5')
+               355          36 LOAD_CONST               3 ('#1473c5')
                
-               346          38 LOAD_CONST               6 ('#1975c5')
+               356          38 LOAD_CONST               6 ('#1975c5')
                
-               347          40 LOAD_CONST               5 ('#ffffff')
+               357          40 LOAD_CONST               5 ('#ffffff')
                
-               349          42 LOAD_CONST               7 ('#3284cb')
+               359          42 LOAD_CONST               7 ('#3284cb')
                
-               350          44 LOAD_CONST               7 ('#3284cb')
+               360          44 LOAD_CONST               7 ('#3284cb')
                
-               351          46 LOAD_CONST               8 ('#fdfdfd')
+               361          46 LOAD_CONST               8 ('#fdfdfd')
                
-               336          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
+               346          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
                             50 BUILD_CONST_KEY_MAP     11
                
-               335          52 PRECALL                  1
+               345          52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
                             68 LOAD_CONST               0 (None)
                             70 RETURN_VALUE
                consts
                   None
                   8
@@ -2439,99 +2568,99 @@
                   ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 334
+               firstlineno 344
                lnotab 0x02011802020202020201020102020201020102020201020102f104ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundAccentButton'
-         firstlineno 333
+         firstlineno 343
          lnotab 0x0a01
       'AdwDrawRoundAccentButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         356           0 RESUME                   0
+         366           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         357          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 357>)
+         367          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 367>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               357           0 RESUME                   0
+               367           0 RESUME                   0
                
-               358           2 LOAD_FAST                0 (self)
+               368           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 357
+               firstlineno 367
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundDarkButton'
-         firstlineno 356
+         firstlineno 366
          lnotab 0x0a01
       'AdwDrawRoundDarkButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a03640284005a0464035300
-         361           0 RESUME                   0
+         371           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundButton2')
                        8 STORE_NAME               2 (__qualname__)
          
-         362          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 362>)
+         372          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 372>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (_draw)
          
-         379          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 379>)
+         389          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 389>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (default_palette)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'AdwDrawRoundButton2'
             code
@@ -2550,29 +2679,29 @@
                   0000000000010064027c005f0700000000000000007c00a0080000000000
                   0000000000000000000000000000007c00a0020000000000000000000000
                   000000000000000000a6000000ab00000000000000000064037a0b00007c
                   00a0030000000000000000000000000000000000000000a6000000ab0000
                   0000000000000064037a0b00007c006a0900000000000000007c006a0a00
                   000000000000007c006a0b0000000000000000ac06a6050000ab05000000
                   00000000007c005f0c000000000000000064005300
-               362           0 RESUME                   0
+               372           0 RESUME                   0
                
-               363           2 LOAD_FAST                0 (self)
+               373           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               365          44 LOAD_FAST                0 (self)
+               375          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect3)
                
-               366          68 LOAD_CONST               2 ('button_frame')
+               376          68 LOAD_CONST               2 ('button_frame')
                
-               367          70 LOAD_CONST               3 (2)
+               377          70 LOAD_CONST               3 (2)
                             72 LOAD_CONST               3 (2)
                             74 LOAD_FAST                0 (self)
                             76 LOAD_METHOD              2 (winfo_width)
                             98 PRECALL                  0
                            102 CALL                     0
                            112 LOAD_CONST               4 (3)
                            114 BINARY_OP               10 (-)
@@ -2581,53 +2710,53 @@
                            142 PRECALL                  0
                            146 CALL                     0
                            156 LOAD_CONST               4 (3)
                            158 BINARY_OP               10 (-)
                            162 LOAD_FAST                0 (self)
                            164 LOAD_ATTR                4 (button_radius)
                
-               368         174 LOAD_FAST                0 (self)
+               378         174 LOAD_FAST                0 (self)
                            176 LOAD_ATTR                5 (_button_border)
                            186 LOAD_FAST                0 (self)
                            188 LOAD_ATTR                6 (_button_back)
                
-               365         198 KW_NAMES                 5
+               375         198 KW_NAMES                 5
                            200 PRECALL                  8
                            204 CALL                     8
                            214 POP_TOP
                
-               371         216 LOAD_CONST               2 ('button_frame')
+               381         216 LOAD_CONST               2 ('button_frame')
                            218 LOAD_FAST                0 (self)
                            220 STORE_ATTR               7 (button_frame)
                
-               373         230 LOAD_FAST                0 (self)
+               383         230 LOAD_FAST                0 (self)
                            232 LOAD_METHOD              8 (create_text)
                
-               374         254 LOAD_FAST                0 (self)
+               384         254 LOAD_FAST                0 (self)
                            256 LOAD_METHOD              2 (winfo_width)
                            278 PRECALL                  0
                            282 CALL                     0
                            292 LOAD_CONST               3 (2)
                            294 BINARY_OP               11 (/)
                            298 LOAD_FAST                0 (self)
                            300 LOAD_METHOD              3 (winfo_height)
                            322 PRECALL                  0
                            326 CALL                     0
                            336 LOAD_CONST               3 (2)
                            338 BINARY_OP               11 (/)
                
-               375         342 LOAD_FAST                0 (self)
+               385         342 LOAD_FAST                0 (self)
                            344 LOAD_ATTR                9 (text)
                            354 LOAD_FAST                0 (self)
                            356 LOAD_ATTR               10 (_button_text_back)
                
-               376         366 LOAD_FAST                0 (self)
+               386         366 LOAD_FAST                0 (self)
                            368 LOAD_ATTR               11 (button_text_font)
                
-               373         378 KW_NAMES                 6
+               383         378 KW_NAMES                 6
                            380 PRECALL                  5
                            384 CALL                     5
                            394 LOAD_FAST                0 (self)
                            396 STORE_ATTR              12 (button_text)
                            406 LOAD_CONST               0 (None)
                            408 RETURN_VALUE
                consts
@@ -2640,66 +2769,66 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_round_rect3', 'winfo_width', 'winfo_height', 'button_radius', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_draw'
-               firstlineno 362
+               firstlineno 372
                lnotab 0x02012a0218010201680118fd12060e021801580118010cfd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               379           0 RESUME                   0
+               389           0 RESUME                   0
                
-               380           2 LOAD_FAST                0 (self)
+               390           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 379
+               firstlineno 389
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '_draw', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundButton2'
-         firstlineno 361
+         firstlineno 371
          lnotab 0x0a010611
       'AdwDrawRoundButton2'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         383           0 RESUME                   0
+         393           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundAccentButton2')
                        8 STORE_NAME               2 (__qualname__)
          
-         384          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 384>)
+         394          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 394>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundAccentButton2'
             code
@@ -2707,45 +2836,45 @@
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564036406640564076407640864099c0ba6010000ab0100
                   00000000000000010064005300
-               384           0 RESUME                   0
+               394           0 RESUME                   0
                
-               385           2 LOAD_FAST                0 (self)
+               395           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               387          26 LOAD_CONST               1 (8)
+               397          26 LOAD_CONST               1 (8)
                
-               389          28 LOAD_CONST               2 (1)
+               399          28 LOAD_CONST               2 (1)
                
-               391          30 LOAD_CONST               3 ('#1473c5')
+               401          30 LOAD_CONST               3 ('#1473c5')
                
-               392          32 LOAD_CONST               4 ('#0067c0')
+               402          32 LOAD_CONST               4 ('#0067c0')
                
-               393          34 LOAD_CONST               5 ('#ffffff')
+               403          34 LOAD_CONST               5 ('#ffffff')
                
-               395          36 LOAD_CONST               3 ('#1473c5')
+               405          36 LOAD_CONST               3 ('#1473c5')
                
-               396          38 LOAD_CONST               6 ('#1975c5')
+               406          38 LOAD_CONST               6 ('#1975c5')
                
-               397          40 LOAD_CONST               5 ('#ffffff')
+               407          40 LOAD_CONST               5 ('#ffffff')
                
-               399          42 LOAD_CONST               7 ('#3284cb')
+               409          42 LOAD_CONST               7 ('#3284cb')
                
-               400          44 LOAD_CONST               7 ('#3284cb')
+               410          44 LOAD_CONST               7 ('#3284cb')
                
-               401          46 LOAD_CONST               8 ('#fdfdfd')
+               411          46 LOAD_CONST               8 ('#fdfdfd')
                
-               386          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
+               396          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
                             50 BUILD_CONST_KEY_MAP     11
                
-               385          52 PRECALL                  1
+               395          52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
                             68 LOAD_CONST               0 (None)
                             70 RETURN_VALUE
                consts
                   None
                   8
@@ -2759,99 +2888,99 @@
                   ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 384
+               firstlineno 394
                lnotab 0x02011802020202020201020102020201020102020201020102f104ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundAccentButton2'
-         firstlineno 383
+         firstlineno 393
          lnotab 0x0a01
       'AdwDrawRoundAccentButton2'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         406           0 RESUME                   0
+         416           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkButton2')
                        8 STORE_NAME               2 (__qualname__)
          
-         407          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 407>)
+         417          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 417>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkButton2'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               407           0 RESUME                   0
+               417           0 RESUME                   0
                
-               408           2 LOAD_FAST                0 (self)
+               418           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 407
+               firstlineno 417
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundDarkButton2'
-         firstlineno 406
+         firstlineno 416
          lnotab 0x0a01
       'AdwDrawRoundDarkButton2'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a03640284005a0464035300
-         411           0 RESUME                   0
+         421           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundButton3')
                        8 STORE_NAME               2 (__qualname__)
          
-         412          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 412>)
+         422          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 422>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (_draw)
          
-         429          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 429>)
+         439          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 439>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (default_palette)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'AdwDrawRoundButton3'
             code
@@ -2873,27 +3002,27 @@
                   00000000007c00a00900000000000000000000000000000000000000007c
                   00a0030000000000000000000000000000000000000000a6000000ab0000
                   0000000000000064037a0b00007c00a00400000000000000000000000000
                   00000000000000a6000000ab00000000000000000064037a0b00007c006a
                   0a00000000000000007c006a0b00000000000000007c006a0c0000000000
                   000000ac06a6050000ab0500000000000000007c005f0d00000000000000
                   0064005300
-               412           0 RESUME                   0
+               422           0 RESUME                   0
                
-               413           2 LOAD_FAST                0 (self)
+               423           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               415          44 LOAD_FAST                0 (self)
+               425          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
-               416          68 LOAD_FAST                0 (self)
+               426          68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                2 (button_border_width)
                             80 LOAD_CONST               2 (1)
                             82 BINARY_OP                0 (+)
                             86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                2 (button_border_width)
                             98 LOAD_CONST               2 (1)
                            100 BINARY_OP                0 (+)
@@ -2914,56 +3043,56 @@
                            204 LOAD_ATTR                2 (button_border_width)
                            214 BINARY_OP               10 (-)
                            218 LOAD_CONST               3 (2)
                            220 BINARY_OP               10 (-)
                            224 LOAD_FAST                0 (self)
                            226 LOAD_ATTR                5 (button_radius)
                
-               417         236 LOAD_FAST                0 (self)
+               427         236 LOAD_FAST                0 (self)
                            238 LOAD_ATTR                2 (button_border_width)
                
-               418         248 LOAD_FAST                0 (self)
+               428         248 LOAD_FAST                0 (self)
                            250 LOAD_ATTR                6 (_button_border)
                            260 LOAD_FAST                0 (self)
                            262 LOAD_ATTR                7 (_button_back)
                
-               415         272 KW_NAMES                 4
+               425         272 KW_NAMES                 4
                            274 PRECALL                  8
                            278 CALL                     8
                            288 POP_TOP
                
-               421         290 LOAD_CONST               5 ('button_frame')
+               431         290 LOAD_CONST               5 ('button_frame')
                            292 LOAD_FAST                0 (self)
                            294 STORE_ATTR               8 (button_frame)
                
-               423         304 LOAD_FAST                0 (self)
+               433         304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              9 (create_text)
                
-               424         328 LOAD_FAST                0 (self)
+               434         328 LOAD_FAST                0 (self)
                            330 LOAD_METHOD              3 (winfo_width)
                            352 PRECALL                  0
                            356 CALL                     0
                            366 LOAD_CONST               3 (2)
                            368 BINARY_OP               11 (/)
                            372 LOAD_FAST                0 (self)
                            374 LOAD_METHOD              4 (winfo_height)
                            396 PRECALL                  0
                            400 CALL                     0
                            410 LOAD_CONST               3 (2)
                            412 BINARY_OP               11 (/)
                
-               425         416 LOAD_FAST                0 (self)
+               435         416 LOAD_FAST                0 (self)
                            418 LOAD_ATTR               10 (text)
                            428 LOAD_FAST                0 (self)
                            430 LOAD_ATTR               11 (_button_text_back)
                
-               426         440 LOAD_FAST                0 (self)
+               436         440 LOAD_FAST                0 (self)
                            442 LOAD_ATTR               12 (button_text_font)
                
-               423         452 KW_NAMES                 6
+               433         452 KW_NAMES                 6
                            454 PRECALL                  5
                            458 CALL                     5
                            468 LOAD_FAST                0 (self)
                            470 STORE_ATTR              13 (button_text)
                            480 LOAD_CONST               0 (None)
                            482 RETURN_VALUE
                consts
@@ -2976,66 +3105,66 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_round_rect4', 'button_border_width', 'winfo_width', 'winfo_height', 'button_radius', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_draw'
-               firstlineno 412
+               firstlineno 422
                lnotab 0x02012a021801a8010c0118fd12060e021801580118010cfd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               429           0 RESUME                   0
+               439           0 RESUME                   0
                
-               430           2 LOAD_FAST                0 (self)
+               440           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 429
+               firstlineno 439
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '_draw', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundButton3'
-         firstlineno 411
+         firstlineno 421
          lnotab 0x0a010611
       'AdwDrawRoundButton3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         433           0 RESUME                   0
+         443           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundAccentButton3')
                        8 STORE_NAME               2 (__qualname__)
          
-         434          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 434>)
+         444          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 444>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundAccentButton3'
             code
@@ -3043,45 +3172,45 @@
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564036406640564076407640864099c0ba6010000ab0100
                   00000000000000010064005300
-               434           0 RESUME                   0
+               444           0 RESUME                   0
                
-               435           2 LOAD_FAST                0 (self)
+               445           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               437          26 LOAD_CONST               1 (8)
+               447          26 LOAD_CONST               1 (8)
                
-               439          28 LOAD_CONST               2 (1)
+               449          28 LOAD_CONST               2 (1)
                
-               441          30 LOAD_CONST               3 ('#1473c5')
+               451          30 LOAD_CONST               3 ('#1473c5')
                
-               442          32 LOAD_CONST               4 ('#0067c0')
+               452          32 LOAD_CONST               4 ('#0067c0')
                
-               443          34 LOAD_CONST               5 ('#ffffff')
+               453          34 LOAD_CONST               5 ('#ffffff')
                
-               445          36 LOAD_CONST               3 ('#1473c5')
+               455          36 LOAD_CONST               3 ('#1473c5')
                
-               446          38 LOAD_CONST               6 ('#1975c5')
+               456          38 LOAD_CONST               6 ('#1975c5')
                
-               447          40 LOAD_CONST               5 ('#ffffff')
+               457          40 LOAD_CONST               5 ('#ffffff')
                
-               449          42 LOAD_CONST               7 ('#3284cb')
+               459          42 LOAD_CONST               7 ('#3284cb')
                
-               450          44 LOAD_CONST               7 ('#3284cb')
+               460          44 LOAD_CONST               7 ('#3284cb')
                
-               451          46 LOAD_CONST               8 ('#fdfdfd')
+               461          46 LOAD_CONST               8 ('#fdfdfd')
                
-               436          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
+               446          48 LOAD_CONST               9 (('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back'))
                             50 BUILD_CONST_KEY_MAP     11
                
-               435          52 PRECALL                  1
+               445          52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
                             68 LOAD_CONST               0 (None)
                             70 RETURN_VALUE
                consts
                   None
                   8
@@ -3095,109 +3224,109 @@
                   ('button_radius', 'button_border_width', 'button_border', 'button_back', 'button_text_back', 'button_active_border', 'button_active_back', 'button_active_text_back', 'button_pressed_border', 'button_pressed_back', 'button_pressed_text_back')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 434
+               firstlineno 444
                lnotab 0x02011802020202020201020102020201020102020201020102f104ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundAccentButton3'
-         firstlineno 433
+         firstlineno 443
          lnotab 0x0a01
       'AdwDrawRoundAccentButton3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         456           0 RESUME                   0
+         466           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkButton3')
                        8 STORE_NAME               2 (__qualname__)
          
-         457          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 457>)
+         467          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 467>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkButton3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               457           0 RESUME                   0
+               467           0 RESUME                   0
                
-               458           2 LOAD_FAST                0 (self)
+               468           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 457
+               firstlineno 467
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawRoundDarkButton3'
-         firstlineno 456
+         firstlineno 466
          lnotab 0x0a01
       'AdwDrawRoundDarkButton3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a026401640164029c02880066016403840a5a
             03640484005a04880078015a055300
                        0 MAKE_CELL                0 (__class__)
          
-         462           2 RESUME                   0
+         472           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicCircularButton')
                       10 STORE_NAME               2 (__qualname__)
          
-         463          12 LOAD_CONST               1 (120)
+         473          12 LOAD_CONST               1 (120)
                       14 LOAD_CONST               1 (120)
                       16 LOAD_CONST               2 (('width', 'height'))
                       18 BUILD_CONST_KEY_MAP      2
                       20 LOAD_CLOSURE             0 (__class__)
                       22 BUILD_TUPLE              1
-                      24 LOAD_CONST               3 (<code object __init__, file "D:\tkadw\tkadw\canvas\button.py", line 463>)
+                      24 LOAD_CONST               3 (<code object __init__, file "D:\tkadw\tkadw\canvas\button.py", line 473>)
                       26 MAKE_FUNCTION           10 (kwdefaults, closure)
                       28 STORE_NAME               3 (__init__)
          
-         466          30 LOAD_CONST               4 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 466>)
+         476          30 LOAD_CONST               4 (<code object _draw, file "D:\tkadw\tkadw\canvas\button.py", line 476>)
                       32 MAKE_FUNCTION            0
                       34 STORE_NAME               4 (_draw)
                       36 LOAD_CLOSURE             0 (__class__)
                       38 COPY                     1
                       40 STORE_NAME               5 (__classcell__)
                       42 RETURN_VALUE
          consts
@@ -3211,17 +3340,17 @@
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c037c017c0264019c027c04a4018e0101
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               463           2 RESUME                   0
+               473           2 RESUME                   0
                
-               464           4 PUSH_NULL
+               474           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                3 (args)
                             44 LOAD_FAST                1 (width)
                             46 LOAD_FAST                2 (height)
@@ -3238,15 +3367,15 @@
                   ('width', 'height')
                names      ('super', '__init__')
                varnames   ('self', 'width', 'height', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '__init__'
-               firstlineno 463
+               firstlineno 473
                lnotab 0x0401
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 9
                flags     : 3
                code
@@ -3260,80 +3389,80 @@
                   0000007c005f0700000000000000007c00a0080000000000000000000000
                   0000000000000000007c00a0020000000000000000000000000000000000
                   000000a6000000ab00000000000000000064057a0b00007c00a003000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0064057a0b00007c006a0900000000000000007c006a0a00000000000000
                   007c006a0b0000000000000000ac06a6050000ab0500000000000000007c
                   005f0c000000000000000064005300
-               466           0 RESUME                   0
+               476           0 RESUME                   0
                
-               467           2 LOAD_FAST                0 (self)
+               477           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               469          44 LOAD_FAST                0 (self)
+               479          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_oval)
                
-               470          68 LOAD_CONST               2 (1.5)
+               480          68 LOAD_CONST               2 (1.5)
                             70 LOAD_CONST               2 (1.5)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
                            116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                
-               471         160 LOAD_FAST                0 (self)
+               481         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (button_border_width)
                
-               472         172 LOAD_FAST                0 (self)
+               482         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (_button_border)
                            184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_button_back)
                
-               469         196 KW_NAMES                 4
+               479         196 KW_NAMES                 4
                            198 PRECALL                  7
                            202 CALL                     7
                            212 LOAD_FAST                0 (self)
                            214 STORE_ATTR               7 (button_frame)
                
-               475         224 LOAD_FAST                0 (self)
+               485         224 LOAD_FAST                0 (self)
                            226 LOAD_METHOD              8 (create_text)
                
-               476         248 LOAD_FAST                0 (self)
+               486         248 LOAD_FAST                0 (self)
                            250 LOAD_METHOD              2 (winfo_width)
                            272 PRECALL                  0
                            276 CALL                     0
                            286 LOAD_CONST               5 (2)
                            288 BINARY_OP               11 (/)
                            292 LOAD_FAST                0 (self)
                            294 LOAD_METHOD              3 (winfo_height)
                            316 PRECALL                  0
                            320 CALL                     0
                            330 LOAD_CONST               5 (2)
                            332 BINARY_OP               11 (/)
                
-               477         336 LOAD_FAST                0 (self)
+               487         336 LOAD_FAST                0 (self)
                            338 LOAD_ATTR                9 (text)
                            348 LOAD_FAST                0 (self)
                            350 LOAD_ATTR               10 (_button_text_back)
                
-               478         360 LOAD_FAST                0 (self)
+               488         360 LOAD_FAST                0 (self)
                            362 LOAD_ATTR               11 (button_text_font)
                
-               475         372 KW_NAMES                 6
+               485         372 KW_NAMES                 6
                            374 PRECALL                  5
                            378 CALL                     5
                            388 LOAD_FAST                0 (self)
                            390 STORE_ATTR              12 (button_text)
                            400 LOAD_CONST               0 (None)
                            402 RETURN_VALUE
                consts
@@ -3346,135 +3475,135 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_oval', 'winfo_width', 'winfo_height', 'button_border_width', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       '_draw'
-               firstlineno 466
+               firstlineno 476
                lnotab 0x02012a0218015c010c0118fd1c061801580118010cfd
          names      ('__name__', '__module__', '__qualname__', '__init__', '_draw', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawBasicCircularButton'
-         firstlineno 462
+         firstlineno 472
          lnotab 0x0c011203
       'AdwDrawBasicCircularButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         482           0 RESUME                   0
+         492           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawCircularButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         483          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 483>)
+         493          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 493>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawCircularButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               483           0 RESUME                   0
+               493           0 RESUME                   0
                
-               484           2 LOAD_FAST                0 (self)
+               494           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 483
+               firstlineno 493
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawCircularButton'
-         firstlineno 482
+         firstlineno 492
          lnotab 0x0a01
       'AdwDrawCircularButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         487           0 RESUME                   0
+         497           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawCircularDarkButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         488          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 488>)
+         498          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\button.py", line 498>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawCircularDarkButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               488           0 RESUME                   0
+               498           0 RESUME                   0
                
-               489           2 LOAD_FAST                0 (self)
+               499           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 488
+               firstlineno 498
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       'AdwDrawCircularDarkButton'
-         firstlineno 487
+         firstlineno 497
          lnotab 0x0a01
       'AdwDrawCircularDarkButton'
       '__main__'
       ('Tk',)
       'Hello'
       ('text',)
       '<<Click>>'
@@ -3482,139 +3611,139 @@
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         498           0 RESUME                   0
+         508           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 498
+         firstlineno 508
          lnotab 0x
       'x'
       5
       ('fill', 'padx', 'pady')
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         502           0 RESUME                   0
+         512           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 502
+         firstlineno 512
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         506           0 RESUME                   0
+         516           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 506
+         firstlineno 516
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         510           0 RESUME                   0
+         520           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 510
+         firstlineno 520
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         514           0 RESUME                   0
+         524           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button6 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button6 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 514
+         firstlineno 524
          lnotab 0x
       None
    names      ('tkinter.font', 'Font', 'nametofont', 'tkadw.canvas.drawengine', 'AdwDrawEngine', 'AdwDrawBasicButton', 'AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawBasicRoundButton', 'AdwDrawRoundButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawBasicCircularButton', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton', '__name__', 'tkinter', 'Tk', 'root', 'button', 'bind', 'pack', 'button4', 'button7', 'button10', 'button13', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\canvas\\button.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c041c7f002e1c051c051c181c731c051c171c051c161c
+      0x00ff020110010c041c7f00381c051c051c181c731c051c171c051c161c
       171c051c161c171c061c141c051c050e010c02140218012e01300218012e
       01300218012e01300218012e01300218012e0130022ce7
```

### Comparing `tkadw-0.1.1/tkadw/canvas/__pycache__/button.cpython-38.pyc` & `tkadw-0.1.2/tkadw/canvas/__pycache__/button.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc` & `tkadw-0.1.2/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xc05a8464 (Sat Jun 10 11:13:04 2023 UTC)
-files sz: 20295
+moddate:  0x04289564 (Fri Jun 23 05:05:08 2023 UTC)
+files sz: 20382
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a01010064025a0264035a0302004700640484
@@ -40,198 +40,244 @@
                 28 MAKE_FUNCTION            0
                 30 LOAD_CONST               5 ('AdwDrawEngine')
                 32 LOAD_NAME                1 (Canvas)
                 34 PRECALL                  3
                 38 CALL                     3
                 48 STORE_NAME               4 (AdwDrawEngine)
    
-   580          50 LOAD_NAME                5 (__name__)
+   583          50 LOAD_NAME                5 (__name__)
                 52 LOAD_CONST               6 ('__main__')
                 54 COMPARE_OP               2 (==)
                 60 POP_JUMP_FORWARD_IF_FALSE   145 (to 352)
    
-   581          62 LOAD_CONST               0 (0)
+   584          62 LOAD_CONST               0 (0)
                 64 LOAD_CONST               7 (('Tk',))
                 66 IMPORT_NAME              0 (tkinter)
                 68 IMPORT_FROM              6 (Tk)
                 70 STORE_NAME               6 (Tk)
                 72 POP_TOP
    
-   583          74 PUSH_NULL
+   586          74 PUSH_NULL
                 76 LOAD_NAME                6 (Tk)
                 78 PRECALL                  0
                 82 CALL                     0
                 92 STORE_NAME               7 (root)
    
-   585          94 PUSH_NULL
+   588          94 PUSH_NULL
                 96 LOAD_NAME                4 (AdwDrawEngine)
                 98 PRECALL                  0
                102 CALL                     0
                112 STORE_NAME               8 (canvas)
    
-   587         114 LOAD_NAME                8 (canvas)
+   590         114 LOAD_NAME                8 (canvas)
                116 LOAD_METHOD              9 (create_round_rect3)
                138 LOAD_CONST               8 (10)
                140 LOAD_CONST               9 (15)
                142 LOAD_CONST               9 (15)
                144 LOAD_CONST              10 (150)
                146 LOAD_CONST              10 (150)
                148 LOAD_CONST              11 (50)
                150 PRECALL                  6
                154 CALL                     6
                164 POP_TOP
    
-   588         166 LOAD_NAME                8 (canvas)
+   591         166 LOAD_NAME                8 (canvas)
                168 LOAD_METHOD             10 (create_round_rect4)
                190 LOAD_CONST              12 (160)
                192 LOAD_CONST              12 (160)
                194 LOAD_CONST              13 (300)
                196 LOAD_CONST              13 (300)
                198 LOAD_CONST              11 (50)
                200 PRECALL                  5
                204 CALL                     5
                214 POP_TOP
    
-   590         216 LOAD_NAME                8 (canvas)
+   593         216 LOAD_NAME                8 (canvas)
                218 LOAD_METHOD             11 (bind)
                240 LOAD_CONST              14 ('<Configure>')
-               242 LOAD_CONST              15 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\drawengine.py", line 590>)
+               242 LOAD_CONST              15 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\drawengine.py", line 593>)
                244 MAKE_FUNCTION            0
                246 PRECALL                  2
                250 CALL                     2
                260 POP_TOP
    
-   592         262 LOAD_NAME                8 (canvas)
+   595         262 LOAD_NAME                8 (canvas)
                264 LOAD_METHOD             12 (pack)
                286 LOAD_CONST              16 ('both')
                288 LOAD_CONST              17 ('yes')
                290 KW_NAMES                18
                292 PRECALL                  2
                296 CALL                     2
                306 POP_TOP
    
-   594         308 LOAD_NAME                7 (root)
+   597         308 LOAD_NAME                7 (root)
                310 LOAD_METHOD             13 (mainloop)
                332 PRECALL                  0
                336 CALL                     0
                346 POP_TOP
                348 LOAD_CONST              19 (None)
                350 RETURN_VALUE
    
-   580     >>  352 LOAD_CONST              19 (None)
+   583     >>  352 LOAD_CONST              19 (None)
                354 RETURN_VALUE
    consts
       0
       ('Canvas',)
       '\n# poly.tcl\n\nproc poly_round {win outline fill args} {\n    if {[llength $args] % 3 != 0 || [llength $args] < 9} {\n        error "wrong # args: should be "poly_round                win outline fill x1 y1 d1 x2 y2 d2 x3 y3 d3 ?...?""\n    }\n\n    # Determine the tag to use.\n    if {![info exists ::poly_next_id]} {\n        set ::poly_next_id 1\n    }\n    set tag poly#$::poly_next_id\n    incr ::poly_next_id\n\n    # Filter out illegal circles and collinear points.\n    set pts [list]\n    lassign [lrange $args 0 4] Ux Uy d Vx Vy\n    foreach {d Wx Wy} [concat [lrange $args 5 end] [lrange $args 0 4]] {\n        set test [expr {$Ux * ($Vy - $Wy) - $Vx * ($Uy - $Wy) +\n                $Wx * ($Uy - $Vy)}]\n        if {($d > 0) && $test != 0} {\n            lappend pts $Vx $Vy $d $test\n            lassign [list $Wx $Wy $Vx $Vy] Vx Vy Ux Uy\n        } else {\n            lassign [list $Wx $Wy] Vx Vy\n        }\n    }\n\n    # V    C    T   W\n    #  *---*----*-+-*-- Given: U, V, W, d\n    #  |\\ /    /|_|     Find:  S, E, T\n    #  | *B   / |\n    #  |/ \\  /  |       The length of ES and ET each is d.\n    # A*   \\/   |\n    #  |   /\\   |       VB bisects angle UVW.  SE _|_ VU; TE _|_ VW.\n    #  |  /  \\  |       B is halfway between A and C.\n    #  | /    \\ |       Angles UVW and SET are not necessarily right.\n    #  |/      \\|       The length of AV and CV each is 1.\n    # S*-+------*E\n    #  |_|       \\      The new polygon is along USTW.\n    # U*          \\     The new arc has center E, radius d, and angle SET, and\n    #  |           \\    it is tangential to VU at S and VW at T.\n\n    # Calculate new polygon vertices and create arcs.\n    set coords [list]\n    lassign [lrange $pts 0 5] Ux Uy d test Vx Vy\n    foreach {d test Wx Wy} [concat [lrange $pts 6 end] [lrange $pts 0 5]] {\n        # Find A and C.\n        foreach {pt x y} [list A $Ux $Uy C $Wx $Wy] {\n            set      k [expr {sqrt(($Vx - $x) ** 2 + ($Vy - $y) ** 2)}]\n            set ${pt}x [expr {($x - $Vx) / $k + $Vx}]\n            set ${pt}y [expr {($y - $Vy) / $k + $Vy}]\n        }\n\n        # Find B.\n        set Bx [expr {($Ax + $Cx) / 2.0}]\n        set By [expr {($Ay + $Cy) / 2.0}]\n\n        # Find the parameters for lines VB and VW.\n        foreach {pt x y} [list B $Bx $By W $Wx $Wy] {\n            set       k [expr {sqrt(($Vx - $x) ** 2 + ($Vy - $y) ** 2)}]\n            set V${pt}a [expr {+($Vy - $y) / $k}]\n            set V${pt}b [expr {-($Vx - $x) / $k}]\n            set V${pt}c [expr {($Vx * $y - $Vy * $x) / $k}]\n        }\n\n        # Find point E.\n        set sign [expr {$test < 0 ? -1 : +1}]\n        set  k [expr {$VWa * $VBb - $VWb * $VBa}]\n        set Ex [expr {(+$VWb * $VBc - ($VWc - $d * $sign) * $VBb) / $k}]\n        set Ey [expr {(-$VWa * $VBc + ($VWc - $d * $sign) * $VBa) / $k}]\n\n        # Find tangent points S and T.\n        foreach {pt x y} [list S $Ux $Uy T $Wx $Wy] {\n            set      k [expr {($Vx - $x) ** 2 + ($Vy - $y) ** 2}]\n            set ${pt}x [expr {($Ex * ($Vx - $x) ** 2 + ($Vy - $y) *\n                              ($Ey * ($Vx - $x) - $Vx * $y + $Vy * $x)) / $k}]\n            set ${pt}y [expr {($Ex * ($Vx - $x) * ($Vy - $y) +\n                              ($Ey * ($Vy - $y) ** 2 + ($Vx - $x) *\n                              ($Vx * $y - $Vy * $x))) / $k}]\n        }\n\n        # Find directions for lines ES and ET.\n        foreach {pt x y} [list S $Sx $Sy T $Tx $Ty] {\n            set E${pt}d [expr {atan2($Ey - $y, $x - $Ex)}]\n        }\n\n        # Find start and extent directions.\n        if {$ESd < 0 && $ETd > 0} {\n            set start  [expr {180 / acos(-1) * $ETd}]\n            set extent [expr {180 / acos(-1) * ($ESd - $ETd)}]\n            if {$sign > 0} {\n                set extent [expr {$extent + 360}]\n            }\n        } else {\n            set start  [expr {180 / acos(-1) * $ESd}]\n            set extent [expr {180 / acos(-1) * ($ETd - $ESd)}]\n            if {$sign < 0 && $ESd > 0 && $ETd < 0} {\n                set extent [expr {$extent + 360}]\n            }\n        }\n\n        # Draw arc.\n        set opts [list                                             [expr {$Ex - $d}] [expr {$Ey - $d}]                [expr {$Ex + $d}] [expr {$Ey + $d}]                -start $start -extent $extent]\n        $win create arc {*}$opts -style pie -tags [list $tag pie]\n        $win create arc {*}$opts -style arc -tags [list $tag arc]\n\n        # Draw border line.\n        if {[info exists prevx]} {\n            $win create line $prevx $prevy $Sx $Sy -tags [list $tag line]\n        } else {\n            lassign [list $Sx $Sy] firstx firsty\n        }\n        lassign [list $Tx $Ty] prevx prevy\n\n        # Remember coordinates for polygon.\n        lappend coords $Sx $Sy $Tx $Ty\n\n        # Rotate vertices.\n        lassign [list $Wx $Wy $Vx $Vy] Vx Vy Ux Uy\n    }\n\n    # Draw final border line.\n    $win create line $prevx $prevy $firstx $firsty -tags [list $tag line]\n\n    # Draw fill polygon.\n    $win create polygon {*}$coords -tags [list $tag poly]\n\n    # Configure colors.\n    $win itemconfigure $tag&&(poly||pie) -fill $fill\n    $win itemconfigure $tag&&pie         -outline ""\n    $win itemconfigure $tag&&line        -fill $outline -capstyle round\n    $win itemconfigure $tag&&arc         -outline $outline\n\n    # Set proper stacking order.\n    $win raise $tag&&poly\n    $win raise $tag&&pie\n    $win raise $tag&&(line||arc)\n\n    return $tag\n}\n       '
       '\n #----------------------------------------------------------------------\n #\n # RoundPoly -- Draw a polygon with rounded corners in the canvas, based\n # off of ideas and code from "Drawing rounded rectangles"\n #\n # Parameters:\n #       w - Path name of the canvas\n #       xy - list of coordinates of the vertices of the polygon\n #       radii - list of radius of the bend each each vertex\n #       args - Other args suitable to a \'polygon\' item on the canvas\n #\n # Results:\n #       Returns the canvas item number of the rounded polygon.\n #\n # Side effects:\n #       Creates a rounded polygon in the canvas.\n #\n #----------------------------------------------------------------------\n \n proc RoundPoly {w xy radii args} {\n    set lenXY [llength $xy]\n    set lenR [llength $radii]\n    if {$lenXY != 2 * $lenR} {\n        error "wrong number of vertices and radii"\n    }\n \n    # Walk down vertices keeping previous, current and next\n    lassign [lrange $xy end-1 end] x0 y0\n    lassign $xy x1 y1\n    eval lappend xy [lrange $xy 0 1]\n    set knots {}                                ;# These are the control points\n \n    for {set i 0} {$i < $lenXY} {incr i 2} {\n        set radius [lindex $radii [expr {$i/2}]]\n        set r [winfo pixels $w $radius]\n \n        lassign [lrange $xy [expr {$i + 2}] [expr {$i + 3}]] x2 y2\n        set z [_RoundPoly2 $x0 $y0 $x1 $y1 $x2 $y2 $r]\n        eval lappend knots $z\n \n        lassign [list $x1 $y1] x0 y0           ;# Current becomes previous\n        lassign [list $x2 $y2] x1 y1           ;# Next becomes current\n    }\n    set n [eval $w create polygon $knots -smooth 1 $args]\n    return $n\n }\n proc _RoundPoly2 {x0 y0 x1 y1 x2 y2 radius} {\n    set d [expr { 2 * $radius }]\n    set maxr 0.75\n \n    set v1x [expr {$x0 - $x1}]\n    set v1y [expr {$y0 - $y1}]\n    set v2x [expr {$x2 - $x1}]\n    set v2y [expr {$y2 - $y1}]\n \n    set vlen1 [expr {sqrt($v1x*$v1x + $v1y*$v1y)}]\n    set vlen2 [expr {sqrt($v2x*$v2x + $v2y*$v2y)}]\n    if {$d > $maxr * $vlen1} {\n        set d [expr {$maxr * $vlen1}]\n    }\n    if {$d > $maxr * $vlen2} {\n        set d [expr {$maxr * $vlen2}]\n    }\n \n    lappend xy [expr {$x1 + $d * $v1x/$vlen1}] [expr {$y1 + $d * $v1y/$vlen1}]\n    lappend xy $x1 $y1\n    lappend xy [expr {$x1 + $d * $v2x/$vlen2}] [expr {$y1 + $d * $v2y/$vlen2}]\n \n    return $xy\n }\n\n'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
-            0x970065005a0164005a02640184005a036414640384015a046415640865
-            056602640984055a0665065a07640a84005a0865085a096416640b650a64
-            0c650a6604640d84055a0b650b5a0c640e84005a0d650d5a0e6416640f84
-            015a0f650f5a10641084005a116411650a6602641284045a1264135300
-         226           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('AdwDrawEngine')
-                       8 STORE_NAME               2 (__qualname__)
+            0x8700970065005a0164005a0288006601640184085a03640284005a0464
+            14640484015a056415640965066602640a84055a0765075a08640b84005a
+            0965095a0a6416640c650b640d650b6604640e84055a0c650c5a0d640f84
+            005a0e650e5a0f6416641084015a1065105a11641184005a126412650b66
+            02641384045a13880078015a145300
+                       0 MAKE_CELL                0 (__class__)
          
-         227          10 LOAD_CONST               1 (<code object win32_high_dpi, file "D:\tkadw\tkadw\canvas\drawengine.py", line 227>)
-                      12 MAKE_FUNCTION            0
-                      14 STORE_NAME               3 (win32_high_dpi)
+         226           2 RESUME                   0
+                       4 LOAD_NAME                0 (__name__)
+                       6 STORE_NAME               1 (__module__)
+                       8 LOAD_CONST               0 ('AdwDrawEngine')
+                      10 STORE_NAME               2 (__qualname__)
          
-         231          16 LOAD_CONST              20 (('x',))
-                      18 LOAD_CONST               3 (<code object draw_gradient, file "D:\tkadw\tkadw\canvas\drawengine.py", line 231>)
-                      20 MAKE_FUNCTION            1 (defaults)
-                      22 STORE_NAME               4 (draw_gradient)
+         227          12 LOAD_CLOSURE             0 (__class__)
+                      14 BUILD_TUPLE              1
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\drawengine.py", line 227>)
+                      18 MAKE_FUNCTION            8 (closure)
+                      20 STORE_NAME               3 (__init__)
          
-         298          24 LOAD_CONST              21 ((5, 2, 'white', 'black'))
-                      26 LOAD_CONST               8 ('radius')
-                      28 LOAD_NAME                5 (float)
-                      30 BUILD_TUPLE              2
-                      32 LOAD_CONST               9 (<code object create_round_rectangle, file "D:\tkadw\tkadw\canvas\drawengine.py", line 298>)
-                      34 MAKE_FUNCTION            5 (defaults, annotations)
-                      36 STORE_NAME               6 (create_round_rectangle)
+         230          22 LOAD_CONST               2 (<code object win32_high_dpi, file "D:\tkadw\tkadw\canvas\drawengine.py", line 230>)
+                      24 MAKE_FUNCTION            0
+                      26 STORE_NAME               4 (win32_high_dpi)
          
-         329          38 LOAD_NAME                6 (create_round_rectangle)
-                      40 STORE_NAME               7 (create_round_rect)
+         234          28 LOAD_CONST              20 (('x',))
+                      30 LOAD_CONST               4 (<code object draw_gradient, file "D:\tkadw\tkadw\canvas\drawengine.py", line 234>)
+                      32 MAKE_FUNCTION            1 (defaults)
+                      34 STORE_NAME               5 (draw_gradient)
          
-         331          42 LOAD_CONST              10 (<code object create_round_rectangle2, file "D:\tkadw\tkadw\canvas\drawengine.py", line 331>)
-                      44 MAKE_FUNCTION            0
-                      46 STORE_NAME               8 (create_round_rectangle2)
+         301          36 LOAD_CONST              21 ((5, 2, 'white', 'black'))
+                      38 LOAD_CONST               9 ('radius')
+                      40 LOAD_NAME                6 (float)
+                      42 BUILD_TUPLE              2
+                      44 LOAD_CONST              10 (<code object create_round_rectangle, file "D:\tkadw\tkadw\canvas\drawengine.py", line 301>)
+                      46 MAKE_FUNCTION            5 (defaults, annotations)
+                      48 STORE_NAME               7 (create_round_rectangle)
          
-         399          48 LOAD_NAME                8 (create_round_rectangle2)
-                      50 STORE_NAME               9 (create_round_rect2)
+         332          50 LOAD_NAME                7 (create_round_rectangle)
+                      52 STORE_NAME               8 (create_round_rect)
          
-         401          52 LOAD_CONST              22 (('black', 'black'))
-                      54 LOAD_CONST              11 ('fill')
-                      56 LOAD_NAME               10 (str)
-                      58 LOAD_CONST              12 ('outline')
-                      60 LOAD_NAME               10 (str)
-                      62 BUILD_TUPLE              4
-                      64 LOAD_CONST              13 (<code object create_round_rectangle3, file "D:\tkadw\tkadw\canvas\drawengine.py", line 401>)
-                      66 MAKE_FUNCTION            5 (defaults, annotations)
-                      68 STORE_NAME              11 (create_round_rectangle3)
+         334          54 LOAD_CONST              11 (<code object create_round_rectangle2, file "D:\tkadw\tkadw\canvas\drawengine.py", line 334>)
+                      56 MAKE_FUNCTION            0
+                      58 STORE_NAME               9 (create_round_rectangle2)
          
-         418          70 LOAD_NAME               11 (create_round_rectangle3)
-                      72 STORE_NAME              12 (create_round_rect3)
+         402          60 LOAD_NAME                9 (create_round_rectangle2)
+                      62 STORE_NAME              10 (create_round_rect2)
          
-         420          74 LOAD_CONST              14 (<code object create_round_rectangle4, file "D:\tkadw\tkadw\canvas\drawengine.py", line 420>)
-                      76 MAKE_FUNCTION            0
-                      78 STORE_NAME              13 (create_round_rectangle4)
+         404          64 LOAD_CONST              22 (('black', 'black'))
+                      66 LOAD_CONST              12 ('fill')
+                      68 LOAD_NAME               11 (str)
+                      70 LOAD_CONST              13 ('outline')
+                      72 LOAD_NAME               11 (str)
+                      74 BUILD_TUPLE              4
+                      76 LOAD_CONST              14 (<code object create_round_rectangle3, file "D:\tkadw\tkadw\canvas\drawengine.py", line 404>)
+                      78 MAKE_FUNCTION            5 (defaults, annotations)
+                      80 STORE_NAME              12 (create_round_rectangle3)
          
-         446          80 LOAD_NAME               13 (create_round_rectangle4)
-                      82 STORE_NAME              14 (create_round_rect4)
+         421          82 LOAD_NAME               12 (create_round_rectangle3)
+                      84 STORE_NAME              13 (create_round_rect3)
          
-         448          84 LOAD_CONST              22 (('black', 'black'))
-                      86 LOAD_CONST              15 (<code object polygon_round, file "D:\tkadw\tkadw\canvas\drawengine.py", line 448>)
-                      88 MAKE_FUNCTION            1 (defaults)
-                      90 STORE_NAME              15 (polygon_round)
+         423          86 LOAD_CONST              15 (<code object create_round_rectangle4, file "D:\tkadw\tkadw\canvas\drawengine.py", line 423>)
+                      88 MAKE_FUNCTION            0
+                      90 STORE_NAME              14 (create_round_rectangle4)
          
-         454          92 LOAD_NAME               15 (polygon_round)
-                      94 STORE_NAME              16 (poly_round)
+         449          92 LOAD_NAME               14 (create_round_rectangle4)
+                      94 STORE_NAME              15 (create_round_rect4)
          
-         456          96 LOAD_CONST              16 (<code object demo_polygon_round, file "D:\tkadw\tkadw\canvas\drawengine.py", line 456>)
-                      98 MAKE_FUNCTION            0
-                     100 STORE_NAME              17 (demo_polygon_round)
+         451          96 LOAD_CONST              22 (('black', 'black'))
+                      98 LOAD_CONST              16 (<code object polygon_round, file "D:\tkadw\tkadw\canvas\drawengine.py", line 451>)
+                     100 MAKE_FUNCTION            1 (defaults)
+                     102 STORE_NAME              16 (polygon_round)
          
-         564         102 LOAD_CONST              17 ('content')
-                     104 LOAD_NAME               10 (str)
-                     106 BUILD_TUPLE              2
-                     108 LOAD_CONST              18 (<code object create_svg_image, file "D:\tkadw\tkadw\canvas\drawengine.py", line 564>)
-                     110 MAKE_FUNCTION            4 (annotations)
-                     112 STORE_NAME              18 (create_svg_image)
-                     114 LOAD_CONST              19 (None)
-                     116 RETURN_VALUE
+         457         104 LOAD_NAME               16 (polygon_round)
+                     106 STORE_NAME              17 (poly_round)
+         
+         459         108 LOAD_CONST              17 (<code object demo_polygon_round, file "D:\tkadw\tkadw\canvas\drawengine.py", line 459>)
+                     110 MAKE_FUNCTION            0
+                     112 STORE_NAME              18 (demo_polygon_round)
+         
+         567         114 LOAD_CONST              18 ('content')
+                     116 LOAD_NAME               11 (str)
+                     118 BUILD_TUPLE              2
+                     120 LOAD_CONST              19 (<code object create_svg_image, file "D:\tkadw\tkadw\canvas\drawengine.py", line 567>)
+                     122 MAKE_FUNCTION            4 (annotations)
+                     124 STORE_NAME              19 (create_svg_image)
+                     126 LOAD_CLOSURE             0 (__class__)
+                     128 COPY                     1
+                     130 STORE_NAME              20 (__classcell__)
+                     132 RETURN_VALUE
          consts
             'AdwDrawEngine'
             code
                argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x950197000200740100000000000000000000a6000000ab000000000000
+                  0000006a0100000000000000007c0169007c02a4018e01010064005300
+                             0 COPY_FREE_VARS           1
+               
+               227           2 RESUME                   0
+               
+               228           4 PUSH_NULL
+                             6 LOAD_GLOBAL              1 (NULL + super)
+                            18 PRECALL                  0
+                            22 CALL                     0
+                            32 LOAD_ATTR                1 (__init__)
+                            42 LOAD_FAST                1 (args)
+                            44 BUILD_MAP                0
+                            46 LOAD_FAST                2 (kwargs)
+                            48 DICT_MERGE               1
+                            50 CALL_FUNCTION_EX         1
+                            52 POP_TOP
+                            54 LOAD_CONST               0 (None)
+                            56 RETURN_VALUE
+               consts
+                  None
+               names      ('super', '__init__')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ('__class__',)
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
+               name       '__init__'
+               firstlineno 227
+               lnotab 0x0401
+            code
+               argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x9700640164026c006d017d0101007c016a020000000000000000a00300
                   000000000000000000000000000000000000006403a6010000ab01000000
                   0000000000010064005300
-               227           0 RESUME                   0
+               230           0 RESUME                   0
                
-               228           2 LOAD_CONST               1 (0)
+               231           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('windll',))
                              6 IMPORT_NAME              0 (ctypes)
                              8 IMPORT_FROM              1 (windll)
                             10 STORE_FAST               1 (windll)
                             12 POP_TOP
                
-               229          14 LOAD_FAST                1 (windll)
+               232          14 LOAD_FAST                1 (windll)
                             16 LOAD_ATTR                2 (shcore)
                             26 LOAD_METHOD              3 (SetProcessDpiAwareness)
                             48 LOAD_CONST               3 (2)
                             50 PRECALL                  1
                             54 CALL                     1
                             64 POP_TOP
                             66 LOAD_CONST               0 (None)
@@ -243,39 +289,39 @@
                   2
                names      ('ctypes', 'windll', 'shcore', 'SetProcessDpiAwareness')
                varnames   ('self', 'windll')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
                name       'win32_high_dpi'
-               firstlineno 227
+               firstlineno 230
                lnotab 0x02010c01
             'x'
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 7
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007c006a0000
                   00000000000000a002000000000000000000000000000000000000000064
                   027c006a0300000000000000007c037c017c02a6050000ab050000000000
                   000000010064005300
-               231           0 RESUME                   0
+               234           0 RESUME                   0
                
-               232           2 LOAD_FAST                0 (self)
+               235           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (tk)
                             14 LOAD_METHOD              1 (eval)
                             36 LOAD_CONST               1 ('\n  proc + {n1 n2} {\n    expr {$n1 + $n2}\n  }\n  proc - {n1 n2} {\n    expr {$n1 - $n2}\n  }\n  proc * {n1 n2} {\n    expr {$n1 * $n2}\n  }\n  proc / {n1 n2} {\n    expr {$n1 / $n2}\n  }\n  proc toInt {n} {\n    expr int($n)\n  }\n  \n  proc drawGradient {win type col1Str col2Str} {\n    $win delete gradient\n    \n    set width [winfo width $win]\n    set height [winfo height $win]\n    \n    lassign [winfo rgb $win $col1Str] r1 g1 b1\n    lassign  [winfo rgb $win $col2Str] r2 g2 b2\n    set rRange [- $r2.0 $r1]\n    set gRange [- $g2.0 $g1]\n    set bRange [- $b2.0 $b1]\n  \n    if {$type == "x"} {\n      set rRatio [/ $rRange $width]\n      set gRatio [/ $gRange $width]\n      set bRatio [/ $bRange $width]\n    \n      for {set x 0} {$x < $width} {incr x} {\n        set nR [toInt [+ $r1 [* $rRatio $x]]]\n        set nG [toInt [+ $g1 [* $gRatio $x]]]\n        set nB [toInt [+ $b1 [* $bRatio $x]]]\n  \n        set col [format {%4.4x} $nR]\n        append col [format {%4.4x} $nG]\n        append col [format {%4.4x} $nB]\n        $win create line $x 0 $x $height -tags gradient -fill #${col}\n      }\n    } else {\n      set rRatio [/ $rRange $height]\n      set gRatio [/ $gRange $height]\n      set bRatio [/ $bRange $height]\n  \n      for {set y 0} {$y < $height} {incr y} {\n        set nR [toInt [+ $r1 [* $rRatio $y]]]\n        set nG [toInt [+ $g1 [* $gRatio $y]]]\n        set nB [toInt [+ $b1 [* $bRatio $y]]]\n  \n        set col [format {%4.4x} $nR]\n        append col [format {%4.4x} $nG]\n        append col [format {%4.4x} $nB]\n        $win create line 0 $y $width $y -tags gradient -fill #${col}\n      }\n    }\n    return $win\n  }\n        ')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               296          54 LOAD_FAST                0 (self)
+               299          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                0 (tk)
                             66 LOAD_METHOD              2 (call)
                             88 LOAD_CONST               2 ('drawGradient')
                             90 LOAD_FAST                0 (self)
                             92 LOAD_ATTR                3 (_w)
                            102 LOAD_FAST                3 (type)
                            104 LOAD_FAST                1 (color1)
@@ -291,15 +337,15 @@
                   'drawGradient'
                names      ('tk', 'eval', 'call', '_w')
                varnames   ('self', 'color1', 'color2', 'type')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
                name       'draw_gradient'
-               firstlineno 231
+               firstlineno 234
                lnotab 0x02013440
             5
             2
             'white'
             'black'
             'radius'
             code
@@ -337,110 +383,110 @@
                   067a0a00007c037c0664017a0b00007a0a00007c047c0964017a0b00007a
                   0a00007c067a0000007c076405ac08a6060000ab0600000000000000007d
                   137c00a00200000000000000000000000000000000000000007c017c0964
                   017a0b00007a0000007c067a0a00007c047c0964017a0b00007a0a00007c
                   037c0964017a0b00007a0a00007c067a0000007c047c0664017a0b00007a
                   0a00007c076405ac08a6060000ab0600000000000000007d147c0a7c0b7c
                   0c7c0d7c0e7c0f7c107c117c127c137c1464099c0b5300
-               298           0 RESUME                   0
+               301           0 RESUME                   0
                
-               300           2 LOAD_FAST                5 (radius)
+               303           2 LOAD_FAST                5 (radius)
                              4 LOAD_CONST               1 (2)
                              6 BINARY_OP                5 (*)
                             10 STORE_FAST               9 (_radius)
                
-               301          12 LOAD_FAST                0 (self)
+               304          12 LOAD_FAST                0 (self)
                             14 LOAD_METHOD              0 (create_arc)
                             36 LOAD_FAST                1 (x1)
                             38 LOAD_FAST                2 (y1)
                             40 LOAD_FAST                1 (x1)
                             42 LOAD_FAST                9 (_radius)
                             44 BINARY_OP                0 (+)
                             48 LOAD_FAST                2 (y1)
                             50 LOAD_FAST                9 (_radius)
                             52 BINARY_OP                0 (+)
                             56 LOAD_CONST               2 (90)
                             58 LOAD_CONST               2 (90)
                             60 LOAD_FAST                6 (width)
                             62 LOAD_FAST                7 (fill)
                
-               302          64 LOAD_FAST                8 (outline)
+               305          64 LOAD_FAST                8 (outline)
                
-               301          66 KW_NAMES                 3
+               304          66 KW_NAMES                 3
                             68 PRECALL                  9
                             72 CALL                     9
                             82 STORE_FAST              10 (nw)
                
-               303          84 LOAD_FAST                0 (self)
+               306          84 LOAD_FAST                0 (self)
                             86 LOAD_METHOD              0 (create_arc)
                            108 LOAD_FAST                1 (x1)
                            110 LOAD_FAST                4 (y2)
                            112 LOAD_FAST                1 (x1)
                            114 LOAD_FAST                9 (_radius)
                            116 BINARY_OP                0 (+)
                            120 LOAD_FAST                4 (y2)
                            122 LOAD_FAST                9 (_radius)
                            124 BINARY_OP               10 (-)
                            128 LOAD_CONST               4 (180)
                            130 LOAD_CONST               2 (90)
                            132 LOAD_FAST                6 (width)
                            134 LOAD_FAST                7 (fill)
                
-               304         136 LOAD_FAST                8 (outline)
+               307         136 LOAD_FAST                8 (outline)
                
-               303         138 KW_NAMES                 3
+               306         138 KW_NAMES                 3
                            140 PRECALL                  9
                            144 CALL                     9
                            154 STORE_FAST              11 (sw)
                
-               305         156 LOAD_FAST                0 (self)
+               308         156 LOAD_FAST                0 (self)
                            158 LOAD_METHOD              0 (create_arc)
                            180 LOAD_FAST                3 (x2)
                            182 LOAD_FAST                9 (_radius)
                            184 BINARY_OP               10 (-)
                            188 LOAD_FAST                2 (y1)
                            190 LOAD_FAST                3 (x2)
                            192 LOAD_FAST                2 (y1)
                            194 LOAD_FAST                9 (_radius)
                            196 BINARY_OP                0 (+)
                            200 LOAD_CONST               5 (0)
                            202 LOAD_CONST               2 (90)
                            204 LOAD_FAST                6 (width)
                            206 LOAD_FAST                7 (fill)
                
-               306         208 LOAD_FAST                8 (outline)
+               309         208 LOAD_FAST                8 (outline)
                
-               305         210 KW_NAMES                 3
+               308         210 KW_NAMES                 3
                            212 PRECALL                  9
                            216 CALL                     9
                            226 STORE_FAST              12 (ne)
                
-               307         228 LOAD_FAST                0 (self)
+               310         228 LOAD_FAST                0 (self)
                            230 LOAD_METHOD              0 (create_arc)
                            252 LOAD_FAST                3 (x2)
                            254 LOAD_FAST                9 (_radius)
                            256 BINARY_OP               10 (-)
                            260 LOAD_FAST                4 (y2)
                            262 LOAD_FAST                3 (x2)
                            264 LOAD_FAST                4 (y2)
                            266 LOAD_FAST                9 (_radius)
                            268 BINARY_OP               10 (-)
                            272 LOAD_CONST               6 (270)
                            274 LOAD_CONST               2 (90)
                            276 LOAD_FAST                6 (width)
                            278 LOAD_FAST                7 (fill)
                
-               308         280 LOAD_FAST                8 (outline)
+               311         280 LOAD_FAST                8 (outline)
                
-               307         282 KW_NAMES                 3
+               310         282 KW_NAMES                 3
                            284 PRECALL                  9
                            288 CALL                     9
                            298 STORE_FAST              13 (se)
                
-               310         300 LOAD_FAST                0 (self)
+               313         300 LOAD_FAST                0 (self)
                            302 LOAD_METHOD              1 (create_line)
                            324 LOAD_FAST                1 (x1)
                            326 LOAD_FAST                2 (y1)
                            328 LOAD_FAST                9 (_radius)
                            330 LOAD_CONST               1 (2)
                            332 BINARY_OP               11 (/)
                            336 BINARY_OP                0 (+)
@@ -453,15 +499,15 @@
                            356 LOAD_FAST                6 (width)
                            358 LOAD_FAST                8 (outline)
                            360 KW_NAMES                 7
                            362 PRECALL                  6
                            366 CALL                     6
                            376 STORE_FAST              14 (w)
                
-               311         378 LOAD_FAST                0 (self)
+               314         378 LOAD_FAST                0 (self)
                            380 LOAD_METHOD              1 (create_line)
                            402 LOAD_FAST                1 (x1)
                            404 LOAD_FAST                9 (_radius)
                            406 LOAD_CONST               1 (2)
                            408 BINARY_OP               11 (/)
                            412 BINARY_OP                0 (+)
                            416 LOAD_FAST                2 (y1)
@@ -474,15 +520,15 @@
                            434 LOAD_FAST                6 (width)
                            436 LOAD_FAST                8 (outline)
                            438 KW_NAMES                 7
                            440 PRECALL                  6
                            444 CALL                     6
                            454 STORE_FAST              15 (n)
                
-               312         456 LOAD_FAST                0 (self)
+               315         456 LOAD_FAST                0 (self)
                            458 LOAD_METHOD              1 (create_line)
                            480 LOAD_FAST                3 (x2)
                            482 LOAD_FAST                2 (y1)
                            484 LOAD_FAST                9 (_radius)
                            486 LOAD_CONST               1 (2)
                            488 BINARY_OP               11 (/)
                            492 BINARY_OP                0 (+)
@@ -495,15 +541,15 @@
                            512 LOAD_FAST                6 (width)
                            514 LOAD_FAST                8 (outline)
                            516 KW_NAMES                 7
                            518 PRECALL                  6
                            522 CALL                     6
                            532 STORE_FAST              16 (e)
                
-               313         534 LOAD_FAST                0 (self)
+               316         534 LOAD_FAST                0 (self)
                            536 LOAD_METHOD              1 (create_line)
                            558 LOAD_FAST                1 (x1)
                            560 LOAD_FAST                9 (_radius)
                            562 LOAD_CONST               1 (2)
                            564 BINARY_OP               11 (/)
                            568 BINARY_OP                0 (+)
                            572 LOAD_FAST                4 (y2)
@@ -516,15 +562,15 @@
                            590 LOAD_FAST                6 (width)
                            592 LOAD_FAST                8 (outline)
                            594 KW_NAMES                 7
                            596 PRECALL                  6
                            600 CALL                     6
                            610 STORE_FAST              17 (s)
                
-               315         612 LOAD_FAST                0 (self)
+               318         612 LOAD_FAST                0 (self)
                            614 LOAD_METHOD              2 (create_rectangle)
                            636 LOAD_FAST                1 (x1)
                            638 LOAD_FAST                9 (_radius)
                            640 LOAD_CONST               1 (2)
                            642 BINARY_OP               11 (/)
                            646 BINARY_OP                0 (+)
                            650 LOAD_FAST                6 (width)
@@ -544,22 +590,22 @@
                            690 LOAD_FAST                2 (y1)
                            692 LOAD_FAST                9 (_radius)
                            694 LOAD_CONST               1 (2)
                            696 BINARY_OP               11 (/)
                            700 BINARY_OP                0 (+)
                            704 LOAD_FAST                7 (fill)
                
-               316         706 LOAD_CONST               5 (0)
+               319         706 LOAD_CONST               5 (0)
                
-               315         708 KW_NAMES                 8
+               318         708 KW_NAMES                 8
                            710 PRECALL                  6
                            714 CALL                     6
                            724 STORE_FAST              18 (top)
                
-               318         726 LOAD_FAST                0 (self)
+               321         726 LOAD_FAST                0 (self)
                            728 LOAD_METHOD              2 (create_rectangle)
                            750 LOAD_FAST                1 (x1)
                            752 LOAD_FAST                6 (width)
                            754 LOAD_CONST               1 (2)
                            756 BINARY_OP               11 (/)
                            760 BINARY_OP                0 (+)
                            764 LOAD_FAST                2 (y1)
@@ -579,22 +625,22 @@
                            802 LOAD_CONST               1 (2)
                            804 BINARY_OP               11 (/)
                            808 BINARY_OP               10 (-)
                            812 LOAD_FAST                6 (width)
                            814 BINARY_OP                0 (+)
                            818 LOAD_FAST                7 (fill)
                
-               319         820 LOAD_CONST               5 (0)
+               322         820 LOAD_CONST               5 (0)
                
-               318         822 KW_NAMES                 8
+               321         822 KW_NAMES                 8
                            824 PRECALL                  6
                            828 CALL                     6
                            838 STORE_FAST              19 (center)
                
-               321         840 LOAD_FAST                0 (self)
+               324         840 LOAD_FAST                0 (self)
                            842 LOAD_METHOD              2 (create_rectangle)
                            864 LOAD_FAST                1 (x1)
                            866 LOAD_FAST                9 (_radius)
                            868 LOAD_CONST               1 (2)
                            870 BINARY_OP               11 (/)
                            874 BINARY_OP                0 (+)
                            878 LOAD_FAST                6 (width)
@@ -614,35 +660,35 @@
                            918 LOAD_FAST                4 (y2)
                            920 LOAD_FAST                6 (width)
                            922 LOAD_CONST               1 (2)
                            924 BINARY_OP               11 (/)
                            928 BINARY_OP               10 (-)
                            932 LOAD_FAST                7 (fill)
                
-               322         934 LOAD_CONST               5 (0)
+               325         934 LOAD_CONST               5 (0)
                
-               321         936 KW_NAMES                 8
+               324         936 KW_NAMES                 8
                            938 PRECALL                  6
                            942 CALL                     6
                            952 STORE_FAST              20 (bottom)
                
-               325         954 LOAD_FAST               10 (nw)
+               328         954 LOAD_FAST               10 (nw)
                            956 LOAD_FAST               11 (sw)
                            958 LOAD_FAST               12 (ne)
                            960 LOAD_FAST               13 (se)
                            962 LOAD_FAST               14 (w)
                            964 LOAD_FAST               15 (n)
                            966 LOAD_FAST               16 (e)
                            968 LOAD_FAST               17 (s)
                
-               326         970 LOAD_FAST               18 (top)
+               329         970 LOAD_FAST               18 (top)
                            972 LOAD_FAST               19 (center)
                            974 LOAD_FAST               20 (bottom)
                
-               324         976 LOAD_CONST               9 (('nw', 'sw', 'ne', 'se', 'w', 'n', 'e', 's', 'top', 'center', 'bottom'))
+               327         976 LOAD_CONST               9 (('nw', 'sw', 'ne', 'se', 'w', 'n', 'e', 's', 'top', 'center', 'bottom'))
                            978 BUILD_CONST_KEY_MAP     11
                            980 RETURN_VALUE
                consts
                   None
                   2
                   90
                   ('start', 'extent', 'width', 'fill', 'outline')
@@ -654,15 +700,15 @@
                   ('nw', 'sw', 'ne', 'se', 'w', 'n', 'e', 's', 'top', 'center', 'bottom')
                names      ('create_arc', 'create_line', 'create_rectangle')
                varnames   ('self', 'x1', 'y1', 'x2', 'y2', 'radius', 'width', 'fill', 'outline', '_radius', 'nw', 'sw', 'ne', 'se', 'w', 'n', 'e', 's', 'top', 'center', 'bottom')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
                name       'create_round_rectangle'
-               firstlineno 298
+               firstlineno 301
                lnotab
                   0x02020a01340102ff1202340102ff1202340102ff1202340102ff12034e
                   014e014e014e025e0102ff12035e0102ff12035e0102ff1204100106fe
             code
                argcount  : 6
                nlocals   : 9
                stacksize : 9
@@ -670,66 +716,66 @@
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007c006a0000
                   00000000000000a002000000000000000000000000000000000000000064
                   027c006a0300000000000000007c017c027c037c047c05a6070000ab0700
                   000000000000007d0802007c006a0400000000000000007c0867017c06a2
                   01520069007c07a4018e0101007c085300
-               331           0 RESUME                   0
+               334           0 RESUME                   0
                
-               333           2 LOAD_FAST                0 (self)
+               336           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (tk)
                             14 LOAD_METHOD              1 (eval)
                             36 LOAD_CONST               1 ("\n#----------------------------------------------------------------------\n#\n# roundRect --\n#\n#       Draw a rounded rectangle in the canvas.\n#\n# Parameters:\n#       w - Path name of the canvas\n#       x0, y0 - Co-ordinates of the upper left corner, in pixels\n#       x3, y3 - Co-ordinates of the lower right corner, in pixels\n#       radius - Radius of the bend at the corners, in any form\n#                acceptable to Tk_GetPixels\n#       args - Other args suitable to a 'polygon' item on the canvas\n#\n# Results:\n#       Returns the canvas item number of the rounded rectangle.\n#\n# Side effects:\n#       Creates a rounded rectangle as a smooth polygon in the canvas.\n#\n#----------------------------------------------------------------------\n\nproc roundRect { w x0 y0 x3 y3 radius args } {\n\nset r [winfo pixels $w $radius]\nset d [expr { 2 * $r }]\n\n# Make sure that the radius of the curve is less than 3/8\n# size of the box!\n\nset maxr 0.75\n\nif { $d > $maxr * ( $x3 - $x0 ) } {\n    set d [expr { $maxr * ( $x3 - $x0 ) }]\n}\nif { $d > $maxr * ( $y3 - $y0 ) } {\n    set d [expr { $maxr * ( $y3 - $y0 ) }]\n}\n\nset x1 [expr { $x0 + $d }]\nset x2 [expr { $x3 - $d }]\nset y1 [expr { $y0 + $d }]\nset y2 [expr { $y3 - $d }]\n\nset cmd [list $w create polygon]\nlappend cmd $x0 $y0\nlappend cmd $x1 $y0\nlappend cmd $x2 $y0\nlappend cmd $x3 $y0\nlappend cmd $x3 $y1\nlappend cmd $x3 $y2\nlappend cmd $x3 $y3\nlappend cmd $x2 $y3\nlappend cmd $x1 $y3\nlappend cmd $x0 $y3\nlappend cmd $x0 $y2\nlappend cmd $x0 $y1\nlappend cmd -smooth 1\nreturn [eval $cmd $args]\n}\n        ")
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               395          54 LOAD_FAST                0 (self)
+               398          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                0 (tk)
                             66 LOAD_METHOD              2 (call)
                             88 LOAD_CONST               2 ('roundRect')
                             90 LOAD_FAST                0 (self)
                             92 LOAD_ATTR                3 (_w)
                            102 LOAD_FAST                1 (x0)
                            104 LOAD_FAST                2 (y0)
                            106 LOAD_FAST                3 (x3)
                            108 LOAD_FAST                4 (y3)
                            110 LOAD_FAST                5 (radius)
                            112 PRECALL                  7
                            116 CALL                     7
                            126 STORE_FAST               8 (rect)
                
-               396         128 PUSH_NULL
+               399         128 PUSH_NULL
                            130 LOAD_FAST                0 (self)
                            132 LOAD_ATTR                4 (itemconfig)
                            142 LOAD_FAST                8 (rect)
                            144 BUILD_LIST               1
                            146 LOAD_FAST                6 (args)
                            148 LIST_EXTEND              1
                            150 LIST_TO_TUPLE
                            152 BUILD_MAP                0
                            154 LOAD_FAST                7 (kwargs)
                            156 DICT_MERGE               1
                            158 CALL_FUNCTION_EX         1
                            160 POP_TOP
                
-               397         162 LOAD_FAST                8 (rect)
+               400         162 LOAD_FAST                8 (rect)
                            164 RETURN_VALUE
                consts
                   None
                   "\n#----------------------------------------------------------------------\n#\n# roundRect --\n#\n#       Draw a rounded rectangle in the canvas.\n#\n# Parameters:\n#       w - Path name of the canvas\n#       x0, y0 - Co-ordinates of the upper left corner, in pixels\n#       x3, y3 - Co-ordinates of the lower right corner, in pixels\n#       radius - Radius of the bend at the corners, in any form\n#                acceptable to Tk_GetPixels\n#       args - Other args suitable to a 'polygon' item on the canvas\n#\n# Results:\n#       Returns the canvas item number of the rounded rectangle.\n#\n# Side effects:\n#       Creates a rounded rectangle as a smooth polygon in the canvas.\n#\n#----------------------------------------------------------------------\n\nproc roundRect { w x0 y0 x3 y3 radius args } {\n\nset r [winfo pixels $w $radius]\nset d [expr { 2 * $r }]\n\n# Make sure that the radius of the curve is less than 3/8\n# size of the box!\n\nset maxr 0.75\n\nif { $d > $maxr * ( $x3 - $x0 ) } {\n    set d [expr { $maxr * ( $x3 - $x0 ) }]\n}\nif { $d > $maxr * ( $y3 - $y0 ) } {\n    set d [expr { $maxr * ( $y3 - $y0 ) }]\n}\n\nset x1 [expr { $x0 + $d }]\nset x2 [expr { $x3 - $d }]\nset y1 [expr { $y0 + $d }]\nset y2 [expr { $y3 - $d }]\n\nset cmd [list $w create polygon]\nlappend cmd $x0 $y0\nlappend cmd $x1 $y0\nlappend cmd $x2 $y0\nlappend cmd $x3 $y0\nlappend cmd $x3 $y1\nlappend cmd $x3 $y2\nlappend cmd $x3 $y3\nlappend cmd $x2 $y3\nlappend cmd $x1 $y3\nlappend cmd $x0 $y3\nlappend cmd $x0 $y2\nlappend cmd $x0 $y1\nlappend cmd -smooth 1\nreturn [eval $cmd $args]\n}\n        "
                   'roundRect'
                names      ('tk', 'eval', 'call', '_w', 'itemconfig')
                varnames   ('self', 'x0', 'y0', 'x3', 'y3', 'radius', 'args', 'kwargs', 'rect')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
                name       'create_round_rectangle2'
-               firstlineno 331
+               firstlineno 334
                lnotab 0x0202343e4a012201
             'fill'
             'outline'
             code
                argcount  : 9
                nlocals   : 12
                stacksize : 12
@@ -737,25 +783,25 @@
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000001007c006a0000
                   00000000000000a002000000000000000000000000000000000000000064
                   027c006a0300000000000000007c027c037c067c047c057c077c087c01a6
                   0a0000ab0a00000000000000007d0b02007c006a0400000000000000007c
                   0b67017c09a201520069007c0aa4018e0101007c0b5300
-               401           0 RESUME                   0
+               404           0 RESUME                   0
                
-               403           2 LOAD_FAST                0 (self)
+               406           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (tk)
                             14 LOAD_METHOD              1 (eval)
                             36 LOAD_CONST               1 ('\nproc roundRect2 {w L T Rad width height fill outline tag} {\n\n  $w create oval $L $T [expr $L + $Rad] [expr $T + $Rad] -fill $fill -outline $outline -tag $tag\n  $w create oval [expr $width-$Rad] $T $width [expr $T + $Rad] -fill $fill -outline $outline -tag $tag\n  $w create oval $L [expr $height-$Rad] [expr $L+$Rad] $height -fill $fill -outline $outline -tag $tag\n  $w create oval [expr $width-$Rad] [expr $height-$Rad] [expr $width] $height -fill $fill -outline $outline -tag $tag\n  $w create rectangle [expr $L + ($Rad/2.0)] $T [expr $width-($Rad/2.0)] $height -fill $fill -outline $outline -tag $tag\n  $w create rectangle $L [expr $T + ($Rad/2.0)] $width [expr $height-($Rad/2.0)] -fill $fill -outline $outline -tag $tag\n}\n            ')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                
-               414          54 LOAD_FAST                0 (self)
+               417          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                0 (tk)
                             66 LOAD_METHOD              2 (call)
                             88 LOAD_CONST               2 ('roundRect2')
                             90 LOAD_FAST                0 (self)
                             92 LOAD_ATTR                3 (_w)
                            102 LOAD_FAST                2 (x)
                            104 LOAD_FAST                3 (y)
@@ -765,41 +811,41 @@
                            112 LOAD_FAST                7 (fill)
                            114 LOAD_FAST                8 (outline)
                            116 LOAD_FAST                1 (tag)
                            118 PRECALL                 10
                            122 CALL                    10
                            132 STORE_FAST              11 (_rect)
                
-               415         134 PUSH_NULL
+               418         134 PUSH_NULL
                            136 LOAD_FAST                0 (self)
                            138 LOAD_ATTR                4 (itemconfig)
                            148 LOAD_FAST               11 (_rect)
                            150 BUILD_LIST               1
                            152 LOAD_FAST                9 (args)
                            154 LIST_EXTEND              1
                            156 LIST_TO_TUPLE
                            158 BUILD_MAP                0
                            160 LOAD_FAST               10 (kwargs)
                            162 DICT_MERGE               1
                            164 CALL_FUNCTION_EX         1
                            166 POP_TOP
                
-               416         168 LOAD_FAST               11 (_rect)
+               419         168 LOAD_FAST               11 (_rect)
                            170 RETURN_VALUE
                consts
                   None
                   '\nproc roundRect2 {w L T Rad width height fill outline tag} {\n\n  $w create oval $L $T [expr $L + $Rad] [expr $T + $Rad] -fill $fill -outline $outline -tag $tag\n  $w create oval [expr $width-$Rad] $T $width [expr $T + $Rad] -fill $fill -outline $outline -tag $tag\n  $w create oval $L [expr $height-$Rad] [expr $L+$Rad] $height -fill $fill -outline $outline -tag $tag\n  $w create oval [expr $width-$Rad] [expr $height-$Rad] [expr $width] $height -fill $fill -outline $outline -tag $tag\n  $w create rectangle [expr $L + ($Rad/2.0)] $T [expr $width-($Rad/2.0)] $height -fill $fill -outline $outline -tag $tag\n  $w create rectangle $L [expr $T + ($Rad/2.0)] $width [expr $height-($Rad/2.0)] -fill $fill -outline $outline -tag $tag\n}\n            '
                   'roundRect2'
                names      ('tk', 'eval', 'call', '_w', 'itemconfig')
                varnames   ('self', 'tag', 'x', 'y', 'width', 'height', 'radius', 'fill', 'outline', 'args', 'kwargs', '_rect')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
                name       'create_round_rectangle3'
-               firstlineno 401
+               firstlineno 404
                lnotab 0x0202340b50012201
             code
                argcount  : 6
                nlocals   : 9
                stacksize : 6
                flags     : 11
                code
@@ -810,235 +856,235 @@
                   0a000091017c0391017c0491017c037c057a0a000091017c0491017c037c
                   057a0a000091017c0491017c017c057a00000091017c0491017c017c057a
                   00000091017c0491017c0191017c0491017c0191017c047c057a0a000091
                   017c0191017c047c057a0a000091017c0191017c027c057a00000091017c
                   0191017c027c057a00000091017c0191017c0291017d0702007c006a0000
                   000000000000007c07660169007c06a401640164026901a4018e017d087c
                   085300
-               420           0 RESUME                   0
+               423           0 RESUME                   0
                
-               421           2 BUILD_LIST               0
+               424           2 BUILD_LIST               0
                              4 LOAD_FAST                1 (x1)
                              6 LOAD_FAST                5 (radius)
                              8 BINARY_OP                0 (+)
                             12 LIST_APPEND              1
                             14 LOAD_FAST                2 (y1)
                             16 LIST_APPEND              1
                
-               422          18 LOAD_FAST                1 (x1)
+               425          18 LOAD_FAST                1 (x1)
                             20 LOAD_FAST                5 (radius)
                             22 BINARY_OP                0 (+)
                
-               421          26 LIST_APPEND              1
+               424          26 LIST_APPEND              1
                
-               422          28 LOAD_FAST                2 (y1)
+               425          28 LOAD_FAST                2 (y1)
                
-               421          30 LIST_APPEND              1
+               424          30 LIST_APPEND              1
                
-               423          32 LOAD_FAST                3 (x2)
+               426          32 LOAD_FAST                3 (x2)
                             34 LOAD_FAST                5 (radius)
                             36 BINARY_OP               10 (-)
                
-               421          40 LIST_APPEND              1
+               424          40 LIST_APPEND              1
                
-               423          42 LOAD_FAST                2 (y1)
+               426          42 LOAD_FAST                2 (y1)
                
-               421          44 LIST_APPEND              1
+               424          44 LIST_APPEND              1
                
-               424          46 LOAD_FAST                3 (x2)
+               427          46 LOAD_FAST                3 (x2)
                             48 LOAD_FAST                5 (radius)
                             50 BINARY_OP               10 (-)
                
-               421          54 LIST_APPEND              1
+               424          54 LIST_APPEND              1
                
-               424          56 LOAD_FAST                2 (y1)
+               427          56 LOAD_FAST                2 (y1)
                
-               421          58 LIST_APPEND              1
+               424          58 LIST_APPEND              1
                
-               425          60 LOAD_FAST                3 (x2)
+               428          60 LOAD_FAST                3 (x2)
                
-               421          62 LIST_APPEND              1
+               424          62 LIST_APPEND              1
                
-               425          64 LOAD_FAST                2 (y1)
+               428          64 LOAD_FAST                2 (y1)
                
-               421          66 LIST_APPEND              1
+               424          66 LIST_APPEND              1
                
-               426          68 LOAD_FAST                3 (x2)
+               429          68 LOAD_FAST                3 (x2)
                
-               421          70 LIST_APPEND              1
+               424          70 LIST_APPEND              1
                
-               426          72 LOAD_FAST                2 (y1)
+               429          72 LOAD_FAST                2 (y1)
                             74 LOAD_FAST                5 (radius)
                             76 BINARY_OP                0 (+)
                
-               421          80 LIST_APPEND              1
+               424          80 LIST_APPEND              1
                
-               427          82 LOAD_FAST                3 (x2)
+               430          82 LOAD_FAST                3 (x2)
                
-               421          84 LIST_APPEND              1
+               424          84 LIST_APPEND              1
                
-               427          86 LOAD_FAST                2 (y1)
+               430          86 LOAD_FAST                2 (y1)
                             88 LOAD_FAST                5 (radius)
                             90 BINARY_OP                0 (+)
                
-               421          94 LIST_APPEND              1
+               424          94 LIST_APPEND              1
                
-               428          96 LOAD_FAST                3 (x2)
+               431          96 LOAD_FAST                3 (x2)
                
-               421          98 LIST_APPEND              1
+               424          98 LIST_APPEND              1
                
-               428         100 LOAD_FAST                4 (y2)
+               431         100 LOAD_FAST                4 (y2)
                            102 LOAD_FAST                5 (radius)
                            104 BINARY_OP               10 (-)
                
-               421         108 LIST_APPEND              1
+               424         108 LIST_APPEND              1
                
-               429         110 LOAD_FAST                3 (x2)
+               432         110 LOAD_FAST                3 (x2)
                
-               421         112 LIST_APPEND              1
+               424         112 LIST_APPEND              1
                
-               429         114 LOAD_FAST                4 (y2)
+               432         114 LOAD_FAST                4 (y2)
                            116 LOAD_FAST                5 (radius)
                            118 BINARY_OP               10 (-)
                
-               421         122 LIST_APPEND              1
+               424         122 LIST_APPEND              1
                
-               430         124 LOAD_FAST                3 (x2)
+               433         124 LOAD_FAST                3 (x2)
                
-               421         126 LIST_APPEND              1
+               424         126 LIST_APPEND              1
                
-               430         128 LOAD_FAST                4 (y2)
+               433         128 LOAD_FAST                4 (y2)
                
-               421         130 LIST_APPEND              1
+               424         130 LIST_APPEND              1
                
-               431         132 LOAD_FAST                3 (x2)
+               434         132 LOAD_FAST                3 (x2)
                            134 LOAD_FAST                5 (radius)
                            136 BINARY_OP               10 (-)
                
-               421         140 LIST_APPEND              1
+               424         140 LIST_APPEND              1
                
-               431         142 LOAD_FAST                4 (y2)
+               434         142 LOAD_FAST                4 (y2)
                
-               421         144 LIST_APPEND              1
+               424         144 LIST_APPEND              1
                
-               432         146 LOAD_FAST                3 (x2)
+               435         146 LOAD_FAST                3 (x2)
                            148 LOAD_FAST                5 (radius)
                            150 BINARY_OP               10 (-)
                
-               421         154 LIST_APPEND              1
+               424         154 LIST_APPEND              1
                
-               432         156 LOAD_FAST                4 (y2)
+               435         156 LOAD_FAST                4 (y2)
                
-               421         158 LIST_APPEND              1
+               424         158 LIST_APPEND              1
                
-               433         160 LOAD_FAST                1 (x1)
+               436         160 LOAD_FAST                1 (x1)
                            162 LOAD_FAST                5 (radius)
                            164 BINARY_OP                0 (+)
                
-               421         168 LIST_APPEND              1
+               424         168 LIST_APPEND              1
                
-               433         170 LOAD_FAST                4 (y2)
+               436         170 LOAD_FAST                4 (y2)
                
-               421         172 LIST_APPEND              1
+               424         172 LIST_APPEND              1
                
-               434         174 LOAD_FAST                1 (x1)
+               437         174 LOAD_FAST                1 (x1)
                            176 LOAD_FAST                5 (radius)
                            178 BINARY_OP                0 (+)
                
-               421         182 LIST_APPEND              1
+               424         182 LIST_APPEND              1
                
-               434         184 LOAD_FAST                4 (y2)
+               437         184 LOAD_FAST                4 (y2)
                
-               421         186 LIST_APPEND              1
+               424         186 LIST_APPEND              1
                
-               435         188 LOAD_FAST                1 (x1)
+               438         188 LOAD_FAST                1 (x1)
                
-               421         190 LIST_APPEND              1
+               424         190 LIST_APPEND              1
                
-               435         192 LOAD_FAST                4 (y2)
+               438         192 LOAD_FAST                4 (y2)
                
-               421         194 LIST_APPEND              1
+               424         194 LIST_APPEND              1
                
-               436         196 LOAD_FAST                1 (x1)
+               439         196 LOAD_FAST                1 (x1)
                
-               421         198 LIST_APPEND              1
+               424         198 LIST_APPEND              1
                
-               436         200 LOAD_FAST                4 (y2)
+               439         200 LOAD_FAST                4 (y2)
                            202 LOAD_FAST                5 (radius)
                            204 BINARY_OP               10 (-)
                
-               421         208 LIST_APPEND              1
+               424         208 LIST_APPEND              1
                
-               437         210 LOAD_FAST                1 (x1)
+               440         210 LOAD_FAST                1 (x1)
                
-               421         212 LIST_APPEND              1
+               424         212 LIST_APPEND              1
                
-               437         214 LOAD_FAST                4 (y2)
+               440         214 LOAD_FAST                4 (y2)
                            216 LOAD_FAST                5 (radius)
                            218 BINARY_OP               10 (-)
                
-               421         222 LIST_APPEND              1
+               424         222 LIST_APPEND              1
                
-               438         224 LOAD_FAST                1 (x1)
+               441         224 LOAD_FAST                1 (x1)
                
-               421         226 LIST_APPEND              1
+               424         226 LIST_APPEND              1
                
-               438         228 LOAD_FAST                2 (y1)
+               441         228 LOAD_FAST                2 (y1)
                            230 LOAD_FAST                5 (radius)
                            232 BINARY_OP                0 (+)
                
-               421         236 LIST_APPEND              1
+               424         236 LIST_APPEND              1
                
-               439         238 LOAD_FAST                1 (x1)
+               442         238 LOAD_FAST                1 (x1)
                
-               421         240 LIST_APPEND              1
+               424         240 LIST_APPEND              1
                
-               439         242 LOAD_FAST                2 (y1)
+               442         242 LOAD_FAST                2 (y1)
                            244 LOAD_FAST                5 (radius)
                            246 BINARY_OP                0 (+)
                
-               421         250 LIST_APPEND              1
+               424         250 LIST_APPEND              1
                
-               440         252 LOAD_FAST                1 (x1)
+               443         252 LOAD_FAST                1 (x1)
                
-               421         254 LIST_APPEND              1
+               424         254 LIST_APPEND              1
                
-               440         256 LOAD_FAST                2 (y1)
+               443         256 LOAD_FAST                2 (y1)
                
-               421         258 LIST_APPEND              1
+               424         258 LIST_APPEND              1
                            260 STORE_FAST               7 (points)
                
-               442         262 PUSH_NULL
+               445         262 PUSH_NULL
                            264 LOAD_FAST                0 (self)
                            266 LOAD_ATTR                0 (create_polygon)
                            276 LOAD_FAST                7 (points)
                            278 BUILD_TUPLE              1
                            280 BUILD_MAP                0
                            282 LOAD_FAST                6 (kwargs)
                            284 DICT_MERGE               1
                            286 LOAD_CONST               1 ('smooth')
                            288 LOAD_CONST               2 (True)
                            290 BUILD_MAP                1
                            292 DICT_MERGE               1
                            294 CALL_FUNCTION_EX         1
                            296 STORE_FAST               8 (_poly)
                
-               444         298 LOAD_FAST                8 (_poly)
+               447         298 LOAD_FAST                8 (_poly)
                            300 RETURN_VALUE
                consts
                   None
                   'smooth'
                   True
                names      ('create_polygon',)
                varnames   ('self', 'x1', 'y1', 'x2', 'y2', 'radius', 'kwargs', 'points', '_poly')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
                name       'create_round_rectangle4'
-               firstlineno 420
+               firstlineno 423
                lnotab
                   0x0201100108ff020102ff020208fe020202fe020308fd020302fd020402
                   fc020402fc020502fb020508fb020602fa020608fa020702f9020708f902
                   0802f8020808f8020902f7020902f7020a08f6020a02f6020b08f5020b02
                   f5020c08f4020c02f4020d08f3020d02f3020e02f2020e02f2020f02f102
                   0f08f1021002f0021008f0021102ef021108ef021202ee021208ee021302
                   ed021302ed04152402
@@ -1050,25 +1096,25 @@
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000740400000000000000000000a6010000ab010000000000
                   00000001007c006a000000000000000000a0010000000000000000000000
                   00000000000000000064017c019b0064027c029b0064027c039b009d06a6
                   010000ab0100000000000000007d0602007c006a0300000000000000007c
                   0667017c04a201520069007c05a4018e0101007c065300
-               448           0 RESUME                   0
+               451           0 RESUME                   0
                
-               449           2 LOAD_FAST                0 (self)
+               452           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (tk)
                             14 LOAD_METHOD              1 (eval)
                             36 LOAD_GLOBAL              4 (poly)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 POP_TOP
                
-               450          64 LOAD_FAST                0 (self)
+               453          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                0 (tk)
                             76 LOAD_METHOD              1 (eval)
                             98 LOAD_CONST               1 ('poly_round ')
                            100 LOAD_FAST                1 (win)
                            102 FORMAT_VALUE             0
                            104 LOAD_CONST               2 (' ')
                            106 LOAD_FAST                2 (outline)
@@ -1077,67 +1123,67 @@
                            112 LOAD_FAST                3 (fill)
                            114 FORMAT_VALUE             0
                            116 BUILD_STRING             6
                            118 PRECALL                  1
                            122 CALL                     1
                            132 STORE_FAST               6 (_poly)
                
-               451         134 PUSH_NULL
+               454         134 PUSH_NULL
                            136 LOAD_FAST                0 (self)
                            138 LOAD_ATTR                3 (itemconfig)
                            148 LOAD_FAST                6 (_poly)
                            150 BUILD_LIST               1
                            152 LOAD_FAST                4 (args)
                            154 LIST_EXTEND              1
                            156 LIST_TO_TUPLE
                            158 BUILD_MAP                0
                            160 LOAD_FAST                5 (kwargs)
                            162 DICT_MERGE               1
                            164 CALL_FUNCTION_EX         1
                            166 POP_TOP
                
-               452         168 LOAD_FAST                6 (_poly)
+               455         168 LOAD_FAST                6 (_poly)
                            170 RETURN_VALUE
                consts
                   None
                   'poly_round '
                   ' '
                names      ('tk', 'eval', 'poly', 'itemconfig')
                varnames   ('self', 'win', 'outline', 'fill', 'args', 'kwargs', '_poly')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
                name       'polygon_round'
-               firstlineno 448
+               firstlineno 451
                lnotab 0x02013e0146012201
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x970064017d017c006a000000000000000000a001000000000000000000
                   0000000000000000000000740400000000000000000000a6010000ab0100
                   0000000000000001007c006a000000000000000000a00100000000000000
                   000000000000000000000000007c01a6010000ab01000000000000000001
                   0064005300
-               456           0 RESUME                   0
+               459           0 RESUME                   0
                
-               457           2 LOAD_CONST               1 ('\n package require Tcl 8.5\n package require Tk\n\n proc draw {win} {\n     global demo\n\n     set sharp_pts [list]\n     set round_pts [list]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {([lindex [$win coords vtx#$id] 0] +\n                       [lindex [$win coords vtx#$id] 2]) / 2}]\n         set y [expr {([lindex [$win coords vtx#$id] 1] +\n                       [lindex [$win coords vtx#$id] 3]) / 2}]\n         lappend sharp_pts $x $y\n         lappend round_pts $x $y $demo(radius)\n     }\n\n     .c delete sharp_poly\n     .c create polygon {*}$sharp_pts -outline gray50 -fill ""             -dash {6 5} -tags {sharp_poly}\n\n     if {[info exists demo(tag)]} {\n         .c delete $demo(tag)\n     }\n     set demo(tag) [poly_round .c $demo(outline) $demo(fill) {*}$round_pts]\n     .c itemconfigure $demo(tag) -width $demo(thickness)\n\n     .c raise vtx\n }\n\n proc down {win x y} {\n     global demo\n\n     $win dtag selected\n     $win addtag selected withtag current\n     $win raise current\n     set demo(last_x) $x\n     set demo(last_y) $y\n }\n \n proc move {win x y} {\n     global demo\n\n     if {[info exists demo(last_x)]} {\n         $win move selected                 [expr {$x - $demo(last_x)}]                 [expr {$y - $demo(last_y)}]\n         set demo(last_x) $x\n         set demo(last_y) $y\n\n         draw $win\n     }\n }\n\n proc main {args} {\n     global demo\n\n     array set demo {\n         num_pts 3       radius 20      thickness 1\n         outline black   fill   white   background gray\n         width   400     height 400\n     }\n     foreach {option value} $args {\n         set option [regsub {^-} $option ""]\n         if {![info exists demo($option)]} {\n             puts "Options: -[join [array names demo] " -"]"\n             exit\n         } else {\n             set demo([regsub {^-} $option ""]) $value\n         }\n     }\n\n     canvas .c -width $demo(width) -height $demo(height) -highlightthickness 0             -background $demo(background)\n     pack .c\n     wm title . "Round Polygon Demo"\n     wm resizable . 0 0\n\n     set 2pi [expr {2 * acos(-1)}]\n     set cx [expr {$demo(width)  / 2}]; set sx [expr {$demo(width)  * 3 / 8}]\n     set cy [expr {$demo(height) / 2}]; set sy [expr {$demo(height) * 3 / 8}]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {$cx + $sx * cos(($id + 0.5) * $2pi / $demo(num_pts))}]\n         set y [expr {$cy - $sy * sin(($id + 0.5) * $2pi / $demo(num_pts))}]\n         .c create oval [expr {$x - 3}] [expr {$y - 3}]                        [expr {$x + 3}] [expr {$y + 3}]                        -tags [list vtx vtx#$id] -fill brown\n     }\n\n     .c bind vtx <Any-Enter> {.c itemconfigure current -fill red}\n     .c bind vtx <Any-Leave> {.c itemconfigure current -fill brown}\n     .c bind vtx <ButtonPress-1> {down .c %x %y}\n     .c bind vtx <ButtonRelease-1> {.c dtag selected}\n     bind .c <B1-Motion> {move .c %x %y}\n\n     focus .c\n     draw .c\n }\n\n main\n\n        ')
+               460           2 LOAD_CONST               1 ('\n package require Tcl 8.5\n package require Tk\n\n proc draw {win} {\n     global demo\n\n     set sharp_pts [list]\n     set round_pts [list]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {([lindex [$win coords vtx#$id] 0] +\n                       [lindex [$win coords vtx#$id] 2]) / 2}]\n         set y [expr {([lindex [$win coords vtx#$id] 1] +\n                       [lindex [$win coords vtx#$id] 3]) / 2}]\n         lappend sharp_pts $x $y\n         lappend round_pts $x $y $demo(radius)\n     }\n\n     .c delete sharp_poly\n     .c create polygon {*}$sharp_pts -outline gray50 -fill ""             -dash {6 5} -tags {sharp_poly}\n\n     if {[info exists demo(tag)]} {\n         .c delete $demo(tag)\n     }\n     set demo(tag) [poly_round .c $demo(outline) $demo(fill) {*}$round_pts]\n     .c itemconfigure $demo(tag) -width $demo(thickness)\n\n     .c raise vtx\n }\n\n proc down {win x y} {\n     global demo\n\n     $win dtag selected\n     $win addtag selected withtag current\n     $win raise current\n     set demo(last_x) $x\n     set demo(last_y) $y\n }\n \n proc move {win x y} {\n     global demo\n\n     if {[info exists demo(last_x)]} {\n         $win move selected                 [expr {$x - $demo(last_x)}]                 [expr {$y - $demo(last_y)}]\n         set demo(last_x) $x\n         set demo(last_y) $y\n\n         draw $win\n     }\n }\n\n proc main {args} {\n     global demo\n\n     array set demo {\n         num_pts 3       radius 20      thickness 1\n         outline black   fill   white   background gray\n         width   400     height 400\n     }\n     foreach {option value} $args {\n         set option [regsub {^-} $option ""]\n         if {![info exists demo($option)]} {\n             puts "Options: -[join [array names demo] " -"]"\n             exit\n         } else {\n             set demo([regsub {^-} $option ""]) $value\n         }\n     }\n\n     canvas .c -width $demo(width) -height $demo(height) -highlightthickness 0             -background $demo(background)\n     pack .c\n     wm title . "Round Polygon Demo"\n     wm resizable . 0 0\n\n     set 2pi [expr {2 * acos(-1)}]\n     set cx [expr {$demo(width)  / 2}]; set sx [expr {$demo(width)  * 3 / 8}]\n     set cy [expr {$demo(height) / 2}]; set sy [expr {$demo(height) * 3 / 8}]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {$cx + $sx * cos(($id + 0.5) * $2pi / $demo(num_pts))}]\n         set y [expr {$cy - $sy * sin(($id + 0.5) * $2pi / $demo(num_pts))}]\n         .c create oval [expr {$x - 3}] [expr {$y - 3}]                        [expr {$x + 3}] [expr {$y + 3}]                        -tags [list vtx vtx#$id] -fill brown\n     }\n\n     .c bind vtx <Any-Enter> {.c itemconfigure current -fill red}\n     .c bind vtx <Any-Leave> {.c itemconfigure current -fill brown}\n     .c bind vtx <ButtonPress-1> {down .c %x %y}\n     .c bind vtx <ButtonRelease-1> {.c dtag selected}\n     bind .c <B1-Motion> {move .c %x %y}\n\n     focus .c\n     draw .c\n }\n\n main\n\n        ')
                              4 STORE_FAST               1 (demo)
                
-               561           6 LOAD_FAST                0 (self)
+               564           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (tk)
                             18 LOAD_METHOD              1 (eval)
                             40 LOAD_GLOBAL              4 (poly)
                             52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
                
-               562          68 LOAD_FAST                0 (self)
+               565          68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                0 (tk)
                             80 LOAD_METHOD              1 (eval)
                            102 LOAD_FAST                1 (demo)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 POP_TOP
                            120 LOAD_CONST               0 (None)
@@ -1147,15 +1193,15 @@
                   '\n package require Tcl 8.5\n package require Tk\n\n proc draw {win} {\n     global demo\n\n     set sharp_pts [list]\n     set round_pts [list]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {([lindex [$win coords vtx#$id] 0] +\n                       [lindex [$win coords vtx#$id] 2]) / 2}]\n         set y [expr {([lindex [$win coords vtx#$id] 1] +\n                       [lindex [$win coords vtx#$id] 3]) / 2}]\n         lappend sharp_pts $x $y\n         lappend round_pts $x $y $demo(radius)\n     }\n\n     .c delete sharp_poly\n     .c create polygon {*}$sharp_pts -outline gray50 -fill ""             -dash {6 5} -tags {sharp_poly}\n\n     if {[info exists demo(tag)]} {\n         .c delete $demo(tag)\n     }\n     set demo(tag) [poly_round .c $demo(outline) $demo(fill) {*}$round_pts]\n     .c itemconfigure $demo(tag) -width $demo(thickness)\n\n     .c raise vtx\n }\n\n proc down {win x y} {\n     global demo\n\n     $win dtag selected\n     $win addtag selected withtag current\n     $win raise current\n     set demo(last_x) $x\n     set demo(last_y) $y\n }\n \n proc move {win x y} {\n     global demo\n\n     if {[info exists demo(last_x)]} {\n         $win move selected                 [expr {$x - $demo(last_x)}]                 [expr {$y - $demo(last_y)}]\n         set demo(last_x) $x\n         set demo(last_y) $y\n\n         draw $win\n     }\n }\n\n proc main {args} {\n     global demo\n\n     array set demo {\n         num_pts 3       radius 20      thickness 1\n         outline black   fill   white   background gray\n         width   400     height 400\n     }\n     foreach {option value} $args {\n         set option [regsub {^-} $option ""]\n         if {![info exists demo($option)]} {\n             puts "Options: -[join [array names demo] " -"]"\n             exit\n         } else {\n             set demo([regsub {^-} $option ""]) $value\n         }\n     }\n\n     canvas .c -width $demo(width) -height $demo(height) -highlightthickness 0             -background $demo(background)\n     pack .c\n     wm title . "Round Polygon Demo"\n     wm resizable . 0 0\n\n     set 2pi [expr {2 * acos(-1)}]\n     set cx [expr {$demo(width)  / 2}]; set sx [expr {$demo(width)  * 3 / 8}]\n     set cy [expr {$demo(height) / 2}]; set sy [expr {$demo(height) * 3 / 8}]\n     for {set id 0} {$id < $demo(num_pts)} {incr id} {\n         set x [expr {$cx + $sx * cos(($id + 0.5) * $2pi / $demo(num_pts))}]\n         set y [expr {$cy - $sy * sin(($id + 0.5) * $2pi / $demo(num_pts))}]\n         .c create oval [expr {$x - 3}] [expr {$y - 3}]                        [expr {$x + 3}] [expr {$y + 3}]                        -tags [list vtx vtx#$id] -fill brown\n     }\n\n     .c bind vtx <Any-Enter> {.c itemconfigure current -fill red}\n     .c bind vtx <Any-Leave> {.c itemconfigure current -fill brown}\n     .c bind vtx <ButtonPress-1> {down .c %x %y}\n     .c bind vtx <ButtonRelease-1> {.c dtag selected}\n     bind .c <B1-Motion> {move .c %x %y}\n\n     focus .c\n     draw .c\n }\n\n main\n\n        '
                names      ('tk', 'eval', 'poly')
                varnames   ('self', 'demo')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
                name       'demo_polygon_round'
-               firstlineno 456
+               firstlineno 459
                lnotab 0x020104683e01
             'content'
             code
                argcount  : 4
                nlocals   : 12
                stacksize : 6
                flags     : 11
@@ -1167,68 +1213,68 @@
                   097c09a00600000000000000000000000000000000000000007c03a60100
                   00ab01000000000000000001007c09a00700000000000000000000000000
                   00000000000000a6000000ab0000000000000000000100640064006400a6
                   020000ab02000000000000000001006e0b23003100730477027803590077
                   01010059000100010002007c067c08ac07a6010000ab0100000000000000
                   007d0a02007c006a0800000000000000007c017c02660264087c0a69017c
                   04a4018e017d0b7c0b5300
-               564           0 RESUME                   0
+               567           0 RESUME                   0
                
-               565           2 LOAD_CONST               1 (0)
+               568           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('mkstemp',))
                              6 IMPORT_NAME              0 (tempfile)
                              8 IMPORT_FROM              1 (mkstemp)
                             10 STORE_FAST               5 (mkstemp)
                             12 POP_TOP
                
-               566          14 LOAD_CONST               1 (0)
+               569          14 LOAD_CONST               1 (0)
                             16 LOAD_CONST               3 (('SvgImage',))
                             18 IMPORT_NAME              2 (tksvg)
                             20 IMPORT_FROM              3 (SvgImage)
                             22 STORE_FAST               6 (SvgImage)
                             24 POP_TOP
                
-               568          26 PUSH_NULL
+               571          26 PUSH_NULL
                             28 LOAD_FAST                5 (mkstemp)
                             30 LOAD_CONST               4 ('.svg')
                             32 KW_NAMES                 5
                             34 PRECALL                  1
                             38 CALL                     1
                             48 UNPACK_SEQUENCE          2
                             52 STORE_FAST               7 (_)
                             54 STORE_FAST               8 (file)
                
-               569          56 LOAD_GLOBAL              9 (NULL + print)
+               572          56 LOAD_GLOBAL              9 (NULL + print)
                             68 LOAD_FAST                8 (file)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 POP_TOP
                
-               570          86 LOAD_GLOBAL             11 (NULL + open)
+               573          86 LOAD_GLOBAL             11 (NULL + open)
                             98 LOAD_FAST                8 (file)
                            100 LOAD_CONST               6 ('w')
                            102 PRECALL                  2
                            106 CALL                     2
                            116 BEFORE_WITH
                            118 STORE_FAST               9 (f)
                
-               571         120 LOAD_FAST                9 (f)
+               574         120 LOAD_FAST                9 (f)
                            122 LOAD_METHOD              6 (write)
                            144 LOAD_FAST                3 (content)
                            146 PRECALL                  1
                            150 CALL                     1
                            160 POP_TOP
                
-               572         162 LOAD_FAST                9 (f)
+               575         162 LOAD_FAST                9 (f)
                            164 LOAD_METHOD              7 (close)
                            186 PRECALL                  0
                            190 CALL                     0
                            200 POP_TOP
                
-               570         202 LOAD_CONST               0 (None)
+               573         202 LOAD_CONST               0 (None)
                            204 LOAD_CONST               0 (None)
                            206 LOAD_CONST               0 (None)
                            208 PRECALL                  2
                            212 CALL                     2
                            222 POP_TOP
                            224 JUMP_FORWARD            11 (to 248)
                        >>  226 PUSH_EXC_INFO
@@ -1239,37 +1285,37 @@
                            236 POP_EXCEPT
                            238 RERAISE                  1
                        >>  240 POP_TOP
                            242 POP_EXCEPT
                            244 POP_TOP
                            246 POP_TOP
                
-               573     >>  248 PUSH_NULL
+               576     >>  248 PUSH_NULL
                            250 LOAD_FAST                6 (SvgImage)
                            252 LOAD_FAST                8 (file)
                            254 KW_NAMES                 7
                            256 PRECALL                  1
                            260 CALL                     1
                            270 STORE_FAST              10 (image)
                
-               575         272 PUSH_NULL
+               578         272 PUSH_NULL
                            274 LOAD_FAST                0 (self)
                            276 LOAD_ATTR                8 (create_image)
                            286 LOAD_FAST                1 (x)
                            288 LOAD_FAST                2 (y)
                            290 BUILD_TUPLE              2
                            292 LOAD_CONST               8 ('image')
                            294 LOAD_FAST               10 (image)
                            296 BUILD_MAP                1
                            298 LOAD_FAST                4 (kwargs)
                            300 DICT_MERGE               1
                            302 CALL_FUNCTION_EX         1
                            304 STORE_FAST              11 (i)
                
-               577         306 LOAD_FAST               11 (i)
+               580         306 LOAD_FAST               11 (i)
                            308 RETURN_VALUE
                ExceptionTable:
                  118 to 200 -> 226 [1] lasti
                  226 to 232 -> 234 [3] lasti
                  240 to 240 -> 234 [3] lasti
                consts
                   None
@@ -1283,28 +1329,29 @@
                   'image'
                names      ('tempfile', 'mkstemp', 'tksvg', 'SvgImage', 'print', 'open', 'write', 'close', 'create_image')
                varnames   ('self', 'x', 'y', 'content', 'kwargs', 'mkstemp', 'SvgImage', '_', 'file', 'f', 'image', 'i')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
                name       'create_svg_image'
-               firstlineno 564
+               firstlineno 567
                lnotab 0x02010c010c021e011e0122012a0128fe2e0318022202
-            None
             ('x',)
             (5, 2, 'white', 'black')
             ('black', 'black')
-         names      ('__name__', '__module__', '__qualname__', 'win32_high_dpi', 'draw_gradient', 'float', 'create_round_rectangle', 'create_round_rect', 'create_round_rectangle2', 'create_round_rect2', 'str', 'create_round_rectangle3', 'create_round_rect3', 'create_round_rectangle4', 'create_round_rect4', 'polygon_round', 'poly_round', 'demo_polygon_round', 'create_svg_image')
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'win32_high_dpi', 'draw_gradient', 'float', 'create_round_rectangle', 'create_round_rect', 'create_round_rectangle2', 'create_round_rect2', 'str', 'create_round_rectangle3', 'create_round_rect3', 'create_round_rectangle4', 'create_round_rect4', 'polygon_round', 'poly_round', 'demo_polygon_round', 'create_svg_image', '__classcell__')
          varnames   ()
          freevars   ()
-         cellvars   ()
+         cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
          name       'AdwDrawEngine'
          firstlineno 226
-         lnotab 0x0a01060408430e1f04020644040212110402061a040208060402066c
+         lnotab
+            0x0c010a03060408430e1f04020644040212110402061a04020806040206
+            6c
       'AdwDrawEngine'
       '__main__'
       ('Tk',)
       10
       15
       150
       50
@@ -1315,15 +1362,15 @@
          argcount  : 1
          nlocals   : 1
          stacksize : 5
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             00000000000000640164026403a6030000ab0300000000000000005300
-         590           0 RESUME                   0
+         593           0 RESUME                   0
                        2 LOAD_GLOBAL              0 (canvas)
                       14 LOAD_METHOD              1 (draw_gradient)
                       36 LOAD_CONST               1 ('#87e9bb')
                       38 LOAD_CONST               2 ('#d3a6f5')
                       40 LOAD_CONST               3 ('x')
                       42 PRECALL                  3
                       46 CALL                     3
@@ -1335,23 +1382,23 @@
             'x'
          names      ('canvas', 'draw_gradient')
          varnames   ('event',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
          name       '<lambda>'
-         firstlineno 590
+         firstlineno 593
          lnotab 0x
       'both'
       'yes'
       ('fill', 'expand')
       None
    names      ('tkinter', 'Canvas', 'poly', 'poly2', 'AdwDrawEngine', '__name__', 'Tk', 'root', 'canvas', 'create_round_rect3', 'create_round_rect4', 'bind', 'pack', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\canvas\\drawengine.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c02047f0015044b1c7f007f00640c010c0214021402340132
+      0x00ff02010c02047f0015044b1c7f007f00670c010c0214021402340132
       022e022e022cf2
```

### Comparing `tkadw-0.1.1/tkadw/canvas/__pycache__/entry.cpython-311.pyc` & `tkadw-0.1.2/tkadw/canvas/__pycache__/entry.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x49149564 (Fri Jun 23 03:40:57 2023 UTC)
-files sz: 22085
+moddate:  0x624e9564 (Fri Jun 23 07:48:50 2023 UTC)
+files sz: 22377
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -58,229 +58,229 @@
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               4 ('AdwDrawBasicEntry')
                 40 LOAD_NAME                4 (AdwDrawEngine)
                 42 PRECALL                  3
                 46 CALL                     3
                 56 STORE_NAME               5 (AdwDrawBasicEntry)
    
-   207          58 PUSH_NULL
+   210          58 PUSH_NULL
                 60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               5 (<code object AdwDrawEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 207>)
+                62 LOAD_CONST               5 (<code object AdwDrawEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 210>)
                 64 MAKE_FUNCTION            0
                 66 LOAD_CONST               6 ('AdwDrawEntry')
                 68 LOAD_NAME                5 (AdwDrawBasicEntry)
                 70 PRECALL                  3
                 74 CALL                     3
                 84 STORE_NAME               6 (AdwDrawEntry)
    
-   212          86 PUSH_NULL
+   215          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object AdwDrawDarkEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 212>)
+                90 LOAD_CONST               7 (<code object AdwDrawDarkEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 215>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('AdwDrawDarkEntry')
                 96 LOAD_NAME                5 (AdwDrawBasicEntry)
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME               7 (AdwDrawDarkEntry)
    
-   218         114 PUSH_NULL
+   221         114 PUSH_NULL
                116 LOAD_BUILD_CLASS
-               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 218>)
+               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 221>)
                120 MAKE_FUNCTION            0
                122 LOAD_CONST              10 ('AdwDrawBasicRoundEntry')
                124 LOAD_NAME                5 (AdwDrawBasicEntry)
                126 PRECALL                  3
                130 CALL                     3
                140 STORE_NAME               8 (AdwDrawBasicRoundEntry)
    
-   396         142 PUSH_NULL
+   400         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object AdwDrawRoundEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 396>)
+               146 LOAD_CONST              11 (<code object AdwDrawRoundEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 400>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('AdwDrawRoundEntry')
                152 LOAD_NAME                8 (AdwDrawBasicRoundEntry)
                154 PRECALL                  3
                158 CALL                     3
                168 STORE_NAME               9 (AdwDrawRoundEntry)
    
-   401         170 PUSH_NULL
+   405         170 PUSH_NULL
                172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 401>)
+               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkEntry, file "D:\tkadw\tkadw\canvas\entry.py", line 405>)
                176 MAKE_FUNCTION            0
                178 LOAD_CONST              14 ('AdwDrawRoundDarkEntry')
                180 LOAD_NAME                8 (AdwDrawBasicRoundEntry)
                182 PRECALL                  3
                186 CALL                     3
                196 STORE_NAME              10 (AdwDrawRoundDarkEntry)
    
-   406         198 PUSH_NULL
+   410         198 PUSH_NULL
                200 LOAD_BUILD_CLASS
-               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 406>)
+               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 410>)
                204 MAKE_FUNCTION            0
                206 LOAD_CONST              16 ('AdwDrawBasicRoundEntry3')
                208 LOAD_NAME                5 (AdwDrawBasicEntry)
                210 PRECALL                  3
                214 CALL                     3
                224 STORE_NAME              11 (AdwDrawBasicRoundEntry3)
    
-   590         226 PUSH_NULL
+   594         226 PUSH_NULL
                228 LOAD_BUILD_CLASS
-               230 LOAD_CONST              17 (<code object AdwDrawRoundEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 590>)
+               230 LOAD_CONST              17 (<code object AdwDrawRoundEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 594>)
                232 MAKE_FUNCTION            0
                234 LOAD_CONST              18 ('AdwDrawRoundEntry3')
                236 LOAD_NAME               11 (AdwDrawBasicRoundEntry3)
                238 PRECALL                  3
                242 CALL                     3
                252 STORE_NAME              12 (AdwDrawRoundEntry3)
    
-   595         254 PUSH_NULL
+   599         254 PUSH_NULL
                256 LOAD_BUILD_CLASS
-               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 595>)
+               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkEntry3, file "D:\tkadw\tkadw\canvas\entry.py", line 599>)
                260 MAKE_FUNCTION            0
                262 LOAD_CONST              20 ('AdwDrawRoundDarkEntry3')
                264 LOAD_NAME               11 (AdwDrawBasicRoundEntry3)
                266 PRECALL                  3
                270 CALL                     3
                280 STORE_NAME              13 (AdwDrawRoundDarkEntry3)
    
-   600         282 LOAD_NAME               14 (__name__)
+   604         282 LOAD_NAME               14 (__name__)
                284 LOAD_CONST              21 ('__main__')
                286 COMPARE_OP               2 (==)
                292 POP_JUMP_FORWARD_IF_FALSE   254 (to 802)
    
-   601         294 LOAD_CONST               0 (0)
+   605         294 LOAD_CONST               0 (0)
                296 LOAD_CONST              22 (('Tk',))
                298 IMPORT_NAME             15 (tkinter)
                300 IMPORT_FROM             16 (Tk)
                302 STORE_NAME              16 (Tk)
                304 POP_TOP
    
-   603         306 PUSH_NULL
+   607         306 PUSH_NULL
                308 LOAD_NAME               16 (Tk)
                310 PRECALL                  0
                314 CALL                     0
                324 STORE_NAME              17 (root)
    
-   605         326 PUSH_NULL
+   609         326 PUSH_NULL
                328 LOAD_NAME                6 (AdwDrawEntry)
                330 LOAD_CONST              23 ('Hello')
                332 KW_NAMES                24
                334 PRECALL                  1
                338 CALL                     1
                348 STORE_NAME              18 (entry1)
    
-   606         350 LOAD_NAME               18 (entry1)
+   610         350 LOAD_NAME               18 (entry1)
                352 LOAD_METHOD             19 (pack)
                374 LOAD_CONST              25 ('x')
                376 LOAD_CONST              26 (5)
                378 LOAD_CONST              26 (5)
                380 KW_NAMES                27
                382 PRECALL                  3
                386 CALL                     3
                396 POP_TOP
    
-   608         398 PUSH_NULL
+   612         398 PUSH_NULL
                400 LOAD_NAME                7 (AdwDrawDarkEntry)
                402 LOAD_CONST              23 ('Hello')
                404 KW_NAMES                24
                406 PRECALL                  1
                410 CALL                     1
                420 STORE_NAME              20 (entry2)
    
-   609         422 LOAD_NAME               20 (entry2)
+   613         422 LOAD_NAME               20 (entry2)
                424 LOAD_METHOD             19 (pack)
                446 LOAD_CONST              25 ('x')
                448 LOAD_CONST              26 (5)
                450 LOAD_CONST              26 (5)
                452 KW_NAMES                27
                454 PRECALL                  3
                458 CALL                     3
                468 POP_TOP
    
-   611         470 PUSH_NULL
+   615         470 PUSH_NULL
                472 LOAD_NAME                9 (AdwDrawRoundEntry)
                474 LOAD_CONST              23 ('Hello')
                476 KW_NAMES                24
                478 PRECALL                  1
                482 CALL                     1
                492 STORE_NAME              21 (entry3)
    
-   612         494 LOAD_NAME               21 (entry3)
+   616         494 LOAD_NAME               21 (entry3)
                496 LOAD_METHOD             19 (pack)
                518 LOAD_CONST              25 ('x')
                520 LOAD_CONST              26 (5)
                522 LOAD_CONST              26 (5)
                524 KW_NAMES                27
                526 PRECALL                  3
                530 CALL                     3
                540 POP_TOP
    
-   614         542 PUSH_NULL
+   618         542 PUSH_NULL
                544 LOAD_NAME               10 (AdwDrawRoundDarkEntry)
                546 LOAD_CONST              23 ('Hello')
                548 KW_NAMES                24
                550 PRECALL                  1
                554 CALL                     1
                564 STORE_NAME              22 (entry4)
    
-   615         566 LOAD_NAME               22 (entry4)
+   619         566 LOAD_NAME               22 (entry4)
                568 LOAD_METHOD             19 (pack)
                590 LOAD_CONST              25 ('x')
                592 LOAD_CONST              26 (5)
                594 LOAD_CONST              26 (5)
                596 KW_NAMES                27
                598 PRECALL                  3
                602 CALL                     3
                612 POP_TOP
    
-   617         614 PUSH_NULL
+   621         614 PUSH_NULL
                616 LOAD_NAME               12 (AdwDrawRoundEntry3)
                618 LOAD_CONST              23 ('Hello')
                620 KW_NAMES                24
                622 PRECALL                  1
                626 CALL                     1
                636 STORE_NAME              23 (entry5)
    
-   618         638 LOAD_NAME               23 (entry5)
+   622         638 LOAD_NAME               23 (entry5)
                640 LOAD_METHOD             19 (pack)
                662 LOAD_CONST              25 ('x')
                664 LOAD_CONST              26 (5)
                666 LOAD_CONST              26 (5)
                668 KW_NAMES                27
                670 PRECALL                  3
                674 CALL                     3
                684 POP_TOP
    
-   620         686 PUSH_NULL
+   624         686 PUSH_NULL
                688 LOAD_NAME               13 (AdwDrawRoundDarkEntry3)
                690 LOAD_CONST              23 ('Hello')
                692 KW_NAMES                24
                694 PRECALL                  1
                698 CALL                     1
                708 STORE_NAME              24 (entry6)
    
-   621         710 LOAD_NAME               24 (entry6)
+   625         710 LOAD_NAME               24 (entry6)
                712 LOAD_METHOD             19 (pack)
                734 LOAD_CONST              25 ('x')
                736 LOAD_CONST              26 (5)
                738 LOAD_CONST              26 (5)
                740 KW_NAMES                27
                742 PRECALL                  3
                746 CALL                     3
                756 POP_TOP
    
-   623         758 LOAD_NAME               17 (root)
+   627         758 LOAD_NAME               17 (root)
                760 LOAD_METHOD             25 (mainloop)
                782 PRECALL                  0
                786 CALL                     0
                796 POP_TOP
                798 LOAD_CONST              28 (None)
                800 RETURN_VALUE
    
-   600     >>  802 LOAD_CONST              28 (None)
+   604     >>  802 LOAD_CONST              28 (None)
                804 RETURN_VALUE
    consts
       0
       ('Font', 'nametofont')
       ('AdwDrawEngine',)
       code
          argcount  : 0
@@ -331,61 +331,61 @@
                       58 MAKE_FUNCTION            0
                       60 STORE_NAME               7 (_other)
          
           53          62 LOAD_CONST              10 (<code object _draw, file "D:\tkadw\tkadw\canvas\entry.py", line 53>)
                       64 MAKE_FUNCTION            0
                       66 STORE_NAME               8 (_draw)
          
-          78          68 LOAD_CONST              23 ((None,))
-                      70 LOAD_CONST              12 (<code object _focus, file "D:\tkadw\tkadw\canvas\entry.py", line 78>)
+          81          68 LOAD_CONST              23 ((None,))
+                      70 LOAD_CONST              12 (<code object _focus, file "D:\tkadw\tkadw\canvas\entry.py", line 81>)
                       72 MAKE_FUNCTION            1 (defaults)
                       74 STORE_NAME               9 (_focus)
          
-          87          76 LOAD_CONST              23 ((None,))
-                      78 LOAD_CONST              13 (<code object _focusout, file "D:\tkadw\tkadw\canvas\entry.py", line 87>)
+          90          76 LOAD_CONST              23 ((None,))
+                      78 LOAD_CONST              13 (<code object _focusout, file "D:\tkadw\tkadw\canvas\entry.py", line 90>)
                       80 MAKE_FUNCTION            1 (defaults)
                       82 STORE_NAME              10 (_focusout)
          
-          96          84 LOAD_CONST              23 ((None,))
-                      86 LOAD_CONST              14 (<code object _click, file "D:\tkadw\tkadw\canvas\entry.py", line 96>)
+          99          84 LOAD_CONST              23 ((None,))
+                      86 LOAD_CONST              14 (<code object _click, file "D:\tkadw\tkadw\canvas\entry.py", line 99>)
                       88 MAKE_FUNCTION            1 (defaults)
                       90 STORE_NAME              11 (_click)
          
-          99          92 LOAD_CONST              23 ((None,))
-                      94 LOAD_CONST              15 (<code object _hover, file "D:\tkadw\tkadw\canvas\entry.py", line 99>)
+         102          92 LOAD_CONST              23 ((None,))
+                      94 LOAD_CONST              15 (<code object _hover, file "D:\tkadw\tkadw\canvas\entry.py", line 102>)
                       96 MAKE_FUNCTION            1 (defaults)
                       98 STORE_NAME              12 (_hover)
          
-         102         100 LOAD_CONST              23 ((None,))
-                     102 LOAD_CONST              16 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\entry.py", line 102>)
+         105         100 LOAD_CONST              23 ((None,))
+                     102 LOAD_CONST              16 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\entry.py", line 105>)
                      104 MAKE_FUNCTION            1 (defaults)
                      106 STORE_NAME              13 (_hover_release)
          
-         113         108 LOAD_CONST              23 ((None,))
+         116         108 LOAD_CONST              23 ((None,))
                      110 LOAD_CONST              17 ('font')
                      112 LOAD_NAME               14 (Font)
                      114 BUILD_TUPLE              2
-                     116 LOAD_CONST              18 (<code object font, file "D:\tkadw\tkadw\canvas\entry.py", line 113>)
+                     116 LOAD_CONST              18 (<code object font, file "D:\tkadw\tkadw\canvas\entry.py", line 116>)
                      118 MAKE_FUNCTION            5 (defaults, annotations)
                      120 STORE_NAME              15 (font)
          
-         119         122 LOAD_CONST              19 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 119>)
+         122         122 LOAD_CONST              19 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 122>)
                      124 MAKE_FUNCTION            0
                      126 STORE_NAME              16 (default_palette)
          
-         122         128 LOAD_CONST              20 (<code object palette_light, file "D:\tkadw\tkadw\canvas\entry.py", line 122>)
+         125         128 LOAD_CONST              20 (<code object palette_light, file "D:\tkadw\tkadw\canvas\entry.py", line 125>)
                      130 MAKE_FUNCTION            0
                      132 STORE_NAME              17 (palette_light)
          
-         144         134 LOAD_CONST              21 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\entry.py", line 144>)
+         147         134 LOAD_CONST              21 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\entry.py", line 147>)
                      136 MAKE_FUNCTION            0
                      138 STORE_NAME              18 (palette_dark)
          
-         166         140 LOAD_CONST              23 ((None,))
-                     142 LOAD_CONST              22 (<code object palette, file "D:\tkadw\tkadw\canvas\entry.py", line 166>)
+         169         140 LOAD_CONST              23 ((None,))
+                     142 LOAD_CONST              22 (<code object palette, file "D:\tkadw\tkadw\canvas\entry.py", line 169>)
                      144 MAKE_FUNCTION            1 (defaults)
                      146 STORE_NAME              19 (palette)
                      148 LOAD_CLOSURE             0 (__class__)
                      150 COPY                     1
                      152 STORE_NAME              20 (__classcell__)
                      154 RETURN_VALUE
          consts
@@ -394,256 +394,257 @@
             40
             ''
             ('width', 'height', 'text')
             'text'
             code
                argcount  : 1
                nlocals   : 8
-               stacksize : 6
+               stacksize : 7
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
-                  0000006a0100000000000000007c047c017c0264019c027c05a4018e0101
-                  00640264036c026d037d066d047d07010002007c06a6000000ab00000000
-                  00000000007c005f0500000000000000007c006a050000000000000000a0
-                  0600000000000000000000000000000000000000007c03a6010000ab0100
-                  00000000000000010002007c077c0064027c006a050000000000000000ac
-                  04a6030000ab0300000000000000007c005f0700000000000000007c00a0
-                  080000000000000000000000000000000000000000a6000000ab00000000
-                  000000000001007c00a00900000000000000000000000000000000000000
-                  00a6000000ab00000000000000000001007c037c005f0a00000000000000
-                  007c006a0b00000000000000007c005f0c00000000000000007c006a0d00
-                  000000000000007c005f0e00000000000000007c006a0f00000000000000
-                  007c005f1000000000000000007c006a1100000000000000007c005f1200
-                  000000000000007c006a1300000000000000007c005f1400000000000000
-                  00742b000000000000000000006405a6010000ab0100000000000000007c
-                  005f1600000000000000007c00a017000000000000000000000000000000
-                  000000000064067c006a1800000000000000006407ac08a6030000ab0300
+                  0000006a0100000000000000007c047c017c02640164029c037c05a4018e
+                  010100640164036c026d037d066d047d07010002007c06a6000000ab0000
+                  000000000000007c005f0500000000000000007c006a0500000000000000
+                  00a00600000000000000000000000000000000000000007c03a6010000ab
+                  010000000000000000010002007c077c0064017c006a0500000000000000
+                  00ac04a6030000ab0300000000000000007c005f0700000000000000007c
+                  00a0080000000000000000000000000000000000000000a6000000ab0000
+                  0000000000000001007c00a0090000000000000000000000000000000000
+                  000000a6000000ab00000000000000000001007c037c005f0a0000000000
+                  0000007c006a0b00000000000000007c005f0c00000000000000007c006a
+                  0d00000000000000007c005f0e00000000000000007c006a0f0000000000
+                  0000007c005f1000000000000000007c006a1100000000000000007c005f
+                  1200000000000000007c006a1300000000000000007c005f140000000000
+                  000000742b000000000000000000006405a6010000ab0100000000000000
+                  007c005f1600000000000000007c00a01700000000000000000000000000
+                  0000000000000064067c006a1800000000000000006407ac08a6030000ab
+                  03000000000000000001007c00a017000000000000000000000000000000
+                  000000000064097c006a1900000000000000006407ac08a6030000ab0300
                   0000000000000001007c00a0170000000000000000000000000000000000
-                  00000064097c006a1900000000000000006407ac08a6030000ab03000000
+                  000000640a7c006a1a00000000000000006407ac08a6030000ab03000000
                   000000000001007c00a01700000000000000000000000000000000000000
-                  00640a7c006a1a00000000000000006407ac08a6030000ab030000000000
+                  00640b7c006a1b00000000000000006407ac08a6030000ab030000000000
                   00000001007c00a017000000000000000000000000000000000000000064
-                  0b7c006a1b00000000000000006407ac08a6030000ab0300000000000000
-                  0001007c00a0170000000000000000000000000000000000000000640c7c
-                  006a1c00000000000000006407ac08a6030000ab03000000000000000001
-                  007c006a070000000000000000a017000000000000000000000000000000
-                  0000000000640c7c006a1c00000000000000006407ac08a6030000ab0300
-                  0000000000000001007c00a0170000000000000000000000000000000000
-                  000000640d7c006a1d00000000000000006407ac08a6030000ab03000000
-                  000000000001007c006a070000000000000000a017000000000000000000
-                  0000000000000000000000640d7c006a1d00000000000000006407ac08a6
-                  030000ab03000000000000000001007c00a0180000000000000000000000
-                  0000000000000000006400a6010000ab0100000000000000000100640053
-                  00
+                  0c7c006a1c00000000000000006407ac08a6030000ab0300000000000000
+                  0001007c006a070000000000000000a01700000000000000000000000000
+                  00000000000000640c7c006a1c00000000000000006407ac08a6030000ab
+                  03000000000000000001007c00a017000000000000000000000000000000
+                  0000000000640d7c006a1d00000000000000006407ac08a6030000ab0300
+                  0000000000000001007c006a070000000000000000a01700000000000000
+                  00000000000000000000000000640d7c006a1d00000000000000006407ac
+                  08a6030000ab03000000000000000001007c00a018000000000000000000
+                  00000000000000000000006400a6010000ab010000000000000000010064
+                  005300
                              0 COPY_FREE_VARS           1
                
                  7           2 RESUME                   0
                
                  9           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                4 (args)
                             44 LOAD_FAST                1 (width)
                             46 LOAD_FAST                2 (height)
-                            48 LOAD_CONST               1 (('width', 'height'))
-                            50 BUILD_CONST_KEY_MAP      2
-                            52 LOAD_FAST                5 (kwargs)
-                            54 DICT_MERGE               1
-                            56 CALL_FUNCTION_EX         1
-                            58 POP_TOP
-               
-                11          60 LOAD_CONST               2 (0)
-                            62 LOAD_CONST               3 (('StringVar', 'Entry'))
-                            64 IMPORT_NAME              2 (tkinter)
-                            66 IMPORT_FROM              3 (StringVar)
-                            68 STORE_FAST               6 (StringVar)
-                            70 IMPORT_FROM              4 (Entry)
-                            72 STORE_FAST               7 (Entry)
-                            74 POP_TOP
-               
-                13          76 PUSH_NULL
-                            78 LOAD_FAST                6 (StringVar)
-                            80 PRECALL                  0
-                            84 CALL                     0
-                            94 LOAD_FAST                0 (self)
-                            96 STORE_ATTR               5 (var)
-               
-                14         106 LOAD_FAST                0 (self)
-                           108 LOAD_ATTR                5 (var)
-                           118 LOAD_METHOD              6 (set)
-                           140 LOAD_FAST                3 (text)
-                           142 PRECALL                  1
-                           146 CALL                     1
-                           156 POP_TOP
-               
-                16         158 PUSH_NULL
-                           160 LOAD_FAST                7 (Entry)
-                           162 LOAD_FAST                0 (self)
-                           164 LOAD_CONST               2 (0)
-                           166 LOAD_FAST                0 (self)
-                           168 LOAD_ATTR                5 (var)
-                           178 KW_NAMES                 4
-                           180 PRECALL                  3
-                           184 CALL                     3
-                           194 LOAD_FAST                0 (self)
-                           196 STORE_ATTR               7 (entry)
-               
-                18         206 LOAD_FAST                0 (self)
-                           208 LOAD_METHOD              8 (_other)
-                           230 PRECALL                  0
-                           234 CALL                     0
-                           244 POP_TOP
-               
-                20         246 LOAD_FAST                0 (self)
-                           248 LOAD_METHOD              9 (default_palette)
-                           270 PRECALL                  0
-                           274 CALL                     0
-                           284 POP_TOP
-               
-                22         286 LOAD_FAST                3 (text)
-                           288 LOAD_FAST                0 (self)
-                           290 STORE_ATTR              10 (text)
-               
-                24         300 LOAD_FAST                0 (self)
-                           302 LOAD_ATTR               11 (entry_back)
-                           312 LOAD_FAST                0 (self)
-                           314 STORE_ATTR              12 (_entry_back)
-               
-                25         324 LOAD_FAST                0 (self)
-                           326 LOAD_ATTR               13 (entry_border)
-                           336 LOAD_FAST                0 (self)
-                           338 STORE_ATTR              14 (_entry_border)
-               
-                26         348 LOAD_FAST                0 (self)
-                           350 LOAD_ATTR               15 (entry_text_back)
-                           360 LOAD_FAST                0 (self)
-                           362 STORE_ATTR              16 (_entry_text_back)
-               
-                27         372 LOAD_FAST                0 (self)
-                           374 LOAD_ATTR               17 (entry_bottom_line)
-                           384 LOAD_FAST                0 (self)
-                           386 STORE_ATTR              18 (_entry_bottom_line)
+                            48 LOAD_CONST               1 (0)
+                            50 LOAD_CONST               2 (('width', 'height', 'highlightthickness'))
+                            52 BUILD_CONST_KEY_MAP      3
+                            54 LOAD_FAST                5 (kwargs)
+                            56 DICT_MERGE               1
+                            58 CALL_FUNCTION_EX         1
+                            60 POP_TOP
+               
+                11          62 LOAD_CONST               1 (0)
+                            64 LOAD_CONST               3 (('StringVar', 'Entry'))
+                            66 IMPORT_NAME              2 (tkinter)
+                            68 IMPORT_FROM              3 (StringVar)
+                            70 STORE_FAST               6 (StringVar)
+                            72 IMPORT_FROM              4 (Entry)
+                            74 STORE_FAST               7 (Entry)
+                            76 POP_TOP
+               
+                13          78 PUSH_NULL
+                            80 LOAD_FAST                6 (StringVar)
+                            82 PRECALL                  0
+                            86 CALL                     0
+                            96 LOAD_FAST                0 (self)
+                            98 STORE_ATTR               5 (var)
+               
+                14         108 LOAD_FAST                0 (self)
+                           110 LOAD_ATTR                5 (var)
+                           120 LOAD_METHOD              6 (set)
+                           142 LOAD_FAST                3 (text)
+                           144 PRECALL                  1
+                           148 CALL                     1
+                           158 POP_TOP
                
-                28         396 LOAD_FAST                0 (self)
-                           398 LOAD_ATTR               19 (entry_bottom_width)
-                           408 LOAD_FAST                0 (self)
-                           410 STORE_ATTR              20 (_entry_bottom_width)
+                16         160 PUSH_NULL
+                           162 LOAD_FAST                7 (Entry)
+                           164 LOAD_FAST                0 (self)
+                           166 LOAD_CONST               1 (0)
+                           168 LOAD_FAST                0 (self)
+                           170 LOAD_ATTR                5 (var)
+                           180 KW_NAMES                 4
+                           182 PRECALL                  3
+                           186 CALL                     3
+                           196 LOAD_FAST                0 (self)
+                           198 STORE_ATTR               7 (entry)
+               
+                18         208 LOAD_FAST                0 (self)
+                           210 LOAD_METHOD              8 (_other)
+                           232 PRECALL                  0
+                           236 CALL                     0
+                           246 POP_TOP
                
-                30         420 LOAD_GLOBAL             43 (NULL + nametofont)
-                           432 LOAD_CONST               5 ('TkDefaultFont')
-                           434 PRECALL                  1
-                           438 CALL                     1
-                           448 LOAD_FAST                0 (self)
-                           450 STORE_ATTR              22 (entry_text_font)
-               
-                32         460 LOAD_FAST                0 (self)
-                           462 LOAD_METHOD             23 (bind)
-                           484 LOAD_CONST               6 ('<Configure>')
-                           486 LOAD_FAST                0 (self)
-                           488 LOAD_ATTR               24 (_draw)
-                           498 LOAD_CONST               7 ('+')
-                           500 KW_NAMES                 8
-                           502 PRECALL                  3
-                           506 CALL                     3
-                           516 POP_TOP
-               
-                33         518 LOAD_FAST                0 (self)
-                           520 LOAD_METHOD             23 (bind)
-                           542 LOAD_CONST               9 ('<Button>')
-                           544 LOAD_FAST                0 (self)
-                           546 LOAD_ATTR               25 (_click)
-                           556 LOAD_CONST               7 ('+')
-                           558 KW_NAMES                 8
-                           560 PRECALL                  3
-                           564 CALL                     3
-                           574 POP_TOP
-               
-                34         576 LOAD_FAST                0 (self)
-                           578 LOAD_METHOD             23 (bind)
-                           600 LOAD_CONST              10 ('<Enter>')
-                           602 LOAD_FAST                0 (self)
-                           604 LOAD_ATTR               26 (_hover)
-                           614 LOAD_CONST               7 ('+')
-                           616 KW_NAMES                 8
-                           618 PRECALL                  3
-                           622 CALL                     3
-                           632 POP_TOP
-               
-                35         634 LOAD_FAST                0 (self)
-                           636 LOAD_METHOD             23 (bind)
-                           658 LOAD_CONST              11 ('<Leave>')
-                           660 LOAD_FAST                0 (self)
-                           662 LOAD_ATTR               27 (_hover_release)
-                           672 LOAD_CONST               7 ('+')
-                           674 KW_NAMES                 8
-                           676 PRECALL                  3
-                           680 CALL                     3
-                           690 POP_TOP
-               
-                36         692 LOAD_FAST                0 (self)
-                           694 LOAD_METHOD             23 (bind)
-                           716 LOAD_CONST              12 ('<FocusIn>')
-                           718 LOAD_FAST                0 (self)
-                           720 LOAD_ATTR               28 (_focus)
-                           730 LOAD_CONST               7 ('+')
-                           732 KW_NAMES                 8
-                           734 PRECALL                  3
-                           738 CALL                     3
-                           748 POP_TOP
-               
-                37         750 LOAD_FAST                0 (self)
-                           752 LOAD_ATTR                7 (entry)
-                           762 LOAD_METHOD             23 (bind)
-                           784 LOAD_CONST              12 ('<FocusIn>')
-                           786 LOAD_FAST                0 (self)
-                           788 LOAD_ATTR               28 (_focus)
-                           798 LOAD_CONST               7 ('+')
-                           800 KW_NAMES                 8
-                           802 PRECALL                  3
-                           806 CALL                     3
-                           816 POP_TOP
-               
-                38         818 LOAD_FAST                0 (self)
-                           820 LOAD_METHOD             23 (bind)
-                           842 LOAD_CONST              13 ('<FocusOut>')
-                           844 LOAD_FAST                0 (self)
-                           846 LOAD_ATTR               29 (_focusout)
-                           856 LOAD_CONST               7 ('+')
-                           858 KW_NAMES                 8
-                           860 PRECALL                  3
-                           864 CALL                     3
-                           874 POP_TOP
-               
-                39         876 LOAD_FAST                0 (self)
-                           878 LOAD_ATTR                7 (entry)
-                           888 LOAD_METHOD             23 (bind)
-                           910 LOAD_CONST              13 ('<FocusOut>')
-                           912 LOAD_FAST                0 (self)
-                           914 LOAD_ATTR               29 (_focusout)
-                           924 LOAD_CONST               7 ('+')
-                           926 KW_NAMES                 8
-                           928 PRECALL                  3
-                           932 CALL                     3
-                           942 POP_TOP
-               
-                41         944 LOAD_FAST                0 (self)
-                           946 LOAD_METHOD             24 (_draw)
-                           968 LOAD_CONST               0 (None)
-                           970 PRECALL                  1
-                           974 CALL                     1
-                           984 POP_TOP
-                           986 LOAD_CONST               0 (None)
-                           988 RETURN_VALUE
+                20         248 LOAD_FAST                0 (self)
+                           250 LOAD_METHOD              9 (default_palette)
+                           272 PRECALL                  0
+                           276 CALL                     0
+                           286 POP_TOP
+               
+                22         288 LOAD_FAST                3 (text)
+                           290 LOAD_FAST                0 (self)
+                           292 STORE_ATTR              10 (text)
+               
+                24         302 LOAD_FAST                0 (self)
+                           304 LOAD_ATTR               11 (entry_back)
+                           314 LOAD_FAST                0 (self)
+                           316 STORE_ATTR              12 (_entry_back)
+               
+                25         326 LOAD_FAST                0 (self)
+                           328 LOAD_ATTR               13 (entry_border)
+                           338 LOAD_FAST                0 (self)
+                           340 STORE_ATTR              14 (_entry_border)
+               
+                26         350 LOAD_FAST                0 (self)
+                           352 LOAD_ATTR               15 (entry_text_back)
+                           362 LOAD_FAST                0 (self)
+                           364 STORE_ATTR              16 (_entry_text_back)
+               
+                27         374 LOAD_FAST                0 (self)
+                           376 LOAD_ATTR               17 (entry_bottom_line)
+                           386 LOAD_FAST                0 (self)
+                           388 STORE_ATTR              18 (_entry_bottom_line)
+               
+                28         398 LOAD_FAST                0 (self)
+                           400 LOAD_ATTR               19 (entry_bottom_width)
+                           410 LOAD_FAST                0 (self)
+                           412 STORE_ATTR              20 (_entry_bottom_width)
+               
+                30         422 LOAD_GLOBAL             43 (NULL + nametofont)
+                           434 LOAD_CONST               5 ('TkDefaultFont')
+                           436 PRECALL                  1
+                           440 CALL                     1
+                           450 LOAD_FAST                0 (self)
+                           452 STORE_ATTR              22 (entry_text_font)
+               
+                32         462 LOAD_FAST                0 (self)
+                           464 LOAD_METHOD             23 (bind)
+                           486 LOAD_CONST               6 ('<Configure>')
+                           488 LOAD_FAST                0 (self)
+                           490 LOAD_ATTR               24 (_draw)
+                           500 LOAD_CONST               7 ('+')
+                           502 KW_NAMES                 8
+                           504 PRECALL                  3
+                           508 CALL                     3
+                           518 POP_TOP
+               
+                33         520 LOAD_FAST                0 (self)
+                           522 LOAD_METHOD             23 (bind)
+                           544 LOAD_CONST               9 ('<Button>')
+                           546 LOAD_FAST                0 (self)
+                           548 LOAD_ATTR               25 (_click)
+                           558 LOAD_CONST               7 ('+')
+                           560 KW_NAMES                 8
+                           562 PRECALL                  3
+                           566 CALL                     3
+                           576 POP_TOP
+               
+                34         578 LOAD_FAST                0 (self)
+                           580 LOAD_METHOD             23 (bind)
+                           602 LOAD_CONST              10 ('<Enter>')
+                           604 LOAD_FAST                0 (self)
+                           606 LOAD_ATTR               26 (_hover)
+                           616 LOAD_CONST               7 ('+')
+                           618 KW_NAMES                 8
+                           620 PRECALL                  3
+                           624 CALL                     3
+                           634 POP_TOP
+               
+                35         636 LOAD_FAST                0 (self)
+                           638 LOAD_METHOD             23 (bind)
+                           660 LOAD_CONST              11 ('<Leave>')
+                           662 LOAD_FAST                0 (self)
+                           664 LOAD_ATTR               27 (_hover_release)
+                           674 LOAD_CONST               7 ('+')
+                           676 KW_NAMES                 8
+                           678 PRECALL                  3
+                           682 CALL                     3
+                           692 POP_TOP
+               
+                36         694 LOAD_FAST                0 (self)
+                           696 LOAD_METHOD             23 (bind)
+                           718 LOAD_CONST              12 ('<FocusIn>')
+                           720 LOAD_FAST                0 (self)
+                           722 LOAD_ATTR               28 (_focus)
+                           732 LOAD_CONST               7 ('+')
+                           734 KW_NAMES                 8
+                           736 PRECALL                  3
+                           740 CALL                     3
+                           750 POP_TOP
+               
+                37         752 LOAD_FAST                0 (self)
+                           754 LOAD_ATTR                7 (entry)
+                           764 LOAD_METHOD             23 (bind)
+                           786 LOAD_CONST              12 ('<FocusIn>')
+                           788 LOAD_FAST                0 (self)
+                           790 LOAD_ATTR               28 (_focus)
+                           800 LOAD_CONST               7 ('+')
+                           802 KW_NAMES                 8
+                           804 PRECALL                  3
+                           808 CALL                     3
+                           818 POP_TOP
+               
+                38         820 LOAD_FAST                0 (self)
+                           822 LOAD_METHOD             23 (bind)
+                           844 LOAD_CONST              13 ('<FocusOut>')
+                           846 LOAD_FAST                0 (self)
+                           848 LOAD_ATTR               29 (_focusout)
+                           858 LOAD_CONST               7 ('+')
+                           860 KW_NAMES                 8
+                           862 PRECALL                  3
+                           866 CALL                     3
+                           876 POP_TOP
+               
+                39         878 LOAD_FAST                0 (self)
+                           880 LOAD_ATTR                7 (entry)
+                           890 LOAD_METHOD             23 (bind)
+                           912 LOAD_CONST              13 ('<FocusOut>')
+                           914 LOAD_FAST                0 (self)
+                           916 LOAD_ATTR               29 (_focusout)
+                           926 LOAD_CONST               7 ('+')
+                           928 KW_NAMES                 8
+                           930 PRECALL                  3
+                           934 CALL                     3
+                           944 POP_TOP
+               
+                41         946 LOAD_FAST                0 (self)
+                           948 LOAD_METHOD             24 (_draw)
+                           970 LOAD_CONST               0 (None)
+                           972 PRECALL                  1
+                           976 CALL                     1
+                           986 POP_TOP
+                           988 LOAD_CONST               0 (None)
+                           990 RETURN_VALUE
                consts
                   None
-                  ('width', 'height')
                   0
+                  ('width', 'height', 'highlightthickness')
                   ('StringVar', 'Entry')
                   ('bd', 'textvariable')
                   'TkDefaultFont'
                   '<Configure>'
                   '+'
                   ('add',)
                   '<Button>'
@@ -655,15 +656,15 @@
                varnames   ('self', 'width', 'height', 'text', 'args', 'kwargs', 'StringVar', 'Entry')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '__init__'
                firstlineno 7
                lnotab
-                  0x0402380210021e0134023002280228020e021801180118011801180228
+                  0x04023a0210021e0134023002280228020e021801180118011801180228
                   023a013a013a013a013a0144013a014402
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -777,60 +778,60 @@
                   00000000007c006a060000000000000000ac04a6070000ab070000000000
                   0000007c005f0700000000000000007c00a0080000000000000000000000
                   0000000000000000007c00a0020000000000000000000000000000000000
                   000000a6000000ab00000000000000000064057a0b00007c00a003000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0064057a0b00007c00a00200000000000000000000000000000000000000
                   00a6000000ab0000000000000000007c006a0400000000000000007a0a00
-                  0064067a0a00007c006a0900000000000000006407190000000000000000
+                  0064067a0a00007c006a0900000000000000006402190000000000000000
                   007a0a00007c00a0030000000000000000000000000000000000000000a6
                   000000ab0000000000000000007c006a0400000000000000007a0a000064
-                  067a0a00007c006a0900000000000000006408190000000000000000007a
-                  0a00007c006a0a0000000000000000ac09a6050000ab0500000000000000
+                  067a0a00007c006a0900000000000000006403190000000000000000007a
+                  0a00007c006a0a0000000000000000ac07a6050000ab0500000000000000
                   007c005f0b00000000000000007c00a00100000000000000000000000000
                   0000000000000064037c00a0030000000000000000000000000000000000
                   000000a6000000ab0000000000000000007c006a0c00000000000000007a
                   0a000064037a0a00007c00a0020000000000000000000000000000000000
                   000000a6000000ab00000000000000000064037a0a00007c00a003000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
-                  00640a7a0a00007c006a0d00000000000000007c006a0d00000000000000
-                  006407ac0ba6070000ab0700000000000000007c005f0e00000000000000
-                  007c006a0c000000000000000064076b0200000000721a7c00a000000000
+                  0064037a0a00007c006a0d00000000000000007c006a0d00000000000000
+                  006402ac08a6070000ab0700000000000000007c005f0e00000000000000
+                  007c006a0c000000000000000064026b0200000000721a7c00a000000000
                   00000000000000000000000000000000007c006a0e0000000000000000a6
                   010000ab01000000000000000001007c00a00f0000000000000000000000
                   0000000000000000007c006a0e00000000000000007c006a0b0000000000
                   000000a6020000ab02000000000000000001007c006a0a00000000000000
                   00a01000000000000000000000000000000000000000007c006a06000000
-                  00000000007c006a110000000000000000ac0ca6020000ab020000000000
-                  000000010064005300
+                  00000000007c006a1100000000000000007c006a110000000000000000ac
+                  09a6030000ab030000000000000000010064005300
                 53           0 RESUME                   0
                
                 54           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
                 56          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_rectangle)
                
-                57          68 LOAD_CONST               2 (1.5)
-                            70 LOAD_CONST               2 (1.5)
+                57          68 LOAD_CONST               2 (0)
+                            70 LOAD_CONST               2 (0)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
-                           110 LOAD_CONST               3 (3)
+                           110 LOAD_CONST               3 (1)
                            112 BINARY_OP               10 (-)
                            116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
-                           154 LOAD_CONST               3 (3)
+                           154 LOAD_CONST               3 (1)
                            156 BINARY_OP               10 (-)
                
                 58         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (entry_border_width)
                
                 59         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (_entry_border)
@@ -866,180 +867,182 @@
                            374 LOAD_FAST                0 (self)
                            376 LOAD_ATTR                4 (entry_border_width)
                            386 BINARY_OP               10 (-)
                            390 LOAD_CONST               6 (5)
                            392 BINARY_OP               10 (-)
                            396 LOAD_FAST                0 (self)
                            398 LOAD_ATTR                9 (entry_padding)
-                           408 LOAD_CONST               7 (0)
+                           408 LOAD_CONST               2 (0)
                            410 BINARY_SUBSCR
                            420 BINARY_OP               10 (-)
-                           424 LOAD_FAST                0 (self)
+               
+                65         424 LOAD_FAST                0 (self)
                            426 LOAD_METHOD              3 (winfo_height)
                            448 PRECALL                  0
                            452 CALL                     0
                            462 LOAD_FAST                0 (self)
                            464 LOAD_ATTR                4 (entry_border_width)
                            474 BINARY_OP               10 (-)
                            478 LOAD_CONST               6 (5)
                            480 BINARY_OP               10 (-)
                            484 LOAD_FAST                0 (self)
                            486 LOAD_ATTR                9 (entry_padding)
-                           496 LOAD_CONST               8 (1)
+                           496 LOAD_CONST               3 (1)
                            498 BINARY_SUBSCR
                            508 BINARY_OP               10 (-)
                
-                65         512 LOAD_FAST                0 (self)
+                66         512 LOAD_FAST                0 (self)
                            514 LOAD_ATTR               10 (entry)
                
-                62         524 KW_NAMES                 9
+                62         524 KW_NAMES                 7
                            526 PRECALL                  5
                            530 CALL                     5
                            540 LOAD_FAST                0 (self)
                            542 STORE_ATTR              11 (entry_text)
                
-                68         552 LOAD_FAST                0 (self)
+                69         552 LOAD_FAST                0 (self)
                            554 LOAD_METHOD              1 (create_rectangle)
-                           576 LOAD_CONST               3 (3)
+                           576 LOAD_CONST               3 (1)
                            578 LOAD_FAST                0 (self)
                            580 LOAD_METHOD              3 (winfo_height)
                            602 PRECALL                  0
                            606 CALL                     0
                            616 LOAD_FAST                0 (self)
                            618 LOAD_ATTR               12 (_entry_bottom_width)
                            628 BINARY_OP               10 (-)
-                           632 LOAD_CONST               3 (3)
+                           632 LOAD_CONST               3 (1)
                            634 BINARY_OP               10 (-)
-                           638 LOAD_FAST                0 (self)
+               
+                70         638 LOAD_FAST                0 (self)
                            640 LOAD_METHOD              2 (winfo_width)
                            662 PRECALL                  0
                            666 CALL                     0
-                           676 LOAD_CONST               3 (3)
+                           676 LOAD_CONST               3 (1)
                            678 BINARY_OP               10 (-)
                            682 LOAD_FAST                0 (self)
                            684 LOAD_METHOD              3 (winfo_height)
                            706 PRECALL                  0
                            710 CALL                     0
-                           720 LOAD_CONST              10 (3.5)
+                           720 LOAD_CONST               3 (1)
                            722 BINARY_OP               10 (-)
                
-                69         726 LOAD_FAST                0 (self)
+                71         726 LOAD_FAST                0 (self)
                            728 LOAD_ATTR               13 (_entry_bottom_line)
                            738 LOAD_FAST                0 (self)
                            740 LOAD_ATTR               13 (_entry_bottom_line)
-                           750 LOAD_CONST               7 (0)
                
-                68         752 KW_NAMES                11
+                72         750 LOAD_CONST               2 (0)
+               
+                69         752 KW_NAMES                 8
                            754 PRECALL                  7
                            758 CALL                     7
                            768 LOAD_FAST                0 (self)
                            770 STORE_ATTR              14 (entry_bottom)
                
-                71         780 LOAD_FAST                0 (self)
+                74         780 LOAD_FAST                0 (self)
                            782 LOAD_ATTR               12 (_entry_bottom_width)
-                           792 LOAD_CONST               7 (0)
+                           792 LOAD_CONST               2 (0)
                            794 COMPARE_OP               2 (==)
                            800 POP_JUMP_FORWARD_IF_FALSE    26 (to 854)
                
-                72         802 LOAD_FAST                0 (self)
+                75         802 LOAD_FAST                0 (self)
                            804 LOAD_METHOD              0 (delete)
                            826 LOAD_FAST                0 (self)
                            828 LOAD_ATTR               14 (entry_bottom)
                            838 PRECALL                  1
                            842 CALL                     1
                            852 POP_TOP
                
-                74     >>  854 LOAD_FAST                0 (self)
+                77     >>  854 LOAD_FAST                0 (self)
                            856 LOAD_METHOD             15 (tag_raise)
                            878 LOAD_FAST                0 (self)
                            880 LOAD_ATTR               14 (entry_bottom)
                            890 LOAD_FAST                0 (self)
                            892 LOAD_ATTR               11 (entry_text)
                            902 PRECALL                  2
                            906 CALL                     2
                            916 POP_TOP
                
-                76         918 LOAD_FAST                0 (self)
+                79         918 LOAD_FAST                0 (self)
                            920 LOAD_ATTR               10 (entry)
                            930 LOAD_METHOD             16 (configure)
                            952 LOAD_FAST                0 (self)
                            954 LOAD_ATTR                6 (_entry_back)
                            964 LOAD_FAST                0 (self)
                            966 LOAD_ATTR               17 (_entry_text_back)
-                           976 KW_NAMES                12
-                           978 PRECALL                  2
-                           982 CALL                     2
-                           992 POP_TOP
-                           994 LOAD_CONST               0 (None)
-                           996 RETURN_VALUE
+                           976 LOAD_FAST                0 (self)
+                           978 LOAD_ATTR               17 (_entry_text_back)
+                           988 KW_NAMES                 9
+                           990 PRECALL                  3
+                           994 CALL                     3
+                          1004 POP_TOP
+                          1006 LOAD_CONST               0 (None)
+                          1008 RETURN_VALUE
                consts
                   None
                   'all'
-                  1.5
-                  3
+                  0
+                  1
                   ('width', 'outline', 'fill')
                   2
                   5
-                  0
-                  1
                   ('width', 'height', 'window')
-                  3.5
                   ('fill', 'outline', 'width')
-                  ('background', 'foreground')
+                  ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_rectangle', 'winfo_width', 'winfo_height', 'entry_border_width', '_entry_border', '_entry_back', 'entry_frame', 'create_window', 'entry_padding', 'entry', 'entry_text', '_entry_bottom_width', '_entry_bottom_line', 'entry_bottom', 'tag_raise', 'configure', '_entry_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_draw'
                firstlineno 53
                lnotab
-                  0x02012a0218015c010c0118fd1c0618015801b0010cfd1c06ae011aff1c
-                  03160134024002
+                  0x02012a0218015c010c0118fd1c0618015801580158010cfc1c07560158
+                  01180102fd1c05160134024002
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-                78           0 RESUME                   0
+                81           0 RESUME                   0
                
-                79           2 LOAD_FAST                0 (self)
+                82           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (entry_focusin_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_entry_back)
                
-                80          26 LOAD_FAST                0 (self)
+                83          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (entry_focusin_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_entry_border)
                
-                81          50 LOAD_FAST                0 (self)
+                84          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (entry_focusin_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_entry_text_back)
                
-                82          74 LOAD_FAST                0 (self)
+                85          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (entry_focusin_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_entry_bottom_line)
                
-                83          98 LOAD_FAST                0 (self)
+                86          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (entry_focusin_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_entry_bottom_width)
                
-                85         122 LOAD_FAST                0 (self)
+                88         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -1047,56 +1050,56 @@
                   None
                names      ('entry_focusin_back', '_entry_back', 'entry_focusin_border', '_entry_border', 'entry_focusin_text_back', '_entry_text_back', 'entry_focusin_bottom_line', '_entry_bottom_line', 'entry_focusin_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_focus'
-               firstlineno 78
+               firstlineno 81
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-                87           0 RESUME                   0
+                90           0 RESUME                   0
                
-                88           2 LOAD_FAST                0 (self)
+                91           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (entry_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_entry_back)
                
-                89          26 LOAD_FAST                0 (self)
+                92          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (entry_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_entry_border)
                
-                90          50 LOAD_FAST                0 (self)
+                93          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (entry_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_entry_text_back)
                
-                91          74 LOAD_FAST                0 (self)
+                94          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (entry_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_entry_bottom_line)
                
-                92          98 LOAD_FAST                0 (self)
+                95          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (entry_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_entry_bottom_width)
                
-                94         122 LOAD_FAST                0 (self)
+                97         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -1104,66 +1107,66 @@
                   None
                names      ('entry_back', '_entry_back', 'entry_border', '_entry_border', 'entry_text_back', '_entry_text_back', 'entry_bottom_line', '_entry_bottom_line', 'entry_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_focusout'
-               firstlineno 87
+               firstlineno 90
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                96           0 RESUME                   0
+                99           0 RESUME                   0
                
-                97           2 LOAD_FAST                0 (self)
+               100           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_set)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('focus_set',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_click'
-               firstlineno 96
+               firstlineno 99
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064005300
-                99           0 RESUME                   0
+               102           0 RESUME                   0
                
-               100           2 LOAD_CONST               1 (True)
+               103           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                   True
                names      ('hover',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_hover'
-               firstlineno 99
+               firstlineno 102
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -1171,177 +1174,177 @@
                   00ab000000000000000000735a64017c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c006a0a00000000000000007c005f0b00000000000000007c00a0
                   0c00000000000000000000000000000000000000006400a6010000ab0100
                   0000000000000001006400530064005300
-               102           0 RESUME                   0
+               105           0 RESUME                   0
                
-               103           2 LOAD_FAST                0 (self)
+               106           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_get)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_JUMP_FORWARD_IF_TRUE    90 (to 222)
                
-               104          42 LOAD_CONST               1 (False)
+               107          42 LOAD_CONST               1 (False)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (hover)
                
-               105          56 LOAD_FAST                0 (self)
+               108          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (entry_back)
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_entry_back)
                
-               106          80 LOAD_FAST                0 (self)
+               109          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (entry_border)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               5 (_entry_border)
                
-               107         104 LOAD_FAST                0 (self)
+               110         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (entry_text_back)
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               7 (_entry_text_back)
                
-               108         128 LOAD_FAST                0 (self)
+               111         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                8 (entry_bottom_line)
                            140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               9 (_entry_bottom_line)
                
-               109         152 LOAD_FAST                0 (self)
+               112         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR               10 (entry_bottom_width)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR              11 (_entry_bottom_width)
                
-               111         176 LOAD_FAST                0 (self)
+               114         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD             12 (_draw)
                            200 LOAD_CONST               0 (None)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                
-               103     >>  222 LOAD_CONST               0 (None)
+               106     >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   False
                names      ('focus_get', 'hover', 'entry_back', '_entry_back', 'entry_border', '_entry_border', 'entry_text_back', '_entry_text_back', 'entry_bottom_line', '_entry_bottom_line', 'entry_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_hover_release'
-               firstlineno 102
+               firstlineno 105
                lnotab 0x020128010e01180118011801180118022ef8
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               113           0 RESUME                   0
+               116           0 RESUME                   0
                
-               114           2 LOAD_FAST                1 (font)
+               117           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               115           6 LOAD_FAST                0 (self)
+               118           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (entry_text_font)
                             18 RETURN_VALUE
                
-               117     >>   20 LOAD_FAST                1 (font)
+               120     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (entry_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('entry_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'font'
-               firstlineno 113
+               firstlineno 116
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               119           0 RESUME                   0
+               122           0 RESUME                   0
                
-               120           2 LOAD_FAST                0 (self)
+               123           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 119
+               firstlineno 122
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 16
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640564086409640a640b640c640d9c0da60100
                   00ab010000000000000000010064005300
-               122           0 RESUME                   0
+               125           0 RESUME                   0
                
-               123           2 LOAD_FAST                0 (self)
+               126           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               125          26 LOAD_CONST               1 ((3, 4))
+               128          26 LOAD_CONST               1 ((3, 4))
                
-               127          28 LOAD_CONST               2 ('#f3f3f3')
+               130          28 LOAD_CONST               2 ('#f3f3f3')
                
-               128          30 LOAD_CONST               3 (1)
+               131          30 LOAD_CONST               3 (1)
                
-               129          32 LOAD_CONST               4 (0)
+               132          32 LOAD_CONST               4 (0)
                
-               131          34 LOAD_CONST               5 ('#eaeaea')
+               134          34 LOAD_CONST               5 ('#eaeaea')
                
-               132          36 LOAD_CONST               6 ('#fdfdfd')
+               135          36 LOAD_CONST               6 ('#fdfdfd')
                
-               133          38 LOAD_CONST               7 ('#5f5f5f')
+               136          38 LOAD_CONST               7 ('#5f5f5f')
                
-               134          40 LOAD_CONST               5 ('#eaeaea')
+               137          40 LOAD_CONST               5 ('#eaeaea')
                
-               136          42 LOAD_CONST               8 ('#e2e2e2')
+               139          42 LOAD_CONST               8 ('#e2e2e2')
                
-               137          44 LOAD_CONST               9 ('#f9f9f9')
+               140          44 LOAD_CONST               9 ('#f9f9f9')
                
-               138          46 LOAD_CONST              10 ('#1a1a1a')
+               141          46 LOAD_CONST              10 ('#1a1a1a')
                
-               139          48 LOAD_CONST              11 ('#185fb4')
+               142          48 LOAD_CONST              11 ('#185fb4')
                
-               140          50 LOAD_CONST              12 (2)
+               143          50 LOAD_CONST              12 (2)
                
-               124          52 LOAD_CONST              13 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
+               127          52 LOAD_CONST              13 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
                             54 BUILD_CONST_KEY_MAP     13
                
-               123          56 PRECALL                  1
+               126          56 PRECALL                  1
                             60 CALL                     1
                             70 POP_TOP
                             72 LOAD_CONST               0 (None)
                             74 RETURN_VALUE
                consts
                   None
                   (3, 4)
@@ -1359,62 +1362,62 @@
                   ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette_light'
-               firstlineno 122
+               firstlineno 125
                lnotab
                   0x0201180202020201020102020201020102010202020102010201020102
                   f004ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 16
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02640364046405640664076408640464096407640a640b640c9c0da60100
                   00ab010000000000000000010064005300
-               144           0 RESUME                   0
+               147           0 RESUME                   0
                
-               145           2 LOAD_FAST                0 (self)
+               148           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               147          26 LOAD_CONST               1 ((3, 4))
+               150          26 LOAD_CONST               1 ((3, 4))
                
-               149          28 LOAD_CONST               2 ('#202020')
+               152          28 LOAD_CONST               2 ('#202020')
                
-               150          30 LOAD_CONST               3 (1)
+               153          30 LOAD_CONST               3 (1)
                
-               152          32 LOAD_CONST               4 ('#454545')
+               155          32 LOAD_CONST               4 ('#454545')
                
-               153          34 LOAD_CONST               5 ('#353535')
+               156          34 LOAD_CONST               5 ('#353535')
                
-               154          36 LOAD_CONST               6 ('#cecece')
+               157          36 LOAD_CONST               6 ('#cecece')
                
-               155          38 LOAD_CONST               7 ('#ffffff')
+               158          38 LOAD_CONST               7 ('#ffffff')
                
-               156          40 LOAD_CONST               8 (0)
+               159          40 LOAD_CONST               8 (0)
                
-               158          42 LOAD_CONST               4 ('#454545')
+               161          42 LOAD_CONST               4 ('#454545')
                
-               159          44 LOAD_CONST               9 ('#2f2f2f')
+               162          44 LOAD_CONST               9 ('#2f2f2f')
                
-               160          46 LOAD_CONST               7 ('#ffffff')
+               163          46 LOAD_CONST               7 ('#ffffff')
                
-               161          48 LOAD_CONST              10 ('#4cc2ff')
+               164          48 LOAD_CONST              10 ('#4cc2ff')
                
-               162          50 LOAD_CONST              11 (2)
+               165          50 LOAD_CONST              11 (2)
                
-               146          52 LOAD_CONST              12 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
+               149          52 LOAD_CONST              12 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
                             54 BUILD_CONST_KEY_MAP     13
                
-               145          56 PRECALL                  1
+               148          56 PRECALL                  1
                             60 CALL                     1
                             70 POP_TOP
                             72 LOAD_CONST               0 (None)
                             74 RETURN_VALUE
                consts
                   None
                   (3, 4)
@@ -1431,15 +1434,15 @@
                   ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette_dark'
-               firstlineno 144
+               firstlineno 147
                lnotab
                   0x0201180202020201020202010201020102010202020102010201020102
                   f004ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 11
@@ -1460,154 +1463,154 @@
                   00000000000000000000006400a6010000ab010000000000000000010064
                   0053002300741c0000000000000000000024007204010059006400530077
                   007803590077017c006a0000000000000000007c006a0100000000000000
                   007c006a0200000000000000007c006a0700000000000000007c006a0300
                   000000000000007c006a0400000000000000007c006a0500000000000000
                   007c006a0800000000000000007c006a0900000000000000007c006a0a00
                   00000000000000640e9c0a5300
-               166           0 RESUME                   0
+               169           0 RESUME                   0
                
-               167           2 LOAD_FAST                1 (dict)
+               170           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE   210 (to 426)
                
-               168           6 LOAD_FAST                1 (dict)
+               171           6 LOAD_FAST                1 (dict)
                              8 LOAD_CONST               1 ('entry_padding')
                             10 BINARY_SUBSCR
                             20 LOAD_FAST                0 (self)
                             22 STORE_ATTR               0 (entry_padding)
                
-               170          32 LOAD_FAST                1 (dict)
+               173          32 LOAD_FAST                1 (dict)
                             34 LOAD_CONST               2 ('entry_frame_back')
                             36 BINARY_SUBSCR
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               1 (entry_frame_back)
                
-               171          58 LOAD_FAST                1 (dict)
+               174          58 LOAD_FAST                1 (dict)
                             60 LOAD_CONST               3 ('entry_border_width')
                             62 BINARY_SUBSCR
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (entry_border_width)
                
-               173          84 LOAD_FAST                1 (dict)
+               176          84 LOAD_FAST                1 (dict)
                             86 LOAD_CONST               4 ('entry_border')
                             88 BINARY_SUBSCR
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               3 (entry_border)
                
-               174         110 LOAD_FAST                1 (dict)
+               177         110 LOAD_FAST                1 (dict)
                            112 LOAD_CONST               5 ('entry_back')
                            114 BINARY_SUBSCR
                            124 LOAD_FAST                0 (self)
                            126 STORE_ATTR               4 (entry_back)
                
-               175         136 LOAD_FAST                1 (dict)
+               178         136 LOAD_FAST                1 (dict)
                            138 LOAD_CONST               6 ('entry_text_back')
                            140 BINARY_SUBSCR
                            150 LOAD_FAST                0 (self)
                            152 STORE_ATTR               5 (entry_text_back)
                
-               176         162 LOAD_FAST                1 (dict)
+               179         162 LOAD_FAST                1 (dict)
                            164 LOAD_CONST               7 ('entry_bottom_line')
                            166 BINARY_SUBSCR
                            176 LOAD_FAST                0 (self)
                            178 STORE_ATTR               6 (entry_bottom_line)
                
-               177         188 LOAD_FAST                1 (dict)
+               180         188 LOAD_FAST                1 (dict)
                            190 LOAD_CONST               8 ('entry_bottom_width')
                            192 BINARY_SUBSCR
                            202 LOAD_FAST                0 (self)
                            204 STORE_ATTR               7 (entry_bottom_width)
                
-               179         214 LOAD_FAST                1 (dict)
+               182         214 LOAD_FAST                1 (dict)
                            216 LOAD_CONST               9 ('entry_focusin_border')
                            218 BINARY_SUBSCR
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (entry_focusin_border)
                
-               180         240 LOAD_FAST                1 (dict)
+               183         240 LOAD_FAST                1 (dict)
                            242 LOAD_CONST              10 ('entry_focusin_back')
                            244 BINARY_SUBSCR
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (entry_focusin_back)
                
-               181         266 LOAD_FAST                1 (dict)
+               184         266 LOAD_FAST                1 (dict)
                            268 LOAD_CONST              11 ('entry_focusin_text_back')
                            270 BINARY_SUBSCR
                            280 LOAD_FAST                0 (self)
                            282 STORE_ATTR              10 (entry_focusin_text_back)
                
-               182         292 LOAD_FAST                1 (dict)
+               185         292 LOAD_FAST                1 (dict)
                            294 LOAD_CONST              12 ('entry_focusin_bottom_line')
                            296 BINARY_SUBSCR
                            306 LOAD_FAST                0 (self)
                            308 STORE_ATTR              11 (entry_focusin_bottom_line)
                
-               183         318 LOAD_FAST                1 (dict)
+               186         318 LOAD_FAST                1 (dict)
                            320 LOAD_CONST              13 ('entry_focusin_bottom_width')
                            322 BINARY_SUBSCR
                            332 LOAD_FAST                0 (self)
                            334 STORE_ATTR              12 (entry_focusin_bottom_width)
                
-               185         344 NOP
+               188         344 NOP
                
-               186         346 LOAD_FAST                0 (self)
+               189         346 LOAD_FAST                0 (self)
                            348 LOAD_METHOD             13 (_draw)
                            370 LOAD_CONST               0 (None)
                            372 PRECALL                  1
                            376 CALL                     1
                            386 POP_TOP
                            388 LOAD_CONST               0 (None)
                            390 RETURN_VALUE
                        >>  392 PUSH_EXC_INFO
                
-               187         394 LOAD_GLOBAL             28 (AttributeError)
+               190         394 LOAD_GLOBAL             28 (AttributeError)
                            406 CHECK_EXC_MATCH
                            408 POP_JUMP_FORWARD_IF_FALSE     4 (to 418)
                            410 POP_TOP
                
-               188         412 POP_EXCEPT
+               191         412 POP_EXCEPT
                            414 LOAD_CONST               0 (None)
                            416 RETURN_VALUE
                
-               187     >>  418 RERAISE                  0
+               190     >>  418 RERAISE                  0
                        >>  420 COPY                     3
                            422 POP_EXCEPT
                            424 RERAISE                  1
                
-               191     >>  426 LOAD_FAST                0 (self)
+               194     >>  426 LOAD_FAST                0 (self)
                            428 LOAD_ATTR                0 (entry_padding)
                
-               193         438 LOAD_FAST                0 (self)
+               196         438 LOAD_FAST                0 (self)
                            440 LOAD_ATTR                1 (entry_frame_back)
                
-               194         450 LOAD_FAST                0 (self)
+               197         450 LOAD_FAST                0 (self)
                            452 LOAD_ATTR                2 (entry_border_width)
                
-               195         462 LOAD_FAST                0 (self)
+               198         462 LOAD_FAST                0 (self)
                            464 LOAD_ATTR                7 (entry_bottom_width)
                
-               197         474 LOAD_FAST                0 (self)
+               200         474 LOAD_FAST                0 (self)
                            476 LOAD_ATTR                3 (entry_border)
                
-               198         486 LOAD_FAST                0 (self)
+               201         486 LOAD_FAST                0 (self)
                            488 LOAD_ATTR                4 (entry_back)
                
-               199         498 LOAD_FAST                0 (self)
+               202         498 LOAD_FAST                0 (self)
                            500 LOAD_ATTR                5 (entry_text_back)
                
-               201         510 LOAD_FAST                0 (self)
+               204         510 LOAD_FAST                0 (self)
                            512 LOAD_ATTR                8 (entry_focusin_border)
                
-               202         522 LOAD_FAST                0 (self)
+               205         522 LOAD_FAST                0 (self)
                            524 LOAD_ATTR                9 (entry_focusin_back)
                
-               203         534 LOAD_FAST                0 (self)
+               206         534 LOAD_FAST                0 (self)
                            536 LOAD_ATTR               10 (entry_focusin_text_back)
                
-               190         546 LOAD_CONST              14 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back'))
+               193         546 LOAD_CONST              14 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back'))
                            548 BUILD_CONST_KEY_MAP     10
                            550 RETURN_VALUE
                ExceptionTable:
                  346 to 386 -> 392 [0]
                  392 to 410 -> 420 [1] lasti
                  418 to 418 -> 420 [1] lasti
                consts
@@ -1628,141 +1631,141 @@
                   ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back')
                names      ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette'
-               firstlineno 166
+               firstlineno 169
                lnotab
                   0x020104011a021a011a021a011a011a011a011a021a011a011a011a011a
                   0202013001120106ff08040c020c010c010c020c010c010c020c010c010c
                   f3
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'set', 'get', '_other', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawBasicEntry'
          firstlineno 6
          lnotab
-            0x0c011a240c030603060406190809080908030803080b0e060603061606
+            0x0c011a240c0306030604061c0809080908030803080b0e060603061606
             16
       'AdwDrawBasicEntry'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         207           0 RESUME                   0
+         210           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawEntry')
                        8 STORE_NAME               2 (__qualname__)
          
-         208          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 208>)
+         211          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 211>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawEntry'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               208           0 RESUME                   0
+               211           0 RESUME                   0
                
-               209           2 LOAD_FAST                0 (self)
+               212           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 208
+               firstlineno 211
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawEntry'
-         firstlineno 207
+         firstlineno 210
          lnotab 0x0a01
       'AdwDrawEntry'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         212           0 RESUME                   0
+         215           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkEntry')
                        8 STORE_NAME               2 (__qualname__)
          
-         213          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 213>)
+         216          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 216>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkEntry'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               213           0 RESUME                   0
+               216           0 RESUME                   0
                
-               214           2 LOAD_FAST                0 (self)
+               217           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 213
+               firstlineno 216
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawDarkEntry'
-         firstlineno 212
+         firstlineno 215
          lnotab 0x0a01
       'AdwDrawDarkEntry'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
@@ -1770,91 +1773,91 @@
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             126404650565067a0700006602640584055a07640684005a086412640784
             015a096412640884015a0a6412640984015a0b6412640a84015a0c641264
             0b84015a0d6412640c650e6602640d84055a0f640e84005a10640f84005a
             11641084005a126412641184015a13880078015a145300
                        0 MAKE_CELL                0 (__class__)
          
-         218           2 RESUME                   0
+         221           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundEntry')
                       10 STORE_NAME               2 (__qualname__)
          
-         219          12 LOAD_CLOSURE             0 (__class__)
+         222          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\entry.py", line 219>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\entry.py", line 222>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         222          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\entry.py", line 222>)
+         225          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\entry.py", line 225>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         226          28 LOAD_CONST              18 ((None,))
+         229          28 LOAD_CONST              18 ((None,))
                       30 LOAD_CONST               4 ('radius')
                       32 LOAD_NAME                5 (float)
                       34 LOAD_NAME                6 (int)
                       36 BINARY_OP                7 (|)
                       40 BUILD_TUPLE              2
-                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\entry.py", line 226>)
+                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\entry.py", line 229>)
                       44 MAKE_FUNCTION            5 (defaults, annotations)
                       46 STORE_NAME               7 (border_radius)
          
-         232          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\entry.py", line 232>)
+         235          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\entry.py", line 235>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               8 (_draw)
          
-         261          54 LOAD_CONST              18 ((None,))
-                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\entry.py", line 261>)
+         265          54 LOAD_CONST              18 ((None,))
+                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\entry.py", line 265>)
                       58 MAKE_FUNCTION            1 (defaults)
                       60 STORE_NAME               9 (_focus)
          
-         270          62 LOAD_CONST              18 ((None,))
-                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\entry.py", line 270>)
+         274          62 LOAD_CONST              18 ((None,))
+                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\entry.py", line 274>)
                       66 MAKE_FUNCTION            1 (defaults)
                       68 STORE_NAME              10 (_focusout)
          
-         279          70 LOAD_CONST              18 ((None,))
-                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\entry.py", line 279>)
+         283          70 LOAD_CONST              18 ((None,))
+                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\entry.py", line 283>)
                       74 MAKE_FUNCTION            1 (defaults)
                       76 STORE_NAME              11 (_click)
          
-         282          78 LOAD_CONST              18 ((None,))
-                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\entry.py", line 282>)
+         286          78 LOAD_CONST              18 ((None,))
+                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\entry.py", line 286>)
                       82 MAKE_FUNCTION            1 (defaults)
                       84 STORE_NAME              12 (_hover)
          
-         285          86 LOAD_CONST              18 ((None,))
-                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\entry.py", line 285>)
+         289          86 LOAD_CONST              18 ((None,))
+                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\entry.py", line 289>)
                       90 MAKE_FUNCTION            1 (defaults)
                       92 STORE_NAME              13 (_hover_release)
          
-         296          94 LOAD_CONST              18 ((None,))
+         300          94 LOAD_CONST              18 ((None,))
                       96 LOAD_CONST              12 ('font')
                       98 LOAD_NAME               14 (Font)
                      100 BUILD_TUPLE              2
-                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\entry.py", line 296>)
+                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\entry.py", line 300>)
                      104 MAKE_FUNCTION            5 (defaults, annotations)
                      106 STORE_NAME              15 (font)
          
-         302         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 302>)
+         306         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 306>)
                      110 MAKE_FUNCTION            0
                      112 STORE_NAME              16 (default_palette)
          
-         305         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\entry.py", line 305>)
+         309         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\entry.py", line 309>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              17 (palette_light)
          
-         329         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\entry.py", line 329>)
+         333         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\entry.py", line 333>)
                      122 MAKE_FUNCTION            0
                      124 STORE_NAME              18 (palette_dark)
          
-         353         126 LOAD_CONST              18 ((None,))
-                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\entry.py", line 353>)
+         357         126 LOAD_CONST              18 ((None,))
+                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\entry.py", line 357>)
                      130 MAKE_FUNCTION            1 (defaults)
                      132 STORE_NAME              19 (palette)
                      134 LOAD_CLOSURE             0 (__class__)
                      136 COPY                     1
                      138 STORE_NAME              20 (__classcell__)
                      140 RETURN_VALUE
          consts
@@ -1865,17 +1868,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               219           2 RESUME                   0
+               222           2 RESUME                   0
                
-               220           4 PUSH_NULL
+               223           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -1888,95 +1891,95 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '__init__'
-               firstlineno 219
+               firstlineno 222
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006401a6020000ab020000000000
                   000000721e7c00a00100000000000000000000000000000000000000007c
                   006a0200000000000000006402ac03a6020000ab02000000000000000001
                   006400530064005300
-               222           0 RESUME                   0
+               225           0 RESUME                   0
                
-               223           2 LOAD_GLOBAL              1 (NULL + hasattr)
+               226           2 LOAD_GLOBAL              1 (NULL + hasattr)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_CONST               1 ('button_frame_back')
                             18 PRECALL                  2
                             22 CALL                     2
                             32 POP_JUMP_FORWARD_IF_FALSE    30 (to 94)
                
-               224          34 LOAD_FAST                0 (self)
+               227          34 LOAD_FAST                0 (self)
                             36 LOAD_METHOD              1 (configure)
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                2 (button_frame_back)
                             70 LOAD_CONST               2 (0)
                             72 KW_NAMES                 3
                             74 PRECALL                  2
                             78 CALL                     2
                             88 POP_TOP
                             90 LOAD_CONST               0 (None)
                             92 RETURN_VALUE
                
-               223     >>   94 LOAD_CONST               0 (None)
+               226     >>   94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                consts
                   None
                   'button_frame_back'
                   0
                   ('background', 'borderwidth')
                names      ('hasattr', 'configure', 'button_frame_back')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_other'
-               firstlineno 222
+               firstlineno 225
                lnotab 0x020120013cff
             None
             'radius'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               226           0 RESUME                   0
+               229           0 RESUME                   0
                
-               227           2 LOAD_FAST                1 (radius)
+               230           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               228           6 LOAD_FAST                0 (self)
+               231           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               230     >>   20 LOAD_FAST                1 (radius)
+               233     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'border_radius'
-               firstlineno 226
+               firstlineno 229
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -2010,29 +2013,29 @@
                   0aa6070000ab0700000000000000007c005f1000000000000000007c006a
                   0e000000000000000064066b0200000000721a7c00a00000000000000000
                   000000000000000000000000007c006a100000000000000000a6010000ab
                   01000000000000000001007c00a011000000000000000000000000000000
                   00000000007c006a1000000000000000007c006a0c0000000000000000a6
                   020000ab02000000000000000001007c006a0b0000000000000000a01200
                   000000000000000000000000000000000000007c006a0700000000000000
-                  007c006a130000000000000000ac0ba6020000ab02000000000000000001
-                  0064005300
-               232           0 RESUME                   0
+                  007c006a1300000000000000007c006a130000000000000000ac0ba60300
+                  00ab030000000000000000010064005300
+               235           0 RESUME                   0
                
-               233           2 LOAD_FAST                0 (self)
+               236           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               235          44 LOAD_FAST                0 (self)
+               238          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect2)
                
-               236          68 LOAD_CONST               2 (2)
+               239          68 LOAD_CONST               2 (2)
                             70 LOAD_CONST               2 (2)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
@@ -2041,233 +2044,236 @@
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                            160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (entry_radius)
                
-               237         172 LOAD_FAST                0 (self)
+               240         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (entry_border_width)
                
-               238         184 LOAD_FAST                0 (self)
+               241         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_entry_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_entry_back)
                
-               235         208 KW_NAMES                 4
+               238         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 LOAD_FAST                0 (self)
                            226 STORE_ATTR               8 (entry_frame)
                
-               241         236 LOAD_FAST                0 (self)
+               244         236 LOAD_FAST                0 (self)
                            238 LOAD_METHOD              9 (create_window)
                
-               242         260 LOAD_FAST                0 (self)
+               245         260 LOAD_FAST                0 (self)
                            262 LOAD_METHOD              2 (winfo_width)
                            284 PRECALL                  0
                            288 CALL                     0
                            298 LOAD_CONST               2 (2)
                            300 BINARY_OP               11 (/)
                            304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              3 (winfo_height)
                            328 PRECALL                  0
                            332 CALL                     0
                            342 LOAD_CONST               2 (2)
                            344 BINARY_OP               11 (/)
                
-               243         348 LOAD_FAST                0 (self)
+               246         348 LOAD_FAST                0 (self)
                            350 LOAD_METHOD              2 (winfo_width)
                            372 PRECALL                  0
                            376 CALL                     0
                            386 LOAD_FAST                0 (self)
                            388 LOAD_ATTR                5 (entry_border_width)
                            398 BINARY_OP               10 (-)
                            402 LOAD_CONST               5 (5)
                            404 BINARY_OP               10 (-)
                            408 LOAD_FAST                0 (self)
                            410 LOAD_ATTR               10 (entry_padding)
                            420 LOAD_CONST               6 (0)
                            422 BINARY_SUBSCR
                            432 BINARY_OP               10 (-)
                
-               244         436 LOAD_FAST                0 (self)
+               247         436 LOAD_FAST                0 (self)
                            438 LOAD_METHOD              3 (winfo_height)
                            460 PRECALL                  0
                            464 CALL                     0
                            474 LOAD_FAST                0 (self)
                            476 LOAD_ATTR                5 (entry_border_width)
                            486 BINARY_OP               10 (-)
                            490 LOAD_CONST               5 (5)
                            492 BINARY_OP               10 (-)
                            496 LOAD_FAST                0 (self)
                            498 LOAD_ATTR               10 (entry_padding)
                            508 LOAD_CONST               7 (1)
                            510 BINARY_SUBSCR
                            520 BINARY_OP               10 (-)
                
-               245         524 LOAD_FAST                0 (self)
+               248         524 LOAD_FAST                0 (self)
                            526 LOAD_ATTR               11 (entry)
                
-               241         536 KW_NAMES                 8
+               244         536 KW_NAMES                 8
                            538 PRECALL                  5
                            542 CALL                     5
                            552 LOAD_FAST                0 (self)
                            554 STORE_ATTR              12 (entry_text)
                
-               248         564 LOAD_FAST                0 (self)
+               251         564 LOAD_FAST                0 (self)
                            566 LOAD_METHOD             13 (create_rectangle)
                            588 LOAD_CONST               3 (3)
                            590 LOAD_FAST                0 (self)
                            592 LOAD_ATTR                4 (entry_radius)
                            602 LOAD_CONST               2 (2)
                            604 BINARY_OP               11 (/)
                            608 BINARY_OP                0 (+)
                
-               249         612 LOAD_FAST                0 (self)
+               252         612 LOAD_FAST                0 (self)
                            614 LOAD_METHOD              3 (winfo_height)
                            636 PRECALL                  0
                            640 CALL                     0
                            650 LOAD_FAST                0 (self)
                            652 LOAD_ATTR               14 (_entry_bottom_width)
                            662 BINARY_OP               10 (-)
                            666 LOAD_CONST               3 (3)
                            668 BINARY_OP               10 (-)
                
-               250         672 LOAD_FAST                0 (self)
+               253         672 LOAD_FAST                0 (self)
                            674 LOAD_METHOD              2 (winfo_width)
                            696 PRECALL                  0
                            700 CALL                     0
                            710 LOAD_CONST               3 (3)
                            712 BINARY_OP               10 (-)
                            716 LOAD_FAST                0 (self)
                            718 LOAD_ATTR                4 (entry_radius)
                            728 LOAD_CONST               2 (2)
                            730 BINARY_OP               11 (/)
                            734 BINARY_OP               10 (-)
                
-               251         738 LOAD_FAST                0 (self)
+               254         738 LOAD_FAST                0 (self)
                            740 LOAD_METHOD              3 (winfo_height)
                            762 PRECALL                  0
                            766 CALL                     0
                            776 LOAD_CONST               9 (3.5)
                            778 BINARY_OP               10 (-)
                
-               252         782 LOAD_FAST                0 (self)
+               255         782 LOAD_FAST                0 (self)
                            784 LOAD_ATTR               15 (_entry_bottom_line)
                            794 LOAD_FAST                0 (self)
                            796 LOAD_ATTR               15 (_entry_bottom_line)
-                           806 LOAD_CONST               6 (0)
                
-               248         808 KW_NAMES                10
+               256         806 LOAD_CONST               6 (0)
+               
+               251         808 KW_NAMES                10
                            810 PRECALL                  7
                            814 CALL                     7
                            824 LOAD_FAST                0 (self)
                            826 STORE_ATTR              16 (entry_bottom)
                
-               254         836 LOAD_FAST                0 (self)
+               258         836 LOAD_FAST                0 (self)
                            838 LOAD_ATTR               14 (_entry_bottom_width)
                            848 LOAD_CONST               6 (0)
                            850 COMPARE_OP               2 (==)
                            856 POP_JUMP_FORWARD_IF_FALSE    26 (to 910)
                
-               255         858 LOAD_FAST                0 (self)
+               259         858 LOAD_FAST                0 (self)
                            860 LOAD_METHOD              0 (delete)
                            882 LOAD_FAST                0 (self)
                            884 LOAD_ATTR               16 (entry_bottom)
                            894 PRECALL                  1
                            898 CALL                     1
                            908 POP_TOP
                
-               257     >>  910 LOAD_FAST                0 (self)
+               261     >>  910 LOAD_FAST                0 (self)
                            912 LOAD_METHOD             17 (tag_raise)
                            934 LOAD_FAST                0 (self)
                            936 LOAD_ATTR               16 (entry_bottom)
                            946 LOAD_FAST                0 (self)
                            948 LOAD_ATTR               12 (entry_text)
                            958 PRECALL                  2
                            962 CALL                     2
                            972 POP_TOP
                
-               259         974 LOAD_FAST                0 (self)
+               263         974 LOAD_FAST                0 (self)
                            976 LOAD_ATTR               11 (entry)
                            986 LOAD_METHOD             18 (configure)
                           1008 LOAD_FAST                0 (self)
                           1010 LOAD_ATTR                7 (_entry_back)
                           1020 LOAD_FAST                0 (self)
                           1022 LOAD_ATTR               19 (_entry_text_back)
-                          1032 KW_NAMES                11
-                          1034 PRECALL                  2
-                          1038 CALL                     2
-                          1048 POP_TOP
-                          1050 LOAD_CONST               0 (None)
-                          1052 RETURN_VALUE
+                          1032 LOAD_FAST                0 (self)
+                          1034 LOAD_ATTR               19 (_entry_text_back)
+                          1044 KW_NAMES                11
+                          1046 PRECALL                  3
+                          1050 CALL                     3
+                          1060 POP_TOP
+                          1062 LOAD_CONST               0 (None)
+                          1064 RETURN_VALUE
                consts
                   None
                   'all'
                   2
                   3
                   ('width', 'outline', 'fill')
                   5
                   0
                   1
                   ('width', 'height', 'window')
                   3.5
                   ('fill', 'outline', 'width')
-                  ('background', 'foreground')
+                  ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_round_rect2', 'winfo_width', 'winfo_height', 'entry_radius', 'entry_border_width', '_entry_border', '_entry_back', 'entry_frame', 'create_window', 'entry_padding', 'entry', 'entry_text', 'create_rectangle', '_entry_bottom_width', '_entry_bottom_line', 'entry_bottom', 'tag_raise', 'configure', '_entry_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_draw'
-               firstlineno 232
+               firstlineno 235
                lnotab
                   0x02012a02180168010c0118fd1c0618015801580158010cfc1c0730013c
-                  0142012c011afc1c06160134024002
+                  0142012c01180102fb1c07160134024002
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               261           0 RESUME                   0
+               265           0 RESUME                   0
                
-               262           2 LOAD_FAST                0 (self)
+               266           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (entry_focusin_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_entry_back)
                
-               263          26 LOAD_FAST                0 (self)
+               267          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (entry_focusin_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_entry_border)
                
-               264          50 LOAD_FAST                0 (self)
+               268          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (entry_focusin_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_entry_text_back)
                
-               265          74 LOAD_FAST                0 (self)
+               269          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (entry_focusin_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_entry_bottom_line)
                
-               266          98 LOAD_FAST                0 (self)
+               270          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (entry_focusin_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_entry_bottom_width)
                
-               268         122 LOAD_FAST                0 (self)
+               272         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -2275,56 +2281,56 @@
                   None
                names      ('entry_focusin_back', '_entry_back', 'entry_focusin_border', '_entry_border', 'entry_focusin_text_back', '_entry_text_back', 'entry_focusin_bottom_line', '_entry_bottom_line', 'entry_focusin_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_focus'
-               firstlineno 261
+               firstlineno 265
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               270           0 RESUME                   0
+               274           0 RESUME                   0
                
-               271           2 LOAD_FAST                0 (self)
+               275           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (entry_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_entry_back)
                
-               272          26 LOAD_FAST                0 (self)
+               276          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (entry_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_entry_border)
                
-               273          50 LOAD_FAST                0 (self)
+               277          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (entry_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_entry_text_back)
                
-               274          74 LOAD_FAST                0 (self)
+               278          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (entry_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_entry_bottom_line)
                
-               275          98 LOAD_FAST                0 (self)
+               279          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (entry_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_entry_bottom_width)
                
-               277         122 LOAD_FAST                0 (self)
+               281         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -2332,66 +2338,66 @@
                   None
                names      ('entry_back', '_entry_back', 'entry_border', '_entry_border', 'entry_text_back', '_entry_text_back', 'entry_bottom_line', '_entry_bottom_line', 'entry_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_focusout'
-               firstlineno 270
+               firstlineno 274
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               279           0 RESUME                   0
+               283           0 RESUME                   0
                
-               280           2 LOAD_FAST                0 (self)
+               284           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_set)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('focus_set',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_click'
-               firstlineno 279
+               firstlineno 283
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064005300
-               282           0 RESUME                   0
+               286           0 RESUME                   0
                
-               283           2 LOAD_CONST               1 (True)
+               287           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                   True
                names      ('hover',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_hover'
-               firstlineno 282
+               firstlineno 286
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -2399,179 +2405,179 @@
                   00ab000000000000000000735a64017c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c006a0a00000000000000007c005f0b00000000000000007c00a0
                   0c00000000000000000000000000000000000000006400a6010000ab0100
                   0000000000000001006400530064005300
-               285           0 RESUME                   0
+               289           0 RESUME                   0
                
-               286           2 LOAD_FAST                0 (self)
+               290           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_get)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_JUMP_FORWARD_IF_TRUE    90 (to 222)
                
-               287          42 LOAD_CONST               1 (False)
+               291          42 LOAD_CONST               1 (False)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (hover)
                
-               288          56 LOAD_FAST                0 (self)
+               292          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (entry_back)
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_entry_back)
                
-               289          80 LOAD_FAST                0 (self)
+               293          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (entry_border)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               5 (_entry_border)
                
-               290         104 LOAD_FAST                0 (self)
+               294         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (entry_text_back)
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               7 (_entry_text_back)
                
-               291         128 LOAD_FAST                0 (self)
+               295         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                8 (entry_bottom_line)
                            140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               9 (_entry_bottom_line)
                
-               292         152 LOAD_FAST                0 (self)
+               296         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR               10 (entry_bottom_width)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR              11 (_entry_bottom_width)
                
-               294         176 LOAD_FAST                0 (self)
+               298         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD             12 (_draw)
                            200 LOAD_CONST               0 (None)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                
-               286     >>  222 LOAD_CONST               0 (None)
+               290     >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   False
                names      ('focus_get', 'hover', 'entry_back', '_entry_back', 'entry_border', '_entry_border', 'entry_text_back', '_entry_text_back', 'entry_bottom_line', '_entry_bottom_line', 'entry_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_hover_release'
-               firstlineno 285
+               firstlineno 289
                lnotab 0x020128010e01180118011801180118022ef8
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               296           0 RESUME                   0
+               300           0 RESUME                   0
                
-               297           2 LOAD_FAST                1 (font)
+               301           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               298           6 LOAD_FAST                0 (self)
+               302           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (entry_text_font)
                             18 RETURN_VALUE
                
-               300     >>   20 LOAD_FAST                1 (font)
+               304     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (entry_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('entry_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'font'
-               firstlineno 296
+               firstlineno 300
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               302           0 RESUME                   0
+               306           0 RESUME                   0
                
-               303           2 LOAD_FAST                0 (self)
+               307           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 302
+               firstlineno 306
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640864066409640a640b640c640d640e9c0ea6
                   010000ab010000000000000000010064005300
-               305           0 RESUME                   0
+               309           0 RESUME                   0
                
-               306           2 LOAD_FAST                0 (self)
+               310           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               308          26 LOAD_CONST               1 (6)
+               312          26 LOAD_CONST               1 (6)
                
-               310          28 LOAD_CONST               2 ((3, 4))
+               314          28 LOAD_CONST               2 ((3, 4))
                
-               312          30 LOAD_CONST               3 ('#f3f3f3')
+               316          30 LOAD_CONST               3 ('#f3f3f3')
                
-               313          32 LOAD_CONST               4 (1)
+               317          32 LOAD_CONST               4 (1)
                
-               314          34 LOAD_CONST               5 (0)
+               318          34 LOAD_CONST               5 (0)
                
-               316          36 LOAD_CONST               6 ('#eaeaea')
+               320          36 LOAD_CONST               6 ('#eaeaea')
                
-               317          38 LOAD_CONST               7 ('#fdfdfd')
+               321          38 LOAD_CONST               7 ('#fdfdfd')
                
-               318          40 LOAD_CONST               8 ('#5f5f5f')
+               322          40 LOAD_CONST               8 ('#5f5f5f')
                
-               319          42 LOAD_CONST               6 ('#eaeaea')
+               323          42 LOAD_CONST               6 ('#eaeaea')
                
-               321          44 LOAD_CONST               9 ('#e2e2e2')
+               325          44 LOAD_CONST               9 ('#e2e2e2')
                
-               322          46 LOAD_CONST              10 ('#f9f9f9')
+               326          46 LOAD_CONST              10 ('#f9f9f9')
                
-               323          48 LOAD_CONST              11 ('#1a1a1a')
+               327          48 LOAD_CONST              11 ('#1a1a1a')
                
-               324          50 LOAD_CONST              12 ('#185fb4')
+               328          50 LOAD_CONST              12 ('#185fb4')
                
-               325          52 LOAD_CONST              13 (2)
+               329          52 LOAD_CONST              13 (2)
                
-               307          54 LOAD_CONST              14 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
+               311          54 LOAD_CONST              14 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
                             56 BUILD_CONST_KEY_MAP     14
                
-               306          58 PRECALL                  1
+               310          58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
                   6
@@ -2590,64 +2596,64 @@
                   ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette_light'
-               firstlineno 305
+               firstlineno 309
                lnotab
                   0x0201180202020202020102010202020102010201020202010201020102
                   0102ee04ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640864096405640a6408640b640c640d9c0ea6
                   010000ab010000000000000000010064005300
-               329           0 RESUME                   0
+               333           0 RESUME                   0
                
-               330           2 LOAD_FAST                0 (self)
+               334           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               332          26 LOAD_CONST               1 (6)
+               336          26 LOAD_CONST               1 (6)
                
-               334          28 LOAD_CONST               2 ((3, 4))
+               338          28 LOAD_CONST               2 ((3, 4))
                
-               336          30 LOAD_CONST               3 ('#202020')
+               340          30 LOAD_CONST               3 ('#202020')
                
-               337          32 LOAD_CONST               4 (1)
+               341          32 LOAD_CONST               4 (1)
                
-               339          34 LOAD_CONST               5 ('#454545')
+               343          34 LOAD_CONST               5 ('#454545')
                
-               340          36 LOAD_CONST               6 ('#353535')
+               344          36 LOAD_CONST               6 ('#353535')
                
-               341          38 LOAD_CONST               7 ('#cecece')
+               345          38 LOAD_CONST               7 ('#cecece')
                
-               342          40 LOAD_CONST               8 ('#ffffff')
+               346          40 LOAD_CONST               8 ('#ffffff')
                
-               343          42 LOAD_CONST               9 (0)
+               347          42 LOAD_CONST               9 (0)
                
-               345          44 LOAD_CONST               5 ('#454545')
+               349          44 LOAD_CONST               5 ('#454545')
                
-               346          46 LOAD_CONST              10 ('#2f2f2f')
+               350          46 LOAD_CONST              10 ('#2f2f2f')
                
-               347          48 LOAD_CONST               8 ('#ffffff')
+               351          48 LOAD_CONST               8 ('#ffffff')
                
-               348          50 LOAD_CONST              11 ('#4cc2ff')
+               352          50 LOAD_CONST              11 ('#4cc2ff')
                
-               349          52 LOAD_CONST              12 (2)
+               353          52 LOAD_CONST              12 (2)
                
-               331          54 LOAD_CONST              13 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
+               335          54 LOAD_CONST              13 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
                             56 BUILD_CONST_KEY_MAP     14
                
-               330          58 PRECALL                  1
+               334          58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
                   6
@@ -2665,15 +2671,15 @@
                   ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette_dark'
-               firstlineno 329
+               firstlineno 333
                lnotab
                   0x0201180202020202020102020201020102010201020202010201020102
                   0102ee04ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 11
@@ -2695,160 +2701,160 @@
                   000000000000006400a6010000ab01000000000000000001006400530023
                   00741e000000000000000000002400720401005900640053007700780359
                   0077017c006a0100000000000000007c006a0200000000000000007c006a
                   0300000000000000007c006a0800000000000000007c006a040000000000
                   0000007c006a0500000000000000007c006a0600000000000000007c006a
                   0900000000000000007c006a0a00000000000000007c006a0b0000000000
                   000000640f9c0a5300
-               353           0 RESUME                   0
+               357           0 RESUME                   0
                
-               354           2 LOAD_FAST                1 (dict)
+               358           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE   223 (to 452)
                
-               355           6 LOAD_FAST                1 (dict)
+               359           6 LOAD_FAST                1 (dict)
                              8 LOAD_CONST               1 ('entry_radius')
                             10 BINARY_SUBSCR
                             20 LOAD_FAST                0 (self)
                             22 STORE_ATTR               0 (entry_radius)
                
-               357          32 LOAD_FAST                1 (dict)
+               361          32 LOAD_FAST                1 (dict)
                             34 LOAD_CONST               2 ('entry_padding')
                             36 BINARY_SUBSCR
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               1 (entry_padding)
                
-               359          58 LOAD_FAST                1 (dict)
+               363          58 LOAD_FAST                1 (dict)
                             60 LOAD_CONST               3 ('entry_frame_back')
                             62 BINARY_SUBSCR
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (entry_frame_back)
                
-               360          84 LOAD_FAST                1 (dict)
+               364          84 LOAD_FAST                1 (dict)
                             86 LOAD_CONST               4 ('entry_border_width')
                             88 BINARY_SUBSCR
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               3 (entry_border_width)
                
-               362         110 LOAD_FAST                1 (dict)
+               366         110 LOAD_FAST                1 (dict)
                            112 LOAD_CONST               5 ('entry_border')
                            114 BINARY_SUBSCR
                            124 LOAD_FAST                0 (self)
                            126 STORE_ATTR               4 (entry_border)
                
-               363         136 LOAD_FAST                1 (dict)
+               367         136 LOAD_FAST                1 (dict)
                            138 LOAD_CONST               6 ('entry_back')
                            140 BINARY_SUBSCR
                            150 LOAD_FAST                0 (self)
                            152 STORE_ATTR               5 (entry_back)
                
-               364         162 LOAD_FAST                1 (dict)
+               368         162 LOAD_FAST                1 (dict)
                            164 LOAD_CONST               7 ('entry_text_back')
                            166 BINARY_SUBSCR
                            176 LOAD_FAST                0 (self)
                            178 STORE_ATTR               6 (entry_text_back)
                
-               365         188 LOAD_FAST                1 (dict)
+               369         188 LOAD_FAST                1 (dict)
                            190 LOAD_CONST               8 ('entry_bottom_line')
                            192 BINARY_SUBSCR
                            202 LOAD_FAST                0 (self)
                            204 STORE_ATTR               7 (entry_bottom_line)
                
-               366         214 LOAD_FAST                1 (dict)
+               370         214 LOAD_FAST                1 (dict)
                            216 LOAD_CONST               9 ('entry_bottom_width')
                            218 BINARY_SUBSCR
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (entry_bottom_width)
                
-               368         240 LOAD_FAST                1 (dict)
+               372         240 LOAD_FAST                1 (dict)
                            242 LOAD_CONST              10 ('entry_focusin_border')
                            244 BINARY_SUBSCR
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (entry_focusin_border)
                
-               369         266 LOAD_FAST                1 (dict)
+               373         266 LOAD_FAST                1 (dict)
                            268 LOAD_CONST              11 ('entry_focusin_back')
                            270 BINARY_SUBSCR
                            280 LOAD_FAST                0 (self)
                            282 STORE_ATTR              10 (entry_focusin_back)
                
-               370         292 LOAD_FAST                1 (dict)
+               374         292 LOAD_FAST                1 (dict)
                            294 LOAD_CONST              12 ('entry_focusin_text_back')
                            296 BINARY_SUBSCR
                            306 LOAD_FAST                0 (self)
                            308 STORE_ATTR              11 (entry_focusin_text_back)
                
-               371         318 LOAD_FAST                1 (dict)
+               375         318 LOAD_FAST                1 (dict)
                            320 LOAD_CONST              13 ('entry_focusin_bottom_line')
                            322 BINARY_SUBSCR
                            332 LOAD_FAST                0 (self)
                            334 STORE_ATTR              12 (entry_focusin_bottom_line)
                
-               372         344 LOAD_FAST                1 (dict)
+               376         344 LOAD_FAST                1 (dict)
                            346 LOAD_CONST              14 ('entry_focusin_bottom_width')
                            348 BINARY_SUBSCR
                            358 LOAD_FAST                0 (self)
                            360 STORE_ATTR              13 (entry_focusin_bottom_width)
                
-               374         370 NOP
+               378         370 NOP
                
-               375         372 LOAD_FAST                0 (self)
+               379         372 LOAD_FAST                0 (self)
                            374 LOAD_METHOD             14 (_draw)
                            396 LOAD_CONST               0 (None)
                            398 PRECALL                  1
                            402 CALL                     1
                            412 POP_TOP
                            414 LOAD_CONST               0 (None)
                            416 RETURN_VALUE
                        >>  418 PUSH_EXC_INFO
                
-               376         420 LOAD_GLOBAL             30 (AttributeError)
+               380         420 LOAD_GLOBAL             30 (AttributeError)
                            432 CHECK_EXC_MATCH
                            434 POP_JUMP_FORWARD_IF_FALSE     4 (to 444)
                            436 POP_TOP
                
-               377         438 POP_EXCEPT
+               381         438 POP_EXCEPT
                            440 LOAD_CONST               0 (None)
                            442 RETURN_VALUE
                
-               376     >>  444 RERAISE                  0
+               380     >>  444 RERAISE                  0
                        >>  446 COPY                     3
                            448 POP_EXCEPT
                            450 RERAISE                  1
                
-               380     >>  452 LOAD_FAST                0 (self)
+               384     >>  452 LOAD_FAST                0 (self)
                            454 LOAD_ATTR                1 (entry_padding)
                
-               382         464 LOAD_FAST                0 (self)
+               386         464 LOAD_FAST                0 (self)
                            466 LOAD_ATTR                2 (entry_frame_back)
                
-               383         476 LOAD_FAST                0 (self)
+               387         476 LOAD_FAST                0 (self)
                            478 LOAD_ATTR                3 (entry_border_width)
                
-               384         488 LOAD_FAST                0 (self)
+               388         488 LOAD_FAST                0 (self)
                            490 LOAD_ATTR                8 (entry_bottom_width)
                
-               386         500 LOAD_FAST                0 (self)
+               390         500 LOAD_FAST                0 (self)
                            502 LOAD_ATTR                4 (entry_border)
                
-               387         512 LOAD_FAST                0 (self)
+               391         512 LOAD_FAST                0 (self)
                            514 LOAD_ATTR                5 (entry_back)
                
-               388         524 LOAD_FAST                0 (self)
+               392         524 LOAD_FAST                0 (self)
                            526 LOAD_ATTR                6 (entry_text_back)
                
-               390         536 LOAD_FAST                0 (self)
+               394         536 LOAD_FAST                0 (self)
                            538 LOAD_ATTR                9 (entry_focusin_border)
                
-               391         548 LOAD_FAST                0 (self)
+               395         548 LOAD_FAST                0 (self)
                            550 LOAD_ATTR               10 (entry_focusin_back)
                
-               392         560 LOAD_FAST                0 (self)
+               396         560 LOAD_FAST                0 (self)
                            562 LOAD_ATTR               11 (entry_focusin_text_back)
                
-               379         572 LOAD_CONST              15 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back'))
+               383         572 LOAD_CONST              15 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back'))
                            574 BUILD_CONST_KEY_MAP     10
                            576 RETURN_VALUE
                ExceptionTable:
                  372 to 412 -> 418 [0]
                  418 to 436 -> 446 [1] lasti
                  444 to 444 -> 446 [1] lasti
                consts
@@ -2870,139 +2876,139 @@
                   ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back')
                names      ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette'
-               firstlineno 353
+               firstlineno 357
                lnotab
                   0x020104011a021a021a011a021a011a011a011a011a021a011a011a011a
                   011a0202013001120106ff08040c020c010c010c020c010c010c020c010c
                   010cf3
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'float', 'int', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawBasicRoundEntry'
-         firstlineno 218
-         lnotab 0x0c010a0306041406061d0809080908030803080b0e06060306180618
+         firstlineno 221
+         lnotab 0x0c010a0306041406061e0809080908030803080b0e06060306180618
       'AdwDrawBasicRoundEntry'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         396           0 RESUME                   0
+         400           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundEntry')
                        8 STORE_NAME               2 (__qualname__)
          
-         397          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 397>)
+         401          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 401>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundEntry'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               397           0 RESUME                   0
+               401           0 RESUME                   0
                
-               398           2 LOAD_FAST                0 (self)
+               402           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 397
+               firstlineno 401
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawRoundEntry'
-         firstlineno 396
+         firstlineno 400
          lnotab 0x0a01
       'AdwDrawRoundEntry'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         401           0 RESUME                   0
+         405           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkEntry')
                        8 STORE_NAME               2 (__qualname__)
          
-         402          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 402>)
+         406          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 406>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkEntry'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               402           0 RESUME                   0
+               406           0 RESUME                   0
                
-               403           2 LOAD_FAST                0 (self)
+               407           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 402
+               firstlineno 406
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawRoundDarkEntry'
-         firstlineno 401
+         firstlineno 405
          lnotab 0x0a01
       'AdwDrawRoundDarkEntry'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
@@ -3010,91 +3016,91 @@
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             126404650565067a0700006602640584055a07640684005a086412640784
             015a096412640884015a0a6412640984015a0b6412640a84015a0c641264
             0b84015a0d6412640c650e6602640d84055a0f640e84005a10640f84005a
             11641084005a126412641184015a13880078015a145300
                        0 MAKE_CELL                0 (__class__)
          
-         406           2 RESUME                   0
+         410           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundEntry3')
                       10 STORE_NAME               2 (__qualname__)
          
-         407          12 LOAD_CLOSURE             0 (__class__)
+         411          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\entry.py", line 407>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\entry.py", line 411>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         410          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\entry.py", line 410>)
+         414          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\entry.py", line 414>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         414          28 LOAD_CONST              18 ((None,))
+         417          28 LOAD_CONST              18 ((None,))
                       30 LOAD_CONST               4 ('radius')
                       32 LOAD_NAME                5 (float)
                       34 LOAD_NAME                6 (int)
                       36 BINARY_OP                7 (|)
                       40 BUILD_TUPLE              2
-                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\entry.py", line 414>)
+                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\entry.py", line 417>)
                       44 MAKE_FUNCTION            5 (defaults, annotations)
                       46 STORE_NAME               7 (border_radius)
          
-         420          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\entry.py", line 420>)
+         423          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\entry.py", line 423>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               8 (_draw)
          
-         455          54 LOAD_CONST              18 ((None,))
-                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\entry.py", line 455>)
+         459          54 LOAD_CONST              18 ((None,))
+                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\entry.py", line 459>)
                       58 MAKE_FUNCTION            1 (defaults)
                       60 STORE_NAME               9 (_focus)
          
-         464          62 LOAD_CONST              18 ((None,))
-                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\entry.py", line 464>)
+         468          62 LOAD_CONST              18 ((None,))
+                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\entry.py", line 468>)
                       66 MAKE_FUNCTION            1 (defaults)
                       68 STORE_NAME              10 (_focusout)
          
-         473          70 LOAD_CONST              18 ((None,))
-                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\entry.py", line 473>)
+         477          70 LOAD_CONST              18 ((None,))
+                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\entry.py", line 477>)
                       74 MAKE_FUNCTION            1 (defaults)
                       76 STORE_NAME              11 (_click)
          
-         476          78 LOAD_CONST              18 ((None,))
-                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\entry.py", line 476>)
+         480          78 LOAD_CONST              18 ((None,))
+                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\entry.py", line 480>)
                       82 MAKE_FUNCTION            1 (defaults)
                       84 STORE_NAME              12 (_hover)
          
-         479          86 LOAD_CONST              18 ((None,))
-                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\entry.py", line 479>)
+         483          86 LOAD_CONST              18 ((None,))
+                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\entry.py", line 483>)
                       90 MAKE_FUNCTION            1 (defaults)
                       92 STORE_NAME              13 (_hover_release)
          
-         490          94 LOAD_CONST              18 ((None,))
+         494          94 LOAD_CONST              18 ((None,))
                       96 LOAD_CONST              12 ('font')
                       98 LOAD_NAME               14 (Font)
                      100 BUILD_TUPLE              2
-                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\entry.py", line 490>)
+                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\entry.py", line 494>)
                      104 MAKE_FUNCTION            5 (defaults, annotations)
                      106 STORE_NAME              15 (font)
          
-         496         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 496>)
+         500         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 500>)
                      110 MAKE_FUNCTION            0
                      112 STORE_NAME              16 (default_palette)
          
-         499         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\entry.py", line 499>)
+         503         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\entry.py", line 503>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              17 (palette_light)
          
-         523         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\entry.py", line 523>)
+         527         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\entry.py", line 527>)
                      122 MAKE_FUNCTION            0
                      124 STORE_NAME              18 (palette_dark)
          
-         547         126 LOAD_CONST              18 ((None,))
-                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\entry.py", line 547>)
+         551         126 LOAD_CONST              18 ((None,))
+                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\entry.py", line 551>)
                      130 MAKE_FUNCTION            1 (defaults)
                      132 STORE_NAME              19 (palette)
                      134 LOAD_CLOSURE             0 (__class__)
                      136 COPY                     1
                      138 STORE_NAME              20 (__classcell__)
                      140 RETURN_VALUE
          consts
@@ -3105,17 +3111,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               407           2 RESUME                   0
+               411           2 RESUME                   0
                
-               408           4 PUSH_NULL
+               412           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -3128,407 +3134,389 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '__init__'
-               firstlineno 407
+               firstlineno 411
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 4
+               stacksize : 5
                flags     : 3
                code
-                  0x97007401000000000000000000007c006401a6020000ab020000000000
-                  000000721e7c00a00100000000000000000000000000000000000000007c
-                  006a0200000000000000006402ac03a6020000ab02000000000000000001
-                  006400530064005300
-               410           0 RESUME                   0
-               
-               411           2 LOAD_GLOBAL              1 (NULL + hasattr)
-                            14 LOAD_FAST                0 (self)
-                            16 LOAD_CONST               1 ('button_frame_back')
-                            18 PRECALL                  2
-                            22 CALL                     2
-                            32 POP_JUMP_FORWARD_IF_FALSE    30 (to 94)
-               
-               412          34 LOAD_FAST                0 (self)
-                            36 LOAD_METHOD              1 (configure)
-                            58 LOAD_FAST                0 (self)
-                            60 LOAD_ATTR                2 (button_frame_back)
-                            70 LOAD_CONST               2 (0)
-                            72 KW_NAMES                 3
-                            74 PRECALL                  2
-                            78 CALL                     2
-                            88 POP_TOP
-                            90 LOAD_CONST               0 (None)
-                            92 RETURN_VALUE
+                  0x97007c00a00000000000000000000000000000000000000000007c006a
+                  010000000000000000a00200000000000000000000000000000000000000
+                  006401a6010000ab0100000000000000006402ac03a6020000ab02000000
+                  0000000000010064005300
+               414           0 RESUME                   0
                
-               411     >>   94 LOAD_CONST               0 (None)
-                            96 RETURN_VALUE
+               415           2 LOAD_FAST                0 (self)
+                             4 LOAD_METHOD              0 (configure)
+                            26 LOAD_FAST                0 (self)
+                            28 LOAD_ATTR                1 (master)
+                            38 LOAD_METHOD              2 (cget)
+                            60 LOAD_CONST               1 ('bg')
+                            62 PRECALL                  1
+                            66 CALL                     1
+                            76 LOAD_CONST               2 (0)
+                            78 KW_NAMES                 3
+                            80 PRECALL                  2
+                            84 CALL                     2
+                            94 POP_TOP
+                            96 LOAD_CONST               0 (None)
+                            98 RETURN_VALUE
                consts
                   None
-                  'button_frame_back'
+                  'bg'
                   0
                   ('background', 'borderwidth')
-               names      ('hasattr', 'configure', 'button_frame_back')
+               names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_other'
-               firstlineno 410
-               lnotab 0x020120013cff
+               firstlineno 414
+               lnotab 0x0201
             None
             'radius'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               414           0 RESUME                   0
+               417           0 RESUME                   0
                
-               415           2 LOAD_FAST                1 (radius)
+               418           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               416           6 LOAD_FAST                0 (self)
+               419           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               418     >>   20 LOAD_FAST                1 (radius)
+               421     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'border_radius'
-               firstlineno 414
+               firstlineno 417
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab01000000000000000001007c00a0010000000000000000000000
-                  0000000000000000007c006a02000000000000000064027a0000007c006a
-                  02000000000000000064027a0000007c00a0030000000000000000000000
-                  000000000000000000a6000000ab0000000000000000007c006a02000000
-                  00000000007a0a000064037a0a00007c00a0040000000000000000000000
-                  000000000000000000a6000000ab0000000000000000007c006a02000000
-                  00000000007a0a000064037a0a00007c006a0500000000000000007c006a
-                  0200000000000000007c006a0600000000000000007c006a070000000000
-                  000000ac04a6080000ab080000000000000000010064057c005f08000000
-                  00000000007c00a00900000000000000000000000000000000000000007c
-                  00a0030000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000064037a0b00007c00a00400000000000000000000000000
-                  00000000000000a6000000ab00000000000000000064037a0b00007c00a0
+                  000000000000000000640264027c00a00200000000000000000000000000
+                  00000000000000a6000000ab00000000000000000064037a0a00007c00a0
                   030000000000000000000000000000000000000000a6000000ab00000000
-                  00000000007c006a0200000000000000007a0a000064067a0a00007c006a
-                  0a00000000000000006407190000000000000000007a0a00007c00a00400
+                  000000000064037a0a00007c006a0400000000000000007c006a05000000
+                  00000000007c006a0600000000000000007c006a070000000000000000ac
+                  04a6080000ab080000000000000000010064057c005f0800000000000000
+                  007c00a00900000000000000000000000000000000000000007c00a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
-                  0000007c006a0200000000000000007a0a000064067a0a00007c006a0a00
-                  000000000000006402190000000000000000007a0a00007c006a0b000000
-                  0000000000ac08a6050000ab0500000000000000007c005f0c0000000000
-                  0000007c00a00d000000000000000000000000000000000000000064097c
-                  006a05000000000000000064067a0b00007a0000007c00a0040000000000
+                  00000064067a0b00007c00a0030000000000000000000000000000000000
+                  000000a6000000ab00000000000000000064067a0b00007c00a002000000
+                  0000000000000000000000000000000000a6000000ab0000000000000000
+                  007c006a0500000000000000007a0a00007c006a0a000000000000000064
+                  02190000000000000000007a0a000064067a0a00007c00a0030000000000
                   000000000000000000000000000000a6000000ab0000000000000000007c
-                  006a0e00000000000000007a0a000064097a0a00007c00a0030000000000
-                  000000000000000000000000000000a6000000ab00000000000000000064
-                  097a0a00007c006a05000000000000000064067a0b00007a0a00007c00a0
-                  040000000000000000000000000000000000000000a6000000ab00000000
-                  0000000000640a7a0a00007c006a0f00000000000000007c006a0f000000
-                  00000000006407ac0ba6070000ab0700000000000000007c005f10000000
-                  00000000007c006a0e000000000000000064076b0200000000721a7c00a0
-                  0000000000000000000000000000000000000000007c006a100000000000
-                  000000a6010000ab01000000000000000001007c00a01100000000000000
-                  000000000000000000000000007c006a1000000000000000007c006a0c00
-                  00000000000000a6020000ab02000000000000000001007c006a0b000000
-                  0000000000a01200000000000000000000000000000000000000007c006a
-                  0700000000000000007c006a130000000000000000ac0ca6020000ab0200
-                  00000000000000010064005300
-               420           0 RESUME                   0
+                  006a0500000000000000007a0a00007c006a0a0000000000000000640319
+                  0000000000000000007a0a000064067a0a00007c006a0b00000000000000
+                  00ac07a6050000ab0500000000000000007c005f0c00000000000000007c
+                  00a00d000000000000000000000000000000000000000064037c006a0400
+                  0000000000000064087a0b00007a0000007c00a003000000000000000000
+                  0000000000000000000000a6000000ab0000000000000000007c006a0e00
+                  000000000000007a0a000064037a0a00007c00a002000000000000000000
+                  0000000000000000000000a6000000ab00000000000000000064037a0a00
+                  007c006a04000000000000000064087a0b00007a0a00007c00a003000000
+                  0000000000000000000000000000000000a6000000ab0000000000000000
+                  0064037a0a00007c006a0f00000000000000007c006a0f00000000000000
+                  006402ac09a6070000ab0700000000000000007c005f1000000000000000
+                  007c006a0e000000000000000064026b0200000000721a7c00a000000000
+                  00000000000000000000000000000000007c006a100000000000000000a6
+                  010000ab01000000000000000001007c00a0110000000000000000000000
+                  0000000000000000007c006a1000000000000000007c006a0c0000000000
+                  000000a6020000ab02000000000000000001007c006a0b00000000000000
+                  00a01200000000000000000000000000000000000000007c006a07000000
+                  00000000007c006a1300000000000000007c006a130000000000000000ac
+                  0aa6030000ab030000000000000000010064005300
+               423           0 RESUME                   0
                
-               421           2 LOAD_FAST                0 (self)
+               424           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               423          44 LOAD_FAST                0 (self)
+               426          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
-               424          68 LOAD_FAST                0 (self)
-                            70 LOAD_ATTR                2 (entry_border_width)
-                            80 LOAD_CONST               2 (1)
-                            82 BINARY_OP                0 (+)
-               
-               425          86 LOAD_FAST                0 (self)
-                            88 LOAD_ATTR                2 (entry_border_width)
-                            98 LOAD_CONST               2 (1)
-                           100 BINARY_OP                0 (+)
-               
-               426         104 LOAD_FAST                0 (self)
-                           106 LOAD_METHOD              3 (winfo_width)
-                           128 PRECALL                  0
-                           132 CALL                     0
-                           142 LOAD_FAST                0 (self)
-                           144 LOAD_ATTR                2 (entry_border_width)
-                           154 BINARY_OP               10 (-)
-                           158 LOAD_CONST               3 (2)
-                           160 BINARY_OP               10 (-)
-               
-               427         164 LOAD_FAST                0 (self)
-                           166 LOAD_METHOD              4 (winfo_height)
-                           188 PRECALL                  0
-                           192 CALL                     0
-                           202 LOAD_FAST                0 (self)
-                           204 LOAD_ATTR                2 (entry_border_width)
-                           214 BINARY_OP               10 (-)
-                           218 LOAD_CONST               3 (2)
-                           220 BINARY_OP               10 (-)
-                           224 LOAD_FAST                0 (self)
-                           226 LOAD_ATTR                5 (entry_radius)
+               427          68 LOAD_CONST               2 (0)
                
-               428         236 LOAD_FAST                0 (self)
-                           238 LOAD_ATTR                2 (entry_border_width)
+               428          70 LOAD_CONST               2 (0)
                
-               429         248 LOAD_FAST                0 (self)
-                           250 LOAD_ATTR                6 (_entry_border)
-                           260 LOAD_FAST                0 (self)
-                           262 LOAD_ATTR                7 (_entry_back)
-               
-               423         272 KW_NAMES                 4
-                           274 PRECALL                  8
-                           278 CALL                     8
-                           288 POP_TOP
+               429          72 LOAD_FAST                0 (self)
+                            74 LOAD_METHOD              2 (winfo_width)
+                            96 PRECALL                  0
+                           100 CALL                     0
+                           110 LOAD_CONST               3 (1)
+                           112 BINARY_OP               10 (-)
                
-               432         290 LOAD_CONST               5 ('button_frame')
-                           292 LOAD_FAST                0 (self)
-                           294 STORE_ATTR               8 (entry_frame)
+               430         116 LOAD_FAST                0 (self)
+                           118 LOAD_METHOD              3 (winfo_height)
+                           140 PRECALL                  0
+                           144 CALL                     0
+                           154 LOAD_CONST               3 (1)
+                           156 BINARY_OP               10 (-)
+               
+               431         160 LOAD_FAST                0 (self)
+                           162 LOAD_ATTR                4 (entry_radius)
+               
+               432         172 LOAD_FAST                0 (self)
+                           174 LOAD_ATTR                5 (entry_border_width)
+               
+               433         184 LOAD_FAST                0 (self)
+                           186 LOAD_ATTR                6 (_entry_border)
+                           196 LOAD_FAST                0 (self)
+                           198 LOAD_ATTR                7 (_entry_back)
+               
+               426         208 KW_NAMES                 4
+                           210 PRECALL                  8
+                           214 CALL                     8
+                           224 POP_TOP
                
-               435         304 LOAD_FAST                0 (self)
-                           306 LOAD_METHOD              9 (create_window)
+               436         226 LOAD_CONST               5 ('button_frame')
+                           228 LOAD_FAST                0 (self)
+                           230 STORE_ATTR               8 (entry_frame)
                
-               436         328 LOAD_FAST                0 (self)
-                           330 LOAD_METHOD              3 (winfo_width)
-                           352 PRECALL                  0
-                           356 CALL                     0
-                           366 LOAD_CONST               3 (2)
-                           368 BINARY_OP               11 (/)
-                           372 LOAD_FAST                0 (self)
-                           374 LOAD_METHOD              4 (winfo_height)
-                           396 PRECALL                  0
-                           400 CALL                     0
-                           410 LOAD_CONST               3 (2)
-                           412 BINARY_OP               11 (/)
-               
-               437         416 LOAD_FAST                0 (self)
-                           418 LOAD_METHOD              3 (winfo_width)
-                           440 PRECALL                  0
-                           444 CALL                     0
-                           454 LOAD_FAST                0 (self)
-                           456 LOAD_ATTR                2 (entry_border_width)
-                           466 BINARY_OP               10 (-)
-                           470 LOAD_CONST               6 (5)
-                           472 BINARY_OP               10 (-)
-                           476 LOAD_FAST                0 (self)
-                           478 LOAD_ATTR               10 (entry_padding)
-                           488 LOAD_CONST               7 (0)
-                           490 BINARY_SUBSCR
-                           500 BINARY_OP               10 (-)
-               
-               438         504 LOAD_FAST                0 (self)
-                           506 LOAD_METHOD              4 (winfo_height)
-                           528 PRECALL                  0
-                           532 CALL                     0
-                           542 LOAD_FAST                0 (self)
-                           544 LOAD_ATTR                2 (entry_border_width)
-                           554 BINARY_OP               10 (-)
-                           558 LOAD_CONST               6 (5)
-                           560 BINARY_OP               10 (-)
-                           564 LOAD_FAST                0 (self)
-                           566 LOAD_ATTR               10 (entry_padding)
-                           576 LOAD_CONST               2 (1)
-                           578 BINARY_SUBSCR
-                           588 BINARY_OP               10 (-)
-               
-               439         592 LOAD_FAST                0 (self)
-                           594 LOAD_ATTR               11 (entry)
-               
-               435         604 KW_NAMES                 8
-                           606 PRECALL                  5
-                           610 CALL                     5
-                           620 LOAD_FAST                0 (self)
-                           622 STORE_ATTR              12 (entry_text)
-               
-               442         632 LOAD_FAST                0 (self)
-                           634 LOAD_METHOD             13 (create_rectangle)
-                           656 LOAD_CONST               9 (3)
-                           658 LOAD_FAST                0 (self)
-                           660 LOAD_ATTR                5 (entry_radius)
-                           670 LOAD_CONST               6 (5)
-                           672 BINARY_OP               11 (/)
-                           676 BINARY_OP                0 (+)
-               
-               443         680 LOAD_FAST                0 (self)
-                           682 LOAD_METHOD              4 (winfo_height)
-                           704 PRECALL                  0
-                           708 CALL                     0
-                           718 LOAD_FAST                0 (self)
-                           720 LOAD_ATTR               14 (_entry_bottom_width)
-                           730 BINARY_OP               10 (-)
-                           734 LOAD_CONST               9 (3)
-                           736 BINARY_OP               10 (-)
-               
-               444         740 LOAD_FAST                0 (self)
-                           742 LOAD_METHOD              3 (winfo_width)
-                           764 PRECALL                  0
-                           768 CALL                     0
-                           778 LOAD_CONST               9 (3)
-                           780 BINARY_OP               10 (-)
-                           784 LOAD_FAST                0 (self)
-                           786 LOAD_ATTR                5 (entry_radius)
-                           796 LOAD_CONST               6 (5)
-                           798 BINARY_OP               11 (/)
-                           802 BINARY_OP               10 (-)
-               
-               445         806 LOAD_FAST                0 (self)
-                           808 LOAD_METHOD              4 (winfo_height)
-                           830 PRECALL                  0
-                           834 CALL                     0
-                           844 LOAD_CONST              10 (3.5)
-                           846 BINARY_OP               10 (-)
-               
-               446         850 LOAD_FAST                0 (self)
-                           852 LOAD_ATTR               15 (_entry_bottom_line)
-                           862 LOAD_FAST                0 (self)
-                           864 LOAD_ATTR               15 (_entry_bottom_line)
-                           874 LOAD_CONST               7 (0)
-               
-               442         876 KW_NAMES                11
-                           878 PRECALL                  7
-                           882 CALL                     7
-                           892 LOAD_FAST                0 (self)
-                           894 STORE_ATTR              16 (entry_bottom)
-               
-               448         904 LOAD_FAST                0 (self)
-                           906 LOAD_ATTR               14 (_entry_bottom_width)
-                           916 LOAD_CONST               7 (0)
-                           918 COMPARE_OP               2 (==)
-                           924 POP_JUMP_FORWARD_IF_FALSE    26 (to 978)
+               438         240 LOAD_FAST                0 (self)
+                           242 LOAD_METHOD              9 (create_window)
                
-               449         926 LOAD_FAST                0 (self)
-                           928 LOAD_METHOD              0 (delete)
+               439         264 LOAD_FAST                0 (self)
+                           266 LOAD_METHOD              2 (winfo_width)
+                           288 PRECALL                  0
+                           292 CALL                     0
+                           302 LOAD_CONST               6 (2)
+                           304 BINARY_OP               11 (/)
+                           308 LOAD_FAST                0 (self)
+                           310 LOAD_METHOD              3 (winfo_height)
+                           332 PRECALL                  0
+                           336 CALL                     0
+                           346 LOAD_CONST               6 (2)
+                           348 BINARY_OP               11 (/)
+               
+               440         352 LOAD_FAST                0 (self)
+                           354 LOAD_METHOD              2 (winfo_width)
+                           376 PRECALL                  0
+                           380 CALL                     0
+                           390 LOAD_FAST                0 (self)
+                           392 LOAD_ATTR                5 (entry_border_width)
+                           402 BINARY_OP               10 (-)
+                           406 LOAD_FAST                0 (self)
+                           408 LOAD_ATTR               10 (entry_padding)
+                           418 LOAD_CONST               2 (0)
+                           420 BINARY_SUBSCR
+                           430 BINARY_OP               10 (-)
+                           434 LOAD_CONST               6 (2)
+                           436 BINARY_OP               10 (-)
+               
+               441         440 LOAD_FAST                0 (self)
+                           442 LOAD_METHOD              3 (winfo_height)
+                           464 PRECALL                  0
+                           468 CALL                     0
+                           478 LOAD_FAST                0 (self)
+                           480 LOAD_ATTR                5 (entry_border_width)
+                           490 BINARY_OP               10 (-)
+                           494 LOAD_FAST                0 (self)
+                           496 LOAD_ATTR               10 (entry_padding)
+                           506 LOAD_CONST               3 (1)
+                           508 BINARY_SUBSCR
+                           518 BINARY_OP               10 (-)
+                           522 LOAD_CONST               6 (2)
+                           524 BINARY_OP               10 (-)
+               
+               442         528 LOAD_FAST                0 (self)
+                           530 LOAD_ATTR               11 (entry)
+               
+               438         540 KW_NAMES                 7
+                           542 PRECALL                  5
+                           546 CALL                     5
+                           556 LOAD_FAST                0 (self)
+                           558 STORE_ATTR              12 (entry_text)
+               
+               445         568 LOAD_FAST                0 (self)
+                           570 LOAD_METHOD             13 (create_rectangle)
+                           592 LOAD_CONST               3 (1)
+                           594 LOAD_FAST                0 (self)
+                           596 LOAD_ATTR                4 (entry_radius)
+                           606 LOAD_CONST               8 (5)
+                           608 BINARY_OP               11 (/)
+                           612 BINARY_OP                0 (+)
+               
+               446         616 LOAD_FAST                0 (self)
+                           618 LOAD_METHOD              3 (winfo_height)
+                           640 PRECALL                  0
+                           644 CALL                     0
+                           654 LOAD_FAST                0 (self)
+                           656 LOAD_ATTR               14 (_entry_bottom_width)
+                           666 BINARY_OP               10 (-)
+                           670 LOAD_CONST               3 (1)
+                           672 BINARY_OP               10 (-)
+               
+               447         676 LOAD_FAST                0 (self)
+                           678 LOAD_METHOD              2 (winfo_width)
+                           700 PRECALL                  0
+                           704 CALL                     0
+                           714 LOAD_CONST               3 (1)
+                           716 BINARY_OP               10 (-)
+                           720 LOAD_FAST                0 (self)
+                           722 LOAD_ATTR                4 (entry_radius)
+                           732 LOAD_CONST               8 (5)
+                           734 BINARY_OP               11 (/)
+                           738 BINARY_OP               10 (-)
+               
+               448         742 LOAD_FAST                0 (self)
+                           744 LOAD_METHOD              3 (winfo_height)
+                           766 PRECALL                  0
+                           770 CALL                     0
+                           780 LOAD_CONST               3 (1)
+                           782 BINARY_OP               10 (-)
+               
+               449         786 LOAD_FAST                0 (self)
+                           788 LOAD_ATTR               15 (_entry_bottom_line)
+                           798 LOAD_FAST                0 (self)
+                           800 LOAD_ATTR               15 (_entry_bottom_line)
+               
+               450         810 LOAD_CONST               2 (0)
+               
+               445         812 KW_NAMES                 9
+                           814 PRECALL                  7
+                           818 CALL                     7
+                           828 LOAD_FAST                0 (self)
+                           830 STORE_ATTR              16 (entry_bottom)
+               
+               452         840 LOAD_FAST                0 (self)
+                           842 LOAD_ATTR               14 (_entry_bottom_width)
+                           852 LOAD_CONST               2 (0)
+                           854 COMPARE_OP               2 (==)
+                           860 POP_JUMP_FORWARD_IF_FALSE    26 (to 914)
+               
+               453         862 LOAD_FAST                0 (self)
+                           864 LOAD_METHOD              0 (delete)
+                           886 LOAD_FAST                0 (self)
+                           888 LOAD_ATTR               16 (entry_bottom)
+                           898 PRECALL                  1
+                           902 CALL                     1
+                           912 POP_TOP
+               
+               455     >>  914 LOAD_FAST                0 (self)
+                           916 LOAD_METHOD             17 (tag_raise)
+                           938 LOAD_FAST                0 (self)
+                           940 LOAD_ATTR               16 (entry_bottom)
                            950 LOAD_FAST                0 (self)
-                           952 LOAD_ATTR               16 (entry_bottom)
-                           962 PRECALL                  1
-                           966 CALL                     1
+                           952 LOAD_ATTR               12 (entry_text)
+                           962 PRECALL                  2
+                           966 CALL                     2
                            976 POP_TOP
                
-               451     >>  978 LOAD_FAST                0 (self)
-                           980 LOAD_METHOD             17 (tag_raise)
-                          1002 LOAD_FAST                0 (self)
-                          1004 LOAD_ATTR               16 (entry_bottom)
-                          1014 LOAD_FAST                0 (self)
-                          1016 LOAD_ATTR               12 (entry_text)
-                          1026 PRECALL                  2
-                          1030 CALL                     2
-                          1040 POP_TOP
-               
-               453        1042 LOAD_FAST                0 (self)
-                          1044 LOAD_ATTR               11 (entry)
-                          1054 LOAD_METHOD             18 (configure)
-                          1076 LOAD_FAST                0 (self)
-                          1078 LOAD_ATTR                7 (_entry_back)
-                          1088 LOAD_FAST                0 (self)
-                          1090 LOAD_ATTR               19 (_entry_text_back)
-                          1100 KW_NAMES                12
-                          1102 PRECALL                  2
-                          1106 CALL                     2
-                          1116 POP_TOP
-                          1118 LOAD_CONST               0 (None)
-                          1120 RETURN_VALUE
+               457         978 LOAD_FAST                0 (self)
+                           980 LOAD_ATTR               11 (entry)
+                           990 LOAD_METHOD             18 (configure)
+                          1012 LOAD_FAST                0 (self)
+                          1014 LOAD_ATTR                7 (_entry_back)
+                          1024 LOAD_FAST                0 (self)
+                          1026 LOAD_ATTR               19 (_entry_text_back)
+                          1036 LOAD_FAST                0 (self)
+                          1038 LOAD_ATTR               19 (_entry_text_back)
+                          1048 KW_NAMES                10
+                          1050 PRECALL                  3
+                          1054 CALL                     3
+                          1064 POP_TOP
+                          1066 LOAD_CONST               0 (None)
+                          1068 RETURN_VALUE
                consts
                   None
                   'all'
+                  0
                   1
-                  2
                   ('width', 'outline', 'fill')
                   'button_frame'
-                  5
-                  0
+                  2
                   ('width', 'height', 'window')
-                  3
-                  3.5
+                  5
                   ('fill', 'outline', 'width')
-                  ('background', 'foreground')
-               names      ('delete', 'create_round_rect4', 'entry_border_width', 'winfo_width', 'winfo_height', 'entry_radius', '_entry_border', '_entry_back', 'entry_frame', 'create_window', 'entry_padding', 'entry', 'entry_text', 'create_rectangle', '_entry_bottom_width', '_entry_bottom_line', 'entry_bottom', 'tag_raise', 'configure', '_entry_text_back')
+                  ('background', 'foreground', 'insertbackground')
+               names      ('delete', 'create_round_rect4', 'winfo_width', 'winfo_height', 'entry_radius', 'entry_border_width', '_entry_border', '_entry_back', 'entry_frame', 'create_window', 'entry_padding', 'entry', 'entry_text', 'create_rectangle', '_entry_bottom_width', '_entry_bottom_line', 'entry_bottom', 'tag_raise', 'configure', '_entry_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_draw'
-               firstlineno 420
+               firstlineno 423
                lnotab
-                  0x02012a021801120112013c0148010c0118fa12090e0318015801580158
-                  010cfc1c0730013c0142012c011afc1c06160134024002
+                  0x02012a021801020102012c012c010c010c0118f9120a0e021801580158
+                  0158010cfc1c0730013c0142012c01180102fb1c07160134024002
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               455           0 RESUME                   0
+               459           0 RESUME                   0
                
-               456           2 LOAD_FAST                0 (self)
+               460           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (entry_focusin_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_entry_back)
                
-               457          26 LOAD_FAST                0 (self)
+               461          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (entry_focusin_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_entry_border)
                
-               458          50 LOAD_FAST                0 (self)
+               462          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (entry_focusin_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_entry_text_back)
                
-               459          74 LOAD_FAST                0 (self)
+               463          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (entry_focusin_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_entry_bottom_line)
                
-               460          98 LOAD_FAST                0 (self)
+               464          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (entry_focusin_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_entry_bottom_width)
                
-               462         122 LOAD_FAST                0 (self)
+               466         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -3536,56 +3524,56 @@
                   None
                names      ('entry_focusin_back', '_entry_back', 'entry_focusin_border', '_entry_border', 'entry_focusin_text_back', '_entry_text_back', 'entry_focusin_bottom_line', '_entry_bottom_line', 'entry_focusin_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_focus'
-               firstlineno 455
+               firstlineno 459
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               464           0 RESUME                   0
+               468           0 RESUME                   0
                
-               465           2 LOAD_FAST                0 (self)
+               469           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (entry_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_entry_back)
                
-               466          26 LOAD_FAST                0 (self)
+               470          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (entry_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_entry_border)
                
-               467          50 LOAD_FAST                0 (self)
+               471          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (entry_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_entry_text_back)
                
-               468          74 LOAD_FAST                0 (self)
+               472          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (entry_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_entry_bottom_line)
                
-               469          98 LOAD_FAST                0 (self)
+               473          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (entry_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_entry_bottom_width)
                
-               471         122 LOAD_FAST                0 (self)
+               475         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -3593,66 +3581,66 @@
                   None
                names      ('entry_back', '_entry_back', 'entry_border', '_entry_border', 'entry_text_back', '_entry_text_back', 'entry_bottom_line', '_entry_bottom_line', 'entry_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_focusout'
-               firstlineno 464
+               firstlineno 468
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               473           0 RESUME                   0
+               477           0 RESUME                   0
                
-               474           2 LOAD_FAST                0 (self)
+               478           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_set)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('focus_set',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_click'
-               firstlineno 473
+               firstlineno 477
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064005300
-               476           0 RESUME                   0
+               480           0 RESUME                   0
                
-               477           2 LOAD_CONST               1 (True)
+               481           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                   True
                names      ('hover',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_hover'
-               firstlineno 476
+               firstlineno 480
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -3660,187 +3648,187 @@
                   00ab000000000000000000735a64017c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c006a0a00000000000000007c005f0b00000000000000007c00a0
                   0c00000000000000000000000000000000000000006400a6010000ab0100
                   0000000000000001006400530064005300
-               479           0 RESUME                   0
+               483           0 RESUME                   0
                
-               480           2 LOAD_FAST                0 (self)
+               484           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_get)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_JUMP_FORWARD_IF_TRUE    90 (to 222)
                
-               481          42 LOAD_CONST               1 (False)
+               485          42 LOAD_CONST               1 (False)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (hover)
                
-               482          56 LOAD_FAST                0 (self)
+               486          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (entry_back)
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_entry_back)
                
-               483          80 LOAD_FAST                0 (self)
+               487          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (entry_border)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               5 (_entry_border)
                
-               484         104 LOAD_FAST                0 (self)
+               488         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (entry_text_back)
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               7 (_entry_text_back)
                
-               485         128 LOAD_FAST                0 (self)
+               489         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                8 (entry_bottom_line)
                            140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               9 (_entry_bottom_line)
                
-               486         152 LOAD_FAST                0 (self)
+               490         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR               10 (entry_bottom_width)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR              11 (_entry_bottom_width)
                
-               488         176 LOAD_FAST                0 (self)
+               492         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD             12 (_draw)
                            200 LOAD_CONST               0 (None)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                
-               480     >>  222 LOAD_CONST               0 (None)
+               484     >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   False
                names      ('focus_get', 'hover', 'entry_back', '_entry_back', 'entry_border', '_entry_border', 'entry_text_back', '_entry_text_back', 'entry_bottom_line', '_entry_bottom_line', 'entry_bottom_width', '_entry_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       '_hover_release'
-               firstlineno 479
+               firstlineno 483
                lnotab 0x020128010e01180118011801180118022ef8
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               490           0 RESUME                   0
+               494           0 RESUME                   0
                
-               491           2 LOAD_FAST                1 (font)
+               495           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               492           6 LOAD_FAST                0 (self)
+               496           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (entry_text_font)
                             18 RETURN_VALUE
                
-               494     >>   20 LOAD_FAST                1 (font)
+               498     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (entry_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('entry_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'font'
-               firstlineno 490
+               firstlineno 494
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               496           0 RESUME                   0
+               500           0 RESUME                   0
                
-               497           2 LOAD_FAST                0 (self)
+               501           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 496
+               firstlineno 500
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640864066409640a640b640c640d640e9c0ea6
                   010000ab010000000000000000010064005300
-               499           0 RESUME                   0
+               503           0 RESUME                   0
                
-               500           2 LOAD_FAST                0 (self)
+               504           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               502          26 LOAD_CONST               1 (6)
+               506          26 LOAD_CONST               1 (13)
                
-               504          28 LOAD_CONST               2 ((3, 4))
+               508          28 LOAD_CONST               2 ((6, 4))
                
-               506          30 LOAD_CONST               3 ('#f3f3f3')
+               510          30 LOAD_CONST               3 ('#f3f3f3')
                
-               507          32 LOAD_CONST               4 (1)
+               511          32 LOAD_CONST               4 (1)
                
-               508          34 LOAD_CONST               5 (0)
+               512          34 LOAD_CONST               5 (0)
                
-               510          36 LOAD_CONST               6 ('#eaeaea')
+               514          36 LOAD_CONST               6 ('#eaeaea')
                
-               511          38 LOAD_CONST               7 ('#fdfdfd')
+               515          38 LOAD_CONST               7 ('#fdfdfd')
                
-               512          40 LOAD_CONST               8 ('#5f5f5f')
+               516          40 LOAD_CONST               8 ('#5f5f5f')
                
-               513          42 LOAD_CONST               6 ('#eaeaea')
+               517          42 LOAD_CONST               6 ('#eaeaea')
                
-               515          44 LOAD_CONST               9 ('#e2e2e2')
+               519          44 LOAD_CONST               9 ('#e2e2e2')
                
-               516          46 LOAD_CONST              10 ('#f9f9f9')
+               520          46 LOAD_CONST              10 ('#f9f9f9')
                
-               517          48 LOAD_CONST              11 ('#1a1a1a')
+               521          48 LOAD_CONST              11 ('#1a1a1a')
                
-               518          50 LOAD_CONST              12 ('#185fb4')
+               522          50 LOAD_CONST              12 ('#185fb4')
                
-               519          52 LOAD_CONST              13 (2)
+               523          52 LOAD_CONST              13 (2)
                
-               501          54 LOAD_CONST              14 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
+               505          54 LOAD_CONST              14 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
                             56 BUILD_CONST_KEY_MAP     14
                
-               500          58 PRECALL                  1
+               504          58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
-                  6
-                  (3, 4)
+                  13
+                  (6, 4)
                   '#f3f3f3'
                   1
                   0
                   '#eaeaea'
                   '#fdfdfd'
                   '#5f5f5f'
                   '#e2e2e2'
@@ -3851,71 +3839,71 @@
                   ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette_light'
-               firstlineno 499
+               firstlineno 503
                lnotab
                   0x0201180202020202020102010202020102010201020202010201020102
                   0102ee04ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640864096405640a6408640b640c640d9c0ea6
                   010000ab010000000000000000010064005300
-               523           0 RESUME                   0
+               527           0 RESUME                   0
                
-               524           2 LOAD_FAST                0 (self)
+               528           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               526          26 LOAD_CONST               1 (6)
+               530          26 LOAD_CONST               1 (13)
                
-               528          28 LOAD_CONST               2 ((3, 4))
+               532          28 LOAD_CONST               2 ((3, 4))
                
-               530          30 LOAD_CONST               3 ('#202020')
+               534          30 LOAD_CONST               3 ('#202020')
                
-               531          32 LOAD_CONST               4 (1)
+               535          32 LOAD_CONST               4 (1)
                
-               533          34 LOAD_CONST               5 ('#454545')
+               537          34 LOAD_CONST               5 ('#454545')
                
-               534          36 LOAD_CONST               6 ('#353535')
+               538          36 LOAD_CONST               6 ('#353535')
                
-               535          38 LOAD_CONST               7 ('#cecece')
+               539          38 LOAD_CONST               7 ('#cecece')
                
-               536          40 LOAD_CONST               8 ('#ffffff')
+               540          40 LOAD_CONST               8 ('#ffffff')
                
-               537          42 LOAD_CONST               9 (0)
+               541          42 LOAD_CONST               9 (0)
                
-               539          44 LOAD_CONST               5 ('#454545')
+               543          44 LOAD_CONST               5 ('#454545')
                
-               540          46 LOAD_CONST              10 ('#2f2f2f')
+               544          46 LOAD_CONST              10 ('#2f2f2f')
                
-               541          48 LOAD_CONST               8 ('#ffffff')
+               545          48 LOAD_CONST               8 ('#ffffff')
                
-               542          50 LOAD_CONST              11 ('#4cc2ff')
+               546          50 LOAD_CONST              11 ('#4cc2ff')
                
-               543          52 LOAD_CONST              12 (2)
+               547          52 LOAD_CONST              12 (2)
                
-               525          54 LOAD_CONST              13 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
+               529          54 LOAD_CONST              13 (('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width'))
                             56 BUILD_CONST_KEY_MAP     14
                
-               524          58 PRECALL                  1
+               528          58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
-                  6
+                  13
                   (3, 4)
                   '#202020'
                   1
                   '#454545'
                   '#353535'
                   '#cecece'
                   '#ffffff'
@@ -3926,15 +3914,15 @@
                   ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette_dark'
-               firstlineno 523
+               firstlineno 527
                lnotab
                   0x0201180202020202020102020201020102010201020202010201020102
                   0102ee04ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 11
@@ -3956,160 +3944,160 @@
                   000000000000006400a6010000ab01000000000000000001006400530023
                   00741e000000000000000000002400720401005900640053007700780359
                   0077017c006a0100000000000000007c006a0200000000000000007c006a
                   0300000000000000007c006a0800000000000000007c006a040000000000
                   0000007c006a0500000000000000007c006a0600000000000000007c006a
                   0900000000000000007c006a0a00000000000000007c006a0b0000000000
                   000000640f9c0a5300
-               547           0 RESUME                   0
+               551           0 RESUME                   0
                
-               548           2 LOAD_FAST                1 (dict)
+               552           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE   223 (to 452)
                
-               549           6 LOAD_FAST                1 (dict)
+               553           6 LOAD_FAST                1 (dict)
                              8 LOAD_CONST               1 ('entry_radius')
                             10 BINARY_SUBSCR
                             20 LOAD_FAST                0 (self)
                             22 STORE_ATTR               0 (entry_radius)
                
-               551          32 LOAD_FAST                1 (dict)
+               555          32 LOAD_FAST                1 (dict)
                             34 LOAD_CONST               2 ('entry_padding')
                             36 BINARY_SUBSCR
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               1 (entry_padding)
                
-               553          58 LOAD_FAST                1 (dict)
+               557          58 LOAD_FAST                1 (dict)
                             60 LOAD_CONST               3 ('entry_frame_back')
                             62 BINARY_SUBSCR
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (entry_frame_back)
                
-               554          84 LOAD_FAST                1 (dict)
+               558          84 LOAD_FAST                1 (dict)
                             86 LOAD_CONST               4 ('entry_border_width')
                             88 BINARY_SUBSCR
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               3 (entry_border_width)
                
-               556         110 LOAD_FAST                1 (dict)
+               560         110 LOAD_FAST                1 (dict)
                            112 LOAD_CONST               5 ('entry_border')
                            114 BINARY_SUBSCR
                            124 LOAD_FAST                0 (self)
                            126 STORE_ATTR               4 (entry_border)
                
-               557         136 LOAD_FAST                1 (dict)
+               561         136 LOAD_FAST                1 (dict)
                            138 LOAD_CONST               6 ('entry_back')
                            140 BINARY_SUBSCR
                            150 LOAD_FAST                0 (self)
                            152 STORE_ATTR               5 (entry_back)
                
-               558         162 LOAD_FAST                1 (dict)
+               562         162 LOAD_FAST                1 (dict)
                            164 LOAD_CONST               7 ('entry_text_back')
                            166 BINARY_SUBSCR
                            176 LOAD_FAST                0 (self)
                            178 STORE_ATTR               6 (entry_text_back)
                
-               559         188 LOAD_FAST                1 (dict)
+               563         188 LOAD_FAST                1 (dict)
                            190 LOAD_CONST               8 ('entry_bottom_line')
                            192 BINARY_SUBSCR
                            202 LOAD_FAST                0 (self)
                            204 STORE_ATTR               7 (entry_bottom_line)
                
-               560         214 LOAD_FAST                1 (dict)
+               564         214 LOAD_FAST                1 (dict)
                            216 LOAD_CONST               9 ('entry_bottom_width')
                            218 BINARY_SUBSCR
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (entry_bottom_width)
                
-               562         240 LOAD_FAST                1 (dict)
+               566         240 LOAD_FAST                1 (dict)
                            242 LOAD_CONST              10 ('entry_focusin_border')
                            244 BINARY_SUBSCR
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (entry_focusin_border)
                
-               563         266 LOAD_FAST                1 (dict)
+               567         266 LOAD_FAST                1 (dict)
                            268 LOAD_CONST              11 ('entry_focusin_back')
                            270 BINARY_SUBSCR
                            280 LOAD_FAST                0 (self)
                            282 STORE_ATTR              10 (entry_focusin_back)
                
-               564         292 LOAD_FAST                1 (dict)
+               568         292 LOAD_FAST                1 (dict)
                            294 LOAD_CONST              12 ('entry_focusin_text_back')
                            296 BINARY_SUBSCR
                            306 LOAD_FAST                0 (self)
                            308 STORE_ATTR              11 (entry_focusin_text_back)
                
-               565         318 LOAD_FAST                1 (dict)
+               569         318 LOAD_FAST                1 (dict)
                            320 LOAD_CONST              13 ('entry_focusin_bottom_line')
                            322 BINARY_SUBSCR
                            332 LOAD_FAST                0 (self)
                            334 STORE_ATTR              12 (entry_focusin_bottom_line)
                
-               566         344 LOAD_FAST                1 (dict)
+               570         344 LOAD_FAST                1 (dict)
                            346 LOAD_CONST              14 ('entry_focusin_bottom_width')
                            348 BINARY_SUBSCR
                            358 LOAD_FAST                0 (self)
                            360 STORE_ATTR              13 (entry_focusin_bottom_width)
                
-               568         370 NOP
+               572         370 NOP
                
-               569         372 LOAD_FAST                0 (self)
+               573         372 LOAD_FAST                0 (self)
                            374 LOAD_METHOD             14 (_draw)
                            396 LOAD_CONST               0 (None)
                            398 PRECALL                  1
                            402 CALL                     1
                            412 POP_TOP
                            414 LOAD_CONST               0 (None)
                            416 RETURN_VALUE
                        >>  418 PUSH_EXC_INFO
                
-               570         420 LOAD_GLOBAL             30 (AttributeError)
+               574         420 LOAD_GLOBAL             30 (AttributeError)
                            432 CHECK_EXC_MATCH
                            434 POP_JUMP_FORWARD_IF_FALSE     4 (to 444)
                            436 POP_TOP
                
-               571         438 POP_EXCEPT
+               575         438 POP_EXCEPT
                            440 LOAD_CONST               0 (None)
                            442 RETURN_VALUE
                
-               570     >>  444 RERAISE                  0
+               574     >>  444 RERAISE                  0
                        >>  446 COPY                     3
                            448 POP_EXCEPT
                            450 RERAISE                  1
                
-               574     >>  452 LOAD_FAST                0 (self)
+               578     >>  452 LOAD_FAST                0 (self)
                            454 LOAD_ATTR                1 (entry_padding)
                
-               576         464 LOAD_FAST                0 (self)
+               580         464 LOAD_FAST                0 (self)
                            466 LOAD_ATTR                2 (entry_frame_back)
                
-               577         476 LOAD_FAST                0 (self)
+               581         476 LOAD_FAST                0 (self)
                            478 LOAD_ATTR                3 (entry_border_width)
                
-               578         488 LOAD_FAST                0 (self)
+               582         488 LOAD_FAST                0 (self)
                            490 LOAD_ATTR                8 (entry_bottom_width)
                
-               580         500 LOAD_FAST                0 (self)
+               584         500 LOAD_FAST                0 (self)
                            502 LOAD_ATTR                4 (entry_border)
                
-               581         512 LOAD_FAST                0 (self)
+               585         512 LOAD_FAST                0 (self)
                            514 LOAD_ATTR                5 (entry_back)
                
-               582         524 LOAD_FAST                0 (self)
+               586         524 LOAD_FAST                0 (self)
                            526 LOAD_ATTR                6 (entry_text_back)
                
-               584         536 LOAD_FAST                0 (self)
+               588         536 LOAD_FAST                0 (self)
                            538 LOAD_ATTR                9 (entry_focusin_border)
                
-               585         548 LOAD_FAST                0 (self)
+               589         548 LOAD_FAST                0 (self)
                            550 LOAD_ATTR               10 (entry_focusin_back)
                
-               586         560 LOAD_FAST                0 (self)
+               590         560 LOAD_FAST                0 (self)
                            562 LOAD_ATTR               11 (entry_focusin_text_back)
                
-               573         572 LOAD_CONST              15 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back'))
+               577         572 LOAD_CONST              15 (('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back'))
                            574 BUILD_CONST_KEY_MAP     10
                            576 RETURN_VALUE
                ExceptionTable:
                  372 to 412 -> 418 [0]
                  418 to 436 -> 446 [1] lasti
                  444 to 444 -> 446 [1] lasti
                consts
@@ -4131,139 +4119,139 @@
                   ('entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_bottom_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back')
                names      ('entry_radius', 'entry_padding', 'entry_frame_back', 'entry_border_width', 'entry_border', 'entry_back', 'entry_text_back', 'entry_bottom_line', 'entry_bottom_width', 'entry_focusin_border', 'entry_focusin_back', 'entry_focusin_text_back', 'entry_focusin_bottom_line', 'entry_focusin_bottom_width', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'palette'
-               firstlineno 547
+               firstlineno 551
                lnotab
                   0x020104011a021a021a011a021a011a011a011a011a021a011a011a011a
                   011a0202013001120106ff08040c020c010c010c020c010c010c020c010c
                   010cf3
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'float', 'int', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawBasicRoundEntry3'
-         firstlineno 406
-         lnotab 0x0c010a030604140606230809080908030803080b0e06060306180618
+         firstlineno 410
+         lnotab 0x0c010a030603140606240809080908030803080b0e06060306180618
       'AdwDrawBasicRoundEntry3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         590           0 RESUME                   0
+         594           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundEntry3')
                        8 STORE_NAME               2 (__qualname__)
          
-         591          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 591>)
+         595          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 595>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundEntry3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               591           0 RESUME                   0
+               595           0 RESUME                   0
                
-               592           2 LOAD_FAST                0 (self)
+               596           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 591
+               firstlineno 595
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawRoundEntry3'
-         firstlineno 590
+         firstlineno 594
          lnotab 0x0a01
       'AdwDrawRoundEntry3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         595           0 RESUME                   0
+         599           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkEntry3')
                        8 STORE_NAME               2 (__qualname__)
          
-         596          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 596>)
+         600          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\entry.py", line 600>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkEntry3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               596           0 RESUME                   0
+               600           0 RESUME                   0
                
-               597           2 LOAD_FAST                0 (self)
+               601           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
                name       'default_palette'
-               firstlineno 596
+               firstlineno 600
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
          name       'AdwDrawRoundDarkEntry3'
-         firstlineno 595
+         firstlineno 599
          lnotab 0x0a01
       'AdwDrawRoundDarkEntry3'
       '__main__'
       ('Tk',)
       'Hello'
       ('text',)
       'x'
@@ -4274,10 +4262,10 @@
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\canvas\\entry.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c041c7f004a1c051c061c7f00331c051c051c7f00391c
+      0x00ff020110010c041c7f004d1c051c061c7f00341c051c051c7f00391c
       051c050c010c021402180130021801300218013002180130021801300218
       0130022ce9
```

### Comparing `tkadw-0.1.1/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc` & `tkadw-0.1.2/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/adwite/button.py` & `tkadw-0.1.2/tkadw/canvas/adwite/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/atomize/button.py` & `tkadw-0.1.2/tkadw/canvas/atomize/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/button.py` & `tkadw-0.1.2/tkadw/canvas/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from tkinter.font import Font, nametofont
 from tkadw.canvas.drawengine import AdwDrawEngine
 
 
 # Button
 class AdwDrawBasicButton(AdwDrawEngine):
     def __init__(self, *args, width=120, height=40, text: str = "", command=None, **kwargs):
-        super().__init__(*args, width=width, height=height, bd=0, **kwargs)
+        super().__init__(*args, width=width, height=height, bd=0, highlightthickness=0, **kwargs)
 
         self._other()
 
         self.default_palette()
 
         self.text = text
 
@@ -26,14 +26,24 @@
         self.bind("<Leave>", self._hover_release, add="+")
 
         if command is not None:
             self.bind("<<Click>>", lambda event: command())
 
         self._draw(None)
 
+    def configure(self, **kwargs):
+        if "command" in kwargs:
+            self.command = kwargs.pop("command")
+            self.bind("<<Click>>", lambda event: self.command())
+        elif "text" in kwargs:
+            self.text = kwargs.pop("text")
+            self._draw(None)
+        else:
+            super().configure(**kwargs)
+
     def _other(self):
         if hasattr(self, "button_frame_back"):
             self.configure(background=self.button_frame_back, borderwidth=0)
 
     def _draw(self, evt):
         self.delete("all")
```

### Comparing `tkadw-0.1.1/tkadw/canvas/demo.tcl` & `tkadw-0.1.2/tkadw/canvas/fun4.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
- #!/bin/sh
- # The next line restarts with tclsh.\
- exec tclsh "$0" ${1+"$@"}
+from tkinter import *
 
+
+root = Tk()
+root.eval("""
  package require Tcl 8.5
  package require Tk
 
  source [file join [file dirname [info script]] poly.tcl]
 
  proc draw {win} {
      global demo
@@ -99,10 +100,11 @@
      .c bind vtx <ButtonRelease-1> {.c dtag selected}
      bind .c <B1-Motion> {move .c %x %y}
 
      focus .c
      draw .c
  }
 
- main {*}$argv
+ main
 
- # vim: set ts=4 sts=4 sw=4 tw=80 et ft=tcl:
+""")
+root.mainloop()
```

### Comparing `tkadw-0.1.1/tkadw/canvas/drawengine.py` & `tkadw-0.1.2/tkadw/canvas/drawengine.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,14 +220,17 @@
     return $xy
  }
 
 """
 
 
 class AdwDrawEngine(Canvas):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
     def win32_high_dpi(self):
         from ctypes import windll
         windll.shcore.SetProcessDpiAwareness(2)
 
     def draw_gradient(self, color1, color2, type="x"):
         self.tk.eval("""
   proc + {n1 n2} {
```

### Comparing `tkadw-0.1.1/tkadw/canvas/entry.py` & `tkadw-0.1.2/tkadw/canvas/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tkadw.canvas.drawengine import AdwDrawEngine
 
 
 # Entry
 class AdwDrawBasicEntry(AdwDrawEngine):
     def __init__(self, *args, width=120, height=40, text: str = "", **kwargs):
 
-        super().__init__(*args, width=width, height=height, **kwargs)
+        super().__init__(*args, width=width, height=height, highlightthickness=0, **kwargs)
 
         from tkinter import StringVar, Entry
 
         self.var = StringVar()
         self.var.set(text)
 
         self.entry = Entry(self, bd=0, textvariable=self.var)
@@ -50,34 +50,37 @@
         if hasattr(self, "button_frame_back"):
             self.configure(background=self.button_frame_back, borderwidth=0)
 
     def _draw(self, evt):
         self.delete("all")
 
         self.entry_frame = self.create_rectangle(
-            1.5, 1.5, self.winfo_width() - 3, self.winfo_height() - 3,
+            0, 0, self.winfo_width() - 1, self.winfo_height() - 1,
             width=self.entry_border_width,
             outline=self._entry_border, fill=self._entry_back,
         )
 
         self.entry_text = self.create_window(
             self.winfo_width() / 2, self.winfo_height() / 2,
-            width=self.winfo_width()-self.entry_border_width-5-self.entry_padding[0], height=self.winfo_height()-self.entry_border_width-5-self.entry_padding[1],
+            width=self.winfo_width() - self.entry_border_width - 5 - self.entry_padding[0],
+            height=self.winfo_height() - self.entry_border_width - 5 - self.entry_padding[1],
             window=self.entry
         )
 
-        self.entry_bottom = self.create_rectangle(3, self.winfo_height()-self._entry_bottom_width-3, self.winfo_width()-3, self.winfo_height()-3.5,
-                                                  fill=self._entry_bottom_line, outline=self._entry_bottom_line, width=0)
+        self.entry_bottom = self.create_rectangle(1, self.winfo_height() - self._entry_bottom_width - 1,
+                                                  self.winfo_width() - 1, self.winfo_height() - 1,
+                                                  fill=self._entry_bottom_line, outline=self._entry_bottom_line,
+                                                  width=0)
 
         if self._entry_bottom_width == 0:
             self.delete(self.entry_bottom)
 
         self.tag_raise(self.entry_bottom, self.entry_text)
 
-        self.entry.configure(background=self._entry_back, foreground=self._entry_text_back)
+        self.entry.configure(background=self._entry_back, foreground=self._entry_text_back, insertbackground=self._entry_text_back)
 
     def _focus(self, evt=None):
         self._entry_back = self.entry_focusin_back
         self._entry_border = self.entry_focusin_border
         self._entry_text_back = self.entry_focusin_text_back
         self._entry_bottom_line = self.entry_focusin_bottom_line
         self._entry_bottom_width = self.entry_focusin_bottom_width
@@ -229,38 +232,39 @@
         else:
             self.button_radius = radius
 
     def _draw(self, evt):
         self.delete("all")
 
         self.entry_frame = self.create_round_rect2(
-            2, 2, self.winfo_width()-3, self.winfo_height()-3, self.entry_radius,
+            2, 2, self.winfo_width() - 3, self.winfo_height() - 3, self.entry_radius,
             width=self.entry_border_width,
             outline=self._entry_border, fill=self._entry_back,
         )
 
         self.entry_text = self.create_window(
             self.winfo_width() / 2, self.winfo_height() / 2,
-            width=self.winfo_width()-self.entry_border_width-5-self.entry_padding[0],
-            height=self.winfo_height()-self.entry_border_width-5-self.entry_padding[1],
+            width=self.winfo_width() - self.entry_border_width - 5 - self.entry_padding[0],
+            height=self.winfo_height() - self.entry_border_width - 5 - self.entry_padding[1],
             window=self.entry
         )
 
-        self.entry_bottom = self.create_rectangle(3+self.entry_radius/2,
-                                                  self.winfo_height()-self._entry_bottom_width-3,
-                                                  self.winfo_width()-3-self.entry_radius/2,
-                                                  self.winfo_height()-3.5,
-                                                  fill=self._entry_bottom_line, outline=self._entry_bottom_line, width=0)
+        self.entry_bottom = self.create_rectangle(3 + self.entry_radius / 2,
+                                                  self.winfo_height() - self._entry_bottom_width - 3,
+                                                  self.winfo_width() - 3 - self.entry_radius / 2,
+                                                  self.winfo_height() - 3.5,
+                                                  fill=self._entry_bottom_line, outline=self._entry_bottom_line,
+                                                  width=0)
 
         if self._entry_bottom_width == 0:
             self.delete(self.entry_bottom)
 
         self.tag_raise(self.entry_bottom, self.entry_text)
 
-        self.entry.configure(background=self._entry_back, foreground=self._entry_text_back)
+        self.entry.configure(background=self._entry_back, foreground=self._entry_text_back, insertbackground=self._entry_text_back)
 
     def _focus(self, evt=None):
         self._entry_back = self.entry_focusin_back
         self._entry_border = self.entry_focusin_border
         self._entry_text_back = self.entry_focusin_text_back
         self._entry_bottom_line = self.entry_focusin_bottom_line
         self._entry_bottom_width = self.entry_focusin_bottom_width
@@ -404,57 +408,57 @@
 
 
 class AdwDrawBasicRoundEntry3(AdwDrawBasicEntry):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def _other(self):
-        if hasattr(self, "button_frame_back"):
-            self.configure(background=self.button_frame_back, borderwidth=0)
+        self.configure(background=self.master.cget("bg"), borderwidth=0)
 
     def border_radius(self, radius: float | int = None):
         if radius is None:
             return self.button_radius
         else:
             self.button_radius = radius
 
     def _draw(self, evt):
         self.delete("all")
 
         self.create_round_rect4(
-            self.entry_border_width + 1,
-            self.entry_border_width + 1,
-            self.winfo_width() - self.entry_border_width -2,
-            self.winfo_height() - self.entry_border_width -2, self.entry_radius,
+            0,
+            0,
+            self.winfo_width() - 1,
+            self.winfo_height() - 1,
+            self.entry_radius,
             width=self.entry_border_width,
             outline=self._entry_border, fill=self._entry_back,
         )
 
         self.entry_frame = "button_frame"
 
-
         self.entry_text = self.create_window(
             self.winfo_width() / 2, self.winfo_height() / 2,
-            width=self.winfo_width()-self.entry_border_width-5-self.entry_padding[0],
-            height=self.winfo_height()-self.entry_border_width-5-self.entry_padding[1],
+            width=self.winfo_width() - self.entry_border_width - self.entry_padding[0] - 2,
+            height=self.winfo_height() - self.entry_border_width - self.entry_padding[1] - 2,
             window=self.entry
         )
 
-        self.entry_bottom = self.create_rectangle(3+self.entry_radius/5,
-                                                  self.winfo_height()-self._entry_bottom_width-3,
-                                                  self.winfo_width()-3-self.entry_radius/5,
-                                                  self.winfo_height()-3.5,
-                                                  fill=self._entry_bottom_line, outline=self._entry_bottom_line, width=0)
+        self.entry_bottom = self.create_rectangle(1 + self.entry_radius / 5,
+                                                  self.winfo_height() - self._entry_bottom_width - 1,
+                                                  self.winfo_width() - 1 - self.entry_radius / 5,
+                                                  self.winfo_height() - 1,
+                                                  fill=self._entry_bottom_line, outline=self._entry_bottom_line,
+                                                  width=0)
 
         if self._entry_bottom_width == 0:
             self.delete(self.entry_bottom)
 
         self.tag_raise(self.entry_bottom, self.entry_text)
 
-        self.entry.configure(background=self._entry_back, foreground=self._entry_text_back)
+        self.entry.configure(background=self._entry_back, foreground=self._entry_text_back, insertbackground=self._entry_text_back)
 
     def _focus(self, evt=None):
         self._entry_back = self.entry_focusin_back
         self._entry_border = self.entry_focusin_border
         self._entry_text_back = self.entry_focusin_text_back
         self._entry_bottom_line = self.entry_focusin_bottom_line
         self._entry_bottom_width = self.entry_focusin_bottom_width
@@ -495,17 +499,17 @@
 
     def default_palette(self):
         self.palette_light()
 
     def palette_light(self):
         self.palette(
             {
-                "entry_radius": 6,
+                "entry_radius": 13,
 
-                "entry_padding": (3, 4),
+                "entry_padding": (6, 4),
 
                 "entry_frame_back": "#f3f3f3",
                 "entry_border_width": 1,
                 "entry_bottom_width": 0,
 
                 "entry_border": "#eaeaea",
                 "entry_back": "#fdfdfd",
@@ -519,15 +523,15 @@
                 "entry_focusin_bottom_width": 2,
             }
         )
 
     def palette_dark(self):
         self.palette(
             {
-                "entry_radius": 6,
+                "entry_radius": 13,
 
                 "entry_padding": (3, 4),
 
                 "entry_frame_back": "#202020",
                 "entry_border_width": 1,
 
                 "entry_border": "#454545",
@@ -616,8 +620,8 @@
 
     entry5 = AdwDrawRoundEntry3(text="Hello")
     entry5.pack(fill="x", padx=5, pady=5)
 
     entry6 = AdwDrawRoundDarkEntry3(text="Hello")
     entry6.pack(fill="x", padx=5, pady=5)
 
-    root.mainloop()
+    root.mainloop()
```

### Comparing `tkadw-0.1.1/tkadw/canvas/fluent/__init__.py` & `tkadw-0.1.2/tkadw/canvas/fluent/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/fun.py` & `tkadw-0.1.2/tkadw/canvas/fun.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/fun2.py` & `tkadw-0.1.2/tkadw/canvas/fun2.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/fun3.py` & `tkadw-0.1.2/tkadw/canvas/fun3.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/fun5.py` & `tkadw-0.1.2/tkadw/canvas/fun5.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/fun6.py` & `tkadw-0.1.2/tkadw/canvas/fun6.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/poly.tcl` & `tkadw-0.1.2/tkadw/canvas/poly.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/canvas/titlebar.py` & `tkadw-0.1.2/tkadw/canvas/titlebar.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/tkite/gtk/button.py` & `tkadw-0.1.2/tkadw/tkite/gtk/button.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,20 +19,41 @@
                 "button_back": "#f6f5f4",
                 "button_text_back": "#2e3436",
 
                 "button_active_border": "#dad6d2",
                 "button_active_back": "#f8f8f7",
                 "button_active_text_back": "#2e3436",
 
-                "button_pressed_border": "#3584e4",
+                "button_pressed_border": "#dad6d2",
                 "button_pressed_back": "#dad6d2",
                 "button_pressed_text_back": "#2e3436",
             }
         )
 
+    def palette_gtk_dark(self):
+        self.palette(
+            {
+                "button_radius": 11,
+
+                "button_border_width": 1.3,
+
+                "button_border": "#1b1b1b",
+                "button_back": "#353535",
+                "button_text_back": "#eeeeec",
+
+                "button_active_border": "#1b1b1b",
+                "button_active_back": "#373737",
+                "button_active_text_back": "#eeeeec",
+
+                "button_pressed_border": "#282828",
+                "button_pressed_back": "#1e1e1e",
+                "button_pressed_text_back": "#eeeeec",
+            }
+        )
+
     def palette_gtk_red(self):
         self.palette(
             {
                 "button_radius": 11,
 
                 "button_border_width": 1.3,
 
@@ -68,32 +89,41 @@
                 "button_pressed_border": "#185fb4",
                 "button_pressed_back": "#1961b9",
                 "button_pressed_text_back": "#ffffff",
             }
         )
 
 
+class GTkDarkButton(GTkButton):
+    def default_palette(self):
+        self.palette_gtk_dark()
+
+
 class GTkDestructiveButton(GTkButton):
     def default_palette(self):
         self.palette_gtk_red()
 
 
 class GTkSuggestedButton(GTkButton):
     def default_palette(self):
         self.palette_gtk_blue()
 
 
 if __name__ == '__main__':
     from tkinter import Tk
 
     root = Tk()
+    root.configure(background="#1e1e1e")
+
+    button = GTkDarkButton(text="GTkButton", command=lambda: print("button1 clicked"))
+    button.pack(fill="x", ipadx=5, padx=5, pady=5)
 
-    button = GTkButton(text="GTkButton", command=lambda: print("button1 clicked"))
-    button.pack(ipadx=5)
+    button2 = GTkDarkButton(text="GTkDarkButton", command=lambda: print("button2 clicked"), background="#1e1e1e")
+    button2.pack(fill="x", ipadx=5, padx=5, pady=5)
 
-    button2 = GTkDestructiveButton(text="GTkDestructiveButton", command=lambda: print("button2 clicked"))
-    button2.pack(ipadx=5)
+    button3 = GTkDestructiveButton(text="GTkDestructiveButton", command=lambda: print("button3 clicked"))
+    button3.pack(fill="x", ipadx=5, padx=5, pady=5)
 
-    button3 = GTkSuggestedButton(text="GTkSuggestedButton", command=lambda: print("button3 clicked"))
-    button3.pack(ipadx=5)
+    button4 = GTkSuggestedButton(text="GTkSuggestedButton", command=lambda: print("button4 clicked"))
+    button4.pack(fill="x", ipadx=5, padx=5, pady=5)
 
     root.mainloop()
```

### Comparing `tkadw-0.1.1/tkadw/tkite/gtk/entry.py` & `tkadw-0.1.2/tkadw/tkite/gtk/entry.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,32 +13,65 @@
             {
                 "entry_radius": 11,
 
                 "entry_padding": (5, 5),
 
                 "entry_frame_back": "#eaeaea",
                 "entry_border_width": 1,
-                "entry_bottom_width": 0,
 
                 "entry_border": "#cdc7c2",
                 "entry_back": "#ffffff",
                 "entry_text_back": "#000000",
                 "entry_bottom_line": "#eaeaea",
+                "entry_bottom_width": 0,
 
                 "entry_focusin_border": "#3584e4",
                 "entry_focusin_back": "#ffffff",
                 "entry_focusin_text_back": "#000000",
                 "entry_focusin_bottom_line": "#185fb4",
                 "entry_focusin_bottom_width": 0,
             }
         )
 
+    def palette_gtk_dark(self):
+        self.palette(
+            {
+                "entry_radius": 11,
+
+                "entry_padding": (5, 5),
+
+                "entry_frame_back": "#eaeaea",
+                "entry_border_width": 1,
+
+                "entry_border": "#1f1f1f",
+                "entry_back": "#2d2d2d",
+                "entry_text_back": "#cccccc",
+                "entry_bottom_line": "#eaeaea",
+                "entry_bottom_width": 0,
+
+                "entry_focusin_border": "#3584e4",
+                "entry_focusin_back": "#2d2d2d",
+                "entry_focusin_text_back": "#ffffff",
+                "entry_focusin_bottom_line": "#3584e4",
+                "entry_focusin_bottom_width": 0,
+            }
+        )
+
+
+class GTkDarkEntry(GTkEntry):
+    def default_palette(self):
+        self.palette_gtk_dark()
+
 
 if __name__ == '__main__':
     from tkinter import Tk
 
     root = Tk()
+    root.configure(background="#1e1e1e")
+
+    entry = GTkDarkEntry(text="GTkEntry")
+    entry.pack(fill="x", ipadx=5, padx=5, pady=5)
 
-    entry = GTkEntry(text="GTkEntry")
-    entry.pack(ipadx=5)
+    entry2 = GTkDarkEntry(text="GTkDarkEntry")
+    entry2.pack(fill="x", ipadx=5, padx=5, pady=5)
 
     root.mainloop()
```

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/__init__.py` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/sun-valley.tcl` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/sun-valley.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/sv.tcl` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/sv.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-disabled.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-hover.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-pressed.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-rest.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-disabled.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-hover.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-pressed.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-rest.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-disabled.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-hover.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-pressed.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-rest.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-off-disabled.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-off-hover.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-off-pressed.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-off-rest.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-on-disabled.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-on-hover.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-on-pressed.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark/switch-on-rest.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/dark.tcl` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-disabled.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-hover.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-pressed.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-rest.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-disabled.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-hover.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-pressed.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-rest.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-disabled.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-hover.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-pressed.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-rest.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-off-disabled.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-off-hover.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-off-pressed.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-off-rest.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-on-disabled.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-on-hover.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-on-pressed.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light/switch-on-rest.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/light.tcl` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/sprites_dark.tcl` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/sprites_dark.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/sprites_light.tcl` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/sprites_light.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/spritesheet_dark.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_dark.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/spritesheet_light.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_light.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/tkadw/ttk/atomize_ttk/theme/spritesheet_light2.png` & `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_light2.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.1/PKG-INFO` & `tkadw-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkadw
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: XiangQinxi
 Author-email: 1379773753@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

